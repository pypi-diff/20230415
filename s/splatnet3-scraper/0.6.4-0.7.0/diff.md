# Comparing `tmp/splatnet3_scraper-0.6.4.tar.gz` & `tmp/splatnet3_scraper-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splatnet3_scraper-0.6.4.tar", max compression
+gzip compressed data, was "splatnet3_scraper-0.7.0.tar", max compression
```

## Comparing `splatnet3_scraper-0.6.4.tar` & `splatnet3_scraper-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0    35589 2023-01-11 07:14:21.667377 splatnet3_scraper-0.6.4/LICENSE.md
--rw-r--r--   0        0        0     1993 2023-02-27 00:31:39.823067 splatnet3_scraper-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     9500 2023-02-16 00:17:30.590888 splatnet3_scraper-0.6.4/README.md
--rw-r--r--   0        0        0       23 2023-02-27 00:31:54.216295 splatnet3_scraper-0.6.4/splatnet3_scraper/__init__.py
--rw-r--r--   0        0        0      277 2023-02-25 10:45:49.839281 splatnet3_scraper-0.6.4/splatnet3_scraper/auth/__init__.py
--rw-r--r--   0        0        0     3155 2023-02-25 22:37:52.880032 splatnet3_scraper-0.6.4/splatnet3_scraper/auth/environment_manager.py
--rw-r--r--   0        0        0      303 2023-02-09 09:30:18.879542 splatnet3_scraper-0.6.4/splatnet3_scraper/auth/exceptions.py
--rw-r--r--   0        0        0    11363 2023-02-16 00:11:26.830374 splatnet3_scraper-0.6.4/splatnet3_scraper/auth/graph_ql_queries.py
--rw-r--r--   0        0        0    42234 2023-02-25 10:45:49.840782 splatnet3_scraper-0.6.4/splatnet3_scraper/auth/nso.py
--rw-r--r--   0        0        0    29610 2023-02-25 10:45:49.841282 splatnet3_scraper-0.6.4/splatnet3_scraper/auth/token_manager.py
--rw-r--r--   0        0        0     1694 2023-01-17 07:37:01.919314 splatnet3_scraper-0.6.4/splatnet3_scraper/constants.py
--rw-r--r--   0        0        0      310 2023-01-17 07:37:01.919812 splatnet3_scraper-0.6.4/splatnet3_scraper/logs.py
--rw-r--r--   0        0        0      230 2023-02-25 10:45:49.841784 splatnet3_scraper-0.6.4/splatnet3_scraper/query/__init__.py
--rw-r--r--   0        0        0    13670 2023-02-25 22:39:39.527531 splatnet3_scraper-0.6.4/splatnet3_scraper/query/config.py
--rw-r--r--   0        0        0    17188 2023-02-16 00:13:22.867522 splatnet3_scraper-0.6.4/splatnet3_scraper/query/handler.py
--rw-r--r--   0        0        0    17473 2023-02-11 00:22:16.781110 splatnet3_scraper-0.6.4/splatnet3_scraper/query/json_parser.py
--rw-r--r--   0        0        0    12269 2023-02-27 00:34:15.660840 splatnet3_scraper-0.6.4/splatnet3_scraper/query/responses.py
--rw-r--r--   0        0        0      119 2023-02-10 04:48:43.127896 splatnet3_scraper-0.6.4/splatnet3_scraper/scraper/__init__.py
--rw-r--r--   0        0        0     9643 2023-02-25 23:05:21.497763 splatnet3_scraper-0.6.4/splatnet3_scraper/scraper/main.py
--rw-r--r--   0        0        0     6324 2023-02-09 09:30:18.884042 splatnet3_scraper-0.6.4/splatnet3_scraper/scraper/query_map.py
--rw-r--r--   0        0        0     6265 2023-02-09 09:30:18.884544 splatnet3_scraper-0.6.4/splatnet3_scraper/utils.py
--rw-r--r--   0        0        0    10492 1970-01-01 00:00:00.000000 splatnet3_scraper-0.6.4/setup.py
--rw-r--r--   0        0        0    10251 1970-01-01 00:00:00.000000 splatnet3_scraper-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0    34915 2023-04-10 05:10:54.759478 splatnet3_scraper-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0    10973 2023-04-10 22:54:23.894487 splatnet3_scraper-0.7.0/README.md
+-rw-r--r--   0        0        0     1916 2023-04-14 04:46:36.743579 splatnet3_scraper-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-04-14 04:46:46.613580 splatnet3_scraper-0.7.0/splatnet3_scraper/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.0/splatnet3_scraper/auth/__init__.py
+-rw-r--r--   0        0        0     3064 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.0/splatnet3_scraper/auth/environment_manager.py
+-rw-r--r--   0        0        0      287 2023-04-10 05:10:54.769478 splatnet3_scraper-0.7.0/splatnet3_scraper/auth/exceptions.py
+-rw-r--r--   0        0        0    10032 2023-04-14 05:52:38.572350 splatnet3_scraper-0.7.0/splatnet3_scraper/auth/graph_ql_queries.py
+-rw-r--r--   0        0        0    41667 2023-04-14 06:45:42.584859 splatnet3_scraper-0.7.0/splatnet3_scraper/auth/nso.py
+-rw-r--r--   0        0        0    28908 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.0/splatnet3_scraper/auth/token_manager.py
+-rw-r--r--   0        0        0     7847 2023-04-14 05:14:08.034820 splatnet3_scraper-0.7.0/splatnet3_scraper/constants.py
+-rw-r--r--   0        0        0      226 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.0/splatnet3_scraper/query/__init__.py
+-rw-r--r--   0        0        0    13307 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.0/splatnet3_scraper/query/config.py
+-rw-r--r--   0        0        0    16840 2023-04-10 05:10:54.769478 splatnet3_scraper-0.7.0/splatnet3_scraper/query/handler.py
+-rw-r--r--   0        0        0    16980 2023-04-10 05:10:54.769478 splatnet3_scraper-0.7.0/splatnet3_scraper/query/json_parser.py
+-rw-r--r--   0        0        0    16777 2023-04-14 00:28:50.154178 splatnet3_scraper-0.7.0/splatnet3_scraper/query/responses.py
+-rw-r--r--   0        0        0      117 2023-04-10 05:10:54.769478 splatnet3_scraper-0.7.0/splatnet3_scraper/scraper/__init__.py
+-rw-r--r--   0        0        0     9382 2023-04-10 05:20:16.704543 splatnet3_scraper-0.7.0/splatnet3_scraper/scraper/main.py
+-rw-r--r--   0        0        0     6182 2023-04-14 04:47:23.115079 splatnet3_scraper-0.7.0/splatnet3_scraper/scraper/query_map.py
+-rw-r--r--   0        0        0    17067 2023-04-14 06:44:33.232112 splatnet3_scraper-0.7.0/splatnet3_scraper/utils.py
+-rw-r--r--   0        0        0    12145 1970-01-01 00:00:00.000000 splatnet3_scraper-0.7.0/setup.py
+-rw-r--r--   0        0        0    11871 1970-01-01 00:00:00.000000 splatnet3_scraper-0.7.0/PKG-INFO
```

### Comparing `splatnet3_scraper-0.6.4/LICENSE.md` & `splatnet3_scraper-0.7.0/LICENSE.md`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,675 +1,675 @@
-### GNU GENERAL PUBLIC LICENSE
-
-Version 3, 29 June 2007
-
-Copyright (C) 2007 Free Software Foundation, Inc.
-<https://fsf.org/>
-
-Everyone is permitted to copy and distribute verbatim copies of this
-license document, but changing it is not allowed.
-
-### Preamble
-
-The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works. By contrast,
-the GNU General Public License is intended to guarantee your freedom
-to share and change all versions of a program--to make sure it remains
-free software for all its users. We, the Free Software Foundation, use
-the GNU General Public License for most of our software; it applies
-also to any other work released this way by its authors. You can apply
-it to your programs, too.
-
-When we speak of free software, we are referring to freedom, not
-price. Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights. Therefore, you
-have certain responsibilities if you distribute copies of the
-software, or if you modify it: responsibilities to respect the freedom
-of others.
-
-For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received. You must make sure that they, too, receive
-or can get the source code. And you must show them these terms so they
-know their rights.
-
-Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software. For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the
-manufacturer can do so. This is fundamentally incompatible with the
-aim of protecting users' freedom to change the software. The
-systematic pattern of such abuse occurs in the area of products for
-individuals to use, which is precisely where it is most unacceptable.
-Therefore, we have designed this version of the GPL to prohibit the
-practice for those products. If such problems arise substantially in
-other domains, we stand ready to extend this provision to those
-domains in future versions of the GPL, as needed to protect the
-freedom of users.
-
-Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish
-to avoid the special danger that patents applied to a free program
-could make it effectively proprietary. To prevent this, the GPL
-assures that patents cannot be used to render the program non-free.
-
-The precise terms and conditions for copying, distribution and
-modification follow.
-
-### TERMS AND CONDITIONS
-
-#### 0. Definitions.
-
-"This License" refers to version 3 of the GNU General Public License.
-
-"Copyright" also means copyright-like laws that apply to other kinds
-of works, such as semiconductor masks.
-
-"The Program" refers to any copyrightable work licensed under this
-License. Each licensee is addressed as "you". "Licensees" and
-"recipients" may be individuals or organizations.
-
-To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of
-an exact copy. The resulting work is called a "modified version" of
-the earlier work or a work "based on" the earlier work.
-
-A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy. Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies. Mere interaction with a user
-through a computer network, with no transfer of a copy, is not
-conveying.
-
-An interactive user interface displays "Appropriate Legal Notices" to
-the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License. If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-#### 1. Source Code.
-
-The "source code" for a work means the preferred form of the work for
-making modifications to it. "Object code" means any non-source form of
-a work.
-
-A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form. A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities. However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work. For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-The Corresponding Source need not include anything that users can
-regenerate automatically from other parts of the Corresponding Source.
-
-The Corresponding Source for a work in source code form is that same
-work.
-
-#### 2. Basic Permissions.
-
-All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met. This License explicitly affirms your unlimited
-permission to run the unmodified Program. The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work. This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-You may make, run and propagate covered works that you do not convey,
-without conditions so long as your license otherwise remains in force.
-You may convey covered works to others for the sole purpose of having
-them make modifications exclusively for you, or provide you with
-facilities for running those works, provided that you comply with the
-terms of this License in conveying all material for which you do not
-control copyright. Those thus making or running the covered works for
-you must do so exclusively on your behalf, under your direction and
-control, on terms that prohibit them from making any copies of your
-copyrighted material outside their relationship with you.
-
-Conveying under any other circumstances is permitted solely under the
-conditions stated below. Sublicensing is not allowed; section 10 makes
-it unnecessary.
-
-#### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such
-circumvention is effected by exercising rights under this License with
-respect to the covered work, and you disclaim any intention to limit
-operation or modification of the work as a means of enforcing, against
-the work's users, your or third parties' legal rights to forbid
-circumvention of technological measures.
-
-#### 4. Conveying Verbatim Copies.
-
-You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-#### 5. Conveying Modified Source Versions.
-
-You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these
-conditions:
-
--   a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
--   b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under
-    section 7. This requirement modifies the requirement in section 4
-    to "keep intact all notices".
--   c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy. This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged. This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
--   d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit. Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-#### 6. Conveying Non-Source Forms.
-
-You may convey a covered work in object code form under the terms of
-sections 4 and 5, provided that you also convey the machine-readable
-Corresponding Source under the terms of this License, in one of these
-ways:
-
--   a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
--   b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the Corresponding
-    Source from a network server at no charge.
--   c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source. This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
--   d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge. You need not require recipients to copy the
-    Corresponding Source along with the object code. If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source. Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
--   e) Convey the object code using peer-to-peer transmission,
-    provided you inform other peers where the object code and
-    Corresponding Source of the work are being offered to the general
-    public at no charge under subsection 6d.
-
-A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal,
-family, or household purposes, or (2) anything designed or sold for
-incorporation into a dwelling. In determining whether a product is a
-consumer product, doubtful cases shall be resolved in favor of
-coverage. For a particular product received by a particular user,
-"normally used" refers to a typical or common use of that class of
-product, regardless of the status of the particular user or of the way
-in which the particular user actually uses, or expects or is expected
-to use, the product. A product is a consumer product regardless of
-whether the product has substantial commercial, industrial or
-non-consumer uses, unless such uses represent the only significant
-mode of use of the product.
-
-"Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to
-install and execute modified versions of a covered work in that User
-Product from a modified version of its Corresponding Source. The
-information must suffice to ensure that the continued functioning of
-the modified object code is in no case prevented or interfered with
-solely because modification has been made.
-
-If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information. But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or
-updates for a work that has been modified or installed by the
-recipient, or for the User Product in which it has been modified or
-installed. Access to a network may be denied when the modification
-itself materially and adversely affects the operation of the network
-or violates the rules and protocols for communication across the
-network.
-
-Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-#### 7. Additional Terms.
-
-"Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law. If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it. (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.) You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders
-of that material) supplement the terms of this License with terms:
-
--   a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
--   b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
--   c) Prohibiting misrepresentation of the origin of that material,
-    or requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
--   d) Limiting the use for publicity purposes of names of licensors
-    or authors of the material; or
--   e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
--   f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions
-    of it) with contractual assumptions of liability to the recipient,
-    for any liability that these contractual assumptions directly
-    impose on those licensors and authors.
-
-All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10. If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term. If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions; the
-above requirements apply either way.
-
-#### 8. Termination.
-
-You may not propagate or modify a covered work except as expressly
-provided under this License. Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-However, if you cease all violation of this License, then your license
-from a particular copyright holder is reinstated (a) provisionally,
-unless and until the copyright holder explicitly and finally
-terminates your license, and (b) permanently, if the copyright holder
-fails to notify you of the violation by some reasonable means prior to
-60 days after the cessation.
-
-Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License. If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-#### 9. Acceptance Not Required for Having Copies.
-
-You are not required to accept this License in order to receive or run
-a copy of the Program. Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance. However,
-nothing other than this License grants you permission to propagate or
-modify any covered work. These actions infringe copyright if you do
-not accept this License. Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-#### 10. Automatic Licensing of Downstream Recipients.
-
-Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License. You are not responsible
-for enforcing compliance by third parties with this License.
-
-An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations. If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License. For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-#### 11. Patents.
-
-A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based. The
-work thus licensed is called the contributor's "contributor version".
-
-A contributor's "essential patent claims" are all patent claims owned
-or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version. For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement). To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients. "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-A patent license is "discriminatory" if it does not include within the
-scope of its coverage, prohibits the exercise of, or is conditioned on
-the non-exercise of one or more of the rights that are specifically
-granted under this License. You may not convey a covered work if you
-are a party to an arrangement with a third party that is in the
-business of distributing software, under which you make payment to the
-third party based on the extent of your activity of conveying the
-work, and under which the third party grants, to any of the parties
-who would receive the covered work from you, a discriminatory patent
-license (a) in connection with copies of the covered work conveyed by
-you (or copies made from those copies), or (b) primarily for and in
-connection with specific products or compilations that contain the
-covered work, unless you entered into that arrangement, or that patent
-license was granted, prior to 28 March 2007.
-
-Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-#### 12. No Surrender of Others' Freedom.
-
-If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License. If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under
-this License and any other pertinent obligations, then as a
-consequence you may not convey it at all. For example, if you agree to
-terms that obligate you to collect a royalty for further conveying
-from those to whom you convey the Program, the only way you could
-satisfy both those terms and this License would be to refrain entirely
-from conveying the Program.
-
-#### 13. Use with the GNU Affero General Public License.
-
-Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work. The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-#### 14. Revised Versions of this License.
-
-The Free Software Foundation may publish revised and/or new versions
-of the GNU General Public License from time to time. Such new versions
-will be similar in spirit to the present version, but may differ in
-detail to address new problems or concerns.
-
-Each version is given a distinguishing version number. If the Program
-specifies that a certain numbered version of the GNU General Public
-License "or any later version" applies to it, you have the option of
-following the terms and conditions either of that numbered version or
-of any later version published by the Free Software Foundation. If the
-Program does not specify a version number of the GNU General Public
-License, you may choose any version ever published by the Free
-Software Foundation.
-
-If the Program specifies that a proxy can decide which future versions
-of the GNU General Public License can be used, that proxy's public
-statement of acceptance of a version permanently authorizes you to
-choose that version for the Program.
-
-Later license versions may give you additional or different
-permissions. However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-#### 15. Disclaimer of Warranty.
-
-THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
-WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
-LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
-A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
-PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
-DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
-CORRECTION.
-
-#### 16. Limitation of Liability.
-
-IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
-CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
-INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
-ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
-NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
-LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
-TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
-PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
-
-#### 17. Interpretation of Sections 15 and 16.
-
-If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-END OF TERMS AND CONDITIONS
-
-### How to Apply These Terms to Your New Programs
-
-If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these
-terms.
-
-To do so, attach the following notices to the program. It is safest to
-attach them to the start of each source file to most effectively state
-the exclusion of warranty; and each file should have at least the
-"copyright" line and a pointer to where the full notice is found.
-
-        <one line to give the program's name and a brief idea of what it does.>
-        Copyright (C) <year>  <name of author>
-
-        This program is free software: you can redistribute it and/or modify
-        it under the terms of the GNU General Public License as published by
-        the Free Software Foundation, either version 3 of the License, or
-        (at your option) any later version.
-
-        This program is distributed in the hope that it will be useful,
-        but WITHOUT ANY WARRANTY; without even the implied warranty of
-        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-        GNU General Public License for more details.
-
-        You should have received a copy of the GNU General Public License
-        along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper
-mail.
-
-If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-        <program>  Copyright (C) <year>  <name of author>
-        This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-        This is free software, and you are welcome to redistribute it
-        under certain conditions; type `show c' for details.
-
-The hypothetical commands \`show w' and \`show c' should show the
-appropriate parts of the General Public License. Of course, your
-program's commands might be different; for a GUI interface, you would
-use an "about box".
-
-You should also get your employer (if you work as a programmer) or
-school, if any, to sign a "copyright disclaimer" for the program, if
-necessary. For more information on this, and how to apply and follow
-the GNU GPL, see <https://www.gnu.org/licenses/>.
-
-The GNU General Public License does not permit incorporating your
-program into proprietary programs. If your program is a subroutine
-library, you may consider it more useful to permit linking proprietary
-applications with the library. If this is what you want to do, use the
-GNU Lesser General Public License instead of this License. But first,
+### GNU GENERAL PUBLIC LICENSE
+
+Version 3, 29 June 2007
+
+Copyright (C) 2007 Free Software Foundation, Inc.
+<https://fsf.org/>
+
+Everyone is permitted to copy and distribute verbatim copies of this
+license document, but changing it is not allowed.
+
+### Preamble
+
+The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works. By contrast,
+the GNU General Public License is intended to guarantee your freedom
+to share and change all versions of a program--to make sure it remains
+free software for all its users. We, the Free Software Foundation, use
+the GNU General Public License for most of our software; it applies
+also to any other work released this way by its authors. You can apply
+it to your programs, too.
+
+When we speak of free software, we are referring to freedom, not
+price. Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights. Therefore, you
+have certain responsibilities if you distribute copies of the
+software, or if you modify it: responsibilities to respect the freedom
+of others.
+
+For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received. You must make sure that they, too, receive
+or can get the source code. And you must show them these terms so they
+know their rights.
+
+Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software. For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the
+manufacturer can do so. This is fundamentally incompatible with the
+aim of protecting users' freedom to change the software. The
+systematic pattern of such abuse occurs in the area of products for
+individuals to use, which is precisely where it is most unacceptable.
+Therefore, we have designed this version of the GPL to prohibit the
+practice for those products. If such problems arise substantially in
+other domains, we stand ready to extend this provision to those
+domains in future versions of the GPL, as needed to protect the
+freedom of users.
+
+Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish
+to avoid the special danger that patents applied to a free program
+could make it effectively proprietary. To prevent this, the GPL
+assures that patents cannot be used to render the program non-free.
+
+The precise terms and conditions for copying, distribution and
+modification follow.
+
+### TERMS AND CONDITIONS
+
+#### 0. Definitions.
+
+"This License" refers to version 3 of the GNU General Public License.
+
+"Copyright" also means copyright-like laws that apply to other kinds
+of works, such as semiconductor masks.
+
+"The Program" refers to any copyrightable work licensed under this
+License. Each licensee is addressed as "you". "Licensees" and
+"recipients" may be individuals or organizations.
+
+To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of
+an exact copy. The resulting work is called a "modified version" of
+the earlier work or a work "based on" the earlier work.
+
+A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy. Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies. Mere interaction with a user
+through a computer network, with no transfer of a copy, is not
+conveying.
+
+An interactive user interface displays "Appropriate Legal Notices" to
+the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License. If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+#### 1. Source Code.
+
+The "source code" for a work means the preferred form of the work for
+making modifications to it. "Object code" means any non-source form of
+a work.
+
+A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form. A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities. However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work. For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+The Corresponding Source need not include anything that users can
+regenerate automatically from other parts of the Corresponding Source.
+
+The Corresponding Source for a work in source code form is that same
+work.
+
+#### 2. Basic Permissions.
+
+All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met. This License explicitly affirms your unlimited
+permission to run the unmodified Program. The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work. This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+You may make, run and propagate covered works that you do not convey,
+without conditions so long as your license otherwise remains in force.
+You may convey covered works to others for the sole purpose of having
+them make modifications exclusively for you, or provide you with
+facilities for running those works, provided that you comply with the
+terms of this License in conveying all material for which you do not
+control copyright. Those thus making or running the covered works for
+you must do so exclusively on your behalf, under your direction and
+control, on terms that prohibit them from making any copies of your
+copyrighted material outside their relationship with you.
+
+Conveying under any other circumstances is permitted solely under the
+conditions stated below. Sublicensing is not allowed; section 10 makes
+it unnecessary.
+
+#### 3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such
+circumvention is effected by exercising rights under this License with
+respect to the covered work, and you disclaim any intention to limit
+operation or modification of the work as a means of enforcing, against
+the work's users, your or third parties' legal rights to forbid
+circumvention of technological measures.
+
+#### 4. Conveying Verbatim Copies.
+
+You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+#### 5. Conveying Modified Source Versions.
+
+You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these
+conditions:
+
+-   a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+-   b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under
+    section 7. This requirement modifies the requirement in section 4
+    to "keep intact all notices".
+-   c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy. This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged. This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+-   d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit. Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+#### 6. Conveying Non-Source Forms.
+
+You may convey a covered work in object code form under the terms of
+sections 4 and 5, provided that you also convey the machine-readable
+Corresponding Source under the terms of this License, in one of these
+ways:
+
+-   a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+-   b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the Corresponding
+    Source from a network server at no charge.
+-   c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source. This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+-   d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge. You need not require recipients to copy the
+    Corresponding Source along with the object code. If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source. Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+-   e) Convey the object code using peer-to-peer transmission,
+    provided you inform other peers where the object code and
+    Corresponding Source of the work are being offered to the general
+    public at no charge under subsection 6d.
+
+A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal,
+family, or household purposes, or (2) anything designed or sold for
+incorporation into a dwelling. In determining whether a product is a
+consumer product, doubtful cases shall be resolved in favor of
+coverage. For a particular product received by a particular user,
+"normally used" refers to a typical or common use of that class of
+product, regardless of the status of the particular user or of the way
+in which the particular user actually uses, or expects or is expected
+to use, the product. A product is a consumer product regardless of
+whether the product has substantial commercial, industrial or
+non-consumer uses, unless such uses represent the only significant
+mode of use of the product.
+
+"Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to
+install and execute modified versions of a covered work in that User
+Product from a modified version of its Corresponding Source. The
+information must suffice to ensure that the continued functioning of
+the modified object code is in no case prevented or interfered with
+solely because modification has been made.
+
+If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information. But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or
+updates for a work that has been modified or installed by the
+recipient, or for the User Product in which it has been modified or
+installed. Access to a network may be denied when the modification
+itself materially and adversely affects the operation of the network
+or violates the rules and protocols for communication across the
+network.
+
+Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+#### 7. Additional Terms.
+
+"Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law. If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it. (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.) You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders
+of that material) supplement the terms of this License with terms:
+
+-   a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+-   b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+-   c) Prohibiting misrepresentation of the origin of that material,
+    or requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+-   d) Limiting the use for publicity purposes of names of licensors
+    or authors of the material; or
+-   e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+-   f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions
+    of it) with contractual assumptions of liability to the recipient,
+    for any liability that these contractual assumptions directly
+    impose on those licensors and authors.
+
+All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10. If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term. If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions; the
+above requirements apply either way.
+
+#### 8. Termination.
+
+You may not propagate or modify a covered work except as expressly
+provided under this License. Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+However, if you cease all violation of this License, then your license
+from a particular copyright holder is reinstated (a) provisionally,
+unless and until the copyright holder explicitly and finally
+terminates your license, and (b) permanently, if the copyright holder
+fails to notify you of the violation by some reasonable means prior to
+60 days after the cessation.
+
+Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License. If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+#### 9. Acceptance Not Required for Having Copies.
+
+You are not required to accept this License in order to receive or run
+a copy of the Program. Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance. However,
+nothing other than this License grants you permission to propagate or
+modify any covered work. These actions infringe copyright if you do
+not accept this License. Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+#### 10. Automatic Licensing of Downstream Recipients.
+
+Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License. You are not responsible
+for enforcing compliance by third parties with this License.
+
+An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations. If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License. For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+#### 11. Patents.
+
+A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based. The
+work thus licensed is called the contributor's "contributor version".
+
+A contributor's "essential patent claims" are all patent claims owned
+or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version. For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement). To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients. "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+A patent license is "discriminatory" if it does not include within the
+scope of its coverage, prohibits the exercise of, or is conditioned on
+the non-exercise of one or more of the rights that are specifically
+granted under this License. You may not convey a covered work if you
+are a party to an arrangement with a third party that is in the
+business of distributing software, under which you make payment to the
+third party based on the extent of your activity of conveying the
+work, and under which the third party grants, to any of the parties
+who would receive the covered work from you, a discriminatory patent
+license (a) in connection with copies of the covered work conveyed by
+you (or copies made from those copies), or (b) primarily for and in
+connection with specific products or compilations that contain the
+covered work, unless you entered into that arrangement, or that patent
+license was granted, prior to 28 March 2007.
+
+Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+#### 12. No Surrender of Others' Freedom.
+
+If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License. If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under
+this License and any other pertinent obligations, then as a
+consequence you may not convey it at all. For example, if you agree to
+terms that obligate you to collect a royalty for further conveying
+from those to whom you convey the Program, the only way you could
+satisfy both those terms and this License would be to refrain entirely
+from conveying the Program.
+
+#### 13. Use with the GNU Affero General Public License.
+
+Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work. The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+#### 14. Revised Versions of this License.
+
+The Free Software Foundation may publish revised and/or new versions
+of the GNU General Public License from time to time. Such new versions
+will be similar in spirit to the present version, but may differ in
+detail to address new problems or concerns.
+
+Each version is given a distinguishing version number. If the Program
+specifies that a certain numbered version of the GNU General Public
+License "or any later version" applies to it, you have the option of
+following the terms and conditions either of that numbered version or
+of any later version published by the Free Software Foundation. If the
+Program does not specify a version number of the GNU General Public
+License, you may choose any version ever published by the Free
+Software Foundation.
+
+If the Program specifies that a proxy can decide which future versions
+of the GNU General Public License can be used, that proxy's public
+statement of acceptance of a version permanently authorizes you to
+choose that version for the Program.
+
+Later license versions may give you additional or different
+permissions. However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+#### 15. Disclaimer of Warranty.
+
+THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT
+WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT
+LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR
+A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND
+PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE
+DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR
+CORRECTION.
+
+#### 16. Limitation of Liability.
+
+IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR
+CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES,
+INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES
+ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT
+NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR
+LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM
+TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER
+PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
+
+#### 17. Interpretation of Sections 15 and 16.
+
+If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+END OF TERMS AND CONDITIONS
+
+### How to Apply These Terms to Your New Programs
+
+If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these
+terms.
+
+To do so, attach the following notices to the program. It is safest to
+attach them to the start of each source file to most effectively state
+the exclusion of warranty; and each file should have at least the
+"copyright" line and a pointer to where the full notice is found.
+
+        <one line to give the program's name and a brief idea of what it does.>
+        Copyright (C) <year>  <name of author>
+
+        This program is free software: you can redistribute it and/or modify
+        it under the terms of the GNU General Public License as published by
+        the Free Software Foundation, either version 3 of the License, or
+        (at your option) any later version.
+
+        This program is distributed in the hope that it will be useful,
+        but WITHOUT ANY WARRANTY; without even the implied warranty of
+        MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+        GNU General Public License for more details.
+
+        You should have received a copy of the GNU General Public License
+        along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper
+mail.
+
+If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+        <program>  Copyright (C) <year>  <name of author>
+        This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+        This is free software, and you are welcome to redistribute it
+        under certain conditions; type `show c' for details.
+
+The hypothetical commands \`show w' and \`show c' should show the
+appropriate parts of the General Public License. Of course, your
+program's commands might be different; for a GUI interface, you would
+use an "about box".
+
+You should also get your employer (if you work as a programmer) or
+school, if any, to sign a "copyright disclaimer" for the program, if
+necessary. For more information on this, and how to apply and follow
+the GNU GPL, see <https://www.gnu.org/licenses/>.
+
+The GNU General Public License does not permit incorporating your
+program into proprietary programs. If your program is a subroutine
+library, you may consider it more useful to permit linking proprietary
+applications with the library. If this is what you want to do, use the
+GNU Lesser General Public License instead of this License. But first,
 please read <https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `splatnet3_scraper-0.6.4/pyproject.toml` & `splatnet3_scraper-0.7.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,78 +1,78 @@
-[tool.poetry]
-name = "splatnet3_scraper"
-version = "0.6.4"
-description = "Scraper for SplatNet 3 for Splatoon 3"
-authors = ["Cesar E Garza <cesar@cegarza.com>"]
-readme = "README.md"
-packages = [{include = "splatnet3_scraper"}]
-license = "GPL-3.0-or-later"
-
-[tool.poetry.dependencies]
-python = "^3.10"
-requests = "^2.28.1"
-pyarrow = {version = "^10.0.1", optional = true, extras = ["parquet"]}
-pandas = {version = "^1.5.3", optional = true, extras = ["examples"]}
-sqlalchemy = {version = "^2.0.1", optional = true, extras = ["examples"]}
-psycopg2 = {version = "^2.9.5", optional = true, extras = ["examples"]}
-
-[tool.poetry.extras]
-parquet = ["pyarrow"]
-examples = ["pandas", "sqlalchemy", "psycopg2"]
-all = ["parquet", "examples"]
-
-[tool.poetry.group.dev.dependencies]
-black = "^22.12.0"
-mypy = "^0.991"
-flake8 = "^6.0.0"
-darglint = "^1.8.1"
-isort = "^5.11.4"
-types-requests = "^2.28.11.7"
-pytest = "^7.2.0"
-coverage = "^7.0.4"
-ipykernel = "^6.19.4"
-genson = "^1.2.2"
-line-profiler = "^4.0.2"
-pytest-lazy-fixture = "^0.6.3"
-freezegun = "^1.2.2"
-pytest-mock = "^3.10.0"
-genbadge = {extras = ["all"], version = "^1.1.0"}
-pytest-html = "^3.2.0"
-sphinx = "^6.1.3"
-ipython = "^8.9.0"
-
-
-
-[tool.poetry.group.docs.dependencies]
-sphinx-immaterial = "^0.11.3"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-[tool.black]
-line-length = 80
-target-version = ['py310']
-
-[tool.isort]
-profile = "black"
-line_length = 80
-skip_glob = "^(tests|splatnet3_scraper)"
-
-[tool.mypy]
-python_version = "3.10"
-ignore_missing_imports = true
-pretty = true
-exclude = [".venv", "tests", "docs", "examples"]
-
-[tool.pytest.ini_options]
-testpaths = "tests"
-addopts = [
-    "-v",
-    "--tb=auto",
-    "--showlocals",
-    "--color=yes",
-]
-markers = [
-    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
-    "internet: marks tests as requiring internet access (deselect with '-m \"not internet\"')",
+[tool.poetry]
+name = "splatnet3_scraper"
+version = "0.7.0"
+description = "Scraper for SplatNet 3 for Splatoon 3"
+authors = ["Cesar E Garza <cesar@cegarza.com>"]
+readme = "README.md"
+packages = [{include = "splatnet3_scraper"}]
+license = "GPL-3.0-or-later"
+
+[tool.poetry.dependencies]
+python = "^3.10"
+requests = "^2.28.1"
+pyarrow = {version = "^10.0.1", optional = true, extras = ["parquet"]}
+pandas = {version = "^1.5.3", optional = true, extras = ["examples"]}
+sqlalchemy = {version = "^2.0.1", optional = true, extras = ["examples"]}
+psycopg2 = {version = "^2.9.5", optional = true, extras = ["examples"]}
+
+[tool.poetry.extras]
+parquet = ["pyarrow"]
+examples = ["pandas", "sqlalchemy", "psycopg2"]
+all = ["parquet", "examples"]
+
+[tool.poetry.group.dev.dependencies]
+black = "^22.12.0"
+mypy = "^0.991"
+flake8 = "^6.0.0"
+darglint = "^1.8.1"
+isort = "^5.11.4"
+types-requests = "^2.28.11.7"
+pytest = "^7.2.0"
+coverage = "^7.0.4"
+ipykernel = "^6.19.4"
+genson = "^1.2.2"
+line-profiler = "^4.0.2"
+pytest-lazy-fixture = "^0.6.3"
+freezegun = "^1.2.2"
+pytest-mock = "^3.10.0"
+genbadge = {extras = ["all"], version = "^1.1.0"}
+pytest-html = "^3.2.0"
+sphinx = "^6.1.3"
+ipython = "^8.9.0"
+
+
+
+[tool.poetry.group.docs.dependencies]
+sphinx-immaterial = "^0.11.3"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 80
+target-version = ['py310']
+
+[tool.isort]
+profile = "black"
+line_length = 80
+skip_glob = "^(tests|splatnet3_scraper)"
+
+[tool.mypy]
+python_version = "3.10"
+ignore_missing_imports = true
+pretty = true
+exclude = [".venv", "tests", "docs", "examples"]
+
+[tool.pytest.ini_options]
+testpaths = "tests"
+addopts = [
+    "-v",
+    "--tb=auto",
+    "--showlocals",
+    "--color=yes",
+]
+markers = [
+    "slow: marks tests as slow (deselect with '-m \"not slow\"')",
+    "internet: marks tests as requiring internet access (deselect with '-m \"not internet\"')",
 ]
```

### Comparing `splatnet3_scraper-0.6.4/README.md` & `splatnet3_scraper-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,147 +1,180 @@
-# SplatNet 3 Scraper
-
-[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.
-
-**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.
-
-## Features
-
-* Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.
-* The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.
-* The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.
-* The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.
-* Compatibility with the configuration file format used by `s3s`.
-* Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:
-  * JSON
-  * gzip-compressed JSON
-  * csv
-  * parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)
-* Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).
-
-## Installation
-
-**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:
-
-```bash
-pip install splatnet3_scraper
-```
-
-Note that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.
-
-## Usage
-
-There are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can't find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.
-
-### Using the `scraper` module
-
-The `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.
-
-This module is currently under active development and is not yet complete. Please check back later for more functions.
-
-### Using the `query` module
-
-The `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.
-
-The `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.
-
-#### Instantiating the `QueryHandler` class by providing a session token
-
-```python
-from splatnet3_scraper.query import QueryHandler
-handler = QueryHandler.from_session_token("session_token")
-handler.query("StageScheduleQuery")
-```
-
-#### Instantiating the `QueryHandler` class by providing the path to a configuration file
-
-```python
-from splatnet3_scraper.query import QueryHandler
-handler = QueryHandler.from_config_file(".splatnet3_scraper")
-handler.query("StageScheduleQuery")
-```
-
-#### Instantiating the `QueryHandler` class by loading environment variables
-
-The following environment variables are supported:
-
-* `SN3S_SESSION_TOKEN`
-* `SN3S_GTOKEN`
-* `SN3S_BULLET_TOKEN`
-
-```python
-from splatnet3_scrape.query import QueryHandler
-handler = QueryHandler.from_env()
-handler.query("StageScheduleQuery")
-```
-
-#### Querying the SplatNet 3 API
-
-The `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:
-
-```python
-from splatnet3_scraper.query import QueryHandler
-handler = QueryHandler.from_env()
-response = handler.query("StageScheduleQuery")
-print(response["xSchedules", "nodes", 0, "vsRule", "name"])
-```
-
-#### Saving and loading responses
-
-The `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:
-
-* JSON
-* gzip-compressed JSON
-* csv
-* parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)
-
-Note: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.
-
-The following code will save the response data to a file named `response.json` in the current directory:
-
-```python
-from splatnet3_scraper.query import QueryHandler
-handler = QueryHandler.from_env()
-response = handler.query("StageScheduleQuery")
-response.parsed_json().to_json("response.json")
-```
-
-Additionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:
-
-```python
-from splatnet3_scraper.query import JSONParser
-parser = JSONParser.from_json("response.json")
-```
-
-## Symbols
-
-| Symbol | Meaning |
-| ------ | ------- |
-| :white_check_mark: | Implemented |
-| :construction: | In progress |
-| :world_map: | Planned |
-| :x: | Not planned |
-
-## Roadmap
-
-| Feature | Status |
-| ------- | ------ |
-| Support for the SplatNet 3 API | :white_check_mark: |
-| Full support for the SplatNet 3 API | :world_map: |
-| Support for the SplatNet 2 API | :x: |
-| Obtaining session tokens | :white_check_mark: |
-| Full documentation | :construction: |
-| Full unit test coverage | :white_check_mark: |
-| Columnar data format support | :construction: |
-| CLI interface | :x: |
-| Integration with stat.ink | :x: |
-| PyPI package | :white_check_mark: |
-| Docker image | :world_map: |
-| Executable binary | :x: |
-
-## Docker Note
-
-This project currently uses the standard library heavily, and as such it is not compatible with the `python:alpine` Docker image. I have no plans to change this. Use the `python:slim` image instead.
-
-QueryHandler is licensed under the GPLv3. See the LICENSE file for more details.
+# SplatNet 3 Scraper
+
+[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.
+
+**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.
+
+## Table of Contents
+
+1. [Features](#features)
+2. [Documentation](#documentation)
+3. [Installation](#installation)
+4. [Usage](#usage)
+   - [Using the `scraper` module](#using-the-scraper-module)
+   - [Using the `query` module](#using-the-query-module)
+   - [Using the `auth` module](#using-the-auth-module)
+5. [Roadmap](#roadmap)
+6. [Contributing](#contributing)
+7. [License](#license)
+
+## Features
+
+- Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.
+- The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.
+- The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.
+- The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.
+- Compatibility with the configuration file format used by `s3s`.
+- Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:
+  - JSON
+  - gzip-compressed JSON
+  - csv
+  - parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)
+- Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).
+
+## Documentation
+
+Detailed documentation for SplatNet 3 Scraper, including usage instructions, examples, and API reference, is available on Read the Docs:
+
+[**SplatNet 3 Scraper Documentation**](https://splatnet3-scraper.readthedocs.io/en/latest/index.html)
+
+We highly recommend referring to the documentation to get the most out of SplatNet 3 Scraper and understand its full capabilities.
+
+## Installation
+
+**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:
+
+```bash
+pip install splatnet3_scraper
+```
+
+Note that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.
+
+## Usage
+
+There are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can't find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.
+
+### Using the `scraper` module
+
+The `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.
+
+This module is currently under active development and is not yet complete. Please check back later for more functions.
+
+### Using the `query` module
+
+The `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.
+
+The `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.
+
+### Using the `auth` module
+
+:warning: **Warning: The `auth` module is intended for advanced users only. Most users should use the `scraper` or `query` modules for a simpler and more convenient experience.**
+
+The `auth` module provides a low-level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication and is designed for advanced developers who need full control over the authentication process.
+
+To use the `auth` module, you will need to import the necessary components and handle the authentication flow manually. Please refer to the [documentation](https://splatnet3-scraper.readthedocs.io/en/latest/index.html) for detailed instructions and examples on how to use the `auth` module.
+
+#### Instantiating the `QueryHandler` class by providing a session token
+
+```python
+from splatnet3_scraper.query import QueryHandler
+handler = QueryHandler.from_session_token("session_token")
+handler.query("StageScheduleQuery")
+```
+
+#### Instantiating the `QueryHandler` class by providing the path to a configuration file
+
+```python
+from splatnet3_scraper.query import QueryHandler
+handler = QueryHandler.from_config_file(".splatnet3_scraper")
+handler.query("StageScheduleQuery")
+```
+
+#### Instantiating the `QueryHandler` class by loading environment variables
+
+The following environment variables are supported:
+
+- `SN3S_SESSION_TOKEN`
+- `SN3S_GTOKEN`
+- `SN3S_BULLET_TOKEN`
+
+```python
+from splatnet3_scrape.query import QueryHandler
+handler = QueryHandler.from_env()
+handler.query("StageScheduleQuery")
+```
+
+#### Querying the SplatNet 3 API
+
+The `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:
+
+```python
+from splatnet3_scraper.query import QueryHandler
+handler = QueryHandler.from_env()
+response = handler.query("StageScheduleQuery")
+print(response["xSchedules", "nodes", 0, "vsRule", "name"])
+```
+
+#### Saving and loading responses
+
+The `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:
+
+- JSON
+- gzip-compressed JSON
+- csv
+- parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)
+
+Note: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.
+
+The following code will save the response data to a file named `response.json` in the current directory:
+
+```python
+from splatnet3_scraper.query import QueryHandler
+handler = QueryHandler.from_env()
+response = handler.query("StageScheduleQuery")
+response.parsed_json().to_json("response.json")
+```
+
+Additionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:
+
+```python
+from splatnet3_scraper.query import JSONParser
+parser = JSONParser.from_json("response.json")
+```
+
+## Symbols
+
+| Symbol | Meaning |
+| ------ | ------- |
+| :white_check_mark: | Implemented |
+| :construction: | In progress |
+| :world_map: | Planned |
+| :x: | Not planned |
+
+## Roadmap
+
+| Feature | Status |
+| ------- | ------ |
+| Support for the SplatNet 3 API | :white_check_mark: |
+| Full support for the SplatNet 3 API | :world_map: |
+| Support for the SplatNet 2 API | :x: |
+| Obtaining session tokens | :white_check_mark: |
+| Full documentation | :construction: |
+| Full unit test coverage | :white_check_mark: |
+| Columnar data format support | :construction: |
+| CLI interface | :x: |
+| Integration with stat.ink | :x: |
+| PyPI package | :white_check_mark: |
+| Docker image | :world_map: |
+| Executable binary | :x: |
+
+## Contributing
+
+We welcome contributions to SplatNet 3 Scraper! For detailed information on how to contribute, please refer to our [CONTRIBUTING.md](./CONTRIBUTING.md) file.
+
+To report issues or request new features, please open an issue on the GitHub repository.
+
+## License
+
+SplatNet 3 Scraper is licensed under the GPLv3. See the [LICENSE](./LICENSE) file for more details.
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/auth/environment_manager.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/auth/environment_manager.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,91 @@
-import os
-
-from splatnet3_scraper.constants import ENV_VAR_NAMES, TOKENS
-
-
-class EnvironmentVariablesManager:
-    """Manages environment variables for the scraper.
-
-    This class is used to manage the environment variables in an easy way. Any
-    environment variable calls should be done through this class, it will handle
-    obtaining the environment variables, allow additional environment variables
-    to be added and defined, and will also handle the base environment variables
-    that are required for this package to work.
-    """
-
-    BASE_TOKENS = [TOKENS.SESSION_TOKEN, TOKENS.GTOKEN, TOKENS.BULLET_TOKEN]
-
-    def __init__(self) -> None:
-        """Initializes the class and sets up the base environment variables."""
-        self.variable_names = {}
-        for token in self.BASE_TOKENS:
-            self.variable_names[token] = ENV_VAR_NAMES[token]
-
-    def token_to_variable(self, token: str) -> str:
-        """Given the token name, returns the environment variable name.
-
-        Args:
-            token (str): The token name.
-
-        Returns:
-            str: The environment variable name.
-        """
-        return self.variable_names[token]
-
-    def variable_to_token(self, variable: str) -> str:
-        """Given the environment variable name, returns the token name.
-
-        Args:
-            variable (str): The environment variable name.
-
-        Raises:
-            KeyError: If the variable is not defined.
-
-        Returns:
-            str: The token name.
-        """
-        for token, variable_name in self.variable_names.items():
-            if variable_name == variable:
-                return token
-        raise KeyError(f"Variable {variable} is not defined.")
-
-    def add_token(self, token_name: str, variable_name: str) -> None:
-        """Adds a new token to the environment variables.
-
-        Args:
-            token_name (str): The token name.
-            variable_name (str): The environment variable name.
-        """
-        self.variable_names[token_name] = variable_name
-
-    def remove_token(self, token_name: str) -> None:
-        """Removes a token from the environment variables.
-
-        Args:
-            token_name (str): The token name.
-
-        Raises:
-            ValueError: If the token is a base token.
-        """
-        if token_name in self.BASE_TOKENS:
-            raise ValueError(f"Cannot remove base token {token_name}.")
-        del self.variable_names[token_name]
-
-    def get(self, token: str) -> str | None:
-        """Gets the environment variable for the given token.
-
-        Args:
-            token (str): The token to get the environment variable for.
-
-        Returns:
-            str | None: The environment variable, or None if it is not set.
-        """
-        return os.environ.get(self.token_to_variable(token))
-
-    def get_all(self) -> dict[str, str | None]:
-        """Gets all the environment variables.
-
-        Returns:
-            dict[str, str]: The environment variables.
-        """
-        return {token: self.get(token) for token in self.variable_names.keys()}
+import os
+
+from splatnet3_scraper.constants import ENV_VAR_NAMES, TOKENS
+
+
+class EnvironmentVariablesManager:
+    """Manages environment variables for the scraper.
+
+    This class is used to manage the environment variables in an easy way. Any
+    environment variable calls should be done through this class, it will handle
+    obtaining the environment variables, allow additional environment variables
+    to be added and defined, and will also handle the base environment variables
+    that are required for this package to work.
+    """
+
+    BASE_TOKENS = [TOKENS.SESSION_TOKEN, TOKENS.GTOKEN, TOKENS.BULLET_TOKEN]
+
+    def __init__(self) -> None:
+        """Initializes the class and sets up the base environment variables."""
+        self.variable_names = {}
+        for token in self.BASE_TOKENS:
+            self.variable_names[token] = ENV_VAR_NAMES[token]
+
+    def token_to_variable(self, token: str) -> str:
+        """Given the token name, returns the environment variable name.
+
+        Args:
+            token (str): The token name.
+
+        Returns:
+            str: The environment variable name.
+        """
+        return self.variable_names[token]
+
+    def variable_to_token(self, variable: str) -> str:
+        """Given the environment variable name, returns the token name.
+
+        Args:
+            variable (str): The environment variable name.
+
+        Raises:
+            KeyError: If the variable is not defined.
+
+        Returns:
+            str: The token name.
+        """
+        for token, variable_name in self.variable_names.items():
+            if variable_name == variable:
+                return token
+        raise KeyError(f"Variable {variable} is not defined.")
+
+    def add_token(self, token_name: str, variable_name: str) -> None:
+        """Adds a new token to the environment variables.
+
+        Args:
+            token_name (str): The token name.
+            variable_name (str): The environment variable name.
+        """
+        self.variable_names[token_name] = variable_name
+
+    def remove_token(self, token_name: str) -> None:
+        """Removes a token from the environment variables.
+
+        Args:
+            token_name (str): The token name.
+
+        Raises:
+            ValueError: If the token is a base token.
+        """
+        if token_name in self.BASE_TOKENS:
+            raise ValueError(f"Cannot remove base token {token_name}.")
+        del self.variable_names[token_name]
+
+    def get(self, token: str) -> str | None:
+        """Gets the environment variable for the given token.
+
+        Args:
+            token (str): The token to get the environment variable for.
+
+        Returns:
+            str | None: The environment variable, or None if it is not set.
+        """
+        return os.environ.get(self.token_to_variable(token))
+
+    def get_all(self) -> dict[str, str | None]:
+        """Gets all the environment variables.
+
+        Returns:
+            dict[str, str]: The environment variables.
+        """
+        return {token: self.get(token) for token in self.variable_names.keys()}
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/auth/graph_ql_queries.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/auth/graph_ql_queries.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,288 +1,266 @@
-from __future__ import annotations
-
-import json
-from typing import Any
-
-import requests
-
-from splatnet3_scraper.constants import (
-    DEFAULT_USER_AGENT,
-    GRAPH_QL_REFERENCE_URL,
-    GRAPHQL_URL,
-    SPLATNET_URL,
-)
-from splatnet3_scraper.utils import get_splatnet_web_version
-
-
-class GraphQLQueries:
-    """The GraphQLQueries class that contains the GraphQL queries used by
-    ``splatnet3_scraper``. The Nintendo Switch Online API only allows persistent
-    queries, so making queries requires using the hashes for said queries. The
-    great folks over at `imink` have a GitHub Actions workflow that checks for
-    and updates the hashes for the queries every five minutes. The hashes are
-    stored in a JSON file that is hosted on GitHub. This class automatically
-    downloads the JSON file and stores the hashes in a dictionary. The hashes
-    are then used to make queries to the Nintendo Switch Online API and can be
-    accessed using their string names.
-    """
-
-    def __init__(self) -> None:
-        """Initializes the GraphQLQueries class. Initializes a requests.Session
-        and stores it in the session attribute. Also gets the hashes for the
-        GraphQL queries and stores them in the hash_map attribute. The hashes
-        are stored in a dictionary where the keys are the names of the queries
-        and the values are the hashes.
-        """
-        self.session = requests.Session()
-        self.hash_map = self.get_hashes()
-
-    def get_hashes(self) -> dict[str, str]:
-        """Gets the hashes for the GraphQL queries.
-
-        Uses requests to get the `imink` GraphQL query hash map JSON file and
-        parses it to get the hashes for the queries. The initial request
-        response contains two keys: ``hash_map`` and ``version``. The
-        ``hash_map`` key is the dictionary that contains the hashes for the
-        queries and is what is returned by this method. The `version` key is the
-        version of the hashes and is used to check if the hashes are up to date,
-        it is used elsewhere in this package, but is not used here.
-
-        Returns:
-            dict[str, str]: The hashes for the GraphQL queries. The keys are
-                the names of the queries and the values are the most up to date
-                hashes for the queries.
-        """
-        response = self.session.get(GRAPH_QL_REFERENCE_URL)
-        hash_map = response.json()["graphql"]["hash_map"]
-        return hash_map
-
-    def get_query(self, query_name: str) -> str:
-        """Gets a GraphQL query hash given the name of the query.
-
-        Uses the hash_map attribute to get the hash for the query, which is
-        then returned. For more information on the valid queries, see the
-        ``queries`` page of the documentation.
-
-        Args:
-            query_name (str): The name of the query.
-
-        Returns:
-            str: The GraphQL query hash.
-        """
-        return self.hash_map[query_name]
-
-    def query_header(
-        self,
-        bullet_token: str,
-        language: str,
-        user_agent: str | None = None,
-        override: dict[str, str] = {},
-    ) -> dict[str, str]:
-        """Generates the headers that are used for the GraphQL queries made for
-        the SplatNet 3 API.
-
-        The headers are generated using the bullet token, language and user
-        agent. Any headers that are passed in the override parameter will
-        override the default headers. An example of the headers that are
-        generated is shown below.
-
-        >>> headers = {
-        ...     "Authorization": f"Bearer {bullet_token}",
-        ...     "Accept-Language": language,
-        ...     "User-Agent": user_agent,
-        ...     "X-Web-View-Ver": web_version,
-        ...     "Content-Type": "application/json",
-        ...     "Accept": "*/*",
-        ...     "Origin": SPLATNET_URL,
-        ...     "X-Requested-With": "com.nintendo.znca",
-        ...     "Referer": (
-        ...         f"{SPLATNET_URL}?"
-        ...         f"lang={language}"
-        ...         f"&na_country={language[-2:]}"
-        ...         f"&na_lang={language}"
-        ...     ),
-        ...     "Accept-Encoding": "gzip, deflate",
-        ... }
-
-        Args:
-            bullet_token (str): The bullet token.
-            language (str): The language code to use, for example, "en-US".
-            user_agent (str | None): The user agent to use. If None, the default
-                user agent will be used. Defaults to None.
-            override (dict[str, str]): Any headers that should override the
-                default headers. Defaults to {}.
-
-        Returns:
-            dict[str, str]: The headers for the GraphQL queries.
-        """
-
-        if user_agent is None:
-            user_agent = DEFAULT_USER_AGENT
-
-        headers = {
-            "Authorization": f"Bearer {bullet_token}",
-            "Accept-Language": language,
-            "User-Agent": user_agent,
-            "X-Web-View-Ver": get_splatnet_web_version(),
-            "Content-Type": "application/json",
-            "Accept": "*/*",
-            "Origin": SPLATNET_URL,
-            "X-Requested-With": "com.nintendo.znca",
-            "Referer": (
-                f"{SPLATNET_URL}?"
-                f"lang={language}"
-                f"&na_country={language[-2:]}"
-                f"&na_lang={language}"
-            ),
-            "Accept-Encoding": "gzip, deflate",
-        }
-        headers.update(override)
-        return headers
-
-    def query_body_hash(
-        self, query_hash: str | bytes, variables: dict[str, Any] = {}
-    ) -> str:
-        """Generates the body for the GraphQL queries, as a string.
-
-        The body is generated using the query hash and the variables that are
-        passed in. The body is a JSON string that contains the query hash and
-        the variables. An example of the body that is generated is shown
-        below.
-
-        >>> body = {
-        ...     "extensions": {
-        ...         "persistedQuery": {
-        ...             "sha256Hash": query_hash,
-        ...             "version": 1,
-        ...         }
-        ...     },
-        ...     "variables": variables,
-        ... }
-
-        Args:
-            query_hash (str | bytes): The hash of the query.
-            variables (dict[str, Any]): The variables to pass to the query. If
-                the query does not take any variables, this can be an empty
-                dictionary. Defaults to {}.
-
-        Returns:
-            str: The body for the GraphQL queries, as a string.
-        """
-        out = {
-            "extensions": {
-                "persistedQuery": {
-                    "sha256Hash": query_hash,
-                    "version": 1,
-                }
-            },
-            "variables": variables,
-        }
-        return json.dumps(out)
-
-    def query_body(
-        self, query_name: str, variables: dict[str, str] = {}
-    ) -> str:
-        """Generates the body for the GraphQL queries, as a string.
-
-        This method is a wrapper around the ``query_body_hash`` method. It gets
-        the query hash using the ``get_query`` method and then calls the
-        ``query_body_hash`` method to generate the body. For more information on
-        the valid queries, see the `queries` page of the documentation.
-
-        Args:
-            query_name (str): The name of the query.
-            variables (dict[str, str]): The variables to pass to the query. If
-                the query does not take any variables, this can be an empty
-                dictionary. Defaults to {}.
-
-        Returns:
-            str: The body for the GraphQL queries, as a string.
-        """
-        query = self.get_query(query_name)
-        return self.query_body_hash(query, variables)
-
-    def query_hash(
-        self,
-        query_hash: str | bytes,
-        bullet_token: str,
-        gtoken: str,
-        language: str,
-        user_agent: str | None = None,
-        variables: dict[str, Any] = {},
-        override: dict[str, Any] = {},
-    ) -> requests.Response:
-        """Makes a GraphQL query using the persisted query hash. This method
-        generates the headers and body for the query and then makes the
-        request. For more information on the valid queries, see the `queries`
-        page of the documentation.
-
-        Args:
-            query_hash (str | bytes): The hash of the query.
-            bullet_token (str): The bullet token.
-            gtoken (str): The gtoken.
-            language (str): The language code to use.
-            user_agent (str | None): The user agent to use. If None, the default
-                user agent will be used. Defaults to None.
-            variables (dict[str, Any]): The variables to pass to the query. If
-                the query does not take any variables, this can be an empty
-                dictionary. Defaults to an empty dictionary.
-            override (dict[str, Any]): Any headers that should override the
-                default headers. Defaults to an empty dictionary.
-
-        Returns:
-            requests.Response: The response from the GraphQL query.
-        """
-        header = self.query_header(bullet_token, language, user_agent, override)
-        body = self.query_body_hash(query_hash, variables)
-        cookies = {
-            "_gtoken": gtoken,
-        }
-        return self.session.post(
-            GRAPHQL_URL, headers=header, data=body, cookies=cookies
-        )
-
-    def query(
-        self,
-        query_name: str,
-        bullet_token: str,
-        gtoken: str,
-        language: str,
-        user_agent: str | None = None,
-        variables: dict[str, Any] = {},
-        override: dict[str, Any] = {},
-    ) -> requests.Response:
-        """Makes a GraphQL query. This method is a wrapper around the
-        ``query_hash`` method. It gets the query hash using the ``get_query``
-        method and then calls the ``query_hash`` method to make the request. For
-        more information on the valid queries, see the `queries` page of the
-        documentation.
-
-        Args:
-            query_name (str): The name of the query.
-            bullet_token (str): The bullet token.
-            gtoken (str): The gtoken.
-            language (str): The language code to use.
-            user_agent (str | None): The user agent to use. If None, the default
-                user agent will be used. Defaults to None.
-            variables (dict[str, Any]): The variables to pass to the query. If
-                the query does not take any variables, this can be an empty
-                dictionary. Defaults to an empty dictionary.
-            override (dict[str, Any]): Any headers that should override the
-                default headers. Defaults to an empty dictionary.
-
-        Returns:
-            requests.Response: The response from the GraphQL query.
-        """
-        query = self.get_query(query_name)
-        return self.query_hash(
-            query,
-            bullet_token,
-            gtoken,
-            language,
-            user_agent,
-            variables,
-            override,
-        )
-
-
-queries = GraphQLQueries()
+from __future__ import annotations
+
+import json
+from typing import Any
+
+import requests
+
+from splatnet3_scraper.constants import (
+    DEFAULT_USER_AGENT,
+    GRAPHQL_URL,
+    SPLATNET_URL,
+)
+from splatnet3_scraper.utils import get_splatnet_hashes, get_splatnet_version
+
+
+class GraphQLQueries:
+    """The GraphQLQueries class that contains the GraphQL queries used by
+    ``splatnet3_scraper``. The Nintendo Switch Online API only allows persistent
+    queries, so making queries requires using the hashes for said queries. The
+    great folks over at `imink` have a GitHub Actions workflow that checks for
+    and updates the hashes for the queries every five minutes. The hashes are
+    stored in a JSON file that is hosted on GitHub. This class automatically
+    downloads the JSON file and stores the hashes in a dictionary. The hashes
+    are then used to make queries to the Nintendo Switch Online API and can be
+    accessed using their string names.
+    """
+
+    def __init__(self) -> None:
+        """Initializes the GraphQLQueries class. Initializes a requests.Session
+        and stores it in the session attribute. Also gets the hashes for the
+        GraphQL queries and stores them in the hash_map attribute. The hashes
+        are stored in a dictionary where the keys are the names of the queries
+        and the values are the hashes.
+        """
+        self.session = requests.Session()
+
+    def get_query(self, query_name: str) -> str:
+        """Gets a GraphQL query hash given the name of the query.
+
+        Uses the hash_map attribute to get the hash for the query, which is
+        then returned. For more information on the valid queries, see the
+        ``queries`` page of the documentation.
+
+        Args:
+            query_name (str): The name of the query.
+
+        Returns:
+            str: The GraphQL query hash.
+        """
+        return get_splatnet_hashes()[query_name]
+
+    def query_header(
+        self,
+        bullet_token: str,
+        language: str,
+        user_agent: str | None = None,
+        override: dict[str, str] = {},
+    ) -> dict[str, str]:
+        """Generates the headers that are used for the GraphQL queries made for
+        the SplatNet 3 API.
+
+        The headers are generated using the bullet token, language and user
+        agent. Any headers that are passed in the override parameter will
+        override the default headers. An example of the headers that are
+        generated is shown below.
+
+        >>> headers = {
+        ...     "Authorization": f"Bearer {bullet_token}",
+        ...     "Accept-Language": language,
+        ...     "User-Agent": user_agent,
+        ...     "X-Web-View-Ver": web_version,
+        ...     "Content-Type": "application/json",
+        ...     "Accept": "*/*",
+        ...     "Origin": SPLATNET_URL,
+        ...     "X-Requested-With": "com.nintendo.znca",
+        ...     "Referer": (
+        ...         f"{SPLATNET_URL}?"
+        ...         f"lang={language}"
+        ...         f"&na_country={language[-2:]}"
+        ...         f"&na_lang={language}"
+        ...     ),
+        ...     "Accept-Encoding": "gzip, deflate",
+        ... }
+
+        Args:
+            bullet_token (str): The bullet token.
+            language (str): The language code to use, for example, "en-US".
+            user_agent (str | None): The user agent to use. If None, the default
+                user agent will be used. Defaults to None.
+            override (dict[str, str]): Any headers that should override the
+                default headers. Defaults to {}.
+
+        Returns:
+            dict[str, str]: The headers for the GraphQL queries.
+        """
+
+        if user_agent is None:
+            user_agent = DEFAULT_USER_AGENT
+
+        headers = {
+            "Authorization": f"Bearer {bullet_token}",
+            "Accept-Language": language,
+            "User-Agent": user_agent,
+            "X-Web-View-Ver": get_splatnet_version(),
+            "Content-Type": "application/json",
+            "Accept": "*/*",
+            "Origin": SPLATNET_URL,
+            "X-Requested-With": "com.nintendo.znca",
+            "Referer": (
+                f"{SPLATNET_URL}?"
+                f"lang={language}"
+                f"&na_country={language[-2:]}"
+                f"&na_lang={language}"
+            ),
+            "Accept-Encoding": "gzip, deflate",
+        }
+        headers.update(override)
+        return headers
+
+    def query_body_hash(
+        self, query_hash: str | bytes, variables: dict[str, Any] = {}
+    ) -> str:
+        """Generates the body for the GraphQL queries, as a string.
+
+        The body is generated using the query hash and the variables that are
+        passed in. The body is a JSON string that contains the query hash and
+        the variables. An example of the body that is generated is shown
+        below.
+
+        >>> body = {
+        ...     "extensions": {
+        ...         "persistedQuery": {
+        ...             "sha256Hash": query_hash,
+        ...             "version": 1,
+        ...         }
+        ...     },
+        ...     "variables": variables,
+        ... }
+
+        Args:
+            query_hash (str | bytes): The hash of the query.
+            variables (dict[str, Any]): The variables to pass to the query. If
+                the query does not take any variables, this can be an empty
+                dictionary. Defaults to {}.
+
+        Returns:
+            str: The body for the GraphQL queries, as a string.
+        """
+        out = {
+            "extensions": {
+                "persistedQuery": {
+                    "sha256Hash": query_hash,
+                    "version": 1,
+                }
+            },
+            "variables": variables,
+        }
+        return json.dumps(out)
+
+    def query_body(
+        self, query_name: str, variables: dict[str, str] = {}
+    ) -> str:
+        """Generates the body for the GraphQL queries, as a string.
+
+        This method is a wrapper around the ``query_body_hash`` method. It gets
+        the query hash using the ``get_query`` method and then calls the
+        ``query_body_hash`` method to generate the body. For more information on
+        the valid queries, see the `queries` page of the documentation.
+
+        Args:
+            query_name (str): The name of the query.
+            variables (dict[str, str]): The variables to pass to the query. If
+                the query does not take any variables, this can be an empty
+                dictionary. Defaults to {}.
+
+        Returns:
+            str: The body for the GraphQL queries, as a string.
+        """
+        query = self.get_query(query_name)
+        return self.query_body_hash(query, variables)
+
+    def query_hash(
+        self,
+        query_hash: str | bytes,
+        bullet_token: str,
+        gtoken: str,
+        language: str,
+        user_agent: str | None = None,
+        variables: dict[str, Any] = {},
+        override: dict[str, Any] = {},
+    ) -> requests.Response:
+        """Makes a GraphQL query using the persisted query hash. This method
+        generates the headers and body for the query and then makes the
+        request. For more information on the valid queries, see the `queries`
+        page of the documentation.
+
+        Args:
+            query_hash (str | bytes): The hash of the query.
+            bullet_token (str): The bullet token.
+            gtoken (str): The gtoken.
+            language (str): The language code to use.
+            user_agent (str | None): The user agent to use. If None, the default
+                user agent will be used. Defaults to None.
+            variables (dict[str, Any]): The variables to pass to the query. If
+                the query does not take any variables, this can be an empty
+                dictionary. Defaults to an empty dictionary.
+            override (dict[str, Any]): Any headers that should override the
+                default headers. Defaults to an empty dictionary.
+
+        Returns:
+            requests.Response: The response from the GraphQL query.
+        """
+        header = self.query_header(bullet_token, language, user_agent, override)
+        body = self.query_body_hash(query_hash, variables)
+        cookies = {
+            "_gtoken": gtoken,
+        }
+        return self.session.post(
+            GRAPHQL_URL, headers=header, data=body, cookies=cookies
+        )
+
+    def query(
+        self,
+        query_name: str,
+        bullet_token: str,
+        gtoken: str,
+        language: str,
+        user_agent: str | None = None,
+        variables: dict[str, Any] = {},
+        override: dict[str, Any] = {},
+    ) -> requests.Response:
+        """Makes a GraphQL query. This method is a wrapper around the
+        ``query_hash`` method. It gets the query hash using the ``get_query``
+        method and then calls the ``query_hash`` method to make the request. For
+        more information on the valid queries, see the `queries` page of the
+        documentation.
+
+        Args:
+            query_name (str): The name of the query.
+            bullet_token (str): The bullet token.
+            gtoken (str): The gtoken.
+            language (str): The language code to use.
+            user_agent (str | None): The user agent to use. If None, the default
+                user agent will be used. Defaults to None.
+            variables (dict[str, Any]): The variables to pass to the query. If
+                the query does not take any variables, this can be an empty
+                dictionary. Defaults to an empty dictionary.
+            override (dict[str, Any]): Any headers that should override the
+                default headers. Defaults to an empty dictionary.
+
+        Returns:
+            requests.Response: The response from the GraphQL query.
+        """
+        query = self.get_query(query_name)
+        return self.query_hash(
+            query,
+            bullet_token,
+            gtoken,
+            language,
+            user_agent,
+            variables,
+            override,
+        )
+
+
+queries = GraphQLQueries()
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/auth/nso.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/auth/nso.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,924 +1,933 @@
-import base64
-import hashlib
-import json
-import os
-import re
-from typing import Callable, Literal, TypeAlias, cast
-
-import requests
-
-from splatnet3_scraper import __version__
-from splatnet3_scraper.auth.exceptions import (
-    FTokenException,
-    NintendoException,
-    SplatNetException,
-)
-from splatnet3_scraper.constants import (
-    APP_VERSION_FALLBACK,
-    DEFAULT_USER_AGENT,
-    IMINK_URL,
-    IOS_APP_URL,
-    SPLATNET_URL,
-    WEB_VIEW_VERSION_FALLBACK,
-)
-from splatnet3_scraper.logs import logger
-from splatnet3_scraper.utils import get_splatnet_web_version, retry
-
-version_re = re.compile(
-    r"(?<=whats\-new\_\_latest\_\_version\"\>Version)\s+\d+\.\d+\.\d+"
-)
-
-FToken_Gen: TypeAlias = Callable[
-    [str, str, Literal[1] | Literal[2]], tuple[str, str, str]
-]
-
-
-class NSO:
-    """The NSO class contains all the logic to proceed through the login flow.
-    This class also holds various properties that are used to make requests to
-    the Nintendo Switch Online API. Login flow is roughly as follows, assuming
-    the user has never generated a session token before:
-
-        1.  Initialize a requests session and store it.
-        2.  Generate a random state and S256 code challenge that will be used
-            to obtain the "session_token". Store them for later use.
-        3.  Generate a login URL using the state and code challenge that the
-            user will open in their browser. The user will then copy a link and
-            feed it back to the program.
-        4.  Parse the URI to obtain the session token code, then use it
-            alongside the code challenge to obtain the ``session_token``. Store
-            it for later use. The session token is valid for 2 years and can be
-            revoked by the user.
-        5.  Use the session token to obtain a user access response from
-            Nintendo. This response will contain an ``id_token`` and a user
-            access token. Store both for later user.
-        6.  Use the user access token to obtain the user information. This is
-            required to obtain the first ``f_token``, for the Nintendo Switch
-            Online API. This is a message authentication code generated from the
-            timestamp and id token in an obscure manner and will be necessary
-            to generate the API access token.
-        7.  Use the Nintendo-obtained ``id_token`` to obtain the first
-            ``f_token``, for the Nintendo Switch Online API. The ``f_token``
-            will also return a timestamp and a request ID.
-        8.  Use the first ``f_token``, the request ID, the timestamp, the user
-            information, the ``id_token`` to obtain the
-            ``web_service_access_token``.
-        9.  Use the ``web_service_access_token`` to obtain the second
-            ``f_token``. This is a message authentication code generated from
-            the timestamp and id token in an obscure manner and will be
-            necessary to generate the ``gtoken``. This step is distinct from
-            step 7, make sure not to use the same ``f_token`` twice.
-        10. Use the second ``f_token``, the request ID, the timestamp, and the
-            ``web_service_access_token`` from step 9, and the id
-            ``4834290508791808`` to obtain the ``gtoken``.
-        11. Use the ``gtoken`` and user information to obtain a
-            ``bullet_token``. This token is valid for 2 hours.
-
-    Once the login flow is complete, the NSO class contains all the necessary
-    values to regenerate the tokens. To minimize the number of objects to track,
-    the NSO class only stores the tokens in memory. The TokenManager class
-    handles the persistence of the tokens to disk.
-    """
-
-    def __init__(self, session: requests.Session) -> None:
-        """Initializes the NSO class. The NSO class contains all the logic and
-        holds all the necessary values to proceed through the login flow.
-
-        The ``__init__`` method sets the following internal variables:
-
-            -   ``session``: The requests session object that is used to make
-                requests to the Nintendo Switch Online API. This is the only
-                variable that is passed in to the ``__init__`` method.
-            -   ``_state``: The internal state variable that is used to obtain
-                the session token. This is a random string that is generated
-                when the ``NSO.state`` property is first accessed, and is used
-                to generate the login URL.
-            -   ``_verifier``: The internal verifier variable that is used to
-                obtain the session token. This is a random string that is
-                generated when the ``NSO.verifier`` property is first accessed,
-                and is used to generate the login URL. The verifier is also
-                used to solve the code challenge, verifying to Nintendo that
-                the user is who they say they are.
-            -   ``_version``: The internal version variable that is used to
-                verify the NSO app version. This is a string that is generated
-                when the ``NSO.version`` property is first accessed, and is
-                used to obtain the session token.
-            -   ``_web_view_version``: The internal web view version variable
-                that is used to verify the NSO app version. This is a string
-                that is generated when the ``NSO.web_view_version`` property is
-                first accessed, and is used to obtain the session token.
-            -   ``_session_token``: A stored session token. This is required to
-                generate all other tokens and information. This is obtained
-                during the login flow and is valid for 2 years.
-            -   ``_user_access_token``: A stored user access token. This is a
-                token that is obtained during the login flow and is used to
-                obtain the user information.
-            -   ``_id_token``: A stored id token. This is a token that is
-                obtained during the login flow and is used to obtain the gtoken.
-            -   ``_gtoken``: A stored gtoken. This is a token that is obtained
-                during the login flow and is used to obtain the bullet token. It
-                is valid for 6 hours and 30 minutes.
-            -   ``_user_info``: A stored user information dictionary. This is
-                obtained during the login flow and is used to obtain the "f"
-                token.
-            -   ``_f_token_function``: A stored function that is used to obtain
-                the "f" token. This function is set to the ``get_ftoken``
-                method by default, and can be set with the
-                ``set_new_f_token_function`` method to use a user-defined
-                function if desired.
-
-
-        Args:
-            session (requests.Session): The NSO class uses a requests session
-                to make requests to the Nintendo Switch Online API. The session
-                object is passed in to the NSO class so that the same session
-                object can be used to make requests to the SplatNet API.
-        """
-        self.session = session
-        self._state: bytes | None = None
-        self._verifier: bytes | None = None
-        self._version: str | None = None
-        self._web_view_version: str | None = None
-        self._session_token: str | None = None
-        self._user_access_token: str | None = None
-        self._id_token: str | None = None
-        self._gtoken: str | None = None
-        self._user_info: dict[str, str] | None = None
-        self._f_token_function: FToken_Gen = self.get_ftoken
-
-    @staticmethod
-    def new_instance() -> "NSO":
-        """Creates a new instance of the NSO class with a new requests session.
-
-        This is the recommended way to create a new instance of the NSO class,
-        as it ensures that the session is a fresh session, however it is not
-        absolutely necessary to instantiate a new NSO class using this method.
-        Passing in a new session to the ``__init__`` method is perfectly fine.
-
-        Returns:
-            NSO: A new instance of the NSO class.
-        """
-        session = requests.Session()
-        return NSO(session=session)
-
-    @property
-    def version(self) -> str:
-        """Returns the current version of the NSO app. Necessary to get the
-        session token. If the version has not been obtained yet, it will be
-        obtained and stored. If the version cannot be obtained, a fallback
-        version will be used.
-
-        Returns:
-            str: The current version of the NSO app.
-        """
-        if self._version is None:
-            self._version = self.get_version()
-        return self._version
-
-    @retry(times=2, exceptions=ValueError)
-    def get_version(self) -> str:
-        """Fetches the current version of the Nintendo Switch Online app from
-        the iOS app store. This is necessary to access the API. This method
-        retries twice if the version cannot be obtained, in case the iOS App
-        Store site is down or slow. If the version cannot be obtained after
-        three attempts, a fallback version defined in the ``constants.py`` file
-        will be used.
-
-        Returns:
-            str: The current version of the NSO app.
-        """
-        # TODO: Replace the iOS app store method with a method that does not
-        # require scraping a website with scraping protection.
-        response = self.session.get(IOS_APP_URL)
-        version = version_re.search(response.text)
-        if version is None:
-            logger.log("Failed to get version from app store, using fallback")
-            return APP_VERSION_FALLBACK
-        return version.group(0).strip()
-
-    @property
-    def state(self) -> bytes:
-        """Returns a base64url encoded random 36 byte string for the auth state.
-        This is used to generate the login URL. To align with node.js's crypto
-        module, padding is removed. If the state has not been obtained yet, it
-        will be obtained and stored by creating a random 36 byte string and then
-        base64url encoding it.
-
-        Returns:
-            bytes: The auth state, without padding. This is used within the
-                login flow to verify that the user is who they say they are.
-        """
-        if self._state is None:
-            self._state = self.generate_new_state()
-        return self._state
-
-    def generate_new_state(self) -> bytes:
-        """Generates a new state.
-
-        Returns:
-            bytes: The auth state, without padding. A random 36 byte string
-                that is base64url encoded.
-        """
-        return base64.urlsafe_b64encode(os.urandom(36))
-
-    @property
-    def verifier(self) -> bytes:
-        """Returns a base64url encoded random 32 byte string for the code
-        verifier. This is used to generate the S256 code challenge. To align
-        with node.js's crypto module, padding is removed. If the verifier has
-        not been obtained yet, it will be obtained and stored by creating a
-        random 32 byte string and then base64url encoding it.
-
-        Returns:
-            bytes: The code verifier, without padding. This is used within the
-                login flow to verify that the user is who they say they are.
-        """
-        if self._verifier is None:
-            self._verifier = self.generate_new_verifier()
-        return self._verifier
-
-    def generate_new_verifier(self) -> bytes:
-        """Generates a new code verifier, which is a random 32 byte string
-        that is base64url encoded and with padding removed. This is used to
-        generate the S256 code challenge.
-
-        Returns:
-            bytes: The code verifier, without padding.
-        """
-        verifier_ = base64.urlsafe_b64encode(os.urandom(32))
-        return verifier_.replace(b"=", b"")
-
-    @property
-    def session_token(self) -> str:
-        """Returns the session token. This cannot be generated and must be set
-        by the user. If the session token has not been set, a ValueError will be
-        raised.
-
-        Raises:
-            ValueError: The session token has not been set.
-
-        Returns:
-            str: The session token.
-        """
-        if self._session_token is None:
-            raise ValueError("Session token is not set.")
-        return self._session_token
-
-    def generate_login_url(self, user_agent: str | None = None) -> str:
-        """Generates the login URL that can be used to obtain the session token.
-
-        This method will generate the login URL that is used to obtain the
-        session token. For full details on how to obtain a session token, see
-        the ``Obtaining a session token`` section of the documentation.
-
-        Args:
-            user_agent (str): The user agent to use. Defaults to the default
-                user agent found in ``constants.py``.
-
-        Returns:
-            str: The login URL that can be used to obtain the session token.
-        """
-        # https://dev.to/mathewthe2/intro-to-nintendo-switch-rest-api-2cm7
-        hash_ = hashlib.sha256()
-        hash_.update(self.verifier)
-        challenge = base64.urlsafe_b64encode(hash_.digest()).replace(b"=", b"")
-
-        header = {
-            "Host": "accounts.nintendo.com",
-            "Connection": "keep-alive",
-            "Cache-Control": "max-age=0",
-            "Upgrade-Insecure-Requests": "1",
-            "User-Agent": user_agent
-            if user_agent is not None
-            else DEFAULT_USER_AGENT,
-            "Accept": (
-                "text/html,"
-                + "application/xhtml+xml,"
-                + "application/xml;q=0.9,"
-                + "image/webp,"
-                + "image/apng,"
-                + "*/*;q=0.8n"
-            ),
-            "DNT": "1",
-            "Accept-Encoding": "gzip,deflate,br",
-        }
-        params = {
-            "state": self.state,
-            "redirect_uri": "npf71b963c1b7b6d119://auth",
-            "client_id": "71b963c1b7b6d119",
-            "scope": ("openid user user.birthday user.mii user.screenName"),
-            "response_type": "session_token_code",
-            "session_token_code_challenge": challenge,
-            "session_token_code_challenge_method": "S256",
-            "theme": "login_form",
-        }
-        login_url = "https://accounts.nintendo.com/connect/1.0.0/authorize"
-        response = self.session.get(
-            login_url, headers=header, params=params  # type: ignore
-        )
-        return response.url
-
-    def parse_npf_uri(self, uri: str) -> str:
-        """Parses the uri returned by the Nintendo login page and extracts the
-        session token code. This is used to pass the challenge and verify that
-        the user is who they say they are.
-
-        Args:
-            uri (str): The uri returned by the Nintendo login page.
-
-        Returns:
-            str: The session token code. This is *NOT* the session token, but is
-                used to obtain the session token.
-        """
-        return uri.split("&")[1][len("session_token_code=") :]
-
-    def get_session_token(self, session_token_code: str) -> str:
-        """Obtains the session token from the session token code.
-
-        This method will obtain the session token from the session token code.
-        It will use provide the session token code to Nintendo's servers
-        alongside the session token code verifier. Nintendo will then verify
-        that the user is who they say they are and return the session token.
-
-        Args:
-            session_token_code (str): The session token code. This is obtained
-                by parsing the uri obtained at the URL returned by
-                ``generate_login_url``.
-
-        Returns:
-            str: The session token. DO NOT SHARE THIS TOKEN WITH ANYONE.
-        """
-        header = {
-            "User-Agent": f"OnlineLounge/{self.version} NASDKAPI Android",
-            "Accept-Language": "en-US",
-            "Accept": "application/json",
-            "Content-Type": "application/x-www-form-urlencoded",
-            "Content-Length": "540",
-            "Host": "accounts.nintendo.com",
-            "Connection": "Keep-Alive",
-            "Accept-Encoding": "gzip",
-        }
-        params = {
-            "client_id": "71b963c1b7b6d119",
-            "session_token_code": session_token_code,
-            "session_token_code_verifier": self.verifier,
-        }
-        uri = "https://accounts.nintendo.com/connect/1.0.0/api/session_token"
-        response = self.session.post(uri, headers=header, data=params)
-        session_token = response.json()["session_token"]
-        self._session_token = session_token
-        return session_token
-
-    def get_user_access_token(self, session_token: str) -> dict:
-        """Obtains the user access token from the session token.
-
-        This method sends a request to Nintendo's servers containing the session
-        token to obtain the user access token and the ``id_token``. The user
-        access token is then used to obtain the user's data, while the
-        ``id_token`` is used to obtain the user's gtoken.
-
-        Args:
-            session_token (str): The session token.
-
-        Returns:
-            dict: The response from Nintendo's servers. This contains two keys
-                of interest: ``access_token`` and ``id_token``. The
-                ``access_token`` is used to obtain the user's data, while the
-                ``id_token`` is used to obtain the user's gtoken.
-        """
-        header = {
-            "Host": "accounts.nintendo.com",
-            "Accept-Encoding": "gzip",
-            "Content-Type": "application/json",
-            "Content-Length": "436",
-            "Accept": "application/json",
-            "Connection": "Keep-Alive",
-            "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 7.1.2)",
-        }
-        body = {
-            "client_id": "71b963c1b7b6d119",
-            "session_token": session_token,
-            "grant_type": (
-                "urn:ietf:params:oauth:grant-type:jwt-bearer-session-token"
-            ),
-        }
-        uri = "https://accounts.nintendo.com/connect/1.0.0/api/token"
-        return self.session.post(uri, headers=header, json=body).json()
-
-    def get_user_info(self, user_access_token: str) -> dict[str, str]:
-        """Obtains the user information from the user access token.
-
-        This method will obtain the user information from the user access token.
-        This includes the user's set language, country, and birthday, which are
-        used to obtain the user's ``gtoken``.
-
-        Args:
-            user_access_token (str): The user access token.
-
-        Returns:
-            dict[str, str]: The user information. This includes the user's set
-                language, country, and birthday.
-        """
-        # Get user information
-        url = "https://api.accounts.nintendo.com/2.0.0/users/me"
-        header = {
-            "User-Agent": "NASDKAPI; Android",
-            "Content-Type": "application/json",
-            "Accept": "application/json",
-            "Authorization": f"Bearer {user_access_token}",
-            "Host": "api.accounts.nintendo.com",
-            "Connection": "Keep-Alive",
-            "Accept-Encoding": "gzip",
-        }
-        response = self.session.get(url, headers=header)
-        return response.json()
-
-    def get_gtoken(
-        self, session_token: str, f_token_url: str | None = None
-    ) -> str:
-        """Obtains the ``gtoken`` from the session token.
-
-        The GameWebToken, or ``gtoken``, is used to authenticate requests to the
-        Nintendo Switch Online API. This method will obtain the ``gtoken`` from
-        the session token. The process of obtaining a ``gtoken`` is as follows:
-
-        1. Obtain the user access token and the ``id_token`` from the session
-                token.
-        2. Use the user access token to obtain the user's information.
-        3. Use the ``id_token`` and the user's information to obtain the first
-                ``f_token``, the request ID, and the timestamp.
-        4. Use the first ``f_token``, the request ID, the timestamp, and the
-                ``id_token`` to obtain the ``web_service_access_token``.
-        5. Use the ``web_service_access_token`` to obtain the second
-                ``f_token``, request ID, and timestamp.
-        6. Use the second ``f_token``, request ID, timestamp, and the
-                ``web_service_access_token`` to obtain the ``gtoken``.
-
-        By default, this method will use a third party's ``f_token`` generation
-        API to obtain the ``f_token``. The API used by default is provided by
-        `imink <https://github.com/imink-app>`_. If you do not trust this URL,
-        you can provide your own URL through the ``f_token_url`` argument, or
-        you can replace the ``f_token`` generation method used with your own
-        through the use of the ``set_new_f_token_function`` method. See the
-        documentation for that method for more information.
-
-        Args:
-            session_token (str): The session token.
-            f_token_url (str): The url to get the user access token from. This
-                defaults to the ftoken generation url provided by `imink`.
-
-        Raises:
-            NintendoException: In the case that the user's access token cannot
-                be obtained from the session token, or the user's information
-                that is returned is invalid.
-
-        Returns:
-            str: The gtoken. This is used to authenticate requests to the
-                Nintendo Switch Online API. This token is valid for 2 hours.
-        """
-        f_token_url = f_token_url if f_token_url is not None else IMINK_URL
-        # Get user access token
-        user_access_response = self.get_user_access_token(session_token)
-        try:
-            self._user_access_token = cast(
-                str, user_access_response["access_token"]
-            )
-            self._id_token = cast(str, user_access_response["id_token"])
-        except (KeyError, TypeError, AttributeError):
-            raise NintendoException(
-                "Failed to get user access token. "
-                + f"Response: {user_access_response}"
-            )
-
-        user_info = self.get_user_info(self._user_access_token)
-        self._user_info = user_info
-        web_service_access_token = self.g_token_generation_phase_1(
-            self._id_token, user_info, f_token_url
-        )
-        gtoken = self.g_token_generation_phase_2(
-            web_service_access_token, f_token_url
-        )
-        self._gtoken = gtoken
-        return gtoken
-
-    def set_new_f_token_function(
-        self, new_function: FToken_Gen | None = None
-    ) -> None:
-        """Sets the function used to generate the ``f_token``.
-
-        This method will set the function used to generate the ``f_token``. The
-        function must take the following arguments:
-
-        1. The ``f_token`` generation url.
-        2. The user's token, either the ``id_token`` for step ``1``, or the
-            ``web_service_access_token`` for step ``2``.
-        3. The step number (either ``1`` or ``2``)
-
-        The function must return a tuple containing the following:
-
-        1. The ``f_token``.
-        2. The request id.
-        3. The timestamp.
-
-        Args:
-            new_function (FToken_Gen): The new function to use to generate the
-                ftoken. This function must take the following arguments:
-
-                1. The ``f_token`` generation url.
-                2. The user's token, either the ``id_token`` for step ``1``, or
-                    the ``web_service_access_token`` for step ``2``.
-                3. The step number (either ``1`` or ``2``)
-
-                The function must return a tuple containing the following:
-
-                1. The ``f_token``.
-                2. The request id.
-                3. The timestamp.
-
-            If this argument is not provided or is ``None``, the default
-            ``f_token`` generation method will be restored.
-        """
-        if new_function is None:
-            self._f_token_function = self.get_ftoken
-        else:
-            self._f_token_function = new_function
-
-    def get_ftoken(
-        self, f_token_url: str, id_token: str, step: Literal[1] | Literal[2]
-    ) -> tuple[str, str, str]:
-        """Given the ``f_token_url``, ``id_token``, and ``step``, returns the
-        ``f_token``, ``request_id``, and ``timestamp`` from the response.
-
-        Note that this is a third party method, and is not officially
-        sanctioned by Nintendo. The default ftoken generation URL used by this
-        library is provided by `imink <https://github.com/imink-app>`_. In
-        the interest of transparency, the following is the entirety of the
-        request header sent to the ftoken generation URL:
-
-        >>> {
-        ...     "User-Agent": f"splatnet3_scraper/{__version__}",
-        ...     "Content-Type": "application/json; charset=utf-8",
-        ... }
-
-        The following is the entirety of the request body sent to the ftoken
-        generation URL:
-
-        >>> {
-        ...     "token": id_token,
-        ...     "hash_method": step,
-        ... }
-
-        As you can see, the only identifying information sent to the ftoken
-        generation URL is the user's ``id_token``, which cannot be used to
-        identify the user without the user's access token, which is not
-        provided to the ftoken generation URL.
-
-        Args:
-            f_token_url (str): URL to use for ``f_token`` generation. This
-                package provides a default URL, but you can provide your own.
-                The default URL is provided by `imink`.
-            id_token (str): ID token from user access token response. This is
-                obtained from the user access token response, and is used to
-                identify the user. This cannot be used to identify the user
-                without the user's access token, which is not provided to the
-                ftoken generation URL.
-            step (Literal[1] | Literal[2]): The step number. This is either
-                ``1`` or ``2``. This is used to identify the step in the
-                ``f_token`` generation process.
-
-        Raises:
-            FTokenException: In the case that the ftoken cannot be obtained
-                from the ftoken generation URL.
-
-        Returns:
-            str: The f token.
-            str: The request ID.
-            str: The timestamp.
-        """
-        header = {
-            "User-Agent": f"splatnet3_scraper/{__version__}",
-            "Content-Type": "application/json; charset=utf-8",
-        }
-        body = {
-            "token": id_token,
-            "hash_method": step,
-        }
-        bodystr = json.dumps(body)
-        response = self.session.post(f_token_url, headers=header, data=bodystr)
-        response_json = response.json()
-        try:
-            f_token = response_json["f"]
-            request_id = response_json["request_id"]
-            timestamp = response_json["timestamp"]
-        except (KeyError, TypeError, AttributeError):
-            raise FTokenException(
-                "Failed to get f token. " + f"Response: {response_json}"
-            )
-        return (f_token, request_id, timestamp)
-
-    @retry(times=1, exceptions=(FTokenException, NintendoException, KeyError))
-    def g_token_generation_phase_1(
-        self,
-        id_token: str,
-        user_info: dict[str, str],
-        f_token_url: str,
-    ) -> str:
-        """First phase of the ``gtoken`` generation process.
-
-        This is the first phase of the ``gtoken`` generation process. This is
-        abstracted away into a separate method to allow the request to be
-        retried once in the event of a failure. This phase involves two steps:
-        first, the ``id_token`` is sent to the ``f_token_url`` in a request to
-        obtain the ``f_token``, which is a ``HMAC`` necessary to obtain the
-        ``gtoken``. The response contains three values: the ``f_token``, the
-        ``request_id``, and the ``timestamp``. These values are then sent to
-        Nintendo's servers along with the  ``id_token`` to obtain the
-        ``gtoken``.
-
-        Args:
-            id_token (str): ID token from user access token response. This is
-                obtained from the user access token response, and is used to
-                identify the user to Nintendo's servers. However, this cannot
-                be used to identify the user by a third party by itself.
-            user_info (dict[str, str]): The dictionary of user info returned by
-                ``get_user_info``. This must contain the keys ``language``,
-                ``birthday``, and ``country``.
-            f_token_url (str): URL to use for f token generation. This package
-                provides a default URL, but you can provide your own. The
-                default URL is provided by `imink`.
-
-        Returns:
-            str: The Web Service Credential Access Token.
-        """
-        f_token, request_id, timestamp = self._f_token_function(
-            f_token_url, id_token, 1
-        )
-        return self.get_web_service_access_token(
-            id_token, user_info, f_token, request_id, timestamp
-        )
-
-    @retry(times=1, exceptions=(FTokenException, NintendoException, KeyError))
-    def g_token_generation_phase_2(
-        self,
-        web_service_access_token: str,
-        f_token_url: str,
-    ) -> str:
-        """Final phase of the ``gtoken`` generation process.
-
-        This is the second phase of the ``gtoken`` generation process. This is
-        abstracted away into a separate method to allow the request to be
-        retried once in the event of a failure. This phase involves two steps:
-        first, the ``web_service_access_token`` is sent to the ``f_token_url``
-        in a request to obtain the ``f_token``, which is a ``HMAC`` necessary to
-        obtain the ``gtoken``. The response contains three values: the
-        ``f_token``, the ``request_id``, and the ``timestamp``. These values are
-        then sent to Nintendo's servers along with the
-        ``web_service_access_token`` to obtain the ``gtoken``.
-
-        Args:
-            web_service_access_token (str): The Web Service Credential Access
-                Token obtained from the first half of the gtoken generation
-                process.
-            f_token_url (str): URL to use for f token generation. This package
-                provides a default URL, but you can provide your own. The
-                default URL is provided by `imink`.
-
-        Returns:
-            str: The gtoken from the response.
-        """
-        f_token, request_id, timestamp = self._f_token_function(
-            f_token_url, web_service_access_token, 2
-        )
-
-        return self.get_gtoken_request(
-            web_service_access_token, f_token, request_id, timestamp
-        )
-
-    def get_web_service_access_token(
-        self,
-        id_token: str,
-        user_info: dict[str, str],
-        f_token: str,
-        request_id: str,
-        timestamp: str,
-    ) -> str:
-        """Given the ``id_token``, user data, ``f_token``, ``request_id``, and
-        ``timestamp``, returns the Web Service Credential Access Token.
-
-        This is the first step of the ``gtoken`` generation process. This will
-        return the Web Service Credential Access Token from Nintendo's servers,
-        which is then used to obtain the ``gtoken``.
-
-        Args:
-            id_token (str): The ``id_token`` from the user access response.
-            user_info (dict[str, str]): The dictionary of user info returned by
-                ``get_user_info``. This must contain the keys ``language``,
-                ``birthday``, and ``country``.
-            f_token (str): The ``f_token`` generated from the ``id_token``. It
-                is important that this is the ``f_token`` generated from the
-                ``id_token`` using the first hashing method and not the second.
-            request_id (str): The ``request_id`` returned alongside the
-                ``f_token`` and ``timestamp``.
-            timestamp (str): The ``timestamp`` returned alongside the
-                ``f_token`` and ``request_id``.
-
-        Returns:
-            str: The Web Service Credential Access Token.
-        """
-        header = {
-            "X-Platform": "Android",
-            "X-ProductVersion": self.version,
-            "Content-Type": "application/json; charset=utf-8",
-            "Content-Length": str(990 + len(f_token)),
-            "Connection": "Keep-Alive",
-            "Accept-Encoding": "gzip",
-            "User-Agent": "com.nintendo.znca/"
-            + self.version
-            + "(Android/7.1.2)",
-        }
-        body = {
-            "parameter": {
-                "f": f_token,
-                "language": user_info["language"],
-                "naBirthday": user_info["birthday"],
-                "naCountry": user_info["country"],
-                "naIdToken": id_token,
-                "requestId": request_id,
-                "timestamp": timestamp,
-            }
-        }
-        url = "https://api-lp1.znc.srv.nintendo.net/v3/Account/Login"
-        response = self.session.post(url, headers=header, json=body).json()
-        return response["result"]["webApiServerCredential"]["accessToken"]
-
-    def get_gtoken_request(
-        self,
-        web_service_access_token: str,
-        f_token: str,
-        request_id: str,
-        timestamp: str,
-    ) -> str:
-        """Given the ``web_service_access_token``, ``f_token``, ``request_id``,
-        and ``timestamp``, returns the ``gtoken``.
-
-        This is named differently from the other ``get_gtoken`` function to
-        avoid confusion. This function specifically makes the request to
-        Nintendo's servers to obtain the ``gtoken`` given the web service access
-        token, ``f_token``, ``request_id``, and ``timestamp``. The other
-        function only takes the ``session_token`` and generates all of the other
-        intermediate tokens to obtain the ``gtoken`` by finally calling this
-        function.
-
-        Args:
-            web_service_access_token (str): The ``web_service_access_token``
-                obtained from the first half of the ``gtoken`` generation
-                process.
-            f_token (str): The ``f_token`` generated from the
-                ``web_service_access_token``. It is important that this is the
-                ``f_token`` generated from the ``web_service_access_token``
-                using the second hashing method and not the first.
-            request_id (str): The ``request_id`` returned alongside the
-                ``f_token`` and ``timestamp``.
-            timestamp (str): The ``timestamp`` returned alongside the
-                ``f_token`` and ``request_id``.
-
-        Returns:
-            str: The ``gtoken``.
-        """
-        header = {
-            "X-Platform": "Android",
-            "X-ProductVersion": self.version,
-            "Authorization": f"Bearer {web_service_access_token}",
-            "Content-Type": "application/json; charset=utf-8",
-            "Content-Length": "391",
-            "Accept-Encoding": "gzip",
-            "User-Agent": f"com.nintendo.znca/{self.version}(Android/7.1.2)",
-        }
-        body = {
-            "parameter": {
-                "f": f_token,
-                "id": 4834290508791808,
-                "registrationToken": web_service_access_token,
-                "requestId": request_id,
-                "timestamp": timestamp,
-            }
-        }
-        url = "https://api-lp1.znc.srv.nintendo.net/v2/Game/GetWebServiceToken"
-        response = self.session.post(url, headers=header, json=body).json()
-        return response["result"]["accessToken"]
-
-    def get_bullet_token(
-        self,
-        gtoken: str,
-        user_info: dict,
-        user_agent: str | None = None,
-    ) -> str:
-        """Given the ``gtoken`` and user information, send a request to SplatNet
-        3 to obtain the bullet token. This token is required to make any
-        requests to SplatNet 3, and is valid for 6 hours and 30 minutes after it
-        is obtained.
-
-        The gtoken is obtained by calling ``get_gtoken`` and the user
-        information is obtained by calling ``get_user_info``. The user
-        information must contain the keys ``language``, ``birthday``, and
-        ``country`` and must align with the values set in the user's Nintendo
-        account. The user agent is optional, and if not provided, the default
-        user agent will be used. It is not recommended to change the user agent
-        from the default unless you know what you are doing.
-
-        Args:
-            gtoken (str): GameWebToken, also known as gtoken. Given by Nintendo.
-                This token is required to make any requests to Nintendo Switch
-                Online services and is valid for 2 hours after it is obtained.
-            user_info (dict): Dictionary containing the user's information. This
-                must contain the keys ``language``, ``birthday``, and
-                ``country`` and must align with the values set in the user's
-                Nintendo account. These values are verified by Nintendo, so if
-                they do not align, no bullet token will be generated.
-            user_agent (str | None): User agent to use for the request. This is
-                optional, and if not provided, the default user agent will be
-                used. It is not recommended to change the user agent from the
-                default unless you know what you are doing. The default user
-                agent can be found in ``constants.py`` as
-                ``DEFAULT_USER_AGENT``. Defaults to None.
-
-        Raises:
-            SplatNetException: Error 401, ``ERROR_INVALID_GAME_WEB_TOKEN``. This
-                indicates that the gtoken is invalid. This can happen if the
-                gtoken is expired or if the provided gtoken was never valid.
-            SplatNetException: Error 403 ``ERROR_OBSOLETE_VERSION``. This
-                indicates that the version provided in request header key
-                ``X-Web-View-Ver`` is outdated. This can happen if the version
-                provided is too old.
-            SplatNetException: Error 204, ``USER_NOT_REGISTERED``. This
-                indicates that there is no game user associated with Splatoon 3,
-                and that the user must play at least one match of Splatoon 3
-                before using this library.
-            NintendoException: If the request does not fail with one of the
-                above errors, this indicates that the request failed for some
-                other reason and this exception will be raised to indicate that
-                the request failed silently.
-
-        Returns:
-            str: The bullet token. This token is required to make any requests
-                to SplatNet 3, and is valid for 6 hours and 30 minutes after it
-                is obtained.
-        """
-        user_agent = (
-            user_agent if user_agent is not None else DEFAULT_USER_AGENT
-        )
-        header = {
-            "Content-Length": "0",
-            "Content-Type": "application/json",
-            "Accept-Language": user_info["language"],
-            "User-Agent": user_agent,
-            "X-Web-View-Ver": self.splatnet_web_version,
-            "X-NACOUNTRY": user_info["country"],
-            "Accept": "*/*",
-            "Origin": SPLATNET_URL,
-            "X-Requested-With": "com.nintendo.znca",
-        }
-        cookies = {
-            "_gtoken": gtoken,
-            "_dnt": "1",
-        }
-        url = SPLATNET_URL + "/api/bullet_tokens"
-        response = self.session.post(url, headers=header, cookies=cookies)
-
-        if response.status_code == 401:
-            raise SplatNetException(
-                "Error 401: Invalid Game Web Token (gtoken)"
-            )
-        elif response.status_code == 403:
-            raise SplatNetException("Error 403: Outdated Version")
-        elif response.status_code == 204:
-            raise SplatNetException(
-                "Error 204: User Not Registered. Please play at least one match"
-                + " of Splatoon 3 before using this library."
-            )
-
-        try:
-            return response.json()["bulletToken"]
-        except KeyError:
-            raise NintendoException("Invalid response from Nintendo")
-
-    @property
-    def splatnet_web_version(self) -> str:
-        """Get the web view version for SplatNet 3. This is used in the request
-        header key ``X-Web-View-Ver`` to indicate the version of the web view
-        that is being used. This is required to make any requests to SplatNet
-        3. If the version cannot be obtained, a fallback version will be used.
-
-        Returns:
-            str: The web view version for SplatNet 3.
-        """
-        if self._web_view_version is not None:
-            return self._web_view_version
-        try:
-            web_version = get_splatnet_web_version()
-            self._web_view_version = web_version
-            return web_version
-        except SplatNetException as e:
-            logger.log(str(e), "warning")
-            logger.log("Using fallback web view version", "warning")
-            return WEB_VIEW_VERSION_FALLBACK
+import base64
+import hashlib
+import json
+import logging
+import os
+import re
+from typing import Callable, Literal, TypeAlias, cast
+
+import requests
+
+from splatnet3_scraper import __version__
+from splatnet3_scraper.auth.exceptions import (
+    FTokenException,
+    NintendoException,
+    SplatNetException,
+)
+from splatnet3_scraper.constants import (
+    APP_VERSION_FALLBACK,
+    DEFAULT_USER_AGENT,
+    IMINK_URL,
+    IOS_APP_URL,
+    SPLATNET_URL,
+    WEB_VIEW_VERSION_FALLBACK,
+)
+from splatnet3_scraper.utils import get_splatnet_version, retry
+
+version_re = re.compile(
+    r"(?<=whats\-new\_\_latest\_\_version\"\>Version)\s+\d+\.\d+\.\d+"
+)
+
+FToken_Gen: TypeAlias = Callable[
+    [str, str, Literal[1] | Literal[2]], tuple[str, str, str]
+]
+
+
+class NSO:
+    """The NSO class contains all the logic to proceed through the login flow.
+    This class also holds various properties that are used to make requests to
+    the Nintendo Switch Online API. Login flow is roughly as follows, assuming
+    the user has never generated a session token before:
+
+        1.  Initialize a requests session and store it.
+        2.  Generate a random state and S256 code challenge that will be used
+            to obtain the "session_token". Store them for later use.
+        3.  Generate a login URL using the state and code challenge that the
+            user will open in their browser. The user will then copy a link and
+            feed it back to the program.
+        4.  Parse the URI to obtain the session token code, then use it
+            alongside the code challenge to obtain the ``session_token``. Store
+            it for later use. The session token is valid for 2 years and can be
+            revoked by the user.
+        5.  Use the session token to obtain a user access response from
+            Nintendo. This response will contain an ``id_token`` and a user
+            access token. Store both for later user.
+        6.  Use the user access token to obtain the user information. This is
+            required to obtain the first ``f_token``, for the Nintendo Switch
+            Online API. This is a message authentication code generated from the
+            timestamp and id token in an obscure manner and will be necessary
+            to generate the API access token.
+        7.  Use the Nintendo-obtained ``id_token`` to obtain the first
+            ``f_token``, for the Nintendo Switch Online API. The ``f_token``
+            will also return a timestamp and a request ID.
+        8.  Use the first ``f_token``, the request ID, the timestamp, the user
+            information, the ``id_token`` to obtain the
+            ``web_service_access_token``.
+        9.  Use the ``web_service_access_token`` to obtain the second
+            ``f_token``. This is a message authentication code generated from
+            the timestamp and id token in an obscure manner and will be
+            necessary to generate the ``gtoken``. This step is distinct from
+            step 7, make sure not to use the same ``f_token`` twice.
+        10. Use the second ``f_token``, the request ID, the timestamp, and the
+            ``web_service_access_token`` from step 9, and the id
+            ``4834290508791808`` to obtain the ``gtoken``.
+        11. Use the ``gtoken`` and user information to obtain a
+            ``bullet_token``. This token is valid for 2 hours.
+
+    Once the login flow is complete, the NSO class contains all the necessary
+    values to regenerate the tokens. To minimize the number of objects to track,
+    the NSO class only stores the tokens in memory. The TokenManager class
+    handles the persistence of the tokens to disk.
+    """
+
+    def __init__(self, session: requests.Session) -> None:
+        """Initializes the NSO class. The NSO class contains all the logic and
+        holds all the necessary values to proceed through the login flow.
+
+        The ``__init__`` method sets the following internal variables:
+
+            -   ``session``: The requests session object that is used to make
+                requests to the Nintendo Switch Online API. This is the only
+                variable that is passed in to the ``__init__`` method.
+            -   ``_state``: The internal state variable that is used to obtain
+                the session token. This is a random string that is generated
+                when the ``NSO.state`` property is first accessed, and is used
+                to generate the login URL.
+            -   ``_verifier``: The internal verifier variable that is used to
+                obtain the session token. This is a random string that is
+                generated when the ``NSO.verifier`` property is first accessed,
+                and is used to generate the login URL. The verifier is also
+                used to solve the code challenge, verifying to Nintendo that
+                the user is who they say they are.
+            -   ``_version``: The internal version variable that is used to
+                verify the NSO app version. This is a string that is generated
+                when the ``NSO.version`` property is first accessed, and is
+                used to obtain the session token.
+            -   ``_web_view_version``: The internal web view version variable
+                that is used to verify the NSO app version. This is a string
+                that is generated when the ``NSO.web_view_version`` property is
+                first accessed, and is used to obtain the session token.
+            -   ``_session_token``: A stored session token. This is required to
+                generate all other tokens and information. This is obtained
+                during the login flow and is valid for 2 years.
+            -   ``_user_access_token``: A stored user access token. This is a
+                token that is obtained during the login flow and is used to
+                obtain the user information.
+            -   ``_id_token``: A stored id token. This is a token that is
+                obtained during the login flow and is used to obtain the gtoken.
+            -   ``_gtoken``: A stored gtoken. This is a token that is obtained
+                during the login flow and is used to obtain the bullet token. It
+                is valid for 6 hours and 30 minutes.
+            -   ``_user_info``: A stored user information dictionary. This is
+                obtained during the login flow and is used to obtain the "f"
+                token.
+            -   ``_f_token_function``: A stored function that is used to obtain
+                the "f" token. This function is set to the ``get_ftoken``
+                method by default, and can be set with the
+                ``set_new_f_token_function`` method to use a user-defined
+                function if desired.
+
+
+        Args:
+            session (requests.Session): The NSO class uses a requests session
+                to make requests to the Nintendo Switch Online API. The session
+                object is passed in to the NSO class so that the same session
+                object can be used to make requests to the SplatNet API.
+        """
+        self.session = session
+        self._state: bytes | None = None
+        self._verifier: bytes | None = None
+        self._version: str | None = None
+        self._web_view_version: str | None = None
+        self._session_token: str | None = None
+        self._user_access_token: str | None = None
+        self._id_token: str | None = None
+        self._gtoken: str | None = None
+        self._user_info: dict[str, str] | None = None
+        self._f_token_function: FToken_Gen = self.get_ftoken
+
+    @staticmethod
+    def new_instance() -> "NSO":
+        """Creates a new instance of the NSO class with a new requests session.
+
+        This is the recommended way to create a new instance of the NSO class,
+        as it ensures that the session is a fresh session, however it is not
+        absolutely necessary to instantiate a new NSO class using this method.
+        Passing in a new session to the ``__init__`` method is perfectly fine.
+
+        Returns:
+            NSO: A new instance of the NSO class.
+        """
+        session = requests.Session()
+        return NSO(session=session)
+
+    @property
+    def version(self) -> str:
+        """Returns the current version of the NSO app. Necessary to get the
+        session token. If the version has not been obtained yet, it will be
+        obtained and stored. If the version cannot be obtained, a fallback
+        version will be used.
+
+        Returns:
+            str: The current version of the NSO app.
+        """
+        if self._version is None:
+            self._version = self.get_version()
+        return self._version
+
+    @retry(times=2, exceptions=ValueError)
+    def get_version(self) -> str:
+        """Fetches the current version of the Nintendo Switch Online app from
+        the iOS app store. This is necessary to access the API. This method
+        retries twice if the version cannot be obtained, in case the iOS App
+        Store site is down or slow. If the version cannot be obtained after
+        three attempts, a fallback version defined in the ``constants.py`` file
+        will be used.
+
+        Returns:
+            str: The current version of the NSO app.
+        """
+        # TODO: Replace the iOS app store method with a method that does not
+        # require scraping a website with scraping protection.
+        response = self.session.get(IOS_APP_URL)
+        version = version_re.search(response.text)
+        if version is None:
+            logging.warning(
+                "Failed to get version from app store, using fallback"
+            )
+            return APP_VERSION_FALLBACK
+        return version.group(0).strip()
+
+    @property
+    def state(self) -> bytes:
+        """Returns a base64url encoded random 36 byte string for the auth state.
+        This is used to generate the login URL. To align with node.js's crypto
+        module, padding is removed. If the state has not been obtained yet, it
+        will be obtained and stored by creating a random 36 byte string and then
+        base64url encoding it.
+
+        Returns:
+            bytes: The auth state, without padding. This is used within the
+                login flow to verify that the user is who they say they are.
+        """
+        if self._state is None:
+            self._state = self.generate_new_state()
+        return self._state
+
+    def generate_new_state(self) -> bytes:
+        """Generates a new state.
+
+        Returns:
+            bytes: The auth state, without padding. A random 36 byte string
+                that is base64url encoded.
+        """
+        return base64.urlsafe_b64encode(os.urandom(36))
+
+    @property
+    def verifier(self) -> bytes:
+        """Returns a base64url encoded random 32 byte string for the code
+        verifier. This is used to generate the S256 code challenge. To align
+        with node.js's crypto module, padding is removed. If the verifier has
+        not been obtained yet, it will be obtained and stored by creating a
+        random 32 byte string and then base64url encoding it.
+
+        Returns:
+            bytes: The code verifier, without padding. This is used within the
+                login flow to verify that the user is who they say they are.
+        """
+        if self._verifier is None:
+            self._verifier = self.generate_new_verifier()
+        return self._verifier
+
+    def generate_new_verifier(self) -> bytes:
+        """Generates a new code verifier, which is a random 32 byte string
+        that is base64url encoded and with padding removed. This is used to
+        generate the S256 code challenge.
+
+        Returns:
+            bytes: The code verifier, without padding.
+        """
+        verifier_ = base64.urlsafe_b64encode(os.urandom(32))
+        return verifier_.replace(b"=", b"")
+
+    @property
+    def session_token(self) -> str:
+        """Returns the session token. This cannot be generated and must be set
+        by the user. If the session token has not been set, a ValueError will be
+        raised.
+
+        Raises:
+            ValueError: The session token has not been set.
+
+        Returns:
+            str: The session token.
+        """
+        if self._session_token is None:
+            raise ValueError("Session token is not set.")
+        return self._session_token
+
+    def generate_login_url(self, user_agent: str | None = None) -> str:
+        """Generates the login URL that can be used to obtain the session token.
+
+        This method will generate the login URL that is used to obtain the
+        session token. For full details on how to obtain a session token, see
+        the ``Obtaining a session token`` section of the documentation.
+
+        Args:
+            user_agent (str): The user agent to use. Defaults to the default
+                user agent found in ``constants.py``.
+
+        Returns:
+            str: The login URL that can be used to obtain the session token.
+        """
+        # https://dev.to/mathewthe2/intro-to-nintendo-switch-rest-api-2cm7
+        hash_ = hashlib.sha256()
+        hash_.update(self.verifier)
+        challenge = base64.urlsafe_b64encode(hash_.digest()).replace(b"=", b"")
+
+        header = {
+            "Host": "accounts.nintendo.com",
+            "Connection": "keep-alive",
+            "Cache-Control": "max-age=0",
+            "Upgrade-Insecure-Requests": "1",
+            "User-Agent": user_agent
+            if user_agent is not None
+            else DEFAULT_USER_AGENT,
+            "Accept": (
+                "text/html,"
+                + "application/xhtml+xml,"
+                + "application/xml;q=0.9,"
+                + "image/webp,"
+                + "image/apng,"
+                + "*/*;q=0.8n"
+            ),
+            "DNT": "1",
+            "Accept-Encoding": "gzip,deflate,br",
+        }
+        params = {
+            "state": self.state,
+            "redirect_uri": "npf71b963c1b7b6d119://auth",
+            "client_id": "71b963c1b7b6d119",
+            "scope": ("openid user user.birthday user.mii user.screenName"),
+            "response_type": "session_token_code",
+            "session_token_code_challenge": challenge,
+            "session_token_code_challenge_method": "S256",
+            "theme": "login_form",
+        }
+        login_url = "https://accounts.nintendo.com/connect/1.0.0/authorize"
+        response = self.session.get(
+            login_url, headers=header, params=params  # type: ignore
+        )
+        return response.url
+
+    def parse_npf_uri(self, uri: str) -> str:
+        """Parses the uri returned by the Nintendo login page and extracts the
+        session token code. This is used to pass the challenge and verify that
+        the user is who they say they are.
+
+        Args:
+            uri (str): The uri returned by the Nintendo login page.
+
+        Returns:
+            str: The session token code. This is *NOT* the session token, but is
+                used to obtain the session token.
+        """
+        return uri.split("&")[1][len("session_token_code=") :]
+
+    def get_session_token(self, session_token_code: str) -> str:
+        """Obtains the session token from the session token code.
+
+        This method will obtain the session token from the session token code.
+        It will use provide the session token code to Nintendo's servers
+        alongside the session token code verifier. Nintendo will then verify
+        that the user is who they say they are and return the session token.
+
+        Args:
+            session_token_code (str): The session token code. This is obtained
+                by parsing the uri obtained at the URL returned by
+                ``generate_login_url``.
+
+        Returns:
+            str: The session token. DO NOT SHARE THIS TOKEN WITH ANYONE.
+        """
+        header = {
+            "User-Agent": f"OnlineLounge/{self.version} NASDKAPI Android",
+            "Accept-Language": "en-US",
+            "Accept": "application/json",
+            "Content-Type": "application/x-www-form-urlencoded",
+            "Content-Length": "540",
+            "Host": "accounts.nintendo.com",
+            "Connection": "Keep-Alive",
+            "Accept-Encoding": "gzip",
+        }
+        params = {
+            "client_id": "71b963c1b7b6d119",
+            "session_token_code": session_token_code,
+            "session_token_code_verifier": self.verifier,
+        }
+        uri = "https://accounts.nintendo.com/connect/1.0.0/api/session_token"
+        response = self.session.post(uri, headers=header, data=params)
+        session_token = response.json()["session_token"]
+        self._session_token = session_token
+        return session_token
+
+    def get_user_access_token(self, session_token: str) -> dict:
+        """Obtains the user access token from the session token.
+
+        This method sends a request to Nintendo's servers containing the session
+        token to obtain the user access token and the ``id_token``. The user
+        access token is then used to obtain the user's data, while the
+        ``id_token`` is used to obtain the user's gtoken.
+
+        Args:
+            session_token (str): The session token.
+
+        Returns:
+            dict: The response from Nintendo's servers. This contains two keys
+                of interest: ``access_token`` and ``id_token``. The
+                ``access_token`` is used to obtain the user's data, while the
+                ``id_token`` is used to obtain the user's gtoken.
+        """
+        header = {
+            "Host": "accounts.nintendo.com",
+            "Accept-Encoding": "gzip",
+            "Content-Type": "application/json",
+            "Content-Length": "436",
+            "Accept": "application/json",
+            "Connection": "Keep-Alive",
+            "User-Agent": "Dalvik/2.1.0 (Linux; U; Android 7.1.2)",
+        }
+        body = {
+            "client_id": "71b963c1b7b6d119",
+            "session_token": session_token,
+            "grant_type": (
+                "urn:ietf:params:oauth:grant-type:jwt-bearer-session-token"
+            ),
+        }
+        uri = "https://accounts.nintendo.com/connect/1.0.0/api/token"
+        return self.session.post(uri, headers=header, json=body).json()
+
+    def get_user_info(self, user_access_token: str) -> dict[str, str]:
+        """Obtains the user information from the user access token.
+
+        This method will obtain the user information from the user access token.
+        This includes the user's set language, country, and birthday, which are
+        used to obtain the user's ``gtoken``.
+
+        Args:
+            user_access_token (str): The user access token.
+
+        Returns:
+            dict[str, str]: The user information. This includes the user's set
+                language, country, and birthday.
+        """
+        # Get user information
+        url = "https://api.accounts.nintendo.com/2.0.0/users/me"
+        header = {
+            "User-Agent": "NASDKAPI; Android",
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+            "Authorization": f"Bearer {user_access_token}",
+            "Host": "api.accounts.nintendo.com",
+            "Connection": "Keep-Alive",
+            "Accept-Encoding": "gzip",
+        }
+        response = self.session.get(url, headers=header)
+        return response.json()
+
+    def get_gtoken(
+        self, session_token: str, f_token_url: str | None = None
+    ) -> str:
+        """Obtains the ``gtoken`` from the session token.
+
+        The GameWebToken, or ``gtoken``, is used to authenticate requests to the
+        Nintendo Switch Online API. This method will obtain the ``gtoken`` from
+        the session token. The process of obtaining a ``gtoken`` is as follows:
+
+        1. Obtain the user access token and the ``id_token`` from the session
+                token.
+        2. Use the user access token to obtain the user's information.
+        3. Use the ``id_token`` and the user's information to obtain the first
+                ``f_token``, the request ID, and the timestamp.
+        4. Use the first ``f_token``, the request ID, the timestamp, and the
+                ``id_token`` to obtain the ``web_service_access_token``.
+        5. Use the ``web_service_access_token`` to obtain the second
+                ``f_token``, request ID, and timestamp.
+        6. Use the second ``f_token``, request ID, timestamp, and the
+                ``web_service_access_token`` to obtain the ``gtoken``.
+
+        By default, this method will use a third party's ``f_token`` generation
+        API to obtain the ``f_token``. The API used by default is provided by
+        `imink <https://github.com/imink-app>`_. If you do not trust this URL,
+        you can provide your own URL through the ``f_token_url`` argument, or
+        you can replace the ``f_token`` generation method used with your own
+        through the use of the ``set_new_f_token_function`` method. See the
+        documentation for that method for more information.
+
+        Args:
+            session_token (str): The session token.
+            f_token_url (str): The url to get the user access token from. This
+                defaults to the ftoken generation url provided by `imink`.
+
+        Raises:
+            NintendoException: In the case that the user's access token cannot
+                be obtained from the session token, or the user's information
+                that is returned is invalid.
+
+        Returns:
+            str: The gtoken. This is used to authenticate requests to the
+                Nintendo Switch Online API. This token is valid for 2 hours.
+        """
+        f_token_url = f_token_url if f_token_url is not None else IMINK_URL
+        # Get user access token
+        logging.info("Getting user access token")
+        user_access_response = self.get_user_access_token(session_token)
+        try:
+            self._user_access_token = cast(
+                str, user_access_response["access_token"]
+            )
+            self._id_token = cast(str, user_access_response["id_token"])
+        except (KeyError, TypeError, AttributeError):
+            raise NintendoException(
+                "Failed to get user access token. "
+                + f"Response: {user_access_response}"
+            )
+
+        logging.info("Getting user info")
+        user_info = self.get_user_info(self._user_access_token)
+        self._user_info = user_info
+        logging.info("Getting Web Service Access Token")
+        web_service_access_token = self.g_token_generation_phase_1(
+            self._id_token, user_info, f_token_url
+        )
+        logging.info("Getting gtoken")
+        gtoken = self.g_token_generation_phase_2(
+            web_service_access_token, f_token_url
+        )
+        self._gtoken = gtoken
+        return gtoken
+
+    def set_new_f_token_function(
+        self, new_function: FToken_Gen | None = None
+    ) -> None:
+        """Sets the function used to generate the ``f_token``.
+
+        This method will set the function used to generate the ``f_token``. The
+        function must take the following arguments:
+
+        1. The ``f_token`` generation url.
+        2. The user's token, either the ``id_token`` for step ``1``, or the
+            ``web_service_access_token`` for step ``2``.
+        3. The step number (either ``1`` or ``2``)
+
+        The function must return a tuple containing the following:
+
+        1. The ``f_token``.
+        2. The request id.
+        3. The timestamp.
+
+        Args:
+            new_function (FToken_Gen): The new function to use to generate the
+                ftoken. This function must take the following arguments:
+
+                1. The ``f_token`` generation url.
+                2. The user's token, either the ``id_token`` for step ``1``, or
+                    the ``web_service_access_token`` for step ``2``.
+                3. The step number (either ``1`` or ``2``)
+
+                The function must return a tuple containing the following:
+
+                1. The ``f_token``.
+                2. The request id.
+                3. The timestamp.
+
+            If this argument is not provided or is ``None``, the default
+            ``f_token`` generation method will be restored.
+        """
+        if new_function is None:
+            logging.info("Restoring default ftoken generation method")
+            self._f_token_function = self.get_ftoken
+        else:
+            logging.info("Setting new ftoken generation method")
+            self._f_token_function = new_function
+
+    def get_ftoken(
+        self, f_token_url: str, id_token: str, step: Literal[1] | Literal[2]
+    ) -> tuple[str, str, str]:
+        """Given the ``f_token_url``, ``id_token``, and ``step``, returns the
+        ``f_token``, ``request_id``, and ``timestamp`` from the response.
+
+        Note that this is a third party method, and is not officially
+        sanctioned by Nintendo. The default ftoken generation URL used by this
+        library is provided by `imink <https://github.com/imink-app>`_. In
+        the interest of transparency, the following is the entirety of the
+        request header sent to the ftoken generation URL:
+
+        >>> {
+        ...     "User-Agent": f"splatnet3_scraper/{__version__}",
+        ...     "Content-Type": "application/json; charset=utf-8",
+        ... }
+
+        The following is the entirety of the request body sent to the ftoken
+        generation URL:
+
+        >>> {
+        ...     "token": id_token,
+        ...     "hash_method": step,
+        ... }
+
+        As you can see, the only identifying information sent to the ftoken
+        generation URL is the user's ``id_token``, which cannot be used to
+        identify the user without the user's access token, which is not
+        provided to the ftoken generation URL.
+
+        Args:
+            f_token_url (str): URL to use for ``f_token`` generation. This
+                package provides a default URL, but you can provide your own.
+                The default URL is provided by `imink`.
+            id_token (str): ID token from user access token response. This is
+                obtained from the user access token response, and is used to
+                identify the user. This cannot be used to identify the user
+                without the user's access token, which is not provided to the
+                ftoken generation URL.
+            step (Literal[1] | Literal[2]): The step number. This is either
+                ``1`` or ``2``. This is used to identify the step in the
+                ``f_token`` generation process.
+
+        Raises:
+            FTokenException: In the case that the ftoken cannot be obtained
+                from the ftoken generation URL.
+
+        Returns:
+            str: The f token.
+            str: The request ID.
+            str: The timestamp.
+        """
+        header = {
+            "User-Agent": f"splatnet3_scraper/{__version__}",
+            "Content-Type": "application/json; charset=utf-8",
+        }
+        body = {
+            "token": id_token,
+            "hash_method": step,
+        }
+        bodystr = json.dumps(body)
+        response = self.session.post(f_token_url, headers=header, data=bodystr)
+        response_json = response.json()
+        try:
+            f_token = response_json["f"]
+            request_id = response_json["request_id"]
+            timestamp = response_json["timestamp"]
+        except (KeyError, TypeError, AttributeError):
+            raise FTokenException(
+                "Failed to get f token. " + f"Response: {response_json}"
+            )
+        return (f_token, request_id, timestamp)
+
+    @retry(times=1, exceptions=(FTokenException, NintendoException, KeyError))
+    def g_token_generation_phase_1(
+        self,
+        id_token: str,
+        user_info: dict[str, str],
+        f_token_url: str,
+    ) -> str:
+        """First phase of the ``gtoken`` generation process.
+
+        This is the first phase of the ``gtoken`` generation process. This is
+        abstracted away into a separate method to allow the request to be
+        retried once in the event of a failure. This phase involves two steps:
+        first, the ``id_token`` is sent to the ``f_token_url`` in a request to
+        obtain the ``f_token``, which is a ``HMAC`` necessary to obtain the
+        ``gtoken``. The response contains three values: the ``f_token``, the
+        ``request_id``, and the ``timestamp``. These values are then sent to
+        Nintendo's servers along with the  ``id_token`` to obtain the
+        ``gtoken``.
+
+        Args:
+            id_token (str): ID token from user access token response. This is
+                obtained from the user access token response, and is used to
+                identify the user to Nintendo's servers. However, this cannot
+                be used to identify the user by a third party by itself.
+            user_info (dict[str, str]): The dictionary of user info returned by
+                ``get_user_info``. This must contain the keys ``language``,
+                ``birthday``, and ``country``.
+            f_token_url (str): URL to use for f token generation. This package
+                provides a default URL, but you can provide your own. The
+                default URL is provided by `imink`.
+
+        Returns:
+            str: The Web Service Credential Access Token.
+        """
+        f_token, request_id, timestamp = self._f_token_function(
+            f_token_url, id_token, 1
+        )
+        return self.get_web_service_access_token(
+            id_token, user_info, f_token, request_id, timestamp
+        )
+
+    @retry(times=1, exceptions=(FTokenException, NintendoException, KeyError))
+    def g_token_generation_phase_2(
+        self,
+        web_service_access_token: str,
+        f_token_url: str,
+    ) -> str:
+        """Final phase of the ``gtoken`` generation process.
+
+        This is the second phase of the ``gtoken`` generation process. This is
+        abstracted away into a separate method to allow the request to be
+        retried once in the event of a failure. This phase involves two steps:
+        first, the ``web_service_access_token`` is sent to the ``f_token_url``
+        in a request to obtain the ``f_token``, which is a ``HMAC`` necessary to
+        obtain the ``gtoken``. The response contains three values: the
+        ``f_token``, the ``request_id``, and the ``timestamp``. These values are
+        then sent to Nintendo's servers along with the
+        ``web_service_access_token`` to obtain the ``gtoken``.
+
+        Args:
+            web_service_access_token (str): The Web Service Credential Access
+                Token obtained from the first half of the gtoken generation
+                process.
+            f_token_url (str): URL to use for f token generation. This package
+                provides a default URL, but you can provide your own. The
+                default URL is provided by `imink`.
+
+        Returns:
+            str: The gtoken from the response.
+        """
+        f_token, request_id, timestamp = self._f_token_function(
+            f_token_url, web_service_access_token, 2
+        )
+
+        return self.get_gtoken_request(
+            web_service_access_token, f_token, request_id, timestamp
+        )
+
+    def get_web_service_access_token(
+        self,
+        id_token: str,
+        user_info: dict[str, str],
+        f_token: str,
+        request_id: str,
+        timestamp: str,
+    ) -> str:
+        """Given the ``id_token``, user data, ``f_token``, ``request_id``, and
+        ``timestamp``, returns the Web Service Credential Access Token.
+
+        This is the first step of the ``gtoken`` generation process. This will
+        return the Web Service Credential Access Token from Nintendo's servers,
+        which is then used to obtain the ``gtoken``.
+
+        Args:
+            id_token (str): The ``id_token`` from the user access response.
+            user_info (dict[str, str]): The dictionary of user info returned by
+                ``get_user_info``. This must contain the keys ``language``,
+                ``birthday``, and ``country``.
+            f_token (str): The ``f_token`` generated from the ``id_token``. It
+                is important that this is the ``f_token`` generated from the
+                ``id_token`` using the first hashing method and not the second.
+            request_id (str): The ``request_id`` returned alongside the
+                ``f_token`` and ``timestamp``.
+            timestamp (str): The ``timestamp`` returned alongside the
+                ``f_token`` and ``request_id``.
+
+        Returns:
+            str: The Web Service Credential Access Token.
+        """
+        header = {
+            "X-Platform": "Android",
+            "X-ProductVersion": self.version,
+            "Content-Type": "application/json; charset=utf-8",
+            "Content-Length": str(990 + len(f_token)),
+            "Connection": "Keep-Alive",
+            "Accept-Encoding": "gzip",
+            "User-Agent": "com.nintendo.znca/"
+            + self.version
+            + "(Android/7.1.2)",
+        }
+        body = {
+            "parameter": {
+                "f": f_token,
+                "language": user_info["language"],
+                "naBirthday": user_info["birthday"],
+                "naCountry": user_info["country"],
+                "naIdToken": id_token,
+                "requestId": request_id,
+                "timestamp": timestamp,
+            }
+        }
+        url = "https://api-lp1.znc.srv.nintendo.net/v3/Account/Login"
+        response = self.session.post(url, headers=header, json=body).json()
+        return response["result"]["webApiServerCredential"]["accessToken"]
+
+    def get_gtoken_request(
+        self,
+        web_service_access_token: str,
+        f_token: str,
+        request_id: str,
+        timestamp: str,
+    ) -> str:
+        """Given the ``web_service_access_token``, ``f_token``, ``request_id``,
+        and ``timestamp``, returns the ``gtoken``.
+
+        This is named differently from the other ``get_gtoken`` function to
+        avoid confusion. This function specifically makes the request to
+        Nintendo's servers to obtain the ``gtoken`` given the web service access
+        token, ``f_token``, ``request_id``, and ``timestamp``. The other
+        function only takes the ``session_token`` and generates all of the other
+        intermediate tokens to obtain the ``gtoken`` by finally calling this
+        function.
+
+        Args:
+            web_service_access_token (str): The ``web_service_access_token``
+                obtained from the first half of the ``gtoken`` generation
+                process.
+            f_token (str): The ``f_token`` generated from the
+                ``web_service_access_token``. It is important that this is the
+                ``f_token`` generated from the ``web_service_access_token``
+                using the second hashing method and not the first.
+            request_id (str): The ``request_id`` returned alongside the
+                ``f_token`` and ``timestamp``.
+            timestamp (str): The ``timestamp`` returned alongside the
+                ``f_token`` and ``request_id``.
+
+        Returns:
+            str: The ``gtoken``.
+        """
+        header = {
+            "X-Platform": "Android",
+            "X-ProductVersion": self.version,
+            "Authorization": f"Bearer {web_service_access_token}",
+            "Content-Type": "application/json; charset=utf-8",
+            "Content-Length": "391",
+            "Accept-Encoding": "gzip",
+            "User-Agent": f"com.nintendo.znca/{self.version}(Android/7.1.2)",
+        }
+        body = {
+            "parameter": {
+                "f": f_token,
+                "id": 4834290508791808,
+                "registrationToken": web_service_access_token,
+                "requestId": request_id,
+                "timestamp": timestamp,
+            }
+        }
+        url = "https://api-lp1.znc.srv.nintendo.net/v2/Game/GetWebServiceToken"
+        response = self.session.post(url, headers=header, json=body).json()
+        return response["result"]["accessToken"]
+
+    def get_bullet_token(
+        self,
+        gtoken: str,
+        user_info: dict,
+        user_agent: str | None = None,
+    ) -> str:
+        """Given the ``gtoken`` and user information, send a request to SplatNet
+        3 to obtain the bullet token. This token is required to make any
+        requests to SplatNet 3, and is valid for 6 hours and 30 minutes after it
+        is obtained.
+
+        The gtoken is obtained by calling ``get_gtoken`` and the user
+        information is obtained by calling ``get_user_info``. The user
+        information must contain the keys ``language``, ``birthday``, and
+        ``country`` and must align with the values set in the user's Nintendo
+        account. The user agent is optional, and if not provided, the default
+        user agent will be used. It is not recommended to change the user agent
+        from the default unless you know what you are doing.
+
+        Args:
+            gtoken (str): GameWebToken, also known as gtoken. Given by Nintendo.
+                This token is required to make any requests to Nintendo Switch
+                Online services and is valid for 2 hours after it is obtained.
+            user_info (dict): Dictionary containing the user's information. This
+                must contain the keys ``language``, ``birthday``, and
+                ``country`` and must align with the values set in the user's
+                Nintendo account. These values are verified by Nintendo, so if
+                they do not align, no bullet token will be generated.
+            user_agent (str | None): User agent to use for the request. This is
+                optional, and if not provided, the default user agent will be
+                used. It is not recommended to change the user agent from the
+                default unless you know what you are doing. The default user
+                agent can be found in ``constants.py`` as
+                ``DEFAULT_USER_AGENT``. Defaults to None.
+
+        Raises:
+            SplatNetException: Error 401, ``ERROR_INVALID_GAME_WEB_TOKEN``. This
+                indicates that the gtoken is invalid. This can happen if the
+                gtoken is expired or if the provided gtoken was never valid.
+            SplatNetException: Error 403 ``ERROR_OBSOLETE_VERSION``. This
+                indicates that the version provided in request header key
+                ``X-Web-View-Ver`` is outdated. This can happen if the version
+                provided is too old.
+            SplatNetException: Error 204, ``USER_NOT_REGISTERED``. This
+                indicates that there is no game user associated with Splatoon 3,
+                and that the user must play at least one match of Splatoon 3
+                before using this library.
+            NintendoException: If the request does not fail with one of the
+                above errors, this indicates that the request failed for some
+                other reason and this exception will be raised to indicate that
+                the request failed silently.
+
+        Returns:
+            str: The bullet token. This token is required to make any requests
+                to SplatNet 3, and is valid for 6 hours and 30 minutes after it
+                is obtained.
+        """
+        logging.info("Getting bullet token")
+        user_agent = (
+            user_agent if user_agent is not None else DEFAULT_USER_AGENT
+        )
+        header = {
+            "Content-Length": "0",
+            "Content-Type": "application/json",
+            "Accept-Language": user_info["language"],
+            "User-Agent": user_agent,
+            "X-Web-View-Ver": self.splatnet_web_version,
+            "X-NACOUNTRY": user_info["country"],
+            "Accept": "*/*",
+            "Origin": SPLATNET_URL,
+            "X-Requested-With": "com.nintendo.znca",
+        }
+        cookies = {
+            "_gtoken": gtoken,
+            "_dnt": "1",
+        }
+        url = SPLATNET_URL + "/api/bullet_tokens"
+        response = self.session.post(url, headers=header, cookies=cookies)
+
+        if response.status_code == 401:
+            raise SplatNetException(
+                "Error 401: Invalid Game Web Token (gtoken)"
+            )
+        elif response.status_code == 403:
+            raise SplatNetException("Error 403: Outdated Version")
+        elif response.status_code == 204:
+            raise SplatNetException(
+                "Error 204: User Not Registered. Please play at least one match"
+                + " of Splatoon 3 before using this library."
+            )
+
+        try:
+            return response.json()["bulletToken"]
+        except KeyError:
+            raise NintendoException("Invalid response from Nintendo")
+
+    @property
+    def splatnet_web_version(self) -> str:
+        """Get the web view version for SplatNet 3. This is used in the request
+        header key ``X-Web-View-Ver`` to indicate the version of the web view
+        that is being used. This is required to make any requests to SplatNet
+        3. If the version cannot be obtained, a fallback version will be used.
+
+        Returns:
+            str: The web view version for SplatNet 3.
+        """
+        if self._web_view_version is not None:
+            return self._web_view_version
+        try:
+            web_version = get_splatnet_version()
+            self._web_view_version = web_version
+            return web_version
+        except SplatNetException as e:
+            logging.warning(str(e))
+            logging.warning("Using fallback web view version")
+            return WEB_VIEW_VERSION_FALLBACK
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/auth/token_manager.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/auth/token_manager.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,702 +1,702 @@
-import configparser
-import json
-import os
-import re
-import time
-from typing import Any, Literal, cast, overload
-
-import requests
-
-from splatnet3_scraper import __version__
-from splatnet3_scraper.auth.environment_manager import (
-    EnvironmentVariablesManager,
-)
-from splatnet3_scraper.auth.exceptions import (
-    NintendoException,
-    SplatNetException,
-)
-from splatnet3_scraper.auth.graph_ql_queries import queries
-from splatnet3_scraper.auth.nso import NSO
-from splatnet3_scraper.constants import (
-    ENV_VAR_NAMES,
-    GRAPH_QL_REFERENCE_URL,
-    TOKEN_EXPIRATIONS,
-    TOKENS,
-)
-from splatnet3_scraper.utils import retry
-
-text_config_re = re.compile(r"\s*=*\s*")
-
-
-class Token:
-    """Class that represents a token. This class is meant to store the token
-    itself, the type of token it is, and the time it was created. It can be used
-    to check if the token is expired or display the time left before it expires.
-    It also provides convenience methods for getting all sorts of metadata about
-    the token.
-    """
-
-    def __init__(self, token: str, token_type: str, timestamp: float) -> None:
-        """Initializes a ``Token`` object. The expiration time is calculated
-        based on the token type, with a default of ``1e10`` seconds (about 316
-        days, this should be basically forever for all intents and purposes; if
-        you have a python session running for that long, you have bigger
-        problems than a token expiring).
-
-        Args:
-            token (str): The value of the token, this is the actual token.
-            token_type (str): The type of token, this is used to identify which
-                type of token it represents, making it easier for the manager
-                to handle the tokens when searching for a specific one. It also
-                determines the expiration time of the token.
-            timestamp (float): The time the token was created, in seconds since
-                the epoch. This is used to determine if the token is expired.
-        """
-        self.token = token
-        self.token_type = token_type
-        self.timestamp = timestamp
-        self.expiration = TOKEN_EXPIRATIONS.get(token_type, 1e10) + timestamp
-
-    @property
-    def is_valid(self) -> bool:
-        """A very rudimentary check to see if the token is valid. This is not
-        a guarantee that the token is valid, but it is a good indicator that
-        it is for most cases. It checks if the token is not None and if it is
-        not an empty string. This usually means that the token is valid, but
-        it is not a guarantee. This is also here in case a future version of
-        the API requires a different check to determine if a token is valid.
-
-        Returns:
-            bool: True if the token is valid (not None and not an empty string)
-                False otherwise.
-        """
-        return (self.token is not None) and (self.token != "")
-
-    @property
-    def is_expired(self) -> bool:
-        """Checks if the token is expired. This is done by comparing the
-        current time to the expiration time of the token. If the current time
-        is greater than the expiration time, the token is expired. This is not
-        a guarantee that the token is expired, but it is a good indicator that
-        it is for most cases.
-
-        Returns:
-            bool: True if the token is expired, False otherwise.
-        """
-        return self.time_left <= 0
-
-    @property
-    def time_left(self) -> float:
-        """Returns the time left before the token expires. If the token is
-        expired, a negative number will be returned. This is not a guarantee
-        that the token is expired, but it is a good indicator that it is for
-        most cases.
-
-        Returns:
-            float: The time left before the token expires.
-        """
-        return self.expiration - time.time()
-
-    @property
-    def time_left_str(self) -> str:
-        """A string representation of the time left before the token expires.
-        If the token is expired, "Expired" will be returned. This is not a
-        guarantee that the token is expired, but it is a good indicator that
-        it is for most cases. If the time left is greater than 100,000 hours,
-        "basically forever" will be returned. If you have a python session
-        running for that long, you have bigger problems than a token expiring.
-
-        Returns:
-            str: A string representation of the time left before the token
-                expires.
-        """
-        time_left = self.time_left
-        if time_left <= 0:
-            return "Expired"
-        mins, secs = divmod(time_left, 60)
-        hours, mins = divmod(mins, 60)
-
-        out = ""
-        if hours > 1e5:
-            return "basically forever"
-        if hours > 0:
-            out += f"{hours:.0f}h "
-        if mins > 0:
-            out += f"{mins:.0f}m "
-        if secs > 0:
-            out += f"{secs:.1f}s"
-        return out.strip()
-
-    def __repr__(self) -> str:
-        out = "Token("
-        spaces = " " * len(out)
-        out += (
-            f"token={self.token[:5]}...,\n"
-            + spaces
-            + f"type={self.token_type},\n"
-            + spaces
-            + "expires in "
-            + self.time_left_str
-            + "\n)"
-        )
-        return out
-
-
-class TokenManager:
-    """Class that manages tokens. This class can be used to add tokens, generate
-    tokens from the ``NSO`` class, check if tokens are expired, load tokens from
-    a configuration file or environment variables, save tokens to disk, and
-    display the time left before tokens expire among other things.
-    """
-
-    def __init__(
-        self,
-        nso: NSO | None = None,
-        *args,
-        env_manager: EnvironmentVariablesManager | None = None,
-    ) -> None:
-        """Initializes a TokenManager object. This will create a new instance
-        of the NSO class if one is not provided.
-
-        Args:
-            nso (NSO | None, optional): An instance of the NSO class. If one is
-                not provided, a new instance will be created. Defaults to None.
-            *args: Additional arguments to pass to the NSO class, currently not
-                used.
-            env_manager (EnvironmentVariablesManager): An instance of the
-                EnvironmentVariablesManager class or a subclass of it. If not
-                provided, a new instance will be created.
-        """
-        nso = nso if nso is not None else NSO.new_instance()
-        self.nso = nso
-        self._tokens: dict[str, Token] = {}
-        self._data: dict[str, str] = {}
-        self.env_manager = (
-            env_manager
-            if env_manager is not None
-            else EnvironmentVariablesManager()
-        )
-
-    def flag_origin(self, origin: str, data: str | None = None) -> None:
-        """Flags the origin of the token manager. This is used to identify where
-        the token manager was loaded from, if anywhere. This is used to help
-        keep track of whether the user wants to save the tokens to disk or not,
-        but can potentially be used for other things in the future. This is
-        called automatically when the token manager is loaded from a config
-        file or environment variables. Subsequent calls to this method will
-        overwrite the previous origin.
-
-        Args:
-            origin (str): The origin of the token manager.
-            data (str | None): Additional data about the origin. For example,
-                if the token manager was loaded from a config file, this would
-                be the path to the config file. On the other hand, if the token
-                manager was loaded from environment variables, this would be
-                None.
-        """
-        self._origin = {"origin": origin, "data": data}
-
-    @property
-    def origin(self) -> dict[str, str | None]:
-        """Gets the origin of the token manager.
-
-        This method is a thin wrapper around the ``_origin`` attribute. If the
-        attribute does not exist, this method will return an empty dictionary
-        but will not create the attribute. The attribute will only be created
-        when the ``flag_origin`` method is called.
-
-        Returns:
-            dict[str, str | None]: The origin of the token manager. This will
-                be a dictionary with two keys: ``origin`` and ``data``. The
-                ``origin`` key will contain a string that describes where the
-                token manager was loaded from. The ``data`` key will contain
-                additional data about the origin. For example, if the token
-                manager was loaded from a config file, this would be the path
-                to the config file. On the other hand, if the token manager was
-                loaded from environment variables, this would be None.
-        """
-        return getattr(self, "_origin", {})
-
-    def add_token(
-        self,
-        token: str | Token,
-        token_type: str | None = None,
-        timestamp: float | None = None,
-    ) -> None:
-        """Adds a token to the manager. If the token provided is a ``string``,
-        the token type must be provided as well. The manager will then create a
-        new Token object and add it to its internal dictionary. If the token
-        provided is a ``Token`` object, the object will be added to the manager
-        as is.
-
-        If the token type is ``session_token``, the token will
-
-        Args:
-            token (str | Token): The token to add to the manager. If a string,
-                the token type must be provided as well. If a ``Token`` object,
-                the token type will be ignored. This field might also be known
-                as the "access token" or "auth token" among other names.
-            token_type (str | None): The type of token. If token is an instance
-                of ``Token``, this will be ignored. If token is a string, this
-                must be provided. Currently the only supported token types that
-                are recognized by the manager are "session_token", "gtoken", and
-                "bullet_token". Defaults to None, which will cause an error to
-                be raised if ``token`` is a string.
-            timestamp (float | None): The time the token was created. If not
-                provided, the current time will be used.
-
-        Raises:
-            ValueError: If the ``token`` provided is a string and ``token_type``
-                is not provided.
-        """
-        if timestamp is None:
-            timestamp = time.time()
-        if isinstance(token, str) and token_type is None:
-            raise ValueError(
-                "arg token_type must be provided if token is a str."
-            )
-        elif isinstance(token, str) and token_type is not None:
-            token_object = Token(token, token_type, timestamp)
-        elif isinstance(token, Token):
-            token_object = token
-
-        self._tokens[token_object.token_type] = token_object
-        if token_object.token_type == TOKENS.GTOKEN:
-            self.nso._gtoken = token_object.token
-        elif token_object.token_type == TOKENS.SESSION_TOKEN:
-            self.nso._session_token = token_object.token
-
-        return
-
-    @overload
-    def get(self, token_type: str, full_token: Literal[False] = ...) -> str:
-        ...
-
-    @overload
-    def get(self, token_type: str, full_token: Literal[True]) -> Token:
-        ...
-
-    @overload
-    def get(self, token_type: str, full_token: bool) -> str | Token:
-        ...
-
-    def get(self, token_type: str, full_token: bool = False) -> str | Token:
-        """Gets a token from the manager given a token type.
-
-        If ``full_token`` is True, the full ``Token`` object will be returned.
-        Otherwise, just the value of the token will be returned. If the token
-        type is not found, a ValueError will be raised.
-
-        Args:
-            token_type (str): The type of the token to get, as defined in the
-                ``Token.token_type`` field.
-            full_token (bool): Whether to return the full ``Token`` object or
-                just the value of the token. Defaults to False.
-
-        Raises:
-            ValueError: If the given token type is not found in the manager.
-
-        Returns:
-            str | Token: The token, either as a string or a ``Token`` object as
-                defined by the ``full_token`` argument.
-        """
-        token_obj = self._tokens.get(token_type, None)
-        if token_obj is None:
-            raise ValueError(f"Token of type {token_type} not found.")
-        if full_token:
-            return token_obj
-        return token_obj.token
-
-    @property
-    def data(self) -> dict[str, Any]:
-        """Returns the full data stored in the manager as a dictionary. This
-        data is not the same as the tokens stored in the manager, but rather
-        additional data that can be used in other places. Examples of keys that
-        might be stored in this dictionary are the user's ``country``, and
-        ``language`` as defined by the Nintendo Account.
-
-        Returns:
-            dict[str, Any]: The data stored in the manager as a dictionary.
-        """
-        return self._data
-
-    def add_session_token(self, token: str) -> None:
-        """Adds a session token to the manager. This is a convenience method
-        that will also set the session token in the NSO class. This
-        functionality is already present in the ``add_token`` method, so this
-        method might be removed in the future.
-
-        Args:
-            token (str): The session token to add to the manager. This field
-                might also be known as the "access token" or "auth token" among
-                other names. This token is used to authenticate with Nintendo
-                services, and is required to query the SplatNet 3 API.
-        """
-        self.add_token(token, TOKENS.SESSION_TOKEN)
-        self.nso._session_token = token
-
-    def generate_gtoken(self) -> None:
-        """Generates a new gtoken from the internal NSO class and adds it to the
-        manager. This is a convenience method that will also set the gtoken in
-        the NSO class. This function requires a session token to already be
-        set, and will raise a ValueError if it is not.
-
-        Raises:
-            ValueError: If the session token has not been set.
-            NintendoException: In the unlikely event that the gtoken has made it
-                through the NSO class but the user info was not set, this error
-                provides a safety net to identify that there was a problem with
-                the gtoken generation. Should not be raised in normal use.
-        """
-        if TOKENS.SESSION_TOKEN not in self._tokens:
-            raise ValueError(
-                "Session token must be set before generating a gtoken."
-            )
-        gtoken = self.nso.get_gtoken(self.nso.session_token)
-        self.add_token(gtoken, TOKENS.GTOKEN)
-        try:
-            user_info = cast(dict[str, str], self.nso._user_info)
-            country = user_info["country"]
-            language = user_info["language"]
-            self._data["country"] = country
-            self._data["language"] = language
-        except (KeyError, TypeError):
-            raise NintendoException(
-                "Unable to get user info. Gtoken may be invalid."
-            )
-
-    @retry(times=1, exceptions=SplatNetException)
-    def generate_bullet_token(self) -> None:
-        """Generates a new bullet token from the internal NSO class and adds it
-        to the manager. This is a convenience method that will also generate a
-        ``gtoken`` if one has not already been generated, or if the user info
-        has not been set. This function requires a session token to already be
-        set, and will raise a ValueError if it is not. If the bullet token is
-        unable to be generated, a SplatNetException will be raised.
-
-        Raises:
-            ValueError: If the session token has not been set.
-            SplatNetException: If the bullet token was unable to be generated.
-        """
-        if TOKENS.SESSION_TOKEN not in self._tokens:
-            raise ValueError(
-                "Session token must be set before generating a bullet token."
-            )
-        if (TOKENS.GTOKEN not in self._tokens) or (self.nso._user_info is None):
-            self.generate_gtoken()
-        bullet_token = self.nso.get_bullet_token(
-            cast(str, self.nso._gtoken), cast(dict, self.nso._user_info)
-        )
-        self.add_token(bullet_token, TOKENS.BULLET_TOKEN)
-        bullet = self.get(TOKENS.BULLET_TOKEN, full_token=True)
-        if (bullet is not None) and not bullet.is_valid:
-            raise SplatNetException(
-                "Bullet token was unable to be generated. This is likely due "
-                "to SplatNet 3 being down. Please try again later."
-            )
-
-    def generate_all_tokens(self) -> None:
-        """Generates all tokens that can be generated from the manager. This
-        is a convenience method that will call the ``generate_gtoken`` and
-        ``generate_bullet_token`` methods in order. This function requires a
-        session token to already be set, and will raise the errors that those
-        methods raise if a session token is not set.
-        """
-        self.generate_gtoken()
-        self.generate_bullet_token()
-
-    @classmethod
-    def from_session_token(cls, session_token: str) -> "TokenManager":
-        """Creates a token manager from a session token.
-
-        Given a session token, this method will create a token manager and add
-        a session token to it. Additionally, it will flag the origin of the
-        session token as "session_token" so that it can be saved to a config
-        file later.
-
-        Args:
-            session_token (str): The session token to use to instantiate the
-                ``TokenManager``.
-
-        Returns:
-            TokenManager: The token manager with the session token added.
-        """
-        manager = cls()
-        manager.add_session_token(session_token)
-        manager.flag_origin("session_token")
-        return manager
-
-    @classmethod
-    def load(cls) -> "TokenManager":
-        """Loads tokens from a config file or environment variables.
-
-        Checks for appropriate tokens in the following order:
-            1. .splatnet3_scraper file
-            2. Environment variables
-            3. tokens.ini file
-
-        Raises:
-            ValueError: If no tokens are found.
-
-        Returns:
-            TokenManager: The token manager with the tokens loaded.
-        """
-        if os.path.exists(".splatnet3_scraper"):
-            return cls.from_config_file(".splatnet3_scraper")
-        elif any([os.environ.get(var) for var in ENV_VAR_NAMES.values()]):
-            return cls.from_env()
-        elif os.path.exists("tokens.ini"):
-            return cls.from_config_file("tokens.ini")
-        else:
-            raise ValueError(
-                "No tokens found. Please create a .splatnet3_scraper file, set "
-                "environment variables, or create a tokens.ini file."
-            )
-
-    @classmethod
-    def from_config_file(cls, path: str) -> "TokenManager":
-        """Loads tokens from a config file.
-
-        Given a path to a config file, this method will create a token manager
-        and add the tokens found in the config file to it. Additionally, it
-        will flag the origin of the tokens as "config_file" so that they can be
-        saved to a config file later. The config file must be in the format of
-        the standard ``configparser`` library, and must have a "tokens" section.
-        The "tokens" section must have a "session_token" option, and may have
-        "gtoken" and "bullet_token" options. An example config file is shown
-        below:
-
-        >>> [tokens]
-        ... session_token = SESSION_TOKEN
-        ... gtoken = GTOKEN
-        ... bullet_token = BULLET_TOKEN
-        ...
-        ... [data]
-        ... country = US
-        ... language = en-US
-        ...
-        ... [options]
-        ... user_agent = USER_AGENT
-
-        Tests the tokens before returning the token manager using the
-        ``test_tokens`` method.
-
-        Args:
-            path (str): The path to the config file.
-
-        Raises:
-            ValueError: If the config file does not have a ``tokens`` section.
-
-        Returns:
-            TokenManager: A newly created token manager with the tokens loaded
-                and the origin of the token manager set to "config_file".
-        """
-        config = configparser.ConfigParser()
-        config.read(path)
-        nso = NSO.new_instance()
-        tokenmanager = cls(nso)
-        tokenmanager.flag_origin("config_file", path)
-
-        if not config.has_section("tokens"):
-            raise ValueError("Config file does not have a 'tokens' section.")
-        for option in config.options("tokens"):
-            token = config.get("tokens", option)
-            if option == TOKENS.SESSION_TOKEN:
-                nso._session_token = token
-            elif option == TOKENS.GTOKEN:
-                nso._gtoken = token
-            tokenmanager.add_token(token, option)
-
-        if not config.has_section("data"):
-            tokenmanager.generate_all_tokens()
-            return tokenmanager
-        for option in config.options("data"):
-            tokenmanager._data[option] = config.get("data", option)
-        tokenmanager.test_tokens()
-        return tokenmanager
-
-    @classmethod
-    def from_text_file(cls, path: str) -> "TokenManager":
-        """Loads tokens from a text file, particularly s3s config files. Not
-        recommended for use, but here for compatibility with s3s config files.
-
-        Requires the text file to be a JSON file that contains a "session_token"
-        key. The value of the "session_token" key will be used as the session
-        token. If the text file also contains an "acc_loc" key, the value of
-        the "acc_loc" key will be used to set the language and country of the
-        data in the token manager.
-
-        Tests the tokens before returning the token manager using the
-        ``test_tokens`` method.
-
-        Args:
-            path (str): The path to the text file.
-
-        Raises:
-            ValueError: If the session token is not found in the JSON file.
-
-        Returns:
-            TokenManager: The token manager with the tokens loaded.
-        """
-        token_manager = cls()
-        with open(path, "r") as f:
-            data = json.load(f)
-
-        if "session_token" not in data:
-            raise ValueError("Session token not found in text file.")
-        token_manager.add_session_token(data["session_token"])
-        token_manager.flag_origin("text_file", path)
-        if "acc_loc" in data:
-            language, country = data["acc_loc"].split("|")
-            token_manager._data["language"] = language
-            token_manager._data["country"] = country
-
-        if "gtoken" in data:
-            token_manager.add_token(data["gtoken"], TOKENS.GTOKEN)
-        if "bullettoken" in data:
-            token_manager.add_token(data["bullettoken"], TOKENS.BULLET_TOKEN)
-        token_manager.test_tokens()
-        return token_manager
-
-    @classmethod
-    def from_env(
-        cls, env_manager: EnvironmentVariablesManager | None = None
-    ) -> "TokenManager":
-        """Loads tokens from environment variables.
-
-        This method will create a token manager and add the tokens found in the
-        environment variables to it. The environment variables that are
-        supported are:
-
-        - SN3S_SESSION_TOKEN
-        - SN3S_GTOKEN
-        - SN3S_BULLET_TOKEN
-
-        The session token environment variable is required, and if it is not
-        set, a ValueError will be raised. The other environment variables are
-        optional and will be generated if they are not set.
-
-        Tests the tokens before returning the token manager using the
-        ``test_tokens`` method.
-
-        Args:
-            env_manager (EnvironmentVariablesManager): The environment variables
-                manager to use. If not provided, a new one will be created.
-
-        Raises:
-            ValueError: If the session token environment variable is not set.
-
-        Returns:
-            TokenManager: The token manager with the tokens loaded.
-        """
-        nso = NSO.new_instance()
-        tokenmanager = cls(nso, env_manager=env_manager)
-        tokens = tokenmanager.env_manager.get_all()
-        for token, value in tokens.items():
-            if token == TOKENS.SESSION_TOKEN:
-                if value is None:
-                    raise ValueError(
-                        "Session token environment variable not set."
-                    )
-                nso._session_token = value
-            elif value is None:
-                continue
-            elif token == TOKENS.GTOKEN:
-                nso._gtoken = value
-            tokenmanager.add_token(value, token)
-        tokenmanager.flag_origin("env")
-        tokenmanager.test_tokens()
-        return tokenmanager
-
-    def save(self, path: str | None = None) -> None:
-        """Saves the tokens to a config file.
-
-        Uses the ``configparser`` module to save the tokens to a config file.
-        The config file will be saved to the path specified by the `path`
-        argument. If the `path` argument is not specified, the config file
-        will be saved to the current working directory with the name
-        ``.splatnet3_scraper``. Does not consider the origin of the tokens, as
-        it is assumed that this method will only be called when the user wants
-        to save the tokens to disk.
-
-        Args:
-            path (str): The path to the config file.
-        """
-        config = configparser.ConfigParser()
-        out_tokens = {}
-        for token_name, token in self._tokens.items():
-            out_tokens[token_name] = token.token
-        config["tokens"] = out_tokens
-        config["data"] = self._data
-        config["metadata"] = {
-            "version": __version__,
-            "class": self.__class__.__name__,
-        }
-        if path is None:
-            path = ".splatnet3_scraper"
-        with open(path, "w") as configfile:
-            config.write(configfile)
-
-    def token_is_valid(self, token_type: str) -> bool:
-        """Given a token type, checks if the token is valid.
-
-        This method will check if the token is valid by checking if the token
-        is expired. This method will not regenerate the token if it is invalid.
-        As mentioned in the ``Token.is_valid`` property, this method will not
-        check if the token is valid by making a request to the API, but rather
-        checks if the token is likely to be expired by comparing the known
-        expiration time of the token to the current time. If the token type is
-        not found, this method will return False.
-
-        Args:
-            token_type (str): The type of token to check.
-
-        Returns:
-            bool: True if the token is valid, False otherwise.
-        """
-        try:
-            token = self.get(token_type, full_token=True)
-        except ValueError:
-            return False
-        return token.is_valid
-
-    def test_tokens(self, user_agent: str | None = None) -> None:
-        """Tests the tokens.
-
-        Checks using the ``token_is_valid`` method to see whether the tokens
-        need to be regenerated. If so, the tokens will be regenerated with the
-        appropriate ``generate_*`` method. Once the tokens are regenerated, it
-        will make a request to the API to check if the tokens are valid. If the
-        request fails, the ``generate_all_tokens`` method will be called. If the
-        requests succeeds, nothing will happen. Once this method is called, the
-        TokenManager can be assumed to have valid tokens and can be used to make
-        requests to the API.
-
-        Args:
-            user_agent (str): The user agent to use when making the request to
-                the API. If not specified, the default user agent will be used.
-
-        Raises:
-            ValueError: If the session token is not set.
-        """
-        if self.get(TOKENS.SESSION_TOKEN) is None:
-            raise ValueError("Session Token is not set.")
-
-        if self.token_is_valid(TOKENS.GTOKEN) is False:
-            self.generate_gtoken()
-
-        if self.token_is_valid(TOKENS.BULLET_TOKEN) is False:
-            self.generate_bullet_token()
-
-        header = queries.query_header(
-            self.get(TOKENS.BULLET_TOKEN), self._data["language"], user_agent
-        )
-
-        response = requests.post(
-            GRAPH_QL_REFERENCE_URL,
-            data=queries.query_body("HomeQuery"),
-            headers=header,
-            cookies={"_gtoken": cast(str, self.get(TOKENS.GTOKEN))},
-        )
-        if response.status_code != 200:
-            self.generate_all_tokens()
+import configparser
+import json
+import os
+import re
+import time
+from typing import Any, Literal, cast, overload
+
+import requests
+
+from splatnet3_scraper import __version__
+from splatnet3_scraper.auth.environment_manager import (
+    EnvironmentVariablesManager,
+)
+from splatnet3_scraper.auth.exceptions import (
+    NintendoException,
+    SplatNetException,
+)
+from splatnet3_scraper.auth.graph_ql_queries import queries
+from splatnet3_scraper.auth.nso import NSO
+from splatnet3_scraper.constants import (
+    ENV_VAR_NAMES,
+    GRAPH_QL_REFERENCE_URL,
+    TOKEN_EXPIRATIONS,
+    TOKENS,
+)
+from splatnet3_scraper.utils import retry
+
+text_config_re = re.compile(r"\s*=*\s*")
+
+
+class Token:
+    """Class that represents a token. This class is meant to store the token
+    itself, the type of token it is, and the time it was created. It can be used
+    to check if the token is expired or display the time left before it expires.
+    It also provides convenience methods for getting all sorts of metadata about
+    the token.
+    """
+
+    def __init__(self, token: str, token_type: str, timestamp: float) -> None:
+        """Initializes a ``Token`` object. The expiration time is calculated
+        based on the token type, with a default of ``1e10`` seconds (about 316
+        days, this should be basically forever for all intents and purposes; if
+        you have a python session running for that long, you have bigger
+        problems than a token expiring).
+
+        Args:
+            token (str): The value of the token, this is the actual token.
+            token_type (str): The type of token, this is used to identify which
+                type of token it represents, making it easier for the manager
+                to handle the tokens when searching for a specific one. It also
+                determines the expiration time of the token.
+            timestamp (float): The time the token was created, in seconds since
+                the epoch. This is used to determine if the token is expired.
+        """
+        self.token = token
+        self.token_type = token_type
+        self.timestamp = timestamp
+        self.expiration = TOKEN_EXPIRATIONS.get(token_type, 1e10) + timestamp
+
+    @property
+    def is_valid(self) -> bool:
+        """A very rudimentary check to see if the token is valid. This is not
+        a guarantee that the token is valid, but it is a good indicator that
+        it is for most cases. It checks if the token is not None and if it is
+        not an empty string. This usually means that the token is valid, but
+        it is not a guarantee. This is also here in case a future version of
+        the API requires a different check to determine if a token is valid.
+
+        Returns:
+            bool: True if the token is valid (not None and not an empty string)
+                False otherwise.
+        """
+        return (self.token is not None) and (self.token != "")
+
+    @property
+    def is_expired(self) -> bool:
+        """Checks if the token is expired. This is done by comparing the
+        current time to the expiration time of the token. If the current time
+        is greater than the expiration time, the token is expired. This is not
+        a guarantee that the token is expired, but it is a good indicator that
+        it is for most cases.
+
+        Returns:
+            bool: True if the token is expired, False otherwise.
+        """
+        return self.time_left <= 0
+
+    @property
+    def time_left(self) -> float:
+        """Returns the time left before the token expires. If the token is
+        expired, a negative number will be returned. This is not a guarantee
+        that the token is expired, but it is a good indicator that it is for
+        most cases.
+
+        Returns:
+            float: The time left before the token expires.
+        """
+        return self.expiration - time.time()
+
+    @property
+    def time_left_str(self) -> str:
+        """A string representation of the time left before the token expires.
+        If the token is expired, "Expired" will be returned. This is not a
+        guarantee that the token is expired, but it is a good indicator that
+        it is for most cases. If the time left is greater than 100,000 hours,
+        "basically forever" will be returned. If you have a python session
+        running for that long, you have bigger problems than a token expiring.
+
+        Returns:
+            str: A string representation of the time left before the token
+                expires.
+        """
+        time_left = self.time_left
+        if time_left <= 0:
+            return "Expired"
+        mins, secs = divmod(time_left, 60)
+        hours, mins = divmod(mins, 60)
+
+        out = ""
+        if hours > 1e5:
+            return "basically forever"
+        if hours > 0:
+            out += f"{hours:.0f}h "
+        if mins > 0:
+            out += f"{mins:.0f}m "
+        if secs > 0:
+            out += f"{secs:.1f}s"
+        return out.strip()
+
+    def __repr__(self) -> str:
+        out = "Token("
+        spaces = " " * len(out)
+        out += (
+            f"token={self.token[:5]}...,\n"
+            + spaces
+            + f"type={self.token_type},\n"
+            + spaces
+            + "expires in "
+            + self.time_left_str
+            + "\n)"
+        )
+        return out
+
+
+class TokenManager:
+    """Class that manages tokens. This class can be used to add tokens, generate
+    tokens from the ``NSO`` class, check if tokens are expired, load tokens from
+    a configuration file or environment variables, save tokens to disk, and
+    display the time left before tokens expire among other things.
+    """
+
+    def __init__(
+        self,
+        nso: NSO | None = None,
+        *args,
+        env_manager: EnvironmentVariablesManager | None = None,
+    ) -> None:
+        """Initializes a TokenManager object. This will create a new instance
+        of the NSO class if one is not provided.
+
+        Args:
+            nso (NSO | None, optional): An instance of the NSO class. If one is
+                not provided, a new instance will be created. Defaults to None.
+            *args: Additional arguments to pass to the NSO class, currently not
+                used.
+            env_manager (EnvironmentVariablesManager): An instance of the
+                EnvironmentVariablesManager class or a subclass of it. If not
+                provided, a new instance will be created.
+        """
+        nso = nso if nso is not None else NSO.new_instance()
+        self.nso = nso
+        self._tokens: dict[str, Token] = {}
+        self._data: dict[str, str] = {}
+        self.env_manager = (
+            env_manager
+            if env_manager is not None
+            else EnvironmentVariablesManager()
+        )
+
+    def flag_origin(self, origin: str, data: str | None = None) -> None:
+        """Flags the origin of the token manager. This is used to identify where
+        the token manager was loaded from, if anywhere. This is used to help
+        keep track of whether the user wants to save the tokens to disk or not,
+        but can potentially be used for other things in the future. This is
+        called automatically when the token manager is loaded from a config
+        file or environment variables. Subsequent calls to this method will
+        overwrite the previous origin.
+
+        Args:
+            origin (str): The origin of the token manager.
+            data (str | None): Additional data about the origin. For example,
+                if the token manager was loaded from a config file, this would
+                be the path to the config file. On the other hand, if the token
+                manager was loaded from environment variables, this would be
+                None.
+        """
+        self._origin = {"origin": origin, "data": data}
+
+    @property
+    def origin(self) -> dict[str, str | None]:
+        """Gets the origin of the token manager.
+
+        This method is a thin wrapper around the ``_origin`` attribute. If the
+        attribute does not exist, this method will return an empty dictionary
+        but will not create the attribute. The attribute will only be created
+        when the ``flag_origin`` method is called.
+
+        Returns:
+            dict[str, str | None]: The origin of the token manager. This will
+                be a dictionary with two keys: ``origin`` and ``data``. The
+                ``origin`` key will contain a string that describes where the
+                token manager was loaded from. The ``data`` key will contain
+                additional data about the origin. For example, if the token
+                manager was loaded from a config file, this would be the path
+                to the config file. On the other hand, if the token manager was
+                loaded from environment variables, this would be None.
+        """
+        return getattr(self, "_origin", {})
+
+    def add_token(
+        self,
+        token: str | Token,
+        token_type: str | None = None,
+        timestamp: float | None = None,
+    ) -> None:
+        """Adds a token to the manager. If the token provided is a ``string``,
+        the token type must be provided as well. The manager will then create a
+        new Token object and add it to its internal dictionary. If the token
+        provided is a ``Token`` object, the object will be added to the manager
+        as is.
+
+        If the token type is ``session_token``, the token will
+
+        Args:
+            token (str | Token): The token to add to the manager. If a string,
+                the token type must be provided as well. If a ``Token`` object,
+                the token type will be ignored. This field might also be known
+                as the "access token" or "auth token" among other names.
+            token_type (str | None): The type of token. If token is an instance
+                of ``Token``, this will be ignored. If token is a string, this
+                must be provided. Currently the only supported token types that
+                are recognized by the manager are "session_token", "gtoken", and
+                "bullet_token". Defaults to None, which will cause an error to
+                be raised if ``token`` is a string.
+            timestamp (float | None): The time the token was created. If not
+                provided, the current time will be used.
+
+        Raises:
+            ValueError: If the ``token`` provided is a string and ``token_type``
+                is not provided.
+        """
+        if timestamp is None:
+            timestamp = time.time()
+        if isinstance(token, str) and token_type is None:
+            raise ValueError(
+                "arg token_type must be provided if token is a str."
+            )
+        elif isinstance(token, str) and token_type is not None:
+            token_object = Token(token, token_type, timestamp)
+        elif isinstance(token, Token):
+            token_object = token
+
+        self._tokens[token_object.token_type] = token_object
+        if token_object.token_type == TOKENS.GTOKEN:
+            self.nso._gtoken = token_object.token
+        elif token_object.token_type == TOKENS.SESSION_TOKEN:
+            self.nso._session_token = token_object.token
+
+        return
+
+    @overload
+    def get(self, token_type: str, full_token: Literal[False] = ...) -> str:
+        ...
+
+    @overload
+    def get(self, token_type: str, full_token: Literal[True]) -> Token:
+        ...
+
+    @overload
+    def get(self, token_type: str, full_token: bool) -> str | Token:
+        ...
+
+    def get(self, token_type: str, full_token: bool = False) -> str | Token:
+        """Gets a token from the manager given a token type.
+
+        If ``full_token`` is True, the full ``Token`` object will be returned.
+        Otherwise, just the value of the token will be returned. If the token
+        type is not found, a ValueError will be raised.
+
+        Args:
+            token_type (str): The type of the token to get, as defined in the
+                ``Token.token_type`` field.
+            full_token (bool): Whether to return the full ``Token`` object or
+                just the value of the token. Defaults to False.
+
+        Raises:
+            ValueError: If the given token type is not found in the manager.
+
+        Returns:
+            str | Token: The token, either as a string or a ``Token`` object as
+                defined by the ``full_token`` argument.
+        """
+        token_obj = self._tokens.get(token_type, None)
+        if token_obj is None:
+            raise ValueError(f"Token of type {token_type} not found.")
+        if full_token:
+            return token_obj
+        return token_obj.token
+
+    @property
+    def data(self) -> dict[str, Any]:
+        """Returns the full data stored in the manager as a dictionary. This
+        data is not the same as the tokens stored in the manager, but rather
+        additional data that can be used in other places. Examples of keys that
+        might be stored in this dictionary are the user's ``country``, and
+        ``language`` as defined by the Nintendo Account.
+
+        Returns:
+            dict[str, Any]: The data stored in the manager as a dictionary.
+        """
+        return self._data
+
+    def add_session_token(self, token: str) -> None:
+        """Adds a session token to the manager. This is a convenience method
+        that will also set the session token in the NSO class. This
+        functionality is already present in the ``add_token`` method, so this
+        method might be removed in the future.
+
+        Args:
+            token (str): The session token to add to the manager. This field
+                might also be known as the "access token" or "auth token" among
+                other names. This token is used to authenticate with Nintendo
+                services, and is required to query the SplatNet 3 API.
+        """
+        self.add_token(token, TOKENS.SESSION_TOKEN)
+        self.nso._session_token = token
+
+    def generate_gtoken(self) -> None:
+        """Generates a new gtoken from the internal NSO class and adds it to the
+        manager. This is a convenience method that will also set the gtoken in
+        the NSO class. This function requires a session token to already be
+        set, and will raise a ValueError if it is not.
+
+        Raises:
+            ValueError: If the session token has not been set.
+            NintendoException: In the unlikely event that the gtoken has made it
+                through the NSO class but the user info was not set, this error
+                provides a safety net to identify that there was a problem with
+                the gtoken generation. Should not be raised in normal use.
+        """
+        if TOKENS.SESSION_TOKEN not in self._tokens:
+            raise ValueError(
+                "Session token must be set before generating a gtoken."
+            )
+        gtoken = self.nso.get_gtoken(self.nso.session_token)
+        self.add_token(gtoken, TOKENS.GTOKEN)
+        try:
+            user_info = cast(dict[str, str], self.nso._user_info)
+            country = user_info["country"]
+            language = user_info["language"]
+            self._data["country"] = country
+            self._data["language"] = language
+        except (KeyError, TypeError):
+            raise NintendoException(
+                "Unable to get user info. Gtoken may be invalid."
+            )
+
+    @retry(times=1, exceptions=SplatNetException)
+    def generate_bullet_token(self) -> None:
+        """Generates a new bullet token from the internal NSO class and adds it
+        to the manager. This is a convenience method that will also generate a
+        ``gtoken`` if one has not already been generated, or if the user info
+        has not been set. This function requires a session token to already be
+        set, and will raise a ValueError if it is not. If the bullet token is
+        unable to be generated, a SplatNetException will be raised.
+
+        Raises:
+            ValueError: If the session token has not been set.
+            SplatNetException: If the bullet token was unable to be generated.
+        """
+        if TOKENS.SESSION_TOKEN not in self._tokens:
+            raise ValueError(
+                "Session token must be set before generating a bullet token."
+            )
+        if (TOKENS.GTOKEN not in self._tokens) or (self.nso._user_info is None):
+            self.generate_gtoken()
+        bullet_token = self.nso.get_bullet_token(
+            cast(str, self.nso._gtoken), cast(dict, self.nso._user_info)
+        )
+        self.add_token(bullet_token, TOKENS.BULLET_TOKEN)
+        bullet = self.get(TOKENS.BULLET_TOKEN, full_token=True)
+        if (bullet is not None) and not bullet.is_valid:
+            raise SplatNetException(
+                "Bullet token was unable to be generated. This is likely due "
+                "to SplatNet 3 being down. Please try again later."
+            )
+
+    def generate_all_tokens(self) -> None:
+        """Generates all tokens that can be generated from the manager. This
+        is a convenience method that will call the ``generate_gtoken`` and
+        ``generate_bullet_token`` methods in order. This function requires a
+        session token to already be set, and will raise the errors that those
+        methods raise if a session token is not set.
+        """
+        self.generate_gtoken()
+        self.generate_bullet_token()
+
+    @classmethod
+    def from_session_token(cls, session_token: str) -> "TokenManager":
+        """Creates a token manager from a session token.
+
+        Given a session token, this method will create a token manager and add
+        a session token to it. Additionally, it will flag the origin of the
+        session token as "session_token" so that it can be saved to a config
+        file later.
+
+        Args:
+            session_token (str): The session token to use to instantiate the
+                ``TokenManager``.
+
+        Returns:
+            TokenManager: The token manager with the session token added.
+        """
+        manager = cls()
+        manager.add_session_token(session_token)
+        manager.flag_origin("session_token")
+        return manager
+
+    @classmethod
+    def load(cls) -> "TokenManager":
+        """Loads tokens from a config file or environment variables.
+
+        Checks for appropriate tokens in the following order:
+            1. .splatnet3_scraper file
+            2. Environment variables
+            3. tokens.ini file
+
+        Raises:
+            ValueError: If no tokens are found.
+
+        Returns:
+            TokenManager: The token manager with the tokens loaded.
+        """
+        if os.path.exists(".splatnet3_scraper"):
+            return cls.from_config_file(".splatnet3_scraper")
+        elif any([os.environ.get(var) for var in ENV_VAR_NAMES.values()]):
+            return cls.from_env()
+        elif os.path.exists("tokens.ini"):
+            return cls.from_config_file("tokens.ini")
+        else:
+            raise ValueError(
+                "No tokens found. Please create a .splatnet3_scraper file, set "
+                "environment variables, or create a tokens.ini file."
+            )
+
+    @classmethod
+    def from_config_file(cls, path: str) -> "TokenManager":
+        """Loads tokens from a config file.
+
+        Given a path to a config file, this method will create a token manager
+        and add the tokens found in the config file to it. Additionally, it
+        will flag the origin of the tokens as "config_file" so that they can be
+        saved to a config file later. The config file must be in the format of
+        the standard ``configparser`` library, and must have a "tokens" section.
+        The "tokens" section must have a "session_token" option, and may have
+        "gtoken" and "bullet_token" options. An example config file is shown
+        below:
+
+        >>> [tokens]
+        ... session_token = SESSION_TOKEN
+        ... gtoken = GTOKEN
+        ... bullet_token = BULLET_TOKEN
+        ...
+        ... [data]
+        ... country = US
+        ... language = en-US
+        ...
+        ... [options]
+        ... user_agent = USER_AGENT
+
+        Tests the tokens before returning the token manager using the
+        ``test_tokens`` method.
+
+        Args:
+            path (str): The path to the config file.
+
+        Raises:
+            ValueError: If the config file does not have a ``tokens`` section.
+
+        Returns:
+            TokenManager: A newly created token manager with the tokens loaded
+                and the origin of the token manager set to "config_file".
+        """
+        config = configparser.ConfigParser()
+        config.read(path)
+        nso = NSO.new_instance()
+        tokenmanager = cls(nso)
+        tokenmanager.flag_origin("config_file", path)
+
+        if not config.has_section("tokens"):
+            raise ValueError("Config file does not have a 'tokens' section.")
+        for option in config.options("tokens"):
+            token = config.get("tokens", option)
+            if option == TOKENS.SESSION_TOKEN:
+                nso._session_token = token
+            elif option == TOKENS.GTOKEN:
+                nso._gtoken = token
+            tokenmanager.add_token(token, option)
+
+        if not config.has_section("data"):
+            tokenmanager.generate_all_tokens()
+            return tokenmanager
+        for option in config.options("data"):
+            tokenmanager._data[option] = config.get("data", option)
+        tokenmanager.test_tokens()
+        return tokenmanager
+
+    @classmethod
+    def from_text_file(cls, path: str) -> "TokenManager":
+        """Loads tokens from a text file, particularly s3s config files. Not
+        recommended for use, but here for compatibility with s3s config files.
+
+        Requires the text file to be a JSON file that contains a "session_token"
+        key. The value of the "session_token" key will be used as the session
+        token. If the text file also contains an "acc_loc" key, the value of
+        the "acc_loc" key will be used to set the language and country of the
+        data in the token manager.
+
+        Tests the tokens before returning the token manager using the
+        ``test_tokens`` method.
+
+        Args:
+            path (str): The path to the text file.
+
+        Raises:
+            ValueError: If the session token is not found in the JSON file.
+
+        Returns:
+            TokenManager: The token manager with the tokens loaded.
+        """
+        token_manager = cls()
+        with open(path, "r") as f:
+            data = json.load(f)
+
+        if "session_token" not in data:
+            raise ValueError("Session token not found in text file.")
+        token_manager.add_session_token(data["session_token"])
+        token_manager.flag_origin("text_file", path)
+        if "acc_loc" in data:
+            language, country = data["acc_loc"].split("|")
+            token_manager._data["language"] = language
+            token_manager._data["country"] = country
+
+        if "gtoken" in data:
+            token_manager.add_token(data["gtoken"], TOKENS.GTOKEN)
+        if "bullettoken" in data:
+            token_manager.add_token(data["bullettoken"], TOKENS.BULLET_TOKEN)
+        token_manager.test_tokens()
+        return token_manager
+
+    @classmethod
+    def from_env(
+        cls, env_manager: EnvironmentVariablesManager | None = None
+    ) -> "TokenManager":
+        """Loads tokens from environment variables.
+
+        This method will create a token manager and add the tokens found in the
+        environment variables to it. The environment variables that are
+        supported are:
+
+        - SN3S_SESSION_TOKEN
+        - SN3S_GTOKEN
+        - SN3S_BULLET_TOKEN
+
+        The session token environment variable is required, and if it is not
+        set, a ValueError will be raised. The other environment variables are
+        optional and will be generated if they are not set.
+
+        Tests the tokens before returning the token manager using the
+        ``test_tokens`` method.
+
+        Args:
+            env_manager (EnvironmentVariablesManager): The environment variables
+                manager to use. If not provided, a new one will be created.
+
+        Raises:
+            ValueError: If the session token environment variable is not set.
+
+        Returns:
+            TokenManager: The token manager with the tokens loaded.
+        """
+        nso = NSO.new_instance()
+        tokenmanager = cls(nso, env_manager=env_manager)
+        tokens = tokenmanager.env_manager.get_all()
+        for token, value in tokens.items():
+            if token == TOKENS.SESSION_TOKEN:
+                if value is None:
+                    raise ValueError(
+                        "Session token environment variable not set."
+                    )
+                nso._session_token = value
+            elif value is None:
+                continue
+            elif token == TOKENS.GTOKEN:
+                nso._gtoken = value
+            tokenmanager.add_token(value, token)
+        tokenmanager.flag_origin("env")
+        tokenmanager.test_tokens()
+        return tokenmanager
+
+    def save(self, path: str | None = None) -> None:
+        """Saves the tokens to a config file.
+
+        Uses the ``configparser`` module to save the tokens to a config file.
+        The config file will be saved to the path specified by the `path`
+        argument. If the `path` argument is not specified, the config file
+        will be saved to the current working directory with the name
+        ``.splatnet3_scraper``. Does not consider the origin of the tokens, as
+        it is assumed that this method will only be called when the user wants
+        to save the tokens to disk.
+
+        Args:
+            path (str): The path to the config file.
+        """
+        config = configparser.ConfigParser()
+        out_tokens = {}
+        for token_name, token in self._tokens.items():
+            out_tokens[token_name] = token.token
+        config["tokens"] = out_tokens
+        config["data"] = self._data
+        config["metadata"] = {
+            "version": __version__,
+            "class": self.__class__.__name__,
+        }
+        if path is None:
+            path = ".splatnet3_scraper"
+        with open(path, "w") as configfile:
+            config.write(configfile)
+
+    def token_is_valid(self, token_type: str) -> bool:
+        """Given a token type, checks if the token is valid.
+
+        This method will check if the token is valid by checking if the token
+        is expired. This method will not regenerate the token if it is invalid.
+        As mentioned in the ``Token.is_valid`` property, this method will not
+        check if the token is valid by making a request to the API, but rather
+        checks if the token is likely to be expired by comparing the known
+        expiration time of the token to the current time. If the token type is
+        not found, this method will return False.
+
+        Args:
+            token_type (str): The type of token to check.
+
+        Returns:
+            bool: True if the token is valid, False otherwise.
+        """
+        try:
+            token = self.get(token_type, full_token=True)
+        except ValueError:
+            return False
+        return token.is_valid
+
+    def test_tokens(self, user_agent: str | None = None) -> None:
+        """Tests the tokens.
+
+        Checks using the ``token_is_valid`` method to see whether the tokens
+        need to be regenerated. If so, the tokens will be regenerated with the
+        appropriate ``generate_*`` method. Once the tokens are regenerated, it
+        will make a request to the API to check if the tokens are valid. If the
+        request fails, the ``generate_all_tokens`` method will be called. If the
+        requests succeeds, nothing will happen. Once this method is called, the
+        TokenManager can be assumed to have valid tokens and can be used to make
+        requests to the API.
+
+        Args:
+            user_agent (str): The user agent to use when making the request to
+                the API. If not specified, the default user agent will be used.
+
+        Raises:
+            ValueError: If the session token is not set.
+        """
+        if self.get(TOKENS.SESSION_TOKEN) is None:
+            raise ValueError("Session Token is not set.")
+
+        if self.token_is_valid(TOKENS.GTOKEN) is False:
+            self.generate_gtoken()
+
+        if self.token_is_valid(TOKENS.BULLET_TOKEN) is False:
+            self.generate_bullet_token()
+
+        header = queries.query_header(
+            self.get(TOKENS.BULLET_TOKEN), self._data["language"], user_agent
+        )
+
+        response = requests.post(
+            GRAPH_QL_REFERENCE_URL,
+            data=queries.query_body("HomeQuery"),
+            headers=header,
+            cookies={"_gtoken": cast(str, self.get(TOKENS.GTOKEN))},
+        )
+        if response.status_code != 200:
+            self.generate_all_tokens()
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/query/config.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/query/config.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,363 +1,363 @@
-import configparser
-from typing import Literal, overload
-
-from splatnet3_scraper.auth import (
-    EnvironmentVariablesManager,
-    Token,
-    TokenManager,
-)
-from splatnet3_scraper.constants import DEFAULT_USER_AGENT, IMINK_URL
-
-
-class Config:
-    """Class that can access the token manager as well as additional options."""
-
-    def __init__(
-        self,
-        config_path: str | None = None,
-        *args,
-        token_manager: TokenManager | None = None,
-    ) -> None:
-        """Initializes the class. If token_manager is given, it will assume that
-        this is a first time initialization and has not been setup yet.
-
-        Token manager will look for tokens in the following order:
-            1. the config_path argument
-            2. check the current working directory for ".splatnet3_scraper"
-            3. check for environment variables for defined tokens
-            4. check the current working directory for "tokens.ini"
-
-        If none of these are found, an exception will be raised.
-
-        Args:
-            config_path (str | None): The path to the config file. If None, it
-                will look for ".splatnet3_scraper" in the current working
-                directory. Defaults to None.
-            *args: These are ignored.
-            token_manager (TokenManager | None): The token manager to use.
-                Keyword argument. If given, it will skip the post-init method.
-                Defaults to None.
-        """
-        self.additional_accepted_options: list[str] = []
-        self.additional_deprecated_options: dict[str, str] = {}
-        self.additional_default_options: dict[str, str] = {}
-
-        if token_manager is None:
-            self.generate_token_manager(config_path)
-            return
-        else:
-            self.config_path = config_path
-
-        self.token_manager = token_manager
-        self.initialize_options()
-
-    def generate_token_manager(self, config_path: str | None = None) -> None:
-        """Generates the token manager.
-
-        Will only be called if the token manager is not given in the constructor
-        or if the ``token_manager`` argument in the constructor is None. This
-        means that the user prefers to use the default loading method for the
-        token manager, which is to look for tokens in the following order:
-
-            1. the config_path argument
-            2. check the current working directory for ".splatnet3_scraper"
-            3. check for environment variables for defined tokens
-            4. check the current working directory for "tokens.ini"
-
-        If none of these are found, an exception will be raised.
-
-        Args:
-            config_path (str | None): The path to the config file. If None, it
-                will look for ".splatnet3_scraper" in the current working
-                directory.
-        """
-        if config_path is not None:
-            self.token_manager = TokenManager.from_config_file(config_path)
-        # cgarza: A little bit of redundancy here, need better method.
-        else:
-            self.token_manager = TokenManager.load()
-
-        config_path = (
-            ".splatnet3_scraper" if config_path is None else config_path
-        )
-
-        self.config_path = config_path
-        self.config = configparser.ConfigParser()
-        self.config.read(config_path)
-        try:
-            self.options = self.config.options("options")
-        except configparser.NoSectionError:
-            self.config.add_section("options")
-            self.options = self.config.options("options")
-        self.manage_options()
-
-        with open(config_path, "w") as configfile:
-            self.config.write(configfile)
-
-    def initialize_options(self) -> None:
-        if getattr(self, "config", None) is not None:
-            return
-
-        origin = self.token_manager.origin
-        self.config = configparser.ConfigParser()
-        self.config.add_section("options")
-        self.options = self.config.options("options")
-
-        if origin["origin"] == "env":
-            # If the tokens are in environment variables, we should check for
-            # any additional tokens in the token's environment manager and add
-            # them to the config variable under the "options" section.
-            tokens = self.token_manager.env_manager.get_all()
-            for token, value in tokens.items():
-                if token in self.token_manager.env_manager.BASE_TOKENS:
-                    continue
-                if value is None:
-                    continue
-                self.config["options"][token] = value
-
-            return
-
-    @classmethod
-    def from_env(
-        cls, env_manager: EnvironmentVariablesManager | None = None
-    ) -> "Config":
-        """Creates a Config instance using the environment variables.
-
-        Args:
-            env_manager (EnvironmentVariablesManager | None): The environment
-                variables manager to use. If None, it will create a new one.
-                Defaults to None.
-
-        Returns:
-            Config: The Config instance.
-        """
-        return cls(token_manager=TokenManager.from_env(env_manager))
-
-    @classmethod
-    def from_s3s_config(cls, config_path: str) -> "Config":
-        """Creates a Config instance using the config file from s3s.
-
-        Args:
-            config_path (str): The path to the config file.
-
-        Returns:
-            Config: The Config instance.
-        """
-        return cls(token_manager=TokenManager.from_text_file(config_path))
-
-    def save(
-        self, path: str | None = None, include_tokens: bool = True
-    ) -> None:
-        """Saves the config file to the given path.
-
-        Args:
-            path (str | None): The path to save the config file to. If the token
-                manager is using environment variables, the tokens section will
-                be removed from the config file. If None, it will save to the
-                path given in the constructor or ".splatnet3_scraper" in the
-                current working directory.
-            include_tokens (bool): Whether or not to include the tokens in the
-                config file. If False, the tokens will be removed from the
-                config file.
-        """
-        # Check if the user has the tokens in a separate file
-        origin = self.token_manager._origin["origin"]
-        if (origin == "env") or (not include_tokens):
-            # Remove the token manager from the config file
-            self.config.remove_section("tokens")
-        if path is None and self.config_path is not None:
-            path = self.config_path
-        elif path is None:
-            path = ".splatnet3_scraper"
-
-        with open(path, "w") as configfile:
-            self.config.write(configfile)
-
-    def manage_options(self) -> None:
-        """Manage the options in the config file.
-
-        This function will move invalid options to the "unknown" section and
-        move deprecated options to the "deprecated" section while replacing them
-        with the new option name.
-        """
-        for option in self.options:
-            if option not in (
-                self.ACCEPTED_OPTIONS + list(self.DEPRECATED_OPTIONS.keys())
-            ):
-                if not self.config.has_section("unknown"):
-                    self.config.add_section("unknown")
-                self.config["unknown"][option] = self.config["options"][option]
-                self.config.remove_option("options", option)
-            if option in self.DEPRECATED_OPTIONS:
-                deprecated_name = option
-                option_name = self.DEPRECATED_OPTIONS[option]
-                if not self.config.has_section("deprecated"):
-                    self.config.add_section("deprecated")
-                # Make a copy of the deprecated option in the deprecated section
-                # and then replace the deprecated option with the new option
-                self.config["deprecated"][deprecated_name] = self.config[
-                    "options"
-                ][deprecated_name]
-                self.config["options"][option_name] = self.config["options"][
-                    deprecated_name
-                ]
-                self.config.remove_option("options", option)
-
-    _ACCEPTED_OPTIONS = [
-        "user_agent",
-        "log_level",
-        "log_file",
-        "export_path",
-        "language",
-        "lang",
-        "country",
-        "stat.ink_api_token",
-        "stat_ink_api_token",
-        "statink_api_token",
-        "f_token_url",
-    ]
-
-    _DEPRECATED_OPTIONS = {
-        "api_key": "stat.ink_api_token",
-        "f_gen": "f_token_url",
-    }
-
-    _DEFAULT_OPTIONS = {
-        "user_agent": DEFAULT_USER_AGENT,
-        "f_gen": IMINK_URL,
-        "export_path": "",
-    }
-
-    @property
-    def ACCEPTED_OPTIONS(self) -> list[str]:
-        return self._ACCEPTED_OPTIONS + self.additional_accepted_options
-
-    @property
-    def DEPRECATED_OPTIONS(self) -> dict[str, str]:
-        return {
-            **self._DEPRECATED_OPTIONS,
-            **self.additional_deprecated_options,
-        }
-
-    @property
-    def DEFAULT_OPTIONS(self) -> dict[str, str]:
-        return {**self._DEFAULT_OPTIONS, **self.additional_default_options}
-
-    def get(self, key: str) -> str:
-        """Get the value of an option. If the option is not set, the default
-        value will be returned.
-
-        Args:
-            key (str): The name of the option.
-
-        Raises:
-            KeyError: If the option is valid, but not set and has no default.
-            KeyError: If the option is not valid.
-
-        Returns:
-            str: The value of the option.
-        """
-        if key in self.ACCEPTED_OPTIONS:
-            if key in self.config["options"]:
-                return self.config["options"][key]
-            elif key in self.DEFAULT_OPTIONS:
-                return self.DEFAULT_OPTIONS[key]
-            else:
-                raise KeyError(f"Option not set and has no default: {key}")
-        elif key in self.DEPRECATED_OPTIONS:
-            return self.get(self.DEPRECATED_OPTIONS[key])
-        else:
-            raise KeyError(f"Invalid option: {key}")
-
-    def get_data(self, key: str) -> str:
-        if not self.config.has_section("data"):
-            self.config.add_section("data")
-            data = self.token_manager.data
-            for k, v in data.items():
-                self.config["data"][k] = v
-        return self.config["data"][key]
-
-    @overload
-    def get_token(self, key: str, full_token: Literal[False] = ...) -> str:
-        ...
-
-    @overload
-    def get_token(self, key: str, full_token: Literal[True]) -> Token:
-        ...
-
-    @overload
-    def get_token(self, key: str, full_token: bool) -> str | Token:
-        ...
-
-    def get_token(self, key: str, full_token: bool = False) -> str | Token:
-        """Get the value of a token.
-
-        Args:
-            key (str): The name of the token.
-            full_token (bool): Whether or not to return the full token. If
-                False, only the token value will be returned.
-
-        Returns:
-            str: The value of the token.
-        """
-        return self.token_manager.get(key, full_token)
-
-    def add_accepted_options(self, options: list[str]) -> None:
-        """Add options to the list of accepted options.
-
-        Args:
-            options (list[str]): The list of options to add.
-        """
-        self.additional_accepted_options.extend(options)
-
-    def add_deprecated_options(self, options: dict[str, str]) -> None:
-        """Add options to the list of deprecated options.
-
-        Args:
-            options (dict[str, str]): The list of options to add.
-        """
-        self.additional_deprecated_options.update(options)
-
-    def add_default_options(self, options: dict[str, str]) -> None:
-        """Add options to the list of default options.
-
-        Args:
-            options (dict[str, str]): The list of options to add.
-        """
-        self.additional_default_options.update(options)
-
-    def remove_accepted_options(self, options: list[str]) -> None:
-        """Remove options from the list of accepted options.
-
-        Args:
-            options (list[str]): The list of options to remove.
-        """
-        for option in options:
-            if option in self.additional_accepted_options:
-                self.additional_accepted_options.remove(option)
-            else:
-                self._ACCEPTED_OPTIONS.remove(option)
-
-    def remove_deprecated_options(self, options: list[str]) -> None:
-        """Remove options from the list of deprecated options.
-
-        Args:
-            options (list[str]): The list of options to remove.
-        """
-        for option in options:
-            if option in self.additional_deprecated_options:
-                self.additional_deprecated_options.pop(option)
-            else:
-                self._DEPRECATED_OPTIONS.pop(option)
-
-    def remove_default_options(self, options: list[str]) -> None:
-        """Remove options from the list of default options.
-
-        Args:
-            options (list[str]): The list of options to remove.
-        """
-        for option in options:
-            if option in self.additional_default_options:
-                self.additional_default_options.pop(option)
-            else:
-                self._DEFAULT_OPTIONS.pop(option)
+import configparser
+from typing import Literal, overload
+
+from splatnet3_scraper.auth import (
+    EnvironmentVariablesManager,
+    Token,
+    TokenManager,
+)
+from splatnet3_scraper.constants import DEFAULT_USER_AGENT, IMINK_URL
+
+
+class Config:
+    """Class that can access the token manager as well as additional options."""
+
+    def __init__(
+        self,
+        config_path: str | None = None,
+        *args,
+        token_manager: TokenManager | None = None,
+    ) -> None:
+        """Initializes the class. If token_manager is given, it will assume that
+        this is a first time initialization and has not been setup yet.
+
+        Token manager will look for tokens in the following order:
+            1. the config_path argument
+            2. check the current working directory for ".splatnet3_scraper"
+            3. check for environment variables for defined tokens
+            4. check the current working directory for "tokens.ini"
+
+        If none of these are found, an exception will be raised.
+
+        Args:
+            config_path (str | None): The path to the config file. If None, it
+                will look for ".splatnet3_scraper" in the current working
+                directory. Defaults to None.
+            *args: These are ignored.
+            token_manager (TokenManager | None): The token manager to use.
+                Keyword argument. If given, it will skip the post-init method.
+                Defaults to None.
+        """
+        self.additional_accepted_options: list[str] = []
+        self.additional_deprecated_options: dict[str, str] = {}
+        self.additional_default_options: dict[str, str] = {}
+
+        if token_manager is None:
+            self.generate_token_manager(config_path)
+            return
+        else:
+            self.config_path = config_path
+
+        self.token_manager = token_manager
+        self.initialize_options()
+
+    def generate_token_manager(self, config_path: str | None = None) -> None:
+        """Generates the token manager.
+
+        Will only be called if the token manager is not given in the constructor
+        or if the ``token_manager`` argument in the constructor is None. This
+        means that the user prefers to use the default loading method for the
+        token manager, which is to look for tokens in the following order:
+
+            1. the config_path argument
+            2. check the current working directory for ".splatnet3_scraper"
+            3. check for environment variables for defined tokens
+            4. check the current working directory for "tokens.ini"
+
+        If none of these are found, an exception will be raised.
+
+        Args:
+            config_path (str | None): The path to the config file. If None, it
+                will look for ".splatnet3_scraper" in the current working
+                directory.
+        """
+        if config_path is not None:
+            self.token_manager = TokenManager.from_config_file(config_path)
+        # cgarza: A little bit of redundancy here, need better method.
+        else:
+            self.token_manager = TokenManager.load()
+
+        config_path = (
+            ".splatnet3_scraper" if config_path is None else config_path
+        )
+
+        self.config_path = config_path
+        self.config = configparser.ConfigParser()
+        self.config.read(config_path)
+        try:
+            self.options = self.config.options("options")
+        except configparser.NoSectionError:
+            self.config.add_section("options")
+            self.options = self.config.options("options")
+        self.manage_options()
+
+        with open(config_path, "w") as configfile:
+            self.config.write(configfile)
+
+    def initialize_options(self) -> None:
+        if getattr(self, "config", None) is not None:
+            return
+
+        origin = self.token_manager.origin
+        self.config = configparser.ConfigParser()
+        self.config.add_section("options")
+        self.options = self.config.options("options")
+
+        if origin["origin"] == "env":
+            # If the tokens are in environment variables, we should check for
+            # any additional tokens in the token's environment manager and add
+            # them to the config variable under the "options" section.
+            tokens = self.token_manager.env_manager.get_all()
+            for token, value in tokens.items():
+                if token in self.token_manager.env_manager.BASE_TOKENS:
+                    continue
+                if value is None:
+                    continue
+                self.config["options"][token] = value
+
+            return
+
+    @classmethod
+    def from_env(
+        cls, env_manager: EnvironmentVariablesManager | None = None
+    ) -> "Config":
+        """Creates a Config instance using the environment variables.
+
+        Args:
+            env_manager (EnvironmentVariablesManager | None): The environment
+                variables manager to use. If None, it will create a new one.
+                Defaults to None.
+
+        Returns:
+            Config: The Config instance.
+        """
+        return cls(token_manager=TokenManager.from_env(env_manager))
+
+    @classmethod
+    def from_s3s_config(cls, config_path: str) -> "Config":
+        """Creates a Config instance using the config file from s3s.
+
+        Args:
+            config_path (str): The path to the config file.
+
+        Returns:
+            Config: The Config instance.
+        """
+        return cls(token_manager=TokenManager.from_text_file(config_path))
+
+    def save(
+        self, path: str | None = None, include_tokens: bool = True
+    ) -> None:
+        """Saves the config file to the given path.
+
+        Args:
+            path (str | None): The path to save the config file to. If the token
+                manager is using environment variables, the tokens section will
+                be removed from the config file. If None, it will save to the
+                path given in the constructor or ".splatnet3_scraper" in the
+                current working directory.
+            include_tokens (bool): Whether or not to include the tokens in the
+                config file. If False, the tokens will be removed from the
+                config file.
+        """
+        # Check if the user has the tokens in a separate file
+        origin = self.token_manager._origin["origin"]
+        if (origin == "env") or (not include_tokens):
+            # Remove the token manager from the config file
+            self.config.remove_section("tokens")
+        if path is None and self.config_path is not None:
+            path = self.config_path
+        elif path is None:
+            path = ".splatnet3_scraper"
+
+        with open(path, "w") as configfile:
+            self.config.write(configfile)
+
+    def manage_options(self) -> None:
+        """Manage the options in the config file.
+
+        This function will move invalid options to the "unknown" section and
+        move deprecated options to the "deprecated" section while replacing them
+        with the new option name.
+        """
+        for option in self.options:
+            if option not in (
+                self.ACCEPTED_OPTIONS + list(self.DEPRECATED_OPTIONS.keys())
+            ):
+                if not self.config.has_section("unknown"):
+                    self.config.add_section("unknown")
+                self.config["unknown"][option] = self.config["options"][option]
+                self.config.remove_option("options", option)
+            if option in self.DEPRECATED_OPTIONS:
+                deprecated_name = option
+                option_name = self.DEPRECATED_OPTIONS[option]
+                if not self.config.has_section("deprecated"):
+                    self.config.add_section("deprecated")
+                # Make a copy of the deprecated option in the deprecated section
+                # and then replace the deprecated option with the new option
+                self.config["deprecated"][deprecated_name] = self.config[
+                    "options"
+                ][deprecated_name]
+                self.config["options"][option_name] = self.config["options"][
+                    deprecated_name
+                ]
+                self.config.remove_option("options", option)
+
+    _ACCEPTED_OPTIONS = [
+        "user_agent",
+        "log_level",
+        "log_file",
+        "export_path",
+        "language",
+        "lang",
+        "country",
+        "stat.ink_api_token",
+        "stat_ink_api_token",
+        "statink_api_token",
+        "f_token_url",
+    ]
+
+    _DEPRECATED_OPTIONS = {
+        "api_key": "stat.ink_api_token",
+        "f_gen": "f_token_url",
+    }
+
+    _DEFAULT_OPTIONS = {
+        "user_agent": DEFAULT_USER_AGENT,
+        "f_gen": IMINK_URL,
+        "export_path": "",
+    }
+
+    @property
+    def ACCEPTED_OPTIONS(self) -> list[str]:
+        return self._ACCEPTED_OPTIONS + self.additional_accepted_options
+
+    @property
+    def DEPRECATED_OPTIONS(self) -> dict[str, str]:
+        return {
+            **self._DEPRECATED_OPTIONS,
+            **self.additional_deprecated_options,
+        }
+
+    @property
+    def DEFAULT_OPTIONS(self) -> dict[str, str]:
+        return {**self._DEFAULT_OPTIONS, **self.additional_default_options}
+
+    def get(self, key: str) -> str:
+        """Get the value of an option. If the option is not set, the default
+        value will be returned.
+
+        Args:
+            key (str): The name of the option.
+
+        Raises:
+            KeyError: If the option is valid, but not set and has no default.
+            KeyError: If the option is not valid.
+
+        Returns:
+            str: The value of the option.
+        """
+        if key in self.ACCEPTED_OPTIONS:
+            if key in self.config["options"]:
+                return self.config["options"][key]
+            elif key in self.DEFAULT_OPTIONS:
+                return self.DEFAULT_OPTIONS[key]
+            else:
+                raise KeyError(f"Option not set and has no default: {key}")
+        elif key in self.DEPRECATED_OPTIONS:
+            return self.get(self.DEPRECATED_OPTIONS[key])
+        else:
+            raise KeyError(f"Invalid option: {key}")
+
+    def get_data(self, key: str) -> str:
+        if not self.config.has_section("data"):
+            self.config.add_section("data")
+            data = self.token_manager.data
+            for k, v in data.items():
+                self.config["data"][k] = v
+        return self.config["data"][key]
+
+    @overload
+    def get_token(self, key: str, full_token: Literal[False] = ...) -> str:
+        ...
+
+    @overload
+    def get_token(self, key: str, full_token: Literal[True]) -> Token:
+        ...
+
+    @overload
+    def get_token(self, key: str, full_token: bool) -> str | Token:
+        ...
+
+    def get_token(self, key: str, full_token: bool = False) -> str | Token:
+        """Get the value of a token.
+
+        Args:
+            key (str): The name of the token.
+            full_token (bool): Whether or not to return the full token. If
+                False, only the token value will be returned.
+
+        Returns:
+            str: The value of the token.
+        """
+        return self.token_manager.get(key, full_token)
+
+    def add_accepted_options(self, options: list[str]) -> None:
+        """Add options to the list of accepted options.
+
+        Args:
+            options (list[str]): The list of options to add.
+        """
+        self.additional_accepted_options.extend(options)
+
+    def add_deprecated_options(self, options: dict[str, str]) -> None:
+        """Add options to the list of deprecated options.
+
+        Args:
+            options (dict[str, str]): The list of options to add.
+        """
+        self.additional_deprecated_options.update(options)
+
+    def add_default_options(self, options: dict[str, str]) -> None:
+        """Add options to the list of default options.
+
+        Args:
+            options (dict[str, str]): The list of options to add.
+        """
+        self.additional_default_options.update(options)
+
+    def remove_accepted_options(self, options: list[str]) -> None:
+        """Remove options from the list of accepted options.
+
+        Args:
+            options (list[str]): The list of options to remove.
+        """
+        for option in options:
+            if option in self.additional_accepted_options:
+                self.additional_accepted_options.remove(option)
+            else:
+                self._ACCEPTED_OPTIONS.remove(option)
+
+    def remove_deprecated_options(self, options: list[str]) -> None:
+        """Remove options from the list of deprecated options.
+
+        Args:
+            options (list[str]): The list of options to remove.
+        """
+        for option in options:
+            if option in self.additional_deprecated_options:
+                self.additional_deprecated_options.pop(option)
+            else:
+                self._DEPRECATED_OPTIONS.pop(option)
+
+    def remove_default_options(self, options: list[str]) -> None:
+        """Remove options from the list of default options.
+
+        Args:
+            options (list[str]): The list of options to remove.
+        """
+        for option in options:
+            if option in self.additional_default_options:
+                self.additional_default_options.pop(option)
+            else:
+                self._DEFAULT_OPTIONS.pop(option)
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/query/handler.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/query/handler.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,348 +1,348 @@
-import json
-
-import requests
-
-from splatnet3_scraper.auth import NSO, TokenManager
-from splatnet3_scraper.auth.exceptions import SplatNetException
-from splatnet3_scraper.auth.graph_ql_queries import queries
-from splatnet3_scraper.constants import TOKENS
-from splatnet3_scraper.query.config import Config
-from splatnet3_scraper.query.responses import QueryResponse
-from splatnet3_scraper.utils import retry
-
-
-class QueryHandler:
-    """The QueryHandler class is the main class of the
-    ``splatnet3_scraper.query`` module. It abstracts away the underlying
-    implementation details of making queries to the SplatNet 3 API and makes it
-    extremely easy to use. Token management is also handled by the QueryHandler
-    so the user does not have to worry about having to regenerate tokens when
-    they expire. The only exception to this is the session token, which the user
-    must handle themselves as it is not possible to regenerate it automatically.
-    The QueryHandler class is initialized with a Config class, which contains
-    all the configuration options that the user can set. The QueryHandler class
-    also contains multiple factory methods to create a new instance of the class
-    to make it setting up the Config class much easier. The primary mode of
-    operating the class is through the ``query`` method, which takes a query
-    name and a dictionary of arguments and returns a QueryResponse object.
-    """
-
-    def __init__(self, config: Config) -> None:
-        """Initializes the class, it is not meant to be instantiated directly,
-        but rather through one of the available factory methods. Still, it can
-        be instantiated directly if the user wants to use a custom Config class.
-
-        Args:
-            config (Config): The Config object to use. This object contains all
-                the configuration options that the user can set, and the
-                QueryHandler class will use these options as they are needed
-                throughout the operation of the class. It is recommended that
-                the user uses the factory methods to create a new instance of
-                the class instead of instantiating it directly, as the factory
-                methods will automatically create a Config object for the user
-                based on the instantiation method they prefer and pass it to the
-                constructor.
-        """
-        self.config = config
-
-    @staticmethod
-    def from_config_file(
-        config_path: str | None = None,
-    ) -> "QueryHandler":
-        """Creates a new instance of the class using a configuration file.
-
-        If the user does not provide a configuration file path, the default path
-        will be used, which is ``.splatnet3_scraper`` in the user's current
-        working directory. The configuration file this method accepts is one
-        that aligns with the standard configuration file format used by the
-        standard library ``configparser`` module. The configuration file must
-        have a ``[Tokens]`` section, which only requires the ``session_token``
-        option to be set. The ``session_token`` option must be set to the user's
-        session token. For a full list of all options that can be set in the
-        config file, see the documentation for the ``Config`` class.
-
-        Args:
-            config_path (str | None): The path to the configuration file. If
-                None, the default configuration file path of
-                ``.splatnet3_scraper`` in the user's current working directory
-                will be used. Defaults to None.
-
-        Returns:
-            QueryHandler: A new instance of the class using the configuration
-                file provided, with all the options set in the configuration
-                file.
-        """
-        config = Config(config_path)
-        return QueryHandler(config)
-
-    @staticmethod
-    def generate_session_token_url(
-        user_agent: str | None = None,
-    ) -> tuple[str, bytes, bytes]:
-        """Generates the URL to use to get the session token.
-
-        This method is used to generate the URL to use to get the session token
-        from the Nintendo Switch Online website. The user must then visit this
-        URL in their browser and log in to their Nintendo account. Once they
-        have logged in, they will be redirected to a page that contains the user
-        profile to select. The user must then select their user profile and
-        then copy the URL from the "select this account" button. The URI of the
-        button will contain the session token code, which the user must then
-        pass to the ``parse_npf_uri`` method to get the session token. This
-        method is currently incomplete and will be updated in the future with
-        its counterpart method to parse the URI and return a ``QueryHandler``
-        object with a valid session token already set in the ``Config`` object
-        and saved to the default configuration path in the user's current
-        working directory.
-
-        Args:
-            user_agent (str | None): The user agent to use when making the
-                initial requests to the Nintendo Switch Online service. If None,
-                the default user agent will be used. It is not recommended to
-                change this unless you know what you are doing. Defaults to
-                None.
-
-        Returns:
-            str: The URL to use to get the session token.
-            bytes: The state ID.
-            bytes: The challenge solution.
-        """
-        nso = NSO.new_instance()
-        url = nso.generate_login_url(user_agent)
-        return url, nso.state, nso.verifier
-
-    @staticmethod
-    def from_session_token(session_token: str) -> "QueryHandler":
-        """Creates a new instance of the class using a session token.
-
-        Given a session token, this method will create a new instance of the
-        class with a valid session token already set in the ``Config`` object.
-        This method is useful if the user already has a session token and does
-        not want to generate an accompanying ``GTOKEN`` and ``BULLET_TOKEN``.
-
-        Args:
-            session_token (str): The session token to use. This token must be
-                valid and not expired or revoked. If the token is invalid, the
-                user will not be able to make any queries to the SplatNet 3 API.
-
-        Returns:
-            QueryHandler: A new instance of the class with a valid session
-                token already set in the ``Config`` object. The ``GTOKEN`` and
-                ``BULLET_TOKEN`` will also have been generated and set in the
-                ``Config`` object.
-        """
-        token_manager = TokenManager.from_session_token(session_token)
-        token_manager.generate_all_tokens()
-        config = Config(token_manager=token_manager)
-        return QueryHandler(config)
-
-    @staticmethod
-    def from_env() -> "QueryHandler":
-        """Creates a new instance of the class using the environment
-        variables.
-
-        This method will create a new instance of the class using the
-        environment variables. This method is useful if the user wants to start
-        up the class in a CI/CD pipeline, a Docker container, or any other
-        environment where the user does not want to store the session token in
-        a file. The environment variables that this method will use are
-        prepended by ``SN3S_`` and are all uppercase. The three environment
-        variables supported are:
-
-        - ``SN3S_SESSION_TOKEN``: The session token to use. This token must be
-            valid and not expired or revoked.
-        - ``SN3S_GTOKEN``: The GTOKEN to use.
-        - ``SN3S_BULLET_TOKEN``: The BULLET_TOKEN to use.
-
-        Returns:
-            QueryHandler: A new instance of the class with a valid session
-                token already set in the ``Config`` object. The ``Config``
-                object is also flagged as using environment variables, so the
-                user does not need to worry about accidentally saving the
-                session token to disk.
-        """
-        config = Config.from_env()
-        return QueryHandler(config)
-
-    @staticmethod
-    def from_s3s_config(path: str) -> "QueryHandler":
-        """Creates a new instance of the class using the ``s3s`` config file.
-
-        This method will create a new instance of the class by reading the
-        ``s3s`` config file. The ``s3s`` config file is a file that is used by
-        ``s3s`` to store the user's data. This method is useful if the user
-        already has a ``s3s`` config file. The ``s3s`` config file is a JSON
-        file that contains the user's session token, G token, bullet token, and
-        other options and data.
-
-        Args:
-            path (str): The path to the s3s config file. This file must be a
-                valid JSON file.
-
-        Returns:
-            QueryHandler: A new instance of the class from the ``s3s`` config
-                file provided.
-        """
-        config = Config.from_s3s_config(path)
-        return QueryHandler(config)
-
-    def __query(
-        self, query_name: str, variables: dict = {}
-    ) -> requests.Response:
-        """Internal method to query Splatnet 3, it does all of the heavy lifting
-        and is used by the other methods to get the data.
-
-        Args:
-            query_name (str): The name of the query to use.
-            variables (dict): The variables to use in the query. Defaults to {}.
-
-        Returns:
-            requests.Response: The response from the query.
-        """
-        return queries.query(
-            query_name,
-            self.config.get_token(TOKENS.BULLET_TOKEN),
-            self.config.get_token(TOKENS.GTOKEN),
-            self.config.get_data("language"),
-            self.config.get("user_agent"),
-            variables=variables,
-        )
-
-    # Repeat code, but I've elected to do this to make it easier to read
-    def __query_hash(
-        self, query_hash: str, variables: dict = {}
-    ) -> requests.Response:
-        """Internal method to query Splatnet 3, it does all of the heavy lifting
-        and is used by the other methods to get the data.
-
-        Args:
-            query_hash (str): The hash of the query to use.
-            variables (dict): The variables to use in the query. Defaults to {}.
-
-        Returns:
-            requests.Response: The response from the query.
-        """
-        return queries.query_hash(
-            query_hash,
-            self.config.get_token(TOKENS.BULLET_TOKEN),
-            self.config.get_token(TOKENS.GTOKEN),
-            self.config.get_data("language"),
-            self.config.get("user_agent"),
-            variables=variables,
-        )
-
-    # Repeat code, but I've elected to do this to make it easier to read
-    @retry(times=1, exceptions=ConnectionError)
-    def query_hash(
-        self, query_hash: str, variables: dict = {}
-    ) -> QueryResponse:
-        """Given a query hash, it will query SplatNet 3 and return the response.
-
-        A convenience function that will use a GraphQL query hash rather than a
-        query name to query SplatNet 3. This method will automatically retry
-        once if the query fails and will regenerate the tokens if the query
-        fails for whatever reason. Some queries require variables to be passed
-        in, and this method will allow the user to pass in those variables. It
-        is not recommended to use this method unless the user knows what they
-        are doing, as the query hashes are not stable and can and do change
-        often and without warning. The user should use the ``query`` method
-        instead as it will compensate for any changes to the query hashes.
-
-        Args:
-            query_hash (str): The query hash to use. This hash must be valid,
-                and must be a string representation rather than a byte
-                representation.
-            variables (dict): The variables to use in the query. Some queries do
-                not require variables and so this argument can be omitted. If
-                the query does require variables and this argument is omitted,
-                then the query will fail and a ``SplatNetException`` will be
-                raised with the error message from SplatNet 3. Defaults to {}.
-
-        Raises:
-            SplatNetException: If the query is successful but returns a JSON
-                object with an ``errors`` key, then this exception will be
-                raised with the error message from SplatNet 3. This generally
-                means that the query was successfully generated and the current
-                tokens are still valid, but the query itself failed for some
-                reason. This can happen if the user did not provide the correct
-                required variables for the query, or if the variables provided
-                were somehow invalid.
-
-        Returns:
-            QueryResponse: The response from the query. This object will contain
-                the data from the query, and will also contain the query hash
-                that was used to generate the query. This is useful for
-                debugging purposes.
-        """
-        response = self.__query_hash(query_hash, variables)
-        if response.status_code != 200:
-            self.config.token_manager.generate_all_tokens()
-            response = self.__query_hash(query_hash, variables)
-
-        if "errors" in response.json():
-            errors = response.json()["errors"]
-            error_message = (
-                "Query was successful but returned at least one error."
-            )
-
-            error_message += " Errors: " + json.dumps(errors, indent=4)
-            raise SplatNetException(error_message)
-
-        return QueryResponse(data=response.json()["data"])
-
-    @retry(times=1, exceptions=ConnectionError)
-    def query(self, query_name: str, variables: dict = {}) -> QueryResponse:
-        """Queries Splatnet 3 and returns the data.
-
-        This method will query SplatNet 3 and return the data from the query.
-        This method will automatically retry once if the query fails and will
-        regenerate the tokens if the query fails for whatever reason. Some
-        queries require variables to be passed in, and this method will allow
-        the user to pass in those variables. This method obtains the query hash
-        from the ``auth`` module and automatically uses the appropriate query
-        hash for the query name provided. As such, it is recommended to use this
-        method rather than the ``query_hash`` method unless the user knows what
-        they are doing.
-
-        Args:
-            query_name (str): The name of the query to use. This name must be
-                valid, and is not case sensitive. For more information on the
-                list of valid queries, see the documentation on the queries that
-                are available.
-            variables (dict): The variables to use in the query. Some queries do
-                not require variables and so this argument can be omitted. If
-                the query does require variables and this argument is omitted,
-                then the query will fail and a ``SplatNetException`` will be
-                raised with the error message from SplatNet 3. Defaults to {}.
-
-        Raises:
-            SplatNetException: If the query is successful but returns a JSON
-                object with an ``errors`` key, then this exception will be
-                raised with the error message from SplatNet 3. This generally
-                means that the query was successfully generated and the current
-                tokens are still valid, but the query itself failed for some
-                reason. This can happen if the user did not provide the correct
-                required variables for the query, or if the variables provided
-                were somehow invalid.
-
-        Returns:
-            QueryResponse: The response from the query. This object will contain
-                the data from the query, and will also contain the query hash
-                that was used to generate the query. This is useful for
-                debugging purposes.
-        """
-        response = self.__query(query_name, variables)
-        if response.status_code != 200:
-            self.config.token_manager.generate_all_tokens()
-            response = self.__query(query_name, variables)
-
-        if "errors" in response.json():
-            errors = response.json()["errors"]
-            error_message = (
-                "Query was successful but returned at least one error."
-            )
-
-            error_message += " Errors: " + json.dumps(errors, indent=4)
-            raise SplatNetException(error_message)
-
-        return QueryResponse(data=response.json()["data"])
+import json
+
+import requests
+
+from splatnet3_scraper.auth import NSO, TokenManager
+from splatnet3_scraper.auth.exceptions import SplatNetException
+from splatnet3_scraper.auth.graph_ql_queries import queries
+from splatnet3_scraper.constants import TOKENS
+from splatnet3_scraper.query.config import Config
+from splatnet3_scraper.query.responses import QueryResponse
+from splatnet3_scraper.utils import retry
+
+
+class QueryHandler:
+    """The QueryHandler class is the main class of the
+    ``splatnet3_scraper.query`` module. It abstracts away the underlying
+    implementation details of making queries to the SplatNet 3 API and makes it
+    extremely easy to use. Token management is also handled by the QueryHandler
+    so the user does not have to worry about having to regenerate tokens when
+    they expire. The only exception to this is the session token, which the user
+    must handle themselves as it is not possible to regenerate it automatically.
+    The QueryHandler class is initialized with a Config class, which contains
+    all the configuration options that the user can set. The QueryHandler class
+    also contains multiple factory methods to create a new instance of the class
+    to make it setting up the Config class much easier. The primary mode of
+    operating the class is through the ``query`` method, which takes a query
+    name and a dictionary of arguments and returns a QueryResponse object.
+    """
+
+    def __init__(self, config: Config) -> None:
+        """Initializes the class, it is not meant to be instantiated directly,
+        but rather through one of the available factory methods. Still, it can
+        be instantiated directly if the user wants to use a custom Config class.
+
+        Args:
+            config (Config): The Config object to use. This object contains all
+                the configuration options that the user can set, and the
+                QueryHandler class will use these options as they are needed
+                throughout the operation of the class. It is recommended that
+                the user uses the factory methods to create a new instance of
+                the class instead of instantiating it directly, as the factory
+                methods will automatically create a Config object for the user
+                based on the instantiation method they prefer and pass it to the
+                constructor.
+        """
+        self.config = config
+
+    @staticmethod
+    def from_config_file(
+        config_path: str | None = None,
+    ) -> "QueryHandler":
+        """Creates a new instance of the class using a configuration file.
+
+        If the user does not provide a configuration file path, the default path
+        will be used, which is ``.splatnet3_scraper`` in the user's current
+        working directory. The configuration file this method accepts is one
+        that aligns with the standard configuration file format used by the
+        standard library ``configparser`` module. The configuration file must
+        have a ``[Tokens]`` section, which only requires the ``session_token``
+        option to be set. The ``session_token`` option must be set to the user's
+        session token. For a full list of all options that can be set in the
+        config file, see the documentation for the ``Config`` class.
+
+        Args:
+            config_path (str | None): The path to the configuration file. If
+                None, the default configuration file path of
+                ``.splatnet3_scraper`` in the user's current working directory
+                will be used. Defaults to None.
+
+        Returns:
+            QueryHandler: A new instance of the class using the configuration
+                file provided, with all the options set in the configuration
+                file.
+        """
+        config = Config(config_path)
+        return QueryHandler(config)
+
+    @staticmethod
+    def generate_session_token_url(
+        user_agent: str | None = None,
+    ) -> tuple[str, bytes, bytes]:
+        """Generates the URL to use to get the session token.
+
+        This method is used to generate the URL to use to get the session token
+        from the Nintendo Switch Online website. The user must then visit this
+        URL in their browser and log in to their Nintendo account. Once they
+        have logged in, they will be redirected to a page that contains the user
+        profile to select. The user must then select their user profile and
+        then copy the URL from the "select this account" button. The URI of the
+        button will contain the session token code, which the user must then
+        pass to the ``parse_npf_uri`` method to get the session token. This
+        method is currently incomplete and will be updated in the future with
+        its counterpart method to parse the URI and return a ``QueryHandler``
+        object with a valid session token already set in the ``Config`` object
+        and saved to the default configuration path in the user's current
+        working directory.
+
+        Args:
+            user_agent (str | None): The user agent to use when making the
+                initial requests to the Nintendo Switch Online service. If None,
+                the default user agent will be used. It is not recommended to
+                change this unless you know what you are doing. Defaults to
+                None.
+
+        Returns:
+            str: The URL to use to get the session token.
+            bytes: The state ID.
+            bytes: The challenge solution.
+        """
+        nso = NSO.new_instance()
+        url = nso.generate_login_url(user_agent)
+        return url, nso.state, nso.verifier
+
+    @staticmethod
+    def from_session_token(session_token: str) -> "QueryHandler":
+        """Creates a new instance of the class using a session token.
+
+        Given a session token, this method will create a new instance of the
+        class with a valid session token already set in the ``Config`` object.
+        This method is useful if the user already has a session token and does
+        not want to generate an accompanying ``GTOKEN`` and ``BULLET_TOKEN``.
+
+        Args:
+            session_token (str): The session token to use. This token must be
+                valid and not expired or revoked. If the token is invalid, the
+                user will not be able to make any queries to the SplatNet 3 API.
+
+        Returns:
+            QueryHandler: A new instance of the class with a valid session
+                token already set in the ``Config`` object. The ``GTOKEN`` and
+                ``BULLET_TOKEN`` will also have been generated and set in the
+                ``Config`` object.
+        """
+        token_manager = TokenManager.from_session_token(session_token)
+        token_manager.generate_all_tokens()
+        config = Config(token_manager=token_manager)
+        return QueryHandler(config)
+
+    @staticmethod
+    def from_env() -> "QueryHandler":
+        """Creates a new instance of the class using the environment
+        variables.
+
+        This method will create a new instance of the class using the
+        environment variables. This method is useful if the user wants to start
+        up the class in a CI/CD pipeline, a Docker container, or any other
+        environment where the user does not want to store the session token in
+        a file. The environment variables that this method will use are
+        prepended by ``SN3S_`` and are all uppercase. The three environment
+        variables supported are:
+
+        - ``SN3S_SESSION_TOKEN``: The session token to use. This token must be
+            valid and not expired or revoked.
+        - ``SN3S_GTOKEN``: The GTOKEN to use.
+        - ``SN3S_BULLET_TOKEN``: The BULLET_TOKEN to use.
+
+        Returns:
+            QueryHandler: A new instance of the class with a valid session
+                token already set in the ``Config`` object. The ``Config``
+                object is also flagged as using environment variables, so the
+                user does not need to worry about accidentally saving the
+                session token to disk.
+        """
+        config = Config.from_env()
+        return QueryHandler(config)
+
+    @staticmethod
+    def from_s3s_config(path: str) -> "QueryHandler":
+        """Creates a new instance of the class using the ``s3s`` config file.
+
+        This method will create a new instance of the class by reading the
+        ``s3s`` config file. The ``s3s`` config file is a file that is used by
+        ``s3s`` to store the user's data. This method is useful if the user
+        already has a ``s3s`` config file. The ``s3s`` config file is a JSON
+        file that contains the user's session token, G token, bullet token, and
+        other options and data.
+
+        Args:
+            path (str): The path to the s3s config file. This file must be a
+                valid JSON file.
+
+        Returns:
+            QueryHandler: A new instance of the class from the ``s3s`` config
+                file provided.
+        """
+        config = Config.from_s3s_config(path)
+        return QueryHandler(config)
+
+    def __query(
+        self, query_name: str, variables: dict = {}
+    ) -> requests.Response:
+        """Internal method to query Splatnet 3, it does all of the heavy lifting
+        and is used by the other methods to get the data.
+
+        Args:
+            query_name (str): The name of the query to use.
+            variables (dict): The variables to use in the query. Defaults to {}.
+
+        Returns:
+            requests.Response: The response from the query.
+        """
+        return queries.query(
+            query_name,
+            self.config.get_token(TOKENS.BULLET_TOKEN),
+            self.config.get_token(TOKENS.GTOKEN),
+            self.config.get_data("language"),
+            self.config.get("user_agent"),
+            variables=variables,
+        )
+
+    # Repeat code, but I've elected to do this to make it easier to read
+    def __query_hash(
+        self, query_hash: str, variables: dict = {}
+    ) -> requests.Response:
+        """Internal method to query Splatnet 3, it does all of the heavy lifting
+        and is used by the other methods to get the data.
+
+        Args:
+            query_hash (str): The hash of the query to use.
+            variables (dict): The variables to use in the query. Defaults to {}.
+
+        Returns:
+            requests.Response: The response from the query.
+        """
+        return queries.query_hash(
+            query_hash,
+            self.config.get_token(TOKENS.BULLET_TOKEN),
+            self.config.get_token(TOKENS.GTOKEN),
+            self.config.get_data("language"),
+            self.config.get("user_agent"),
+            variables=variables,
+        )
+
+    # Repeat code, but I've elected to do this to make it easier to read
+    @retry(times=1, exceptions=ConnectionError)
+    def query_hash(
+        self, query_hash: str, variables: dict = {}
+    ) -> QueryResponse:
+        """Given a query hash, it will query SplatNet 3 and return the response.
+
+        A convenience function that will use a GraphQL query hash rather than a
+        query name to query SplatNet 3. This method will automatically retry
+        once if the query fails and will regenerate the tokens if the query
+        fails for whatever reason. Some queries require variables to be passed
+        in, and this method will allow the user to pass in those variables. It
+        is not recommended to use this method unless the user knows what they
+        are doing, as the query hashes are not stable and can and do change
+        often and without warning. The user should use the ``query`` method
+        instead as it will compensate for any changes to the query hashes.
+
+        Args:
+            query_hash (str): The query hash to use. This hash must be valid,
+                and must be a string representation rather than a byte
+                representation.
+            variables (dict): The variables to use in the query. Some queries do
+                not require variables and so this argument can be omitted. If
+                the query does require variables and this argument is omitted,
+                then the query will fail and a ``SplatNetException`` will be
+                raised with the error message from SplatNet 3. Defaults to {}.
+
+        Raises:
+            SplatNetException: If the query is successful but returns a JSON
+                object with an ``errors`` key, then this exception will be
+                raised with the error message from SplatNet 3. This generally
+                means that the query was successfully generated and the current
+                tokens are still valid, but the query itself failed for some
+                reason. This can happen if the user did not provide the correct
+                required variables for the query, or if the variables provided
+                were somehow invalid.
+
+        Returns:
+            QueryResponse: The response from the query. This object will contain
+                the data from the query, and will also contain the query hash
+                that was used to generate the query. This is useful for
+                debugging purposes.
+        """
+        response = self.__query_hash(query_hash, variables)
+        if response.status_code != 200:
+            self.config.token_manager.generate_all_tokens()
+            response = self.__query_hash(query_hash, variables)
+
+        if "errors" in response.json():
+            errors = response.json()["errors"]
+            error_message = (
+                "Query was successful but returned at least one error."
+            )
+
+            error_message += " Errors: " + json.dumps(errors, indent=4)
+            raise SplatNetException(error_message)
+
+        return QueryResponse(data=response.json()["data"])
+
+    @retry(times=1, exceptions=ConnectionError)
+    def query(self, query_name: str, variables: dict = {}) -> QueryResponse:
+        """Queries Splatnet 3 and returns the data.
+
+        This method will query SplatNet 3 and return the data from the query.
+        This method will automatically retry once if the query fails and will
+        regenerate the tokens if the query fails for whatever reason. Some
+        queries require variables to be passed in, and this method will allow
+        the user to pass in those variables. This method obtains the query hash
+        from the ``auth`` module and automatically uses the appropriate query
+        hash for the query name provided. As such, it is recommended to use this
+        method rather than the ``query_hash`` method unless the user knows what
+        they are doing.
+
+        Args:
+            query_name (str): The name of the query to use. This name must be
+                valid, and is not case sensitive. For more information on the
+                list of valid queries, see the documentation on the queries that
+                are available.
+            variables (dict): The variables to use in the query. Some queries do
+                not require variables and so this argument can be omitted. If
+                the query does require variables and this argument is omitted,
+                then the query will fail and a ``SplatNetException`` will be
+                raised with the error message from SplatNet 3. Defaults to {}.
+
+        Raises:
+            SplatNetException: If the query is successful but returns a JSON
+                object with an ``errors`` key, then this exception will be
+                raised with the error message from SplatNet 3. This generally
+                means that the query was successfully generated and the current
+                tokens are still valid, but the query itself failed for some
+                reason. This can happen if the user did not provide the correct
+                required variables for the query, or if the variables provided
+                were somehow invalid.
+
+        Returns:
+            QueryResponse: The response from the query. This object will contain
+                the data from the query, and will also contain the query hash
+                that was used to generate the query. This is useful for
+                debugging purposes.
+        """
+        response = self.__query(query_name, variables)
+        if response.status_code != 200:
+            self.config.token_manager.generate_all_tokens()
+            response = self.__query(query_name, variables)
+
+        if "errors" in response.json():
+            errors = response.json()["errors"]
+            error_message = (
+                "Query was successful but returned at least one error."
+            )
+
+            error_message += " Errors: " + json.dumps(errors, indent=4)
+            raise SplatNetException(error_message)
+
+        return QueryResponse(data=response.json()["data"])
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/query/json_parser.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/query/json_parser.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,493 +1,493 @@
-import ast
-import csv
-import gzip
-import hashlib
-import json
-from typing import Any, Callable, Literal, overload
-
-from splatnet3_scraper.utils import delinearize_json, linearize_json
-
-
-class LinearJSON:
-    """Class containing methods for linearized JSON objects."""
-
-    def __init__(
-        self, header: list[str] | tuple[str, ...], data: list[list] | list
-    ) -> None:
-        """Initializes a LinearJSON.
-
-        Args:
-            header (list[str]): The header of the JSON object.
-            data (list[Any]): The data of the JSON object.
-        """
-        self.header = header
-        self.data = data if isinstance(data[0], list) else [data]
-        self.__validate()
-
-    @staticmethod
-    def from_json(object: dict[str, Any]) -> "LinearJSON":
-        """Creates a LinearJSON object from a JSON object.
-
-        Args:
-            object (dict[str, Any]): The JSON object to convert.
-
-        Returns:
-            LinearJSON: The LinearJSON object.
-        """
-        header, data = linearize_json(object)
-        return LinearJSON(header, [data])
-
-    @staticmethod
-    def hash(obj: list[str] | tuple[str, ...]) -> str:
-        """Returns the hash of the header.
-
-        Args:
-            obj (list[str] | tuple[str, ...]): The header to hash.
-
-        Returns:
-            str: The hash of the header.
-        """
-        header_tuple = tuple(obj)
-        # Use a stable hash function to ensure the same hash is generated
-        # across different Python versions
-        return hashlib.sha256(str(header_tuple).encode()).hexdigest()
-
-    def hashed_header(self) -> str:
-        """Returns the hash of the header.
-
-        Returns:
-            str: The hash of the header.
-        """
-        return self.hash(self.header)
-
-    def delinearize(self) -> dict[str, list[dict[str, Any]]]:
-        """Delinearizes the JSON object into a big JSON object.
-
-        Returns:
-            dict[str, list[dict[str, Any]]]: The big JSON object.
-        """
-        out: dict[str, list[dict[str, Any]]] = {"data": []}
-        for row in self.data:
-            out["data"].append(delinearize_json(self.header, row))
-        return out
-
-    def __eq__(self, other: object) -> bool:
-        """Returns whether the other object is equal to this object.
-
-        Args:
-            other (object): The other object to compare.
-
-        Returns:
-            bool: Whether the other object is equal to this object.
-        """
-        if isinstance(other, LinearJSON):
-            return self.header == other.header and self.data == other.data
-        elif isinstance(other, list):
-            return self.header == other[0] and self.data == other[1:]
-        return False
-
-    def __validate(self) -> None:
-        """Validates the header and data of the LinearJSON object.
-
-        Raises:
-            ValueError: If the header and data are not the same length.
-        """
-        for row in self.data:
-            try:
-                assert len(row) == len(self.header)
-            except AssertionError:
-                raise ValueError("The header and data are not the same length.")
-
-    def __standardize_new_header(self, new_header: list[str]) -> None:
-        """If the new header is different from the current header, this method
-        will remove columns from the data that are not in the new header and add
-        None values for columns that are in the new header but not the current
-        header.
-
-        Raises:
-            ValueError: If the new header has duplicate columns.
-
-        Args:
-            new_header (list[str]): The new header.
-        """
-        new_header_columns = [x for x in new_header if x not in self.header]
-        removed_header_columns = [x for x in self.header if x not in new_header]
-
-        # Check if the new header has any duplicates and raise an error if so
-        if len(new_header) != len(set(new_header)):
-            raise ValueError("The new header has duplicate columns.")
-
-        if (not new_header_columns) and (not removed_header_columns):
-            return
-        new_data = []
-        for row in self.data:
-            new_row: list[Any] = []
-            for col in new_header:
-                if col in new_header_columns:
-                    new_row.append(None)
-                elif col in removed_header_columns:
-                    # Shouldn't happen, but making the logic explicit
-                    continue
-                else:
-                    original_index = self.header.index(col)
-                    new_row.append(row[original_index])
-
-            new_data.append(new_row)
-        self.header = new_header
-        self.data = new_data
-
-    @staticmethod
-    def merge_headers(left: "LinearJSON", right: "LinearJSON") -> list[str]:
-        """Merges the headers of the two given LinearJSON objects.
-
-        Args:
-            left (LinearJSON): The left LinearJSON object to merge.
-            right (LinearJSON): The right LinearJSON object to merge.
-
-        Returns:
-            list[str]: The new header.
-        """
-        new_header_set = set(left.header).union(set(right.header))
-        new_header = list(new_header_set)
-        new_header = sorted(new_header, key=lambda x: (len(x), x))
-        return new_header
-
-    def append(self, other: "LinearJSON") -> None:
-        """Appends a LinearJSON object to this one. If the headers are not the
-        same, the headers will be merged and the data will be standardized to
-        the new header.
-
-        Args:
-            other (LinearJSON): The other LinearJSON object to append.
-        """
-        if self.header != other.header:
-            new_header = self.merge_headers(self, other)
-            # New header will have new columns anywhere in the header, so we
-            # need to identify the new columns and insert None values for them
-            # in the data
-            obj_list: list[LinearJSON] = [self, other]
-            for obj in obj_list:
-                obj.__standardize_new_header(new_header)
-        self.data.extend(other.data)
-
-    def transpose(self) -> list[list[Any]]:
-        """Transposes the data.
-
-        Returns:
-            list[list[Any]]: The transposed data.
-        """
-        return [list(x) for x in zip(*self.data)]
-
-    @overload
-    def stringify(self, include_header: Literal[True] = ...) -> tuple[str, str]:
-        ...
-
-    @overload
-    def stringify(self, include_header: Literal[False]) -> str:
-        ...
-
-    @overload
-    def stringify(self, include_header: bool) -> str | tuple[str, str]:
-        ...
-
-    def stringify(
-        self,
-        include_header: bool = True,
-    ) -> str | tuple[str, str]:
-        """Stringifies the LinearJSON object. If include_header is True, then
-        the header and data are returned as a tuple. Otherwise, only the data
-        is returned as a string.
-
-        Args:
-            include_header (bool): Whether to include the header. Defaults to
-                True.
-
-        Returns:
-            str | tuple[str, str]: The header and data as a string, or just the
-                data as a string.
-        """
-        data = self.data
-        data_str = []
-        for row in data:
-            out_row = []
-            # If the row has a comma, then we need to wrap the row in quotes
-            for col in row:
-                if isinstance(col, str) and "," in col:
-                    out_col = f'"{col}"'
-                else:
-                    out_col = str(col)
-                out_row.append(out_col)
-            data_str.append(",".join(out_row))
-        data_str_out = "\n".join(data_str)
-        if include_header:
-            header_str = ",".join(self.header)
-            return header_str, data_str_out
-        return data_str_out
-
-    def remove_columns(self, columns: list[str]) -> None:
-        """Removes columns from the LinearJSON object.
-
-        Args:
-            columns (list[str]): The columns to remove. If a column is not in
-                the header, it will be ignored.
-        """
-        new_header = [x for x in self.header if x not in columns]
-        self.__standardize_new_header(new_header)
-
-    def remove_url_columns(self) -> None:
-        """Removes columns that are URLs from the LinearJSON object."""
-        url_columns = [x for x in self.header if x.lower().endswith("url")]
-        self.remove_columns(url_columns)
-
-
-class JSONParser:
-    """Class containing JSON methods for saving and loading data."""
-
-    def __init__(self, data: dict[str, Any] | list[dict[str, Any]]) -> None:
-        """Initializes a JSONParser.
-
-        Args:
-            data (dict[str, Any] | list[dict[str, Any]]): The data to parse.
-        """
-        if isinstance(data, dict):
-            data = [data]
-        self.data = data
-
-    def __len__(self) -> int:
-        return len(self.data)
-
-    def __eq__(self, other: object) -> bool:
-        if isinstance(other, JSONParser):
-            return self.data == other.data
-        return False
-
-    def __repr__(self) -> str:
-        return f"JSONParser({len(self)} rows)"
-
-    def __to_linear_json(self) -> LinearJSON:
-        """Converts the JSON object to a LinearJSON object.
-
-        Returns:
-            LinearJSON: The LinearJSON object.
-        """
-        header, data = linearize_json(self.data[0])
-        out = LinearJSON(header, data)
-        for row in self.data[1:]:
-            header, data = linearize_json(row)
-            out.append(LinearJSON(header, data))
-        return out
-
-    def remove_columns(self, columns: list[str]) -> None:
-        """Removes columns from the data.
-
-        Args:
-            columns (list[str]): The columns to remove.
-        """
-        linear_json = self.__to_linear_json()
-        linear_json.remove_columns(columns)
-        self.data = linear_json.delinearize()["data"]
-
-    def remove_url_columns(self) -> None:
-        """Removes URL columns from the data."""
-        linear_json = self.__to_linear_json()
-        linear_json.remove_url_columns()
-        self.data = linear_json.delinearize()["data"]
-
-    def to_csv(self, path: str) -> None:
-        """Saves the JSON object to a CSV file.
-
-        Given the JSON Parser's data, this method will save the data to a CSV by
-        linearizing the JSON object. Given the following example JSON object:
-
-        >>> json = {
-        ...     "a": 1,
-        ...     "b": {
-        ...         "c": 2,
-        ...         "d": 3,
-        ...     },
-        ...     "e": [4, 5, 6],
-        ...     "f": [
-        ...         {"g": 7, "h": 8},
-        ...         {"g": 9, "h": 10},
-        ...     ],
-        ... }
-
-        The following CSV file will be created with spaces added for clarity:
-
-        >>> "a, b.c, b.d, e;0, e;1, e;2, f;0.g, f;0.h, f;1.g, f;1.h"
-        ... "1, 2, 3, 4, 5, 6, 7, 8, 9, 10"
-
-        Args:
-            path (str): The path to save the CSV file to.
-        """
-        linear_json = self.__to_linear_json()
-        with open(path, "w", encoding="utf-8") as f:
-            header, data = linear_json.stringify()
-            f.write(header + "\n")
-            f.write(data)
-
-    def __to_json(self, path: str, use_gzip: bool, **kwargs) -> None:
-        """Saves the JSON object to a JSON file. Any keyword arguments are
-        passed to the json.dump method. If gzip is True, the file will be
-        compressed with gzip.
-
-        Args:
-            path (str): The path to save the JSON file to.
-            use_gzip (bool): Whether or not to compress the file with gzip.
-            **kwargs: Any keyword arguments to pass to the json.dump method.
-        """
-        default_kwargs: dict[str, Any] = {"indent": 4}
-        default_kwargs.update(kwargs)
-        if use_gzip:
-            open_function: Callable = gzip.open
-            open_kwargs = {"mode": "wt", "encoding": "utf-8"}
-        else:
-            open_function = open
-            open_kwargs = {"mode": "w", "encoding": "utf-8"}
-
-        with open_function(path, **open_kwargs) as f:
-            json.dump(self.data, f, **default_kwargs)
-
-    def to_json(self, path: str, **kwargs) -> None:
-        """Saves the JSON object to a JSON file. Any keyword arguments are
-        passed to the json.dump method.
-
-        Args:
-            path (str): The path to save the JSON file to.
-            **kwargs: Keyword arguments to pass to the json.dump method.
-        """
-        self.__to_json(path, False, **kwargs)
-
-    def to_gzipped_json(self, path: str, **kwargs) -> None:
-        """Saves the JSON object to a gzipped JSON file. Any keyword arguments
-        are passed to the json.dump method.
-
-        Args:
-            path (str): The path to save the gzipped JSON file to.
-            **kwargs: Keyword arguments to pass to the json.dump method.
-        """
-        self.__to_json(path, True, **kwargs)
-
-    def to_parquet(self, path: str, **kwargs) -> None:
-        """Saves the JSON object to a Parquet file. Any keyword arguments are
-        passed to the pandas.DataFrame.to_parquet method.
-
-        Args:
-            path (str): The path to save the Parquet file to.
-            **kwargs: Keyword arguments to pass to the pq.write_table method.
-
-        Raises:
-            ImportError: If the parquet extra is not installed.
-        """
-        try:
-            import numpy as np
-            import pyarrow as pa
-            import pyarrow.parquet as pq
-        except ImportError:
-            raise ImportError(
-                "parquet format requires the [parquet] extra to be installed. "
-                'Try "pip install splatnet3_scraper[parquet]" or "poetry '
-                'install --extras parquet" if you are developing.'
-            )
-        linear_json = self.__to_linear_json()
-        numpy_data = np.array(linear_json.data)
-        arrays = [pa.array(data) for data in numpy_data.T]
-        del numpy_data
-        table = pa.Table.from_arrays(arrays, names=linear_json.header)
-        pq.write_table(table, path, **kwargs)
-
-    @staticmethod
-    def automatic_type_conversion(row: list[str]) -> list[Any]:
-        """Converts a row of strings to the most appropriate type.
-
-        Args:
-            row (list[str]): The row of strings to convert.
-
-        Returns:
-            list[Any]: The converted row.
-        """
-        converted_row = []
-        for col in row:
-            try:
-                value = ast.literal_eval(col)
-            except (ValueError, SyntaxError):
-                value = None if col == "" else col
-            converted_row.append(value)
-        return converted_row
-
-    @classmethod
-    def from_csv(cls, path: str) -> "JSONParser":
-        """Loads a JSON object from a CSV file.
-
-        Args:
-            path (str): The path to load the CSV file from.
-
-        Returns:
-            JSONParser: The JSONParser object.
-        """
-        with open(path, "r", encoding="utf-8") as f:
-            reader = csv.reader(
-                f,
-                quotechar='"',
-                delimiter=",",
-                quoting=csv.QUOTE_MINIMAL,
-                skipinitialspace=True,
-            )
-            header = next(reader)
-            data = [JSONParser.automatic_type_conversion(row) for row in reader]
-        delinearized_data = [delinearize_json(header, row) for row in data]
-        return cls(delinearized_data)
-
-    @classmethod
-    def from_json(cls, path: str) -> "JSONParser":
-        """Loads a JSON object from a JSON file.
-
-        Args:
-            path (str): The path to load the JSON file from.
-
-        Returns:
-            JSONParser: The JSONParser object.
-        """
-        with open(path, "r", encoding="utf-8") as f:
-            return cls(json.load(f))
-
-    @classmethod
-    def from_gzipped_json(cls, path: str) -> "JSONParser":
-        """Loads a JSON object from a gzipped JSON file.
-
-        Args:
-            path (str): The path to load the gzipped JSON file from.
-
-        Returns:
-            JSONParser: The JSONParser object.
-        """
-        with gzip.open(path, "rt", encoding="utf-8") as f:
-            return cls(json.load(f))
-
-    @classmethod
-    def from_parquet(cls, path: str) -> "JSONParser":
-        """Loads a JSON object from a Parquet file.
-
-        Args:
-            path (str): The path to load the Parquet file from.
-
-        Raises:
-            ImportError: If the parquet extra is not installed.
-
-        Returns:
-            JSONParser: The JSONParser object.
-        """
-        try:
-            import numpy as np
-            import pyarrow.parquet as pq
-        except ImportError:
-            raise ImportError(
-                "parquet format requires the [parquet] extra to be installed. "
-                'Try "pip install splatnet3_scraper[parquet]" or "poetry '
-                'install --extras parquet" if you are developing.'
-            )
-        table = pq.read_table(path)
-        data = [table.column(i).to_numpy() for i in range(len(table.columns))]
-        out_data = np.array(data).T
-        header = [field.name for field in table.schema]
-        return cls(delinearize_json(header, out_data.tolist()))
+import ast
+import csv
+import gzip
+import hashlib
+import json
+from typing import Any, Callable, Literal, overload
+
+from splatnet3_scraper.utils import delinearize_json, linearize_json
+
+
+class LinearJSON:
+    """Class containing methods for linearized JSON objects."""
+
+    def __init__(
+        self, header: list[str] | tuple[str, ...], data: list[list] | list
+    ) -> None:
+        """Initializes a LinearJSON.
+
+        Args:
+            header (list[str]): The header of the JSON object.
+            data (list[Any]): The data of the JSON object.
+        """
+        self.header = header
+        self.data = data if isinstance(data[0], list) else [data]
+        self.__validate()
+
+    @staticmethod
+    def from_json(object: dict[str, Any]) -> "LinearJSON":
+        """Creates a LinearJSON object from a JSON object.
+
+        Args:
+            object (dict[str, Any]): The JSON object to convert.
+
+        Returns:
+            LinearJSON: The LinearJSON object.
+        """
+        header, data = linearize_json(object)
+        return LinearJSON(header, [data])
+
+    @staticmethod
+    def hash(obj: list[str] | tuple[str, ...]) -> str:
+        """Returns the hash of the header.
+
+        Args:
+            obj (list[str] | tuple[str, ...]): The header to hash.
+
+        Returns:
+            str: The hash of the header.
+        """
+        header_tuple = tuple(obj)
+        # Use a stable hash function to ensure the same hash is generated
+        # across different Python versions
+        return hashlib.sha256(str(header_tuple).encode()).hexdigest()
+
+    def hashed_header(self) -> str:
+        """Returns the hash of the header.
+
+        Returns:
+            str: The hash of the header.
+        """
+        return self.hash(self.header)
+
+    def delinearize(self) -> dict[str, list[dict[str, Any]]]:
+        """Delinearizes the JSON object into a big JSON object.
+
+        Returns:
+            dict[str, list[dict[str, Any]]]: The big JSON object.
+        """
+        out: dict[str, list[dict[str, Any]]] = {"data": []}
+        for row in self.data:
+            out["data"].append(delinearize_json(self.header, row))
+        return out
+
+    def __eq__(self, other: object) -> bool:
+        """Returns whether the other object is equal to this object.
+
+        Args:
+            other (object): The other object to compare.
+
+        Returns:
+            bool: Whether the other object is equal to this object.
+        """
+        if isinstance(other, LinearJSON):
+            return self.header == other.header and self.data == other.data
+        elif isinstance(other, list):
+            return self.header == other[0] and self.data == other[1:]
+        return False
+
+    def __validate(self) -> None:
+        """Validates the header and data of the LinearJSON object.
+
+        Raises:
+            ValueError: If the header and data are not the same length.
+        """
+        for row in self.data:
+            try:
+                assert len(row) == len(self.header)
+            except AssertionError:
+                raise ValueError("The header and data are not the same length.")
+
+    def __standardize_new_header(self, new_header: list[str]) -> None:
+        """If the new header is different from the current header, this method
+        will remove columns from the data that are not in the new header and add
+        None values for columns that are in the new header but not the current
+        header.
+
+        Raises:
+            ValueError: If the new header has duplicate columns.
+
+        Args:
+            new_header (list[str]): The new header.
+        """
+        new_header_columns = [x for x in new_header if x not in self.header]
+        removed_header_columns = [x for x in self.header if x not in new_header]
+
+        # Check if the new header has any duplicates and raise an error if so
+        if len(new_header) != len(set(new_header)):
+            raise ValueError("The new header has duplicate columns.")
+
+        if (not new_header_columns) and (not removed_header_columns):
+            return
+        new_data = []
+        for row in self.data:
+            new_row: list[Any] = []
+            for col in new_header:
+                if col in new_header_columns:
+                    new_row.append(None)
+                elif col in removed_header_columns:
+                    # Shouldn't happen, but making the logic explicit
+                    continue
+                else:
+                    original_index = self.header.index(col)
+                    new_row.append(row[original_index])
+
+            new_data.append(new_row)
+        self.header = new_header
+        self.data = new_data
+
+    @staticmethod
+    def merge_headers(left: "LinearJSON", right: "LinearJSON") -> list[str]:
+        """Merges the headers of the two given LinearJSON objects.
+
+        Args:
+            left (LinearJSON): The left LinearJSON object to merge.
+            right (LinearJSON): The right LinearJSON object to merge.
+
+        Returns:
+            list[str]: The new header.
+        """
+        new_header_set = set(left.header).union(set(right.header))
+        new_header = list(new_header_set)
+        new_header = sorted(new_header, key=lambda x: (len(x), x))
+        return new_header
+
+    def append(self, other: "LinearJSON") -> None:
+        """Appends a LinearJSON object to this one. If the headers are not the
+        same, the headers will be merged and the data will be standardized to
+        the new header.
+
+        Args:
+            other (LinearJSON): The other LinearJSON object to append.
+        """
+        if self.header != other.header:
+            new_header = self.merge_headers(self, other)
+            # New header will have new columns anywhere in the header, so we
+            # need to identify the new columns and insert None values for them
+            # in the data
+            obj_list: list[LinearJSON] = [self, other]
+            for obj in obj_list:
+                obj.__standardize_new_header(new_header)
+        self.data.extend(other.data)
+
+    def transpose(self) -> list[list[Any]]:
+        """Transposes the data.
+
+        Returns:
+            list[list[Any]]: The transposed data.
+        """
+        return [list(x) for x in zip(*self.data)]
+
+    @overload
+    def stringify(self, include_header: Literal[True] = ...) -> tuple[str, str]:
+        ...
+
+    @overload
+    def stringify(self, include_header: Literal[False]) -> str:
+        ...
+
+    @overload
+    def stringify(self, include_header: bool) -> str | tuple[str, str]:
+        ...
+
+    def stringify(
+        self,
+        include_header: bool = True,
+    ) -> str | tuple[str, str]:
+        """Stringifies the LinearJSON object. If include_header is True, then
+        the header and data are returned as a tuple. Otherwise, only the data
+        is returned as a string.
+
+        Args:
+            include_header (bool): Whether to include the header. Defaults to
+                True.
+
+        Returns:
+            str | tuple[str, str]: The header and data as a string, or just the
+                data as a string.
+        """
+        data = self.data
+        data_str = []
+        for row in data:
+            out_row = []
+            # If the row has a comma, then we need to wrap the row in quotes
+            for col in row:
+                if isinstance(col, str) and "," in col:
+                    out_col = f'"{col}"'
+                else:
+                    out_col = str(col)
+                out_row.append(out_col)
+            data_str.append(",".join(out_row))
+        data_str_out = "\n".join(data_str)
+        if include_header:
+            header_str = ",".join(self.header)
+            return header_str, data_str_out
+        return data_str_out
+
+    def remove_columns(self, columns: list[str]) -> None:
+        """Removes columns from the LinearJSON object.
+
+        Args:
+            columns (list[str]): The columns to remove. If a column is not in
+                the header, it will be ignored.
+        """
+        new_header = [x for x in self.header if x not in columns]
+        self.__standardize_new_header(new_header)
+
+    def remove_url_columns(self) -> None:
+        """Removes columns that are URLs from the LinearJSON object."""
+        url_columns = [x for x in self.header if x.lower().endswith("url")]
+        self.remove_columns(url_columns)
+
+
+class JSONParser:
+    """Class containing JSON methods for saving and loading data."""
+
+    def __init__(self, data: dict[str, Any] | list[dict[str, Any]]) -> None:
+        """Initializes a JSONParser.
+
+        Args:
+            data (dict[str, Any] | list[dict[str, Any]]): The data to parse.
+        """
+        if isinstance(data, dict):
+            data = [data]
+        self.data = data
+
+    def __len__(self) -> int:
+        return len(self.data)
+
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, JSONParser):
+            return self.data == other.data
+        return False
+
+    def __repr__(self) -> str:
+        return f"JSONParser({len(self)} rows)"
+
+    def __to_linear_json(self) -> LinearJSON:
+        """Converts the JSON object to a LinearJSON object.
+
+        Returns:
+            LinearJSON: The LinearJSON object.
+        """
+        header, data = linearize_json(self.data[0])
+        out = LinearJSON(header, data)
+        for row in self.data[1:]:
+            header, data = linearize_json(row)
+            out.append(LinearJSON(header, data))
+        return out
+
+    def remove_columns(self, columns: list[str]) -> None:
+        """Removes columns from the data.
+
+        Args:
+            columns (list[str]): The columns to remove.
+        """
+        linear_json = self.__to_linear_json()
+        linear_json.remove_columns(columns)
+        self.data = linear_json.delinearize()["data"]
+
+    def remove_url_columns(self) -> None:
+        """Removes URL columns from the data."""
+        linear_json = self.__to_linear_json()
+        linear_json.remove_url_columns()
+        self.data = linear_json.delinearize()["data"]
+
+    def to_csv(self, path: str) -> None:
+        """Saves the JSON object to a CSV file.
+
+        Given the JSON Parser's data, this method will save the data to a CSV by
+        linearizing the JSON object. Given the following example JSON object:
+
+        >>> json = {
+        ...     "a": 1,
+        ...     "b": {
+        ...         "c": 2,
+        ...         "d": 3,
+        ...     },
+        ...     "e": [4, 5, 6],
+        ...     "f": [
+        ...         {"g": 7, "h": 8},
+        ...         {"g": 9, "h": 10},
+        ...     ],
+        ... }
+
+        The following CSV file will be created with spaces added for clarity:
+
+        >>> "a, b.c, b.d, e;0, e;1, e;2, f;0.g, f;0.h, f;1.g, f;1.h"
+        ... "1, 2, 3, 4, 5, 6, 7, 8, 9, 10"
+
+        Args:
+            path (str): The path to save the CSV file to.
+        """
+        linear_json = self.__to_linear_json()
+        with open(path, "w", encoding="utf-8") as f:
+            header, data = linear_json.stringify()
+            f.write(header + "\n")
+            f.write(data)
+
+    def __to_json(self, path: str, use_gzip: bool, **kwargs) -> None:
+        """Saves the JSON object to a JSON file. Any keyword arguments are
+        passed to the json.dump method. If gzip is True, the file will be
+        compressed with gzip.
+
+        Args:
+            path (str): The path to save the JSON file to.
+            use_gzip (bool): Whether or not to compress the file with gzip.
+            **kwargs: Any keyword arguments to pass to the json.dump method.
+        """
+        default_kwargs: dict[str, Any] = {"indent": 4}
+        default_kwargs.update(kwargs)
+        if use_gzip:
+            open_function: Callable = gzip.open
+            open_kwargs = {"mode": "wt", "encoding": "utf-8"}
+        else:
+            open_function = open
+            open_kwargs = {"mode": "w", "encoding": "utf-8"}
+
+        with open_function(path, **open_kwargs) as f:
+            json.dump(self.data, f, **default_kwargs)
+
+    def to_json(self, path: str, **kwargs) -> None:
+        """Saves the JSON object to a JSON file. Any keyword arguments are
+        passed to the json.dump method.
+
+        Args:
+            path (str): The path to save the JSON file to.
+            **kwargs: Keyword arguments to pass to the json.dump method.
+        """
+        self.__to_json(path, False, **kwargs)
+
+    def to_gzipped_json(self, path: str, **kwargs) -> None:
+        """Saves the JSON object to a gzipped JSON file. Any keyword arguments
+        are passed to the json.dump method.
+
+        Args:
+            path (str): The path to save the gzipped JSON file to.
+            **kwargs: Keyword arguments to pass to the json.dump method.
+        """
+        self.__to_json(path, True, **kwargs)
+
+    def to_parquet(self, path: str, **kwargs) -> None:
+        """Saves the JSON object to a Parquet file. Any keyword arguments are
+        passed to the pandas.DataFrame.to_parquet method.
+
+        Args:
+            path (str): The path to save the Parquet file to.
+            **kwargs: Keyword arguments to pass to the pq.write_table method.
+
+        Raises:
+            ImportError: If the parquet extra is not installed.
+        """
+        try:
+            import numpy as np
+            import pyarrow as pa
+            import pyarrow.parquet as pq
+        except ImportError:
+            raise ImportError(
+                "parquet format requires the [parquet] extra to be installed. "
+                'Try "pip install splatnet3_scraper[parquet]" or "poetry '
+                'install --extras parquet" if you are developing.'
+            )
+        linear_json = self.__to_linear_json()
+        numpy_data = np.array(linear_json.data)
+        arrays = [pa.array(data) for data in numpy_data.T]
+        del numpy_data
+        table = pa.Table.from_arrays(arrays, names=linear_json.header)
+        pq.write_table(table, path, **kwargs)
+
+    @staticmethod
+    def automatic_type_conversion(row: list[str]) -> list[Any]:
+        """Converts a row of strings to the most appropriate type.
+
+        Args:
+            row (list[str]): The row of strings to convert.
+
+        Returns:
+            list[Any]: The converted row.
+        """
+        converted_row = []
+        for col in row:
+            try:
+                value = ast.literal_eval(col)
+            except (ValueError, SyntaxError):
+                value = None if col == "" else col
+            converted_row.append(value)
+        return converted_row
+
+    @classmethod
+    def from_csv(cls, path: str) -> "JSONParser":
+        """Loads a JSON object from a CSV file.
+
+        Args:
+            path (str): The path to load the CSV file from.
+
+        Returns:
+            JSONParser: The JSONParser object.
+        """
+        with open(path, "r", encoding="utf-8") as f:
+            reader = csv.reader(
+                f,
+                quotechar='"',
+                delimiter=",",
+                quoting=csv.QUOTE_MINIMAL,
+                skipinitialspace=True,
+            )
+            header = next(reader)
+            data = [JSONParser.automatic_type_conversion(row) for row in reader]
+        delinearized_data = [delinearize_json(header, row) for row in data]
+        return cls(delinearized_data)
+
+    @classmethod
+    def from_json(cls, path: str) -> "JSONParser":
+        """Loads a JSON object from a JSON file.
+
+        Args:
+            path (str): The path to load the JSON file from.
+
+        Returns:
+            JSONParser: The JSONParser object.
+        """
+        with open(path, "r", encoding="utf-8") as f:
+            return cls(json.load(f))
+
+    @classmethod
+    def from_gzipped_json(cls, path: str) -> "JSONParser":
+        """Loads a JSON object from a gzipped JSON file.
+
+        Args:
+            path (str): The path to load the gzipped JSON file from.
+
+        Returns:
+            JSONParser: The JSONParser object.
+        """
+        with gzip.open(path, "rt", encoding="utf-8") as f:
+            return cls(json.load(f))
+
+    @classmethod
+    def from_parquet(cls, path: str) -> "JSONParser":
+        """Loads a JSON object from a Parquet file.
+
+        Args:
+            path (str): The path to load the Parquet file from.
+
+        Raises:
+            ImportError: If the parquet extra is not installed.
+
+        Returns:
+            JSONParser: The JSONParser object.
+        """
+        try:
+            import numpy as np
+            import pyarrow.parquet as pq
+        except ImportError:
+            raise ImportError(
+                "parquet format requires the [parquet] extra to be installed. "
+                'Try "pip install splatnet3_scraper[parquet]" or "poetry '
+                'install --extras parquet" if you are developing.'
+            )
+        table = pq.read_table(path)
+        data = [table.column(i).to_numpy() for i in range(len(table.columns))]
+        out_data = np.array(data).T
+        header = [field.name for field in table.schema]
+        return cls(delinearize_json(header, out_data.tolist()))
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/scraper/main.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/scraper/main.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,261 +1,261 @@
-from typing import Literal, cast, overload
-
-from splatnet3_scraper.query import QueryHandler, QueryResponse
-from splatnet3_scraper.scraper.query_map import QueryMap
-
-
-class SplatNet_Scraper:
-    """This class offers a user-level interface for pulling data from SplatNet
-    3. It is built upon the QueryHandler class and provides a top-level
-    API that orchestrates multiple queries together to reduce the amount of work
-    needed to pull data that users are likely to want.
-    """
-
-    def __init__(self, query_handler: QueryHandler) -> None:
-        """Initializes a SplatNet_Scraper.
-
-        Args:
-            query_handler (QueryHandler): The query handler to use.
-        """
-        self._query_handler = query_handler
-
-    @staticmethod
-    def from_session_token(session_token: str) -> "SplatNet_Scraper":
-        """Creates a SplatNet_Scraper instance using the given session token.
-
-        Args:
-            session_token (str): The session token to use.
-
-        Returns:
-            SplatNet_Scraper: The SplatNet_Scraper instance.
-        """
-        query_handler = QueryHandler.from_session_token(session_token)
-        return SplatNet_Scraper(query_handler)
-
-    @staticmethod
-    def from_config_file(config_path: str | None = None) -> "SplatNet_Scraper":
-        """Creates a SplatNet_Scraper instance using the given config file.
-
-        Args:
-            config_path (str | None): The path to the config file. If None, it
-                will look for ".splatnet3_scraper" in the current working
-                directory.
-
-        Returns:
-            SplatNet_Scraper: The SplatNet_Scraper instance.
-        """
-        query_handler = QueryHandler.from_config_file(config_path)
-        return SplatNet_Scraper(query_handler)
-
-    @staticmethod
-    def from_env() -> "SplatNet_Scraper":
-        """Creates a SplatNet_Scraper instance using the environment variables.
-
-        Environment variables:
-            SN3S_SESSION_TOKEN: The session token to use.
-            SN3S_GTOKEN: The gtoken to use.
-            SN3S_BULLET_TOKEN: The bullet token to use.
-
-        Returns:
-            SplatNet_Scraper: The SplatNet_Scraper instance.
-        """
-        query_handler = QueryHandler.from_env()
-        return SplatNet_Scraper(query_handler)
-
-    @staticmethod
-    def from_s3s_config(config_path: str) -> "SplatNet_Scraper":
-        """Creates a SplatNet_Scraper instance using the config file from s3s.
-
-        Args:
-            config_path (str): The path to the config file.
-
-        Returns:
-            SplatNet_Scraper: The SplatNet_Scraper instance.
-        """
-        query_handler = QueryHandler.from_s3s_config(config_path)
-        return SplatNet_Scraper(query_handler)
-
-    def __query(self, query: str, variables: dict = {}) -> QueryResponse:
-        """Convenience function for querying.
-
-        Args:
-            query (str): The query to run.
-            variables (dict): The variables to pass to the query. Defaults to
-                an empty dict.
-
-        Returns:
-            QueryResponse: The QueryResponse.
-        """
-        return self._query_handler.query(query, variables)
-
-    def __detailed_vs_or_coop(
-        self,
-        query: str,
-        limit: int | None = None,
-        existing_ids: list[str] | str | None = None,
-    ) -> tuple[QueryResponse, list[QueryResponse]]:
-        """Gets the detailed results for a vs battle or coop battle.
-
-        Args:
-            query (str): The query to run.
-            limit (int | None): The maximum number of battles to get. If None,
-                it will get all battles. Defaults to None.
-            existing_ids (list[str] | str | None): The existing IDs to check
-                against. If a string is passed, it will return the results
-                upon finding the first match. If a list is passed, it will
-                return the results of all matches not in the list. If None,
-                it will return all results. Defaults to None.
-
-        Raises:
-            ValueError: If the query is not a vs battle or coop battle.
-
-        Returns:
-            tuple:
-                QueryResponse: The summary query response.
-                list[QueryResponse]: The list of detailed query responses
-                    associated with each battle until the limit is reached.
-        """
-        if query not in (
-            QueryMap.SALMON,
-            QueryMap.TURF,
-            QueryMap.ANARCHY,
-            QueryMap.XBATTLE,
-            QueryMap.PRIVATE,
-        ):
-            raise ValueError(f"Invalid query: {query}")
-
-        if query in (QueryMap.SALMON, QueryMap.SALMON_DETAIL):
-            detail_query = QueryMap.SALMON_DETAIL
-            variable_name = "coopHistoryDetailId"
-        else:
-            detail_query = QueryMap.VS_DETAIL
-            variable_name = "vsResultId"
-
-        _limit = -1 if limit is None else limit
-
-        # Get the list of battles
-        summary_query = self.__query(query)
-
-        # Top level key depends on the game mode, but there is only one.
-        top_level_key = summary_query.keys()[0]
-        history_groups = summary_query[top_level_key, "historyGroups", "nodes"]
-        out: list[QueryResponse] = []
-        idx = 0
-
-        for group in history_groups:
-            group = cast(QueryResponse, group)
-            for game in group["historyDetails", "nodes"]:
-                game = cast(QueryResponse, game)
-                if idx == _limit:
-                    return summary_query, out
-                idx += 1
-                game_id = game["id"]
-
-                if isinstance(existing_ids, str):
-                    if game_id == existing_ids:
-                        return summary_query, out
-                elif isinstance(existing_ids, list):
-                    if game_id in existing_ids:
-                        idx -= 1
-                        continue
-
-                variables = {variable_name: game_id}
-                detailed_game = self.__query(detail_query, variables)
-                out.append(detailed_game)
-
-        return summary_query, out
-
-    @overload
-    def get_vs_battles(
-        self,
-        mode: str,
-        detail: Literal[False],
-        limit: int | None = None,
-        existing_ids: list[str] | str | None = None,
-    ) -> QueryResponse:
-        ...
-
-    @overload
-    def get_vs_battles(
-        self,
-        mode: str,
-        detail: Literal[True],
-        limit: int | None = None,
-        existing_ids: list[str] | str | None = None,
-    ) -> tuple[QueryResponse, list[QueryResponse]]:
-        ...
-
-    @overload
-    def get_vs_battles(
-        self,
-        mode: str,
-        detail: bool = False,
-        limit: int | None = None,
-        existing_ids: list[str] | str | None = None,
-    ) -> QueryResponse | tuple[QueryResponse, list[QueryResponse]]:
-        ...
-
-    def get_vs_battles(
-        self,
-        mode: str,
-        detail: bool = False,
-        limit: int | None = None,
-        existing_ids: list[str] | str | None = None,
-    ) -> QueryResponse | tuple[QueryResponse, list[QueryResponse]]:
-        """Gets the vs battles.
-
-        Args:
-            mode (str): The mode to get the battles for. Some values are:
-                "turf", "anarchy", "xbattle", "private",
-            detail (bool): Whether to get the detailed results or not.
-                Defaults to False.
-            limit (int | None): The maximum number of battles to get. If None,
-                it will get all battles. Defaults to None.
-            existing_ids (list[str] | str | None): The existing IDs to check
-                against. If a string is passed, it will return the results
-                upon finding the first match. If a list is passed, it will
-                return the results of all matches not in the list. If None,
-                it will return all results. Defaults to None.
-
-        Raises:
-            ValueError: If the mode is not valid.
-
-        Returns:
-            QueryResponse : The summary query response, returned regardless of
-                the value of detail.
-            (list[QueryResponse]): The list of detailed query responses
-                associated with each battle until the limit is reached. Only
-                returned if detail is True, along with the summary query
-                response.
-        """
-        mapped_query = QueryMap.get(mode)
-        if mapped_query == QueryMap.SALMON:
-            raise ValueError("Use get_coop_battles for salmon run battles.")
-
-        if mapped_query in (
-            QueryMap.TURF_DETAIL,
-            QueryMap.ANARCHY_DETAIL,
-            QueryMap.XBATTLE_DETAIL,
-            QueryMap.PRIVATE_DETAIL,
-        ):
-            non_detail_map = {
-                QueryMap.TURF_DETAIL: QueryMap.TURF,
-                QueryMap.ANARCHY_DETAIL: QueryMap.ANARCHY,
-                QueryMap.XBATTLE_DETAIL: QueryMap.XBATTLE,
-                QueryMap.PRIVATE_DETAIL: QueryMap.PRIVATE,
-            }
-            mapped_query = non_detail_map[mapped_query]
-            detail = True
-
-        if mapped_query not in (
-            QueryMap.TURF,
-            QueryMap.ANARCHY,
-            QueryMap.XBATTLE,
-            QueryMap.PRIVATE,
-        ):
-            raise ValueError(f"Invalid mode: {mode}")
-
-        if detail:
-            return self.__detailed_vs_or_coop(mapped_query, limit, existing_ids)
-        else:
-            return self.__query(mapped_query)
+from typing import Literal, cast, overload
+
+from splatnet3_scraper.query import QueryHandler, QueryResponse
+from splatnet3_scraper.scraper.query_map import QueryMap
+
+
+class SplatNet_Scraper:
+    """This class offers a user-level interface for pulling data from SplatNet
+    3. It is built upon the QueryHandler class and provides a top-level
+    API that orchestrates multiple queries together to reduce the amount of work
+    needed to pull data that users are likely to want.
+    """
+
+    def __init__(self, query_handler: QueryHandler) -> None:
+        """Initializes a SplatNet_Scraper.
+
+        Args:
+            query_handler (QueryHandler): The query handler to use.
+        """
+        self._query_handler = query_handler
+
+    @staticmethod
+    def from_session_token(session_token: str) -> "SplatNet_Scraper":
+        """Creates a SplatNet_Scraper instance using the given session token.
+
+        Args:
+            session_token (str): The session token to use.
+
+        Returns:
+            SplatNet_Scraper: The SplatNet_Scraper instance.
+        """
+        query_handler = QueryHandler.from_session_token(session_token)
+        return SplatNet_Scraper(query_handler)
+
+    @staticmethod
+    def from_config_file(config_path: str | None = None) -> "SplatNet_Scraper":
+        """Creates a SplatNet_Scraper instance using the given config file.
+
+        Args:
+            config_path (str | None): The path to the config file. If None, it
+                will look for ".splatnet3_scraper" in the current working
+                directory.
+
+        Returns:
+            SplatNet_Scraper: The SplatNet_Scraper instance.
+        """
+        query_handler = QueryHandler.from_config_file(config_path)
+        return SplatNet_Scraper(query_handler)
+
+    @staticmethod
+    def from_env() -> "SplatNet_Scraper":
+        """Creates a SplatNet_Scraper instance using the environment variables.
+
+        Environment variables:
+            SN3S_SESSION_TOKEN: The session token to use.
+            SN3S_GTOKEN: The gtoken to use.
+            SN3S_BULLET_TOKEN: The bullet token to use.
+
+        Returns:
+            SplatNet_Scraper: The SplatNet_Scraper instance.
+        """
+        query_handler = QueryHandler.from_env()
+        return SplatNet_Scraper(query_handler)
+
+    @staticmethod
+    def from_s3s_config(config_path: str) -> "SplatNet_Scraper":
+        """Creates a SplatNet_Scraper instance using the config file from s3s.
+
+        Args:
+            config_path (str): The path to the config file.
+
+        Returns:
+            SplatNet_Scraper: The SplatNet_Scraper instance.
+        """
+        query_handler = QueryHandler.from_s3s_config(config_path)
+        return SplatNet_Scraper(query_handler)
+
+    def __query(self, query: str, variables: dict = {}) -> QueryResponse:
+        """Convenience function for querying.
+
+        Args:
+            query (str): The query to run.
+            variables (dict): The variables to pass to the query. Defaults to
+                an empty dict.
+
+        Returns:
+            QueryResponse: The QueryResponse.
+        """
+        return self._query_handler.query(query, variables)
+
+    def __detailed_vs_or_coop(
+        self,
+        query: str,
+        limit: int | None = None,
+        existing_ids: list[str] | str | None = None,
+    ) -> tuple[QueryResponse, list[QueryResponse]]:
+        """Gets the detailed results for a vs battle or coop battle.
+
+        Args:
+            query (str): The query to run.
+            limit (int | None): The maximum number of battles to get. If None,
+                it will get all battles. Defaults to None.
+            existing_ids (list[str] | str | None): The existing IDs to check
+                against. If a string is passed, it will return the results
+                upon finding the first match. If a list is passed, it will
+                return the results of all matches not in the list. If None,
+                it will return all results. Defaults to None.
+
+        Raises:
+            ValueError: If the query is not a vs battle or coop battle.
+
+        Returns:
+            tuple:
+                QueryResponse: The summary query response.
+                list[QueryResponse]: The list of detailed query responses
+                    associated with each battle until the limit is reached.
+        """
+        if query not in (
+            QueryMap.SALMON,
+            QueryMap.TURF,
+            QueryMap.ANARCHY,
+            QueryMap.XBATTLE,
+            QueryMap.PRIVATE,
+        ):
+            raise ValueError(f"Invalid query: {query}")
+
+        if query in (QueryMap.SALMON, QueryMap.SALMON_DETAIL):
+            detail_query = QueryMap.SALMON_DETAIL
+            variable_name = "coopHistoryDetailId"
+        else:
+            detail_query = QueryMap.VS_DETAIL
+            variable_name = "vsResultId"
+
+        _limit = -1 if limit is None else limit
+
+        # Get the list of battles
+        summary_query = self.__query(query)
+
+        # Top level key depends on the game mode, but there is only one.
+        top_level_key = summary_query.keys()[0]
+        history_groups = summary_query[top_level_key, "historyGroups", "nodes"]
+        out: list[QueryResponse] = []
+        idx = 0
+
+        for group in history_groups:
+            group = cast(QueryResponse, group)
+            for game in group["historyDetails", "nodes"]:
+                game = cast(QueryResponse, game)
+                if idx == _limit:
+                    return summary_query, out
+                idx += 1
+                game_id = game["id"]
+
+                if isinstance(existing_ids, str):
+                    if game_id == existing_ids:
+                        return summary_query, out
+                elif isinstance(existing_ids, list):
+                    if game_id in existing_ids:
+                        idx -= 1
+                        continue
+
+                variables = {variable_name: game_id}
+                detailed_game = self.__query(detail_query, variables)
+                out.append(detailed_game)
+
+        return summary_query, out
+
+    @overload
+    def get_vs_battles(
+        self,
+        mode: str,
+        detail: Literal[False],
+        limit: int | None = None,
+        existing_ids: list[str] | str | None = None,
+    ) -> QueryResponse:
+        ...
+
+    @overload
+    def get_vs_battles(
+        self,
+        mode: str,
+        detail: Literal[True],
+        limit: int | None = None,
+        existing_ids: list[str] | str | None = None,
+    ) -> tuple[QueryResponse, list[QueryResponse]]:
+        ...
+
+    @overload
+    def get_vs_battles(
+        self,
+        mode: str,
+        detail: bool = False,
+        limit: int | None = None,
+        existing_ids: list[str] | str | None = None,
+    ) -> QueryResponse | tuple[QueryResponse, list[QueryResponse]]:
+        ...
+
+    def get_vs_battles(
+        self,
+        mode: str,
+        detail: bool = False,
+        limit: int | None = None,
+        existing_ids: list[str] | str | None = None,
+    ) -> QueryResponse | tuple[QueryResponse, list[QueryResponse]]:
+        """Gets the vs battles.
+
+        Args:
+            mode (str): The mode to get the battles for. Some values are:
+                "turf", "anarchy", "xbattle", "private",
+            detail (bool): Whether to get the detailed results or not.
+                Defaults to False.
+            limit (int | None): The maximum number of battles to get. If None,
+                it will get all battles. Defaults to None.
+            existing_ids (list[str] | str | None): The existing IDs to check
+                against. If a string is passed, it will return the results
+                upon finding the first match. If a list is passed, it will
+                return the results of all matches not in the list. If None,
+                it will return all results. Defaults to None.
+
+        Raises:
+            ValueError: If the mode is not valid.
+
+        Returns:
+            QueryResponse : The summary query response, returned regardless of
+                the value of detail.
+            (list[QueryResponse]): The list of detailed query responses
+                associated with each battle until the limit is reached. Only
+                returned if detail is True, along with the summary query
+                response.
+        """
+        mapped_query = QueryMap.get(mode)
+        if mapped_query == QueryMap.SALMON:
+            raise ValueError("Use get_coop_battles for salmon run battles.")
+
+        if mapped_query in (
+            QueryMap.TURF_DETAIL,
+            QueryMap.ANARCHY_DETAIL,
+            QueryMap.XBATTLE_DETAIL,
+            QueryMap.PRIVATE_DETAIL,
+        ):
+            non_detail_map = {
+                QueryMap.TURF_DETAIL: QueryMap.TURF,
+                QueryMap.ANARCHY_DETAIL: QueryMap.ANARCHY,
+                QueryMap.XBATTLE_DETAIL: QueryMap.XBATTLE,
+                QueryMap.PRIVATE_DETAIL: QueryMap.PRIVATE,
+            }
+            mapped_query = non_detail_map[mapped_query]
+            detail = True
+
+        if mapped_query not in (
+            QueryMap.TURF,
+            QueryMap.ANARCHY,
+            QueryMap.XBATTLE,
+            QueryMap.PRIVATE,
+        ):
+            raise ValueError(f"Invalid mode: {mode}")
+
+        if detail:
+            return self.__detailed_vs_or_coop(mapped_query, limit, existing_ids)
+        else:
+            return self.__query(mapped_query)
```

### Comparing `splatnet3_scraper-0.6.4/splatnet3_scraper/scraper/query_map.py` & `splatnet3_scraper-0.7.0/splatnet3_scraper/scraper/query_map.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,142 +1,142 @@
-class QueryMap:
-    BANKARA_BATTLE_HISTORIES = "BankaraBattleHistoriesQuery"
-    BANKARA_BATTLE_HISTORIES_REFETCH = "BankaraBattleHistoriesRefetchQuery"
-    BATTLE_HISTORY_CURRENT_PLAYER = "BattleHistoryCurrentPlayerQuery"
-    CATALOG = "CatalogQuery"
-    CHECKIN = "CheckinQuery"
-    CHECKIN_QR = "CheckinWithQRCodeMutation"
-    CONFIGURE_ANALYTICS = "ConfigureAnalyticsQuery"
-    COOP_HISTORY_DETAIL = "CoopHistoryDetailQuery"
-    COOP_HISTORY_DETAIL_REFETCH = "CoopHistoryDetailRefetchQuery"
-    COOP_HISTORY = "CoopHistoryQuery"
-    COOP_PAGER_LATEST_COOP = "CoopPagerLatestCoopQuery"
-    COOP_RECORD_BIG_RUN_RECORD_CONTAINER_PAGINATION = (
-        "CoopRecordBigRunRecordContainerPaginationQuery"
-    )
-    COOP_RECORD = "CoopRecordQuery"
-    COOP_RECORD_REFETCH = "CoopRecordRefetchQuery"
-    CREATE_MY_OUTFIT_MUTATION = "CreateMyOutfitMutation"
-    DETAIL_FEST_RECORD_DETAIL = "DetailFestRecordDetailQuery"
-    DETAIL_FEST_REFETCH = "DetailFestRefethQuery"
-    DETAIL_FEST_VOTING_STATUS_REFETCH = "DetailFestVotingStatusRefethQuery"
-    DETAIL_RANKING = "DetailRankingQuery"
-    DETAIL_TAB_VIEW_WEAPON_TOPS_AR_REFETCH = (
-        "DetailTabViewWeaponTopsArRefetchQuery"
-    )
-    DETAIL_TAB_VIEW_WEAPON_TOPS_CL_REFETCH = (
-        "DetailTabViewWeaponTopsClRefetchQuery"
-    )
-    DETAIL_TAB_VIEW_WEAPON_TOPS_GL_REFETCH = (
-        "DetailTabViewWeaponTopsGlRefetchQuery"
-    )
-    DETAIL_TAB_VIEW_WEAPON_TOPS_LF_REFETCH = (
-        "DetailTabViewWeaponTopsLFRefetchQuery"
-    )
-    DETAIL_TAB_VIEW_X_RANKING_AR_REFETCH = "DetailTabViewXRankingArRefetchQuery"
-    DETAIL_TAB_VIEW_X_RANKING_CL_REFETCH = "DetailTabViewXRankingClRefetchQuery"
-    DETAIL_TAB_VIEW_X_RANKING_GL_REFETCH = "DetailTabViewXRankingGlRefetchQuery"
-    DETAIL_TAB_VIEW_X_RANKING_LF_REFETCH = "DetailTabViewXRankingLFRefetchQuery"
-    DETAIL_VOTING_STATUS = "DetailVotingStatusQuery"
-    DOWNLOAD_SEARCH_REPLAY = "DownloadSearchReplayQuery"
-    FEST_RECORD = "FestRecordQuery"
-    FEST_RECORD_REFETCH = "FestRecordRefetchQuery"
-    FRIEND_LIST = "FriendListQuery"
-    FRIEND_LIST_REFETCH = "FriendListRefetchQuery"
-    GESOTOWN = "GesotownQuery"
-    GESOTOWN_REFETCH = "GesotownRefetchQuery"
-    HERO_HISTORY = "HeroHistoryQuery"
-    HERO_HISTORY_REFETCH = "HeroHistoryRefetchQuery"
-    HISTORY_RECORD = "HistoryRecordQuery"
-    HISTORY_RECORD_REFETCH = "HistoryRecordRefetchQuery"
-    HOME = "HomeQuery"
-    JOURNEY_CHALLENGE_DETAIL = "JourneyChallengeDetailQuery"
-    JOURNEY_CHALLENGE_DETAIL_REFETCH = "JourneyChallengeDetailRefetchQuery"
-    JOURNEY = "JourneyQuery"
-    JOURNEY_REFETCH = "JourneyRefetchQuery"
-    LATEST_BATTLE_HISTORIES = "LatestBattleHistoriesQuery"
-    LATEST_BATTLE_HISTORIES_REFETCH = "LatestBattleHistoriesRefetchQuery"
-    MY_OUTFITS_DETAIL = "MyOutfitsDetailQuery"
-    MY_OUTFITS = "MyOutfitsQuery"
-    MY_OUTFITS_REFETCH = "MyOutfitsRefetchQuery"
-    PAGER_LATEST_VS_DETAIL = "PagerLatestVsDetailQuery"
-    PAGER_UPDATE_BATTLE_HISTORIES_BY_VS_MODE = (
-        "PagerUpdateBattleHistoriesByVsModeQuery"
-    )
-    PHOTO_ALBUM = "PhotoAlbumQuery"
-    PHOTO_ALBUM_REFETCH = "PhotoAlbumRefetchQuery"
-    PRIVATE_BATTLE_HISTORIES = "PrivateBattleHistoriesQuery"
-    PRIVATE_BATTLE_HISTORIES_REFETCH = "PrivateBattleHistoriesRefetchQuery"
-    RANKING_HOLDERS_FEST_TEAM_RANKING_HOLDERS_PAGINATION = (
-        "RankingHoldersFestTeamRankingHoldersPaginationQuery"
-    )
-    REGULAR_BATTLE_HISTORIES = "RegularBattleHistoriesQuery"
-    REGULAR_BATTLE_HISTORIES_REFETCH = "RegularBattleHistoriesRefetchQuery"
-    REPLAY_MODAL_RESERVE_REPLAY_DOWNLOAD_MUTATION = (
-        "ReplayModalReserveReplayDownloadMutation"
-    )
-    REPLAY = "ReplayQuery"
-    REPLAY_UPLOADED_REPLAY_LIST_REFETCH = "ReplayUploadedReplayListRefetchQuery"
-    SALE_GEAR_DETAIL_ORDER_GESOTOWN_GEAR_MUTATION = (
-        "SaleGearDetailOrderGesotownGearMutation"
-    )
-    SALE_GEAR_DETAIL = "SaleGearDetailQuery"
-    SETTING = "SettingQuery"
-    STAGE_RECORD = "StageRecordQuery"
-    STAGE_RECORDS_REFETCH = "StageRecordsRefetchQuery"
-    STAGE_SCHEDULE = "StageScheduleQuery"
-    SUPPORT_BUTTON_SUPPORT_CHALLENGE_MUTATION = (
-        "SupportButton_SupportChallengeMutation"
-    )
-    UPDATE_MY_OUTFIT_MUTATION = "UpdateMyOutfitMutation"
-    VOTES_UPDATE_FEST_VOTE_MUTATION = "VotesUpdateFestVoteMutation"
-    VS_HISTORY_DETAIL_PAGER_REFETCH = "VsHistoryDetailPagerRefetchQuery"
-    VS_HISTORY_DETAIL = "VsHistoryDetailQuery"
-    WEAPON_RECORD = "WeaponRecordQuery"
-    WEAPON_RECORDS_REFETCH = "WeaponRecordsRefetchQuery"
-    X_BATTLE_HISTORIES = "XBattleHistoriesQuery"
-    X_BATTLE_HISTORIES_REFETCH = "XBattleHistoriesRefetchQuery"
-    X_RANKING_DETAIL = "XRankingDetailQuery"
-    X_RANKING_DETAIL_REFETCH = "XRankingDetailRefetchQuery"
-    X_RANKING = "XRankingQuery"
-    X_RANKING_REFETCH = "XRankingRefetchQuery"
-    MY_OUTFIT_COMMON_DATA_EQUIPMENTS = "myOutfitCommonDataEquipmentsQuery"
-    MY_OUTFIT_COMMON_DATA_FILTERING_CONDITION = (
-        "myOutfitCommonDataFilteringConditionQuery"
-    )
-    REFETCHABLE_COOP_HISTORY_COOP_RESULT = (
-        "refetchableCoopHistory_coopResultQuery"
-    )
-    USE_CURRENT_FEST = "useCurrentFestQuery"
-
-    # Convenience aliases
-    VS_DETAIL = "VsHistoryDetailQuery"
-    SALMON_DETAIL = "CoopHistoryDetailQuery"
-    ANARCHY = "BankaraBattleHistoriesQuery"
-    REGULAR = "RegularBattleHistoriesQuery"
-    XBATTLE = "XBattleHistoriesQuery"
-    PRIVATE = "PrivateBattleHistoriesQuery"
-    LATEST = "LatestBattleHistoriesQuery"
-    SALMON = "CoopHistoryQuery"
-    SALMON_RUN = "CoopHistoryQuery"
-    TURF = "RegularBattleHistoriesQuery"
-    COOP = "CoopHistoryQuery"
-    ANARCHY_DETAIL = "VsHistoryDetailQuery"
-    TURF_DETAIL = "VsHistoryDetailQuery"
-    REGULAR_DETAIL = "VsHistoryDetailQuery"
-    X_DETAIL = "VsHistoryDetailQuery"
-    XBATTLE_DETAIL = "VsHistoryDetailQuery"
-    PRIVATE_DETAIL = "VsHistoryDetailQuery"
-    LATEST_DETAIL = "VsHistoryDetailQuery"
-    COOP_DETAIL = "CoopHistoryDetailQuery"
-
-    @staticmethod
-    def get(query: str) -> str:
-        """Gets the query from the query map.
-
-        Args:
-            query (str): The query to get.
-
-        Returns:
-            str: The query.
-        """
-        return getattr(QueryMap, query.upper())
+class QueryMap:
+    BANKARA_BATTLE_HISTORIES = "BankaraBattleHistoriesQuery"
+    BANKARA_BATTLE_HISTORIES_REFETCH = "BankaraBattleHistoriesRefetchQuery"
+    BATTLE_HISTORY_CURRENT_PLAYER = "BattleHistoryCurrentPlayerQuery"
+    CATALOG = "CatalogQuery"
+    CHECKIN = "CheckinQuery"
+    CHECKIN_QR = "CheckinWithQRCodeMutation"
+    CONFIGURE_ANALYTICS = "ConfigureAnalyticsQuery"
+    COOP_HISTORY_DETAIL = "CoopHistoryDetailQuery"
+    COOP_HISTORY_DETAIL_REFETCH = "CoopHistoryDetailRefetchQuery"
+    COOP_HISTORY = "CoopHistoryQuery"
+    COOP_PAGER_LATEST_COOP = "CoopPagerLatestCoopQuery"
+    COOP_RECORD_BIG_RUN_RECORD_CONTAINER_PAGINATION = (
+        "CoopRecordBigRunRecordContainerPaginationQuery"
+    )
+    COOP_RECORD = "CoopRecordQuery"
+    COOP_RECORD_REFETCH = "CoopRecordRefetchQuery"
+    CREATE_MY_OUTFIT_MUTATION = "CreateMyOutfitMutation"
+    DETAIL_FEST_RECORD_DETAIL = "DetailFestRecordDetailQuery"
+    DETAIL_FEST_REFETCH = "DetailFestRefethQuery"
+    DETAIL_FEST_VOTING_STATUS_REFETCH = "DetailFestVotingStatusRefethQuery"
+    DETAIL_RANKING = "DetailRankingQuery"
+    DETAIL_TAB_VIEW_WEAPON_TOPS_AR_REFETCH = (
+        "DetailTabViewWeaponTopsArRefetchQuery"
+    )
+    DETAIL_TAB_VIEW_WEAPON_TOPS_CL_REFETCH = (
+        "DetailTabViewWeaponTopsClRefetchQuery"
+    )
+    DETAIL_TAB_VIEW_WEAPON_TOPS_GL_REFETCH = (
+        "DetailTabViewWeaponTopsGlRefetchQuery"
+    )
+    DETAIL_TAB_VIEW_WEAPON_TOPS_LF_REFETCH = (
+        "DetailTabViewWeaponTopsLFRefetchQuery"
+    )
+    DETAIL_TAB_VIEW_X_RANKING_AR_REFETCH = "DetailTabViewXRankingArRefetchQuery"
+    DETAIL_TAB_VIEW_X_RANKING_CL_REFETCH = "DetailTabViewXRankingClRefetchQuery"
+    DETAIL_TAB_VIEW_X_RANKING_GL_REFETCH = "DetailTabViewXRankingGlRefetchQuery"
+    DETAIL_TAB_VIEW_X_RANKING_LF_REFETCH = "DetailTabViewXRankingLFRefetchQuery"
+    DETAIL_VOTING_STATUS = "DetailVotingStatusQuery"
+    DOWNLOAD_SEARCH_REPLAY = "DownloadSearchReplayQuery"
+    FEST_RECORD = "FestRecordQuery"
+    FEST_RECORD_REFETCH = "FestRecordRefetchQuery"
+    FRIEND_LIST = "FriendListQuery"
+    FRIEND_LIST_REFETCH = "FriendListRefetchQuery"
+    GESOTOWN = "GesotownQuery"
+    GESOTOWN_REFETCH = "GesotownRefetchQuery"
+    HERO_HISTORY = "HeroHistoryQuery"
+    HERO_HISTORY_REFETCH = "HeroHistoryRefetchQuery"
+    HISTORY_RECORD = "HistoryRecordQuery"
+    HISTORY_RECORD_REFETCH = "HistoryRecordRefetchQuery"
+    HOME = "HomeQuery"
+    JOURNEY_CHALLENGE_DETAIL = "JourneyChallengeDetailQuery"
+    JOURNEY_CHALLENGE_DETAIL_REFETCH = "JourneyChallengeDetailRefetchQuery"
+    JOURNEY = "JourneyQuery"
+    JOURNEY_REFETCH = "JourneyRefetchQuery"
+    LATEST_BATTLE_HISTORIES = "LatestBattleHistoriesQuery"
+    LATEST_BATTLE_HISTORIES_REFETCH = "LatestBattleHistoriesRefetchQuery"
+    MY_OUTFITS_DETAIL = "MyOutfitsDetailQuery"
+    MY_OUTFITS = "MyOutfitsQuery"
+    MY_OUTFITS_REFETCH = "MyOutfitsRefetchQuery"
+    PAGER_LATEST_VS_DETAIL = "PagerLatestVsDetailQuery"
+    PAGER_UPDATE_BATTLE_HISTORIES_BY_VS_MODE = (
+        "PagerUpdateBattleHistoriesByVsModeQuery"
+    )
+    PHOTO_ALBUM = "PhotoAlbumQuery"
+    PHOTO_ALBUM_REFETCH = "PhotoAlbumRefetchQuery"
+    PRIVATE_BATTLE_HISTORIES = "PrivateBattleHistoriesQuery"
+    PRIVATE_BATTLE_HISTORIES_REFETCH = "PrivateBattleHistoriesRefetchQuery"
+    RANKING_HOLDERS_FEST_TEAM_RANKING_HOLDERS_PAGINATION = (
+        "RankingHoldersFestTeamRankingHoldersPaginationQuery"
+    )
+    REGULAR_BATTLE_HISTORIES = "RegularBattleHistoriesQuery"
+    REGULAR_BATTLE_HISTORIES_REFETCH = "RegularBattleHistoriesRefetchQuery"
+    REPLAY_MODAL_RESERVE_REPLAY_DOWNLOAD_MUTATION = (
+        "ReplayModalReserveReplayDownloadMutation"
+    )
+    REPLAY = "ReplayQuery"
+    REPLAY_UPLOADED_REPLAY_LIST_REFETCH = "ReplayUploadedReplayListRefetchQuery"
+    SALE_GEAR_DETAIL_ORDER_GESOTOWN_GEAR_MUTATION = (
+        "SaleGearDetailOrderGesotownGearMutation"
+    )
+    SALE_GEAR_DETAIL = "SaleGearDetailQuery"
+    SETTING = "SettingQuery"
+    STAGE_RECORD = "StageRecordQuery"
+    STAGE_RECORDS_REFETCH = "StageRecordsRefetchQuery"
+    STAGE_SCHEDULE = "StageScheduleQuery"
+    SUPPORT_BUTTON_SUPPORT_CHALLENGE_MUTATION = (
+        "SupportButton_SupportChallengeMutation"
+    )
+    UPDATE_MY_OUTFIT_MUTATION = "UpdateMyOutfitMutation"
+    VOTES_UPDATE_FEST_VOTE_MUTATION = "VotesUpdateFestVoteMutation"
+    VS_HISTORY_DETAIL_PAGER_REFETCH = "VsHistoryDetailPagerRefetchQuery"
+    VS_HISTORY_DETAIL = "VsHistoryDetailQuery"
+    WEAPON_RECORD = "WeaponRecordQuery"
+    WEAPON_RECORDS_REFETCH = "WeaponRecordsRefetchQuery"
+    X_BATTLE_HISTORIES = "XBattleHistoriesQuery"
+    X_BATTLE_HISTORIES_REFETCH = "XBattleHistoriesRefetchQuery"
+    X_RANKING_DETAIL = "XRankingDetailQuery"
+    X_RANKING_DETAIL_REFETCH = "XRankingDetailRefetchQuery"
+    X_RANKING = "XRankingQuery"
+    X_RANKING_REFETCH = "XRankingRefetchQuery"
+    MY_OUTFIT_COMMON_DATA_EQUIPMENTS = "myOutfitCommonDataEquipmentsQuery"
+    MY_OUTFIT_COMMON_DATA_FILTERING_CONDITION = (
+        "myOutfitCommonDataFilteringConditionQuery"
+    )
+    REFETCHABLE_COOP_HISTORY_COOP_RESULT = (
+        "refetchableCoopHistory_coopResultQuery"
+    )
+    USE_CURRENT_FEST = "useCurrentFestQuery"
+
+    # Convenience aliases
+    VS_DETAIL = "VsHistoryDetailQuery"
+    SALMON_DETAIL = "CoopHistoryDetailQuery"
+    ANARCHY = "BankaraBattleHistoriesQuery"
+    REGULAR = "RegularBattleHistoriesQuery"
+    XBATTLE = "XBattleHistoriesQuery"
+    PRIVATE = "PrivateBattleHistoriesQuery"
+    LATEST = "LatestBattleHistoriesQuery"
+    SALMON = "CoopHistoryQuery"
+    SALMON_RUN = "CoopHistoryQuery"
+    TURF = "RegularBattleHistoriesQuery"
+    COOP = "CoopHistoryQuery"
+    ANARCHY_DETAIL = "VsHistoryDetailQuery"
+    TURF_DETAIL = "VsHistoryDetailQuery"
+    REGULAR_DETAIL = "VsHistoryDetailQuery"
+    X_DETAIL = "VsHistoryDetailQuery"
+    XBATTLE_DETAIL = "VsHistoryDetailQuery"
+    PRIVATE_DETAIL = "VsHistoryDetailQuery"
+    LATEST_DETAIL = "VsHistoryDetailQuery"
+    COOP_DETAIL = "CoopHistoryDetailQuery"
+
+    @staticmethod
+    def get(query: str) -> str:
+        """Gets the query from the query map.
+
+        Args:
+            query (str): The query to get.
+
+        Returns:
+            str: The query.
+        """
+        return getattr(QueryMap, query.upper())
```

### Comparing `splatnet3_scraper-0.6.4/setup.py` & `splatnet3_scraper-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,203 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: splatnet3-scraper
+Version: 0.7.0
+Summary: Scraper for SplatNet 3 for Splatoon 3
+License: GPL-3.0-or-later
+Author: Cesar E Garza
+Author-email: cesar@cegarza.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: all
+Provides-Extra: examples
+Provides-Extra: parquet
+Requires-Dist: pandas[examples] (>=1.5.3,<2.0.0) ; extra == "examples"
+Requires-Dist: psycopg2[examples] (>=2.9.5,<3.0.0) ; extra == "examples"
+Requires-Dist: pyarrow[parquet] (>=10.0.1,<11.0.0) ; extra == "parquet"
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: sqlalchemy[examples] (>=2.0.1,<3.0.0) ; extra == "examples"
+Description-Content-Type: text/markdown
 
-packages = \
-['splatnet3_scraper',
- 'splatnet3_scraper.auth',
- 'splatnet3_scraper.query',
- 'splatnet3_scraper.scraper']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.28.1,<3.0.0']
-
-extras_require = \
-{'examples': ['pandas[examples]>=1.5.3,<2.0.0',
-              'sqlalchemy[examples]>=2.0.1,<3.0.0',
-              'psycopg2[examples]>=2.9.5,<3.0.0'],
- 'parquet': ['pyarrow[parquet]>=10.0.1,<11.0.0']}
-
-setup_kwargs = {
-    'name': 'splatnet3-scraper',
-    'version': '0.6.4',
-    'description': 'Scraper for SplatNet 3 for Splatoon 3',
-    'long_description': '# SplatNet 3 Scraper\n\n[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.\n\n**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.\n\n## Features\n\n* Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.\n* The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.\n* The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.\n* The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.\n* Compatibility with the configuration file format used by `s3s`.\n* Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:\n  * JSON\n  * gzip-compressed JSON\n  * csv\n  * parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n* Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).\n\n## Installation\n\n**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:\n\n```bash\npip install splatnet3_scraper\n```\n\nNote that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.\n\n## Usage\n\nThere are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can\'t find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.\n\n### Using the `scraper` module\n\nThe `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.\n\nThis module is currently under active development and is not yet complete. Please check back later for more functions.\n\n### Using the `query` module\n\nThe `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.\n\nThe `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.\n\n#### Instantiating the `QueryHandler` class by providing a session token\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_session_token("session_token")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by providing the path to a configuration file\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_config_file(".splatnet3_scraper")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by loading environment variables\n\nThe following environment variables are supported:\n\n* `SN3S_SESSION_TOKEN`\n* `SN3S_GTOKEN`\n* `SN3S_BULLET_TOKEN`\n\n```python\nfrom splatnet3_scrape.query import QueryHandler\nhandler = QueryHandler.from_env()\nhandler.query("StageScheduleQuery")\n```\n\n#### Querying the SplatNet 3 API\n\nThe `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nprint(response["xSchedules", "nodes", 0, "vsRule", "name"])\n```\n\n#### Saving and loading responses\n\nThe `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:\n\n* JSON\n* gzip-compressed JSON\n* csv\n* parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n\nNote: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.\n\nThe following code will save the response data to a file named `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nresponse.parsed_json().to_json("response.json")\n```\n\nAdditionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import JSONParser\nparser = JSONParser.from_json("response.json")\n```\n\n## Symbols\n\n| Symbol | Meaning |\n| ------ | ------- |\n| :white_check_mark: | Implemented |\n| :construction: | In progress |\n| :world_map: | Planned |\n| :x: | Not planned |\n\n## Roadmap\n\n| Feature | Status |\n| ------- | ------ |\n| Support for the SplatNet 3 API | :white_check_mark: |\n| Full support for the SplatNet 3 API | :world_map: |\n| Support for the SplatNet 2 API | :x: |\n| Obtaining session tokens | :white_check_mark: |\n| Full documentation | :construction: |\n| Full unit test coverage | :white_check_mark: |\n| Columnar data format support | :construction: |\n| CLI interface | :x: |\n| Integration with stat.ink | :x: |\n| PyPI package | :white_check_mark: |\n| Docker image | :world_map: |\n| Executable binary | :x: |\n\n## Docker Note\n\nThis project currently uses the standard library heavily, and as such it is not compatible with the `python:alpine` Docker image. I have no plans to change this. Use the `python:slim` image instead.\n\nQueryHandler is licensed under the GPLv3. See the LICENSE file for more details.\n',
-    'author': 'Cesar E Garza',
-    'author_email': 'cesar@cegarza.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.10,<4.0',
-}
+# SplatNet 3 Scraper
 
+[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.
+
+**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.
+
+## Table of Contents
+
+1. [Features](#features)
+2. [Documentation](#documentation)
+3. [Installation](#installation)
+4. [Usage](#usage)
+   - [Using the `scraper` module](#using-the-scraper-module)
+   - [Using the `query` module](#using-the-query-module)
+   - [Using the `auth` module](#using-the-auth-module)
+5. [Roadmap](#roadmap)
+6. [Contributing](#contributing)
+7. [License](#license)
+
+## Features
+
+- Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.
+- The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.
+- The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.
+- The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.
+- Compatibility with the configuration file format used by `s3s`.
+- Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:
+  - JSON
+  - gzip-compressed JSON
+  - csv
+  - parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)
+- Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).
+
+## Documentation
+
+Detailed documentation for SplatNet 3 Scraper, including usage instructions, examples, and API reference, is available on Read the Docs:
+
+[**SplatNet 3 Scraper Documentation**](https://splatnet3-scraper.readthedocs.io/en/latest/index.html)
+
+We highly recommend referring to the documentation to get the most out of SplatNet 3 Scraper and understand its full capabilities.
+
+## Installation
+
+**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:
+
+```bash
+pip install splatnet3_scraper
+```
+
+Note that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.
+
+## Usage
+
+There are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can't find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.
+
+### Using the `scraper` module
+
+The `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.
+
+This module is currently under active development and is not yet complete. Please check back later for more functions.
+
+### Using the `query` module
+
+The `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.
+
+The `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.
+
+### Using the `auth` module
+
+:warning: **Warning: The `auth` module is intended for advanced users only. Most users should use the `scraper` or `query` modules for a simpler and more convenient experience.**
+
+The `auth` module provides a low-level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication and is designed for advanced developers who need full control over the authentication process.
+
+To use the `auth` module, you will need to import the necessary components and handle the authentication flow manually. Please refer to the [documentation](https://splatnet3-scraper.readthedocs.io/en/latest/index.html) for detailed instructions and examples on how to use the `auth` module.
+
+#### Instantiating the `QueryHandler` class by providing a session token
+
+```python
+from splatnet3_scraper.query import QueryHandler
+handler = QueryHandler.from_session_token("session_token")
+handler.query("StageScheduleQuery")
+```
+
+#### Instantiating the `QueryHandler` class by providing the path to a configuration file
+
+```python
+from splatnet3_scraper.query import QueryHandler
+handler = QueryHandler.from_config_file(".splatnet3_scraper")
+handler.query("StageScheduleQuery")
+```
+
+#### Instantiating the `QueryHandler` class by loading environment variables
+
+The following environment variables are supported:
+
+- `SN3S_SESSION_TOKEN`
+- `SN3S_GTOKEN`
+- `SN3S_BULLET_TOKEN`
+
+```python
+from splatnet3_scrape.query import QueryHandler
+handler = QueryHandler.from_env()
+handler.query("StageScheduleQuery")
+```
+
+#### Querying the SplatNet 3 API
+
+The `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:
+
+```python
+from splatnet3_scraper.query import QueryHandler
+handler = QueryHandler.from_env()
+response = handler.query("StageScheduleQuery")
+print(response["xSchedules", "nodes", 0, "vsRule", "name"])
+```
+
+#### Saving and loading responses
+
+The `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:
+
+- JSON
+- gzip-compressed JSON
+- csv
+- parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)
+
+Note: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.
+
+The following code will save the response data to a file named `response.json` in the current directory:
+
+```python
+from splatnet3_scraper.query import QueryHandler
+handler = QueryHandler.from_env()
+response = handler.query("StageScheduleQuery")
+response.parsed_json().to_json("response.json")
+```
+
+Additionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:
+
+```python
+from splatnet3_scraper.query import JSONParser
+parser = JSONParser.from_json("response.json")
+```
+
+## Symbols
+
+| Symbol | Meaning |
+| ------ | ------- |
+| :white_check_mark: | Implemented |
+| :construction: | In progress |
+| :world_map: | Planned |
+| :x: | Not planned |
+
+## Roadmap
+
+| Feature | Status |
+| ------- | ------ |
+| Support for the SplatNet 3 API | :white_check_mark: |
+| Full support for the SplatNet 3 API | :world_map: |
+| Support for the SplatNet 2 API | :x: |
+| Obtaining session tokens | :white_check_mark: |
+| Full documentation | :construction: |
+| Full unit test coverage | :white_check_mark: |
+| Columnar data format support | :construction: |
+| CLI interface | :x: |
+| Integration with stat.ink | :x: |
+| PyPI package | :white_check_mark: |
+| Docker image | :world_map: |
+| Executable binary | :x: |
+
+## Contributing
+
+We welcome contributions to SplatNet 3 Scraper! For detailed information on how to contribute, please refer to our [CONTRIBUTING.md](./CONTRIBUTING.md) file.
+
+To report issues or request new features, please open an issue on the GitHub repository.
+
+## License
+
+SplatNet 3 Scraper is licensed under the GPLv3. See the [LICENSE](./LICENSE) file for more details.
 
-setup(**setup_kwargs)
```

### Comparing `splatnet3_scraper-0.6.4/PKG-INFO` & `splatnet3_scraper-0.7.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,170 +1,40 @@
-Metadata-Version: 2.1
-Name: splatnet3-scraper
-Version: 0.6.4
-Summary: Scraper for SplatNet 3 for Splatoon 3
-License: GPL-3.0-or-later
-Author: Cesar E Garza
-Author-email: cesar@cegarza.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Provides-Extra: all
-Provides-Extra: examples
-Provides-Extra: parquet
-Requires-Dist: pandas[examples] (>=1.5.3,<2.0.0) ; extra == "examples"
-Requires-Dist: psycopg2[examples] (>=2.9.5,<3.0.0) ; extra == "examples"
-Requires-Dist: pyarrow[parquet] (>=10.0.1,<11.0.0) ; extra == "parquet"
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: sqlalchemy[examples] (>=2.0.1,<3.0.0) ; extra == "examples"
-Description-Content-Type: text/markdown
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-# SplatNet 3 Scraper
+packages = \
+['splatnet3_scraper',
+ 'splatnet3_scraper.auth',
+ 'splatnet3_scraper.query',
+ 'splatnet3_scraper.scraper']
+
+package_data = \
+{'': ['*']}
+
+install_requires = \
+['requests>=2.28.1,<3.0.0']
+
+extras_require = \
+{'examples': ['pandas[examples]>=1.5.3,<2.0.0',
+              'sqlalchemy[examples]>=2.0.1,<3.0.0',
+              'psycopg2[examples]>=2.9.5,<3.0.0'],
+ 'parquet': ['pyarrow[parquet]>=10.0.1,<11.0.0']}
+
+setup_kwargs = {
+    'name': 'splatnet3-scraper',
+    'version': '0.7.0',
+    'description': 'Scraper for SplatNet 3 for Splatoon 3',
+    'long_description': '# SplatNet 3 Scraper\n\n[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.\n\n**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.\n\n## Table of Contents\n\n1. [Features](#features)\n2. [Documentation](#documentation)\n3. [Installation](#installation)\n4. [Usage](#usage)\n   - [Using the `scraper` module](#using-the-scraper-module)\n   - [Using the `query` module](#using-the-query-module)\n   - [Using the `auth` module](#using-the-auth-module)\n5. [Roadmap](#roadmap)\n6. [Contributing](#contributing)\n7. [License](#license)\n\n## Features\n\n- Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.\n- The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.\n- The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.\n- The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.\n- Compatibility with the configuration file format used by `s3s`.\n- Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:\n  - JSON\n  - gzip-compressed JSON\n  - csv\n  - parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n- Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).\n\n## Documentation\n\nDetailed documentation for SplatNet 3 Scraper, including usage instructions, examples, and API reference, is available on Read the Docs:\n\n[**SplatNet 3 Scraper Documentation**](https://splatnet3-scraper.readthedocs.io/en/latest/index.html)\n\nWe highly recommend referring to the documentation to get the most out of SplatNet 3 Scraper and understand its full capabilities.\n\n## Installation\n\n**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:\n\n```bash\npip install splatnet3_scraper\n```\n\nNote that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.\n\n## Usage\n\nThere are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can\'t find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.\n\n### Using the `scraper` module\n\nThe `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.\n\nThis module is currently under active development and is not yet complete. Please check back later for more functions.\n\n### Using the `query` module\n\nThe `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.\n\nThe `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.\n\n### Using the `auth` module\n\n:warning: **Warning: The `auth` module is intended for advanced users only. Most users should use the `scraper` or `query` modules for a simpler and more convenient experience.**\n\nThe `auth` module provides a low-level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication and is designed for advanced developers who need full control over the authentication process.\n\nTo use the `auth` module, you will need to import the necessary components and handle the authentication flow manually. Please refer to the [documentation](https://splatnet3-scraper.readthedocs.io/en/latest/index.html) for detailed instructions and examples on how to use the `auth` module.\n\n#### Instantiating the `QueryHandler` class by providing a session token\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_session_token("session_token")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by providing the path to a configuration file\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_config_file(".splatnet3_scraper")\nhandler.query("StageScheduleQuery")\n```\n\n#### Instantiating the `QueryHandler` class by loading environment variables\n\nThe following environment variables are supported:\n\n- `SN3S_SESSION_TOKEN`\n- `SN3S_GTOKEN`\n- `SN3S_BULLET_TOKEN`\n\n```python\nfrom splatnet3_scrape.query import QueryHandler\nhandler = QueryHandler.from_env()\nhandler.query("StageScheduleQuery")\n```\n\n#### Querying the SplatNet 3 API\n\nThe `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nprint(response["xSchedules", "nodes", 0, "vsRule", "name"])\n```\n\n#### Saving and loading responses\n\nThe `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:\n\n- JSON\n- gzip-compressed JSON\n- csv\n- parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)\n\nNote: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.\n\nThe following code will save the response data to a file named `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import QueryHandler\nhandler = QueryHandler.from_env()\nresponse = handler.query("StageScheduleQuery")\nresponse.parsed_json().to_json("response.json")\n```\n\nAdditionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:\n\n```python\nfrom splatnet3_scraper.query import JSONParser\nparser = JSONParser.from_json("response.json")\n```\n\n## Symbols\n\n| Symbol | Meaning |\n| ------ | ------- |\n| :white_check_mark: | Implemented |\n| :construction: | In progress |\n| :world_map: | Planned |\n| :x: | Not planned |\n\n## Roadmap\n\n| Feature | Status |\n| ------- | ------ |\n| Support for the SplatNet 3 API | :white_check_mark: |\n| Full support for the SplatNet 3 API | :world_map: |\n| Support for the SplatNet 2 API | :x: |\n| Obtaining session tokens | :white_check_mark: |\n| Full documentation | :construction: |\n| Full unit test coverage | :white_check_mark: |\n| Columnar data format support | :construction: |\n| CLI interface | :x: |\n| Integration with stat.ink | :x: |\n| PyPI package | :white_check_mark: |\n| Docker image | :world_map: |\n| Executable binary | :x: |\n\n## Contributing\n\nWe welcome contributions to SplatNet 3 Scraper! For detailed information on how to contribute, please refer to our [CONTRIBUTING.md](./CONTRIBUTING.md) file.\n\nTo report issues or request new features, please open an issue on the GitHub repository.\n\n## License\n\nSplatNet 3 Scraper is licensed under the GPLv3. See the [LICENSE](./LICENSE) file for more details.\n',
+    'author': 'Cesar E Garza',
+    'author_email': 'cesar@cegarza.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'extras_require': extras_require,
+    'python_requires': '>=3.10,<4.0',
+}
 
-[![Tests Status](./reports/junit/tests-badge.svg?dummy=8484744)](https://htmlpreview.github.io/?https://github.com/cesaregarza/SplatNet3_Scraper/blob/main/reports/junit/report.html) ![Coverage Status](./reports/coverage/coverage-badge.svg?dummy=8484744) ![Flake8 Status](./reports/flake8/flake8-badge.svg?dummy=8484744) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-**SplatNet 3 Scraper** is a Python library for scraping data from the Splatoon 3 SplatNet 3 API. It is designed to be as lightweight as possible, with minimal dependencies to make it easy to integrate into other projects.
-
-**SplatNet 3 Scraper** started as a fork of **[s3s](https://github.com/frozenpandaman/s3s)**, but has since been rewritten from scratch while incorporating much of the login flow logic of s3s. As a result, I am deeply indebted to the authors of s3s for their work. This project would not have been possible without their efforts.
-
-## Features
-
-* Lightweight and minimal dependencies. Only requires the `requests` library. Requires Python 3.10 or later.
-* The `scraper` module provides a user-level API that enables a quick and easy way to get data from the SplatNet 3 API, only requiring the user to provide their session token.
-* The `query` module provides a high-level API that provides a simple way to make queries to the SplatNet 3 API. It automatically handles authentication and query handling, and provides a simple interface for accessing the response data.
-* The `auth` module provides a low level API that allows for more fine-grained control over the scraping process. It greatly simplifies the process of authentication.
-* Compatibility with the configuration file format used by `s3s`.
-* Responses from the SplatNet 3 API can be saved and loaded from disk, currently supporting the following formats:
-  * JSON
-  * gzip-compressed JSON
-  * csv
-  * parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)
-* Heavily documented codebase, with extensive docstrings and type annotations for nearly all functions and classes. The documentation is also available on [Read the Docs](https://splatnet3-scraper.readthedocs.io/en/latest/index.html).
-
-## Installation
-
-**SplatNet 3 Scraper** is currently under active development but is currently available on PyPI. It can be installed using pip:
-
-```bash
-pip install splatnet3_scraper
-```
-
-Note that the current versions of **SplatNet 3 Scraper** are currently `v0.x.y`, which means that the API is not guaranteed to be stable and may change at any moment. As such, it is highly recommended that you pin the version of **SplatNet 3 Scraper** that you are using until the API is stabilized with the release of `v1.0.0`.
-
-## Usage
-
-There are three ways to use **SplatNet 3 Scraper**. The first is to use the `scraper` module, which provides a top-level API that greatly simplifies the process of retrieving commonly requested data from SplatNet 3. This module is greatly recommended for most users. The second is to use the `query` module, which provides a high-level API that provides a simple interface to make queries to the SplatNet 3 API. This module is recommended for developers who can't find what they need with the `scraper` module. The third is to use the `auth` module, which provides a low-level API that gives the user the most control over the scraping process. This module is recommended for advanced developers who need to have full control over the authentication process. Whichever module you choose to use, all of them require providing a session token.
-
-### Using the `scraper` module
-
-The `scraper` module is by far the easiest way to get data from the SplatNet 3 API and the module that is recommended for most users, especially those who are not highly experienced with Python. The `scraper` module provides multiple functions that can be used to retrieve commonly requested data from the SplatNet 3 API. The `scraper` module is designed to be used by users who are not highly experienced with Python or users who do not need to have full control over the scraping process.
-
-This module is currently under active development and is not yet complete. Please check back later for more functions.
-
-### Using the `query` module
-
-The `query` module is an easy-to-use module that enables fast and painless querying to the SplatNet 3 API. It handles authentication and query handling automagically, and provides a simple interface for accessing the response data. The `query` module is designed to be used by advanced users who need more control over the queries they make to the SplatNet 3 API. If you are looking for a simple way to get data from the SplatNet 3 API, you should use the `scraper` module instead.
-
-The `query` module provides the `QueryHandler` class, which is used to make queries to the SplatNet 3 API. The `QueryHandler` class can be instantiated in one of a few ways: by providing a session token, by providing the path to a configuration file, or by loading environment variables.
-
-#### Instantiating the `QueryHandler` class by providing a session token
-
-```python
-from splatnet3_scraper.query import QueryHandler
-handler = QueryHandler.from_session_token("session_token")
-handler.query("StageScheduleQuery")
-```
-
-#### Instantiating the `QueryHandler` class by providing the path to a configuration file
-
-```python
-from splatnet3_scraper.query import QueryHandler
-handler = QueryHandler.from_config_file(".splatnet3_scraper")
-handler.query("StageScheduleQuery")
-```
-
-#### Instantiating the `QueryHandler` class by loading environment variables
-
-The following environment variables are supported:
-
-* `SN3S_SESSION_TOKEN`
-* `SN3S_GTOKEN`
-* `SN3S_BULLET_TOKEN`
-
-```python
-from splatnet3_scrape.query import QueryHandler
-handler = QueryHandler.from_env()
-handler.query("StageScheduleQuery")
-```
-
-#### Querying the SplatNet 3 API
-
-The `QueryHandler` class provides a `query` method that can be used to make queries to the SplatNet 3 API. The `query` method takes a single argument, which is the name of the query to make. The `query` method returns a `QueryResponse` object, which contains the response data from the SplatNet 3 API. The `QueryResponse` object provides a `data` property that can be used to access the response data. The `QueryResponse` module also supports numpy-style indexing, which can be used to quickly and clearly access specific parts of the response data. For example, the following code will print the game mode name of the the current stage rotation schedule:
-
-```python
-from splatnet3_scraper.query import QueryHandler
-handler = QueryHandler.from_env()
-response = handler.query("StageScheduleQuery")
-print(response["xSchedules", "nodes", 0, "vsRule", "name"])
-```
-
-#### Saving and loading responses
-
-The `QueryResponse` class provides a `parsed_json` method that can be used to generate a `JSONParser` object from the response data. The `JSONParser` class provides multiple ways of interacting with the given data, including the ability to save the data to disk in a variety of formats. There are currently four different formats that are supported and can be used by passing the desired format to a `to_*` method such as `to_json`. The following formats are supported:
-
-* JSON
-* gzip-compressed JSON
-* csv
-* parquet (by installing `splatnet3_scraper[parquet]` or the `pyarrow` library)
-
-Note: csv and parquet formats work by converting the response data from a nested dictionary to a columnar format. This is not recommended for single queries, but can be useful for interacting with large amounts of data as it deduplicates the JSON structure and allows for more efficient storage and querying.
-
-The following code will save the response data to a file named `response.json` in the current directory:
-
-```python
-from splatnet3_scraper.query import QueryHandler
-handler = QueryHandler.from_env()
-response = handler.query("StageScheduleQuery")
-response.parsed_json().to_json("response.json")
-```
-
-Additionally, the `JSONParser` class provides a `from_*` method that can be used to load data from a file. The following code will load the response data from the file `response.json` in the current directory:
-
-```python
-from splatnet3_scraper.query import JSONParser
-parser = JSONParser.from_json("response.json")
-```
-
-## Symbols
-
-| Symbol | Meaning |
-| ------ | ------- |
-| :white_check_mark: | Implemented |
-| :construction: | In progress |
-| :world_map: | Planned |
-| :x: | Not planned |
-
-## Roadmap
-
-| Feature | Status |
-| ------- | ------ |
-| Support for the SplatNet 3 API | :white_check_mark: |
-| Full support for the SplatNet 3 API | :world_map: |
-| Support for the SplatNet 2 API | :x: |
-| Obtaining session tokens | :white_check_mark: |
-| Full documentation | :construction: |
-| Full unit test coverage | :white_check_mark: |
-| Columnar data format support | :construction: |
-| CLI interface | :x: |
-| Integration with stat.ink | :x: |
-| PyPI package | :white_check_mark: |
-| Docker image | :world_map: |
-| Executable binary | :x: |
-
-## Docker Note
-
-This project currently uses the standard library heavily, and as such it is not compatible with the `python:alpine` Docker image. I have no plans to change this. Use the `python:slim` image instead.
-
-QueryHandler is licensed under the GPLv3. See the LICENSE file for more details.
 
+setup(**setup_kwargs)
```

