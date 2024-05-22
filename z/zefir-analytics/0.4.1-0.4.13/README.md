# Comparing `tmp/zefir-analytics-0.4.1.tar.gz` & `tmp/zefir-analytics-0.4.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zefir-analytics-0.4.1.tar", last modified: Thu Mar 21 14:35:50 2024, max compression
+gzip compressed data, was "zefir-analytics-0.4.13.tar", last modified: Wed May 22 17:39:52 2024, max compression
```

## Comparing `zefir-analytics-0.4.1.tar` & `zefir-analytics-0.4.13.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 kruksik   (1000) kruksik   (1000)        0 2024-03-21 14:35:50.729480 zefir-analytics-0.4.1/
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)    34523 2024-02-06 10:20:41.000000 zefir-analytics-0.4.1/LICENSE.txt
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)    42408 2024-03-21 14:35:50.729480 zefir-analytics-0.4.1/PKG-INFO
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     1475 2024-02-06 10:20:41.000000 zefir-analytics-0.4.1/README.md
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     2650 2024-03-21 14:34:13.000000 zefir-analytics-0.4.1/pyproject.toml
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)       38 2024-03-21 14:35:50.729480 zefir-analytics-0.4.1/setup.cfg
-drwxr-xr-x   0 kruksik   (1000) kruksik   (1000)        0 2024-03-21 14:35:50.729480 zefir-analytics-0.4.1/zefir_analytics/
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)      846 2024-03-21 14:34:13.000000 zefir-analytics-0.4.1/zefir_analytics/__init__.py
-drwxr-xr-x   0 kruksik   (1000) kruksik   (1000)        0 2024-03-21 14:35:50.729480 zefir-analytics-0.4.1/zefir_analytics/_engine/
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     1474 2024-03-21 14:34:13.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/__init__.py
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     1103 2024-02-16 15:43:57.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/constants.py
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     3133 2024-03-21 14:34:13.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/data_loader.py
-drwxr-xr-x   0 kruksik   (1000) kruksik   (1000)        0 2024-03-21 14:35:50.729480 zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)      735 2024-02-06 10:20:41.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/__init__.py
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     3659 2024-02-06 10:20:41.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/aggregated_consumer_parameters_over_years.py
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     4598 2024-02-06 10:20:41.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/lbs_parameters_over_years.py
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     4246 2024-02-16 15:43:57.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/line_parameters_over_years.py
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)    27713 2024-03-21 14:34:13.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/source_parameters_over_years.py
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     1380 2024-02-16 15:43:57.000000 zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/utils.py
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)     6157 2024-03-21 14:34:13.000000 zefir-analytics-0.4.1/zefir_analytics/zefir_engine.py
-drwxr-xr-x   0 kruksik   (1000) kruksik   (1000)        0 2024-03-21 14:35:50.729480 zefir-analytics-0.4.1/zefir_analytics.egg-info/
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)    42408 2024-03-21 14:35:50.000000 zefir-analytics-0.4.1/zefir_analytics.egg-info/PKG-INFO
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)      781 2024-03-21 14:35:50.000000 zefir-analytics-0.4.1/zefir_analytics.egg-info/SOURCES.txt
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)        1 2024-03-21 14:35:50.000000 zefir-analytics-0.4.1/zefir_analytics.egg-info/dependency_links.txt
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)      217 2024-03-21 14:35:50.000000 zefir-analytics-0.4.1/zefir_analytics.egg-info/requires.txt
--rw-r--r--   0 kruksik   (1000) kruksik   (1000)       16 2024-03-21 14:35:50.000000 zefir-analytics-0.4.1/zefir_analytics.egg-info/top_level.txt
+drwxr-xr-x   0 akartashov  (1000) akartashov  (1000)        0 2024-05-22 17:39:52.515311 zefir-analytics-0.4.13/
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)    35184 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/LICENSE.txt
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)    42617 2024-05-22 17:39:52.515311 zefir-analytics-0.4.13/PKG-INFO
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     1766 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/README.md
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     2759 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/pyproject.toml
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)       38 2024-05-22 17:39:52.515311 zefir-analytics-0.4.13/setup.cfg
+drwxr-xr-x   0 akartashov  (1000) akartashov  (1000)        0 2024-05-22 17:39:52.505311 zefir-analytics-0.4.13/zefir_analytics/
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)      870 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/__init__.py
+drwxr-xr-x   0 akartashov  (1000) akartashov  (1000)        0 2024-05-22 17:39:52.515311 zefir-analytics-0.4.13/zefir_analytics/_engine/
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     1511 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/__init__.py
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     1200 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/constants.py
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     3729 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/data_loader.py
+drwxr-xr-x   0 akartashov  (1000) akartashov  (1000)        0 2024-05-22 17:39:52.515311 zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)      750 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/__init__.py
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     7312 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/aggregated_consumer_parameters_over_years.py
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     4716 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/lbs_parameters_over_years.py
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     4362 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/line_parameters_over_years.py
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)    37359 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/source_parameters_over_years.py
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     1620 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/utils.py
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)     6771 2024-05-22 17:39:13.000000 zefir-analytics-0.4.13/zefir_analytics/zefir_engine.py
+drwxr-xr-x   0 akartashov  (1000) akartashov  (1000)        0 2024-05-22 17:39:52.515311 zefir-analytics-0.4.13/zefir_analytics.egg-info/
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)    42617 2024-05-22 17:39:52.000000 zefir-analytics-0.4.13/zefir_analytics.egg-info/PKG-INFO
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)      781 2024-05-22 17:39:52.000000 zefir-analytics-0.4.13/zefir_analytics.egg-info/SOURCES.txt
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)        1 2024-05-22 17:39:52.000000 zefir-analytics-0.4.13/zefir_analytics.egg-info/dependency_links.txt
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)      210 2024-05-22 17:39:52.000000 zefir-analytics-0.4.13/zefir_analytics.egg-info/requires.txt
+-rw-r--r--   0 akartashov  (1000) akartashov  (1000)       16 2024-05-22 17:39:52.000000 zefir-analytics-0.4.13/zefir_analytics.egg-info/top_level.txt
```

### Comparing `zefir-analytics-0.4.1/LICENSE.txt` & `zefir-analytics-0.4.13/LICENSE.txt`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,661 +1,661 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  Developers that use our General Public Licenses protect your rights
-with two steps: (1) assert copyright on the software, and (2) offer
-you this License which gives you legal permission to copy, distribute
-and/or modify the software.
-
-  A secondary benefit of defending all users' freedom is that
-improvements made in alternate versions of the program, if they
-receive widespread use, become available for other developers to
-incorporate.  Many developers of free software are heartened and
-encouraged by the resulting cooperation.  However, in the case of
-software used on network servers, this result may fail to come about.
-The GNU General Public License permits making a modified version and
-letting the public access it on a server without ever releasing its
-source code to the public.
-
-  The GNU Affero General Public License is designed specifically to
-ensure that, in such cases, the modified source code becomes available
-to the community.  It requires the operator of a network server to
-provide the source code of the modified version running there to the
-users of that server.  Therefore, public use of a modified version, on
-a publicly accessible server, gives the public access to the source
-code of the modified version.
-
-  An older license, called the Affero General Public License and
-published by Affero, was designed to accomplish similar goals.  This is
-a different license, not a version of the Affero GPL, but Affero has
-released a new version of the Affero GPL which permits relicensing under
-this license.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU Affero General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Remote Network Interaction; Use with the GNU General Public License.
-
-  Notwithstanding any other provision of this License, if you modify the
-Program, your modified version must prominently offer all users
-interacting with it remotely through a computer network (if your version
-supports such interaction) an opportunity to receive the Corresponding
-Source of your version by providing access to the Corresponding Source
-from a network server at no charge, through some standard or customary
-means of facilitating copying of software.  This Corresponding Source
-shall include the Corresponding Source for any work covered by version 3
-of the GNU General Public License that is incorporated pursuant to the
-following paragraph.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published
-    by the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
-
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <https://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+                    GNU AFFERO GENERAL PUBLIC LICENSE
+                       Version 3, 19 November 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU Affero General Public License is a free, copyleft license for
+software and other kinds of works, specifically designed to ensure
+cooperation with the community in the case of network server software.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+our General Public Licenses are intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  Developers that use our General Public Licenses protect your rights
+with two steps: (1) assert copyright on the software, and (2) offer
+you this License which gives you legal permission to copy, distribute
+and/or modify the software.
+
+  A secondary benefit of defending all users' freedom is that
+improvements made in alternate versions of the program, if they
+receive widespread use, become available for other developers to
+incorporate.  Many developers of free software are heartened and
+encouraged by the resulting cooperation.  However, in the case of
+software used on network servers, this result may fail to come about.
+The GNU General Public License permits making a modified version and
+letting the public access it on a server without ever releasing its
+source code to the public.
+
+  The GNU Affero General Public License is designed specifically to
+ensure that, in such cases, the modified source code becomes available
+to the community.  It requires the operator of a network server to
+provide the source code of the modified version running there to the
+users of that server.  Therefore, public use of a modified version, on
+a publicly accessible server, gives the public access to the source
+code of the modified version.
+
+  An older license, called the Affero General Public License and
+published by Affero, was designed to accomplish similar goals.  This is
+a different license, not a version of the Affero GPL, but Affero has
+released a new version of the Affero GPL which permits relicensing under
+this license.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU Affero General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Remote Network Interaction; Use with the GNU General Public License.
+
+  Notwithstanding any other provision of this License, if you modify the
+Program, your modified version must prominently offer all users
+interacting with it remotely through a computer network (if your version
+supports such interaction) an opportunity to receive the Corresponding
+Source of your version by providing access to the Corresponding Source
+from a network server at no charge, through some standard or customary
+means of facilitating copying of software.  This Corresponding Source
+shall include the Corresponding Source for any work covered by version 3
+of the GNU General Public License that is incorporated pursuant to the
+following paragraph.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the work with which it is combined will remain governed by version
+3 of the GNU General Public License.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU Affero General Public License from time to time.  Such new versions
+will be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU Affero General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU Affero General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU Affero General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU Affero General Public License as published
+    by the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU Affero General Public License for more details.
+
+    You should have received a copy of the GNU Affero General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If your software can interact with users remotely through a computer
+network, you should also make sure that it provides a way for users to
+get its source.  For example, if your program is a web application, its
+interface could display a "Source" link that leads users to an archive
+of the code.  There are many ways you could offer source, and different
+solutions will be better for different programs; see section 13 for the
+specific requirements.
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU AGPL, see
+<https://www.gnu.org/licenses/>.
```

### Comparing `zefir-analytics-0.4.1/PKG-INFO` & `zefir-analytics-0.4.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zefir-analytics
-Version: 0.4.1
+Version: 0.4.13
 Author-email: Narodowe Centrum Badań Jądrowych <office@idea.edu.pl>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -671,15 +671,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy~=1.24.2
 Requires-Dist: pandas==2.0.1
-Requires-Dist: pyzefir==0.4.1
+Requires-Dist: pyzefir
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest==7.4.4; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
 Requires-Dist: pytest-mock~=3.11.1; extra == "dev"
@@ -731,27 +731,35 @@
 ```
 Remove temporary directories such as .venv, .mypy_cache, .pytest_cache etc.
 ```bash
 make clean
 ```
 ## Available methods in Zefir Engine objects
 * source_params:
-  * get_generation_sum
-  * get_dump_energy_sum
-  * get_load_sum
-  * get_installed_capacity
-  * get_generation_demand
-  * get_fuel_usage
   * get_capex_opex
+  * get_costs_per_tech_type
+  * get_dump_energy_sum
   * get_emission
+  * get_ets_cost
+  * get_fuel_availability_per_tech
+  * get_fuel_cost
+  * get_fuel_cost_per_tech
+  * get_fuel_usage
+  * get_generation_demand
+  * get_generation_sum
+  * get_installed_capacity
+  * get_load_sum
+  * get_var_costs
 * aggregated_consumer_params:
+  * get_aggregate_elements_type_attachments
+  * get_aggregate_parameters
   * get_fractions
   * get_n_consumers
-  * get_yearly_energy_usage
   * get_total_yearly_energy_usage
-  * get_fractions
+  * get_yearly_energy_usage
 * lbs_params:
-  * get_lbs_fraction
   * get_lbs_capacity
+  * get_lbs_fraction
 * line_params:
+  * get_capacity
   * get_flow
   * get_transmission_fee
```

### Comparing `zefir-analytics-0.4.1/pyproject.toml` & `zefir-analytics-0.4.13/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-[build-system]
-requires = ["setuptools == 69.0.3"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "zefir-analytics"
-dynamic = ["version"]
-authors = [
-    {name = "Narodowe Centrum Badań Jądrowych", email = "office@idea.edu.pl"},
-]
-readme = "README.md"
-license = {file = "LICENSE.txt"}
-classifiers = [
-    "Environment :: Console",
-    "Intended Audience :: Science/Research",
-    "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
-    "Natural Language :: English",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3.11",
-    "Topic :: Scientific/Engineering",
-]
-
-dependencies = [
-    "numpy~=1.24.2",
-    "pandas==2.0.1",
-    "pyzefir==0.4.1"
-]
-
-[project.optional-dependencies]
-dev = [
-    "pre-commit",
-    "pytest==7.4.4",
-    "flake8",
-    "black==24.2.0",
-    "pytest-cov~=4.1.0",
-    "pytest-mock~=3.11.1",
-    "pytest-lazy-fixture~=0.6.3",
-    "pylama[mccabe,pycodestyle,pyflakes,radon,mypy,toml]",
-    "tox",
-]
-
-[tool.setuptools.dynamic]
-version = {attr = "zefir_analytics.__version__"}
-
-[tool.setuptools.packages.find]
-include = ["zefir_analytics*"]
-exclude = ["docs*", "tests*"]
-
-[tool.coverage.report]
-exclude_lines = [
-    "if __name__ == .__main__.:",
-    "raise AssertionError",
-    "if TYPE_CHECKING:",
-    "raise NotImplementedError",
-]
-
-[tool.bumpversion]
-current_version = "0.4.1"
-commit = true
-tag = false
-parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
-serialize = [
-    "{major}.{minor}.{patch}",
-]
-
-[[tool.bumpversion.files]]
-filename = "zefir_analytics/__init__.py"
-
-[tool.mypy]
-ignore_missing_imports = true
-disallow_untyped_defs = true
-disallow_incomplete_defs = true
-check_untyped_defs = true
-disallow_untyped_decorators = false
-
-[tool.mypy-tests]
-disallow_untyped_decorators = false
-
-[tool.tox]
-legacy_tox_ini = """
-    [tox]
-    envlist = py311
-    isolated_build = True
-
-    [testenv]
-    usedevelop = True
-    deps = .[dev]
-
-    [testenv:unit]
-    commands =
-            python -m pytest -vvv --cov-report term --cov-report xml:coverage.xml \
-             --cov=zefir_analytics --junitxml=report.xml tests/unit
-
-    [testenv:fast_integration]
-    commands =
-            python -m pytest -vvv -m "not long_test" tests/integration
-
-    [testenv:integration]
-    commands =
-            python -m pytest -vvv tests/integration
-
-    [coverage]
-    xml_report = true
-    html_report = true
-"""
-
-[tool.pytest.ini_options]
-addopts = "--cov-report term --cov-report xml:coverage.xml"
-
-[tool.pylama.linter.pycodestyle]
-max_line_length = 120
-[tool.pylama.linter.pylint]
-max_line_length = 120
-[tool.pylama.linter.radon]
-no_assert = true
-
+[build-system]
+requires = ["setuptools == 69.0.3"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "zefir-analytics"
+dynamic = ["version"]
+authors = [
+    {name = "Narodowe Centrum Badań Jądrowych", email = "office@idea.edu.pl"},
+]
+readme = "README.md"
+license = {file = "LICENSE.txt"}
+classifiers = [
+    "Environment :: Console",
+    "Intended Audience :: Science/Research",
+    "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Scientific/Engineering",
+]
+
+dependencies = [
+    "numpy~=1.24.2",
+    "pandas==2.0.1",
+    "pyzefir"
+]
+
+[project.optional-dependencies]
+dev = [
+    "pre-commit",
+    "pytest==7.4.4",
+    "flake8",
+    "black==24.2.0",
+    "pytest-cov~=4.1.0",
+    "pytest-mock~=3.11.1",
+    "pytest-lazy-fixture~=0.6.3",
+    "pylama[mccabe,pycodestyle,pyflakes,radon,mypy,toml]",
+    "tox",
+]
+
+[tool.setuptools.dynamic]
+version = {attr = "zefir_analytics.__version__"}
+
+[tool.setuptools.packages.find]
+include = ["zefir_analytics*"]
+exclude = ["docs*", "tests*"]
+
+[tool.coverage.report]
+exclude_lines = [
+    "if __name__ == .__main__.:",
+    "raise AssertionError",
+    "if TYPE_CHECKING:",
+    "raise NotImplementedError",
+]
+
+[tool.bumpversion]
+current_version = "0.4.13"
+commit = true
+tag = false
+parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
+serialize = [
+    "{major}.{minor}.{patch}",
+]
+
+[[tool.bumpversion.files]]
+filename = "zefir_analytics/__init__.py"
+
+[tool.mypy]
+ignore_missing_imports = true
+disallow_untyped_defs = true
+disallow_incomplete_defs = true
+check_untyped_defs = true
+disallow_untyped_decorators = false
+
+[tool.mypy-tests]
+disallow_untyped_decorators = false
+
+[tool.tox]
+legacy_tox_ini = """
+    [tox]
+    envlist = py311
+    isolated_build = True
+
+    [testenv]
+    usedevelop = True
+    deps = .[dev]
+
+    [testenv:unit]
+    commands =
+            python -m pytest -vvv tests/unit
+
+    [testenv:fast_integration]
+    commands =
+            python -m pytest -vvv -m "not long_test" --cov-report term --cov-report xml:coverage.xml \
+            --cov=zefir_analytics --junitxml=report.xml tests/integration
+
+    [testenv:integration]
+    commands =
+            python -m pytest -vvv tests/integration
+
+    [coverage]
+    xml_report = true
+    html_report = true
+"""
+
+[tool.pytest.ini_options]
+addopts = "--cov-report term --cov-report xml:coverage.xml"
+
+[tool.pylama.linter.pycodestyle]
+max_line_length = 120
+[tool.pylama.linter.pylint]
+max_line_length = 120
+[tool.pylama.linter.radon]
+no_assert = true
+
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics/__init__.py` & `zefir-analytics-0.4.13/zefir_analytics/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# ZefirAnalytics
-# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-__version__ = "0.4.1"
-
-from zefir_analytics.zefir_engine import ZefirEngine
-
-__all__ = [
-    "ZefirEngine",
-]
+# ZefirAnalytics
+# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+__version__ = "0.4.13"
+
+from zefir_analytics.zefir_engine import ZefirEngine
+
+__all__ = [
+    "ZefirEngine",
+]
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics/_engine/__init__.py` & `zefir-analytics-0.4.13/zefir_analytics/_engine/__init__.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-# ZefirAnalytics
-# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-from zefir_analytics._engine.data_loader import DataLoader
-from zefir_analytics._engine.data_queries.aggregated_consumer_parameters_over_years import (
-    AggregatedConsumerParametersOverYearsQuery,
-)
-from zefir_analytics._engine.data_queries.lbs_parameters_over_years import (
-    LbsParametersOverYearsQuery,
-)
-from zefir_analytics._engine.data_queries.line_parameters_over_years import (
-    LineParametersOverYearsQuery,
-)
-from zefir_analytics._engine.data_queries.source_parameters_over_years import (
-    SourceParametersOverYearsQuery,
-)
-
-__all__ = [
-    "DataLoader",
-    "SourceParametersOverYearsQuery",
-    "LineParametersOverYearsQuery",
-    "AggregatedConsumerParametersOverYearsQuery",
-    "LbsParametersOverYearsQuery",
-]
+# ZefirAnalytics
+# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from zefir_analytics._engine.data_loader import DataLoader
+from zefir_analytics._engine.data_queries.aggregated_consumer_parameters_over_years import (
+    AggregatedConsumerParametersOverYearsQuery,
+)
+from zefir_analytics._engine.data_queries.lbs_parameters_over_years import (
+    LbsParametersOverYearsQuery,
+)
+from zefir_analytics._engine.data_queries.line_parameters_over_years import (
+    LineParametersOverYearsQuery,
+)
+from zefir_analytics._engine.data_queries.source_parameters_over_years import (
+    SourceParametersOverYearsQuery,
+)
+
+__all__ = [
+    "DataLoader",
+    "SourceParametersOverYearsQuery",
+    "LineParametersOverYearsQuery",
+    "AggregatedConsumerParametersOverYearsQuery",
+    "LbsParametersOverYearsQuery",
+]
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics/_engine/constants.py` & `zefir-analytics-0.4.13/zefir_analytics/_engine/constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-# ZefirAnalytics
-# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-from typing import Final
-
-ENERGY_TYPE_LABEL: Final[str] = "Energy Type"
-NETWORK_ELEMENT_NAME: Final[str] = "Network element name"
-NETWORK_ELEMENT_TYPE: Final[str] = "Network element type"
-YEARS_LABEL: Final[str] = "Year"
-FUEL_LABEL: Final[str] = "Fuel"
-EMISSION_LABEL: Final[str] = "Emission"
-COST_TYPE_LABEL: Final[str] = "Cost Type"
-HOUR_LABEL: Final[str] = "Hour"
+# ZefirAnalytics
+# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from typing import Final
+
+ENERGY_TYPE_LABEL: Final[str] = "Energy Type"
+NETWORK_ELEMENT_NAME: Final[str] = "Network element name"
+NETWORK_ELEMENT_TYPE: Final[str] = "Network element type"
+YEARS_LABEL: Final[str] = "Year"
+FUEL_LABEL: Final[str] = "Fuel"
+EMISSION_LABEL: Final[str] = "Emission"
+COST_TYPE_LABEL: Final[str] = "Cost Type"
+HOUR_LABEL: Final[str] = "Hour"
+OBJECTIVE_FUNCTION_FILE_NAME: Final[str] = "Objective_func_value.csv"
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/__init__.py` & `zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/__init__.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# ZefirAnalytics
-# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# ZefirAnalytics
+# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/lbs_parameters_over_years.py` & `zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/lbs_parameters_over_years.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,118 +1,118 @@
-# ZefirAnalytics
-# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-from itertools import chain
-
-import numpy as np
-import pandas as pd
-from pyzefir.model.network import Network
-
-from zefir_analytics._engine.data_queries import utils as data_utils
-
-
-class LbsParametersOverYearsQuery:
-    def __init__(
-        self,
-        network: Network,
-        fractions_results: dict[str, dict[str, pd.DataFrame]],
-        generator_results: dict[str, dict[str, pd.DataFrame]],
-        storage_results: dict[str, dict[str, pd.DataFrame]],
-    ) -> None:
-        self._network = network
-        self._fractions_results = fractions_results
-        self._generator_results = generator_results
-        self._storage_results = storage_results
-
-    @property
-    def lbs_names(self) -> list[str]:
-        lbs_names = {
-            col
-            for df in self._fractions_results["fraction"].values()
-            for col in df.columns
-        }
-        return list(lbs_names)
-
-    def _get_lbs_fraction(self, lbs_name: str) -> pd.DataFrame:
-        df = pd.DataFrame(
-            {
-                key: df[lbs_name]
-                for key, df in self._fractions_results["fraction"].items()
-            }
-        )
-        df_filtered = df.loc[:, (df != 0.0).any()]
-        if df_filtered.empty:
-            for agg in df.columns:
-                if lbs_name in self._network.aggregated_consumers[agg].available_stacks:
-                    return pd.DataFrame({agg: np.zeros(len(df.index))}, index=df.index)
-        return df_filtered
-
-    def _get_lbs_capacity(self, lbs_name: str) -> pd.DataFrame:
-        gen_attach, storage_attach = self._get_attached_sources(lbs_name)
-        fraction_factor = self._get_fraction_factor(lbs_name)
-        df_gen = self._generator_results["capacity"]["capacity"][gen_attach]
-        df_stor = self._storage_results["capacity"]["capacity"][storage_attach]
-        df_gen = df_gen.div(fraction_factor, axis=0).fillna(0.0).replace(np.inf, 0.0)
-        df_stor = df_stor.div(fraction_factor, axis=0).fillna(0.0).replace(np.inf, 0.0)
-        return pd.concat([df_gen, df_stor], axis=1)
-
-    def _get_attached_sources(self, lbs_name: str) -> tuple[list[str], list[str]]:
-        buses_attached = [
-            bus
-            for buses in self._network.local_balancing_stacks[lbs_name].buses.values()
-            for bus in buses
-        ]
-
-        generators = list(
-            chain.from_iterable(
-                self._network.buses[bus_name].generators for bus_name in buses_attached
-            )
-        )
-
-        storages = list(
-            chain.from_iterable(
-                self._network.buses[bus_name].storages for bus_name in buses_attached
-            )
-        )
-
-        return generators, storages
-
-    def _get_fraction_factor(self, lbs_name: str) -> np.ndarray:
-        df_fraction = self._get_lbs_fraction(lbs_name)
-        df_fraction = df_fraction.loc[:, (df_fraction != 0.0).any()]
-        if df_fraction.empty:
-            return np.zeros(len(df_fraction.index))
-        n_con_series = self._network.aggregated_consumers[
-            list(df_fraction.columns).pop()
-        ].n_consumers
-        return (df_fraction.squeeze() * n_con_series[df_fraction.index]).to_numpy()
-
-    def get_lbs_fraction(
-        self, lbs_name: str | list[str] | None = None
-    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
-        return (
-            data_utils.argument_condition(lbs_name, self._get_lbs_fraction)
-            if lbs_name is not None
-            else data_utils.argument_condition(self.lbs_names, self._get_lbs_fraction)
-        )
-
-    def get_lbs_capacity(
-        self, lbs_name: str | list[str] | None = None
-    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
-        return (
-            data_utils.argument_condition(lbs_name, self._get_lbs_capacity)
-            if lbs_name is not None
-            else data_utils.argument_condition(self.lbs_names, self._get_lbs_capacity)
-        )
+# ZefirAnalytics
+# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from itertools import chain
+
+import numpy as np
+import pandas as pd
+from pyzefir.model.network import Network
+
+from zefir_analytics._engine.data_queries import utils as data_utils
+
+
+class LbsParametersOverYearsQuery:
+    def __init__(
+        self,
+        network: Network,
+        fractions_results: dict[str, dict[str, pd.DataFrame]],
+        generator_results: dict[str, dict[str, pd.DataFrame]],
+        storage_results: dict[str, dict[str, pd.DataFrame]],
+    ) -> None:
+        self._network = network
+        self._fractions_results = fractions_results
+        self._generator_results = generator_results
+        self._storage_results = storage_results
+
+    @property
+    def lbs_names(self) -> list[str]:
+        lbs_names = {
+            col
+            for df in self._fractions_results["fraction"].values()
+            for col in df.columns
+        }
+        return list(lbs_names)
+
+    def _get_lbs_fraction(self, lbs_name: str) -> pd.DataFrame:
+        df = pd.DataFrame(
+            {
+                key: df[lbs_name]
+                for key, df in self._fractions_results["fraction"].items()
+            }
+        )
+        df_filtered = df.loc[:, (df != 0.0).any()]
+        if df_filtered.empty:
+            for agg in df.columns:
+                if lbs_name in self._network.aggregated_consumers[agg].available_stacks:
+                    return pd.DataFrame({agg: np.zeros(len(df.index))}, index=df.index)
+        return df_filtered
+
+    def _get_lbs_capacity(self, lbs_name: str) -> pd.DataFrame:
+        gen_attach, storage_attach = self._get_attached_sources(lbs_name)
+        fraction_factor = self._get_fraction_factor(lbs_name)
+        df_gen = self._generator_results["capacity"]["capacity"][gen_attach]
+        df_stor = self._storage_results["capacity"]["capacity"][storage_attach]
+        df_gen = df_gen.div(fraction_factor, axis=0).fillna(0.0).replace(np.inf, 0.0)
+        df_stor = df_stor.div(fraction_factor, axis=0).fillna(0.0).replace(np.inf, 0.0)
+        return pd.concat([df_gen, df_stor], axis=1)
+
+    def _get_attached_sources(self, lbs_name: str) -> tuple[list[str], list[str]]:
+        buses_attached = [
+            bus
+            for buses in self._network.local_balancing_stacks[lbs_name].buses.values()
+            for bus in buses
+        ]
+
+        generators = list(
+            chain.from_iterable(
+                self._network.buses[bus_name].generators for bus_name in buses_attached
+            )
+        )
+
+        storages = list(
+            chain.from_iterable(
+                self._network.buses[bus_name].storages for bus_name in buses_attached
+            )
+        )
+
+        return generators, storages
+
+    def _get_fraction_factor(self, lbs_name: str) -> np.ndarray:
+        df_fraction = self._get_lbs_fraction(lbs_name)
+        df_fraction = df_fraction.loc[:, (df_fraction != 0.0).any()]
+        if df_fraction.empty:
+            return np.zeros(len(df_fraction.index))
+        n_con_series = self._network.aggregated_consumers[
+            list(df_fraction.columns).pop()
+        ].n_consumers
+        return (df_fraction.squeeze() * n_con_series[df_fraction.index]).to_numpy()
+
+    def get_lbs_fraction(
+        self, lbs_name: str | list[str] | None = None
+    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
+        return (
+            data_utils.argument_condition(lbs_name, self._get_lbs_fraction)
+            if lbs_name is not None
+            else data_utils.argument_condition(self.lbs_names, self._get_lbs_fraction)
+        )
+
+    def get_lbs_capacity(
+        self, lbs_name: str | list[str] | None = None
+    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
+        return (
+            data_utils.argument_condition(lbs_name, self._get_lbs_capacity)
+            if lbs_name is not None
+            else data_utils.argument_condition(self.lbs_names, self._get_lbs_capacity)
+        )
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/line_parameters_over_years.py` & `zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/line_parameters_over_years.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,116 +1,116 @@
-# ZefirAnalytics
-# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-import numpy as np
-import pandas as pd
-from pyzefir.model.network import Network
-
-from zefir_analytics._engine.constants import YEARS_LABEL
-from zefir_analytics._engine.data_queries import utils as data_utils
-
-
-class LineParametersOverYearsQuery:
-    def __init__(
-        self,
-        network: Network,
-        line_results: dict[str, dict[str, pd.DataFrame]],
-        hour_sample: np.ndarray,
-        hourly_scale: float,
-    ) -> None:
-        self._network = network
-        self._line_results = line_results
-        self._hourly_scale = hourly_scale
-        self._hour_sample = hour_sample
-
-    @property
-    def line_names(self) -> list[str]:
-        return list(self._line_results["flow"].keys())
-
-    @staticmethod
-    def _get_yearly_summary(
-        df: pd.DataFrame, column_name: str, operation: str
-    ) -> pd.DataFrame:
-        df = df.agg(axis=0, func=operation).to_frame(column_name)
-        df.index.name = YEARS_LABEL
-        df.index = df.index.astype(int)
-        return df
-
-    def _get_flow(self, line_name: str) -> pd.DataFrame:
-        return (
-            self._get_yearly_summary(
-                self._line_results["flow"][line_name], "Total energy volume", "sum"
-            )
-            * self._hourly_scale
-        )
-
-    def _get_flow_hourly(self, line_name: str) -> pd.DataFrame:
-        df = self._line_results["flow"][line_name]
-        df.columns = df.columns.astype(int)
-        df = df.rename_axis(YEARS_LABEL, axis="columns")
-        return df.T.stack().to_frame("Total energy volume")
-
-    def _get_transmission_fee(self, line_name: str) -> pd.DataFrame:
-        df_flow = self._line_results["flow"][line_name]
-        if tf_name := self._network.lines[line_name].transmission_fee:
-            series_tf = (
-                self._network.transmission_fees[tf_name]
-                .fee.iloc[self._hour_sample]
-                .reset_index(drop=True)
-            )
-            df = df_flow.mul(series_tf.values[:None], axis=0)
-        else:
-            df = df_flow * 0.0
-        return (
-            self._get_yearly_summary(df, "Transmission fee total cost", "sum")
-            * self._hourly_scale
-        )
-
-    def get_flow(
-        self,
-        line_name: str | list[str] | None = None,
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
-        if is_hours_resolution:
-            return (
-                data_utils.argument_condition(line_name, self._get_flow_hourly)
-                if line_name is not None
-                else data_utils.argument_condition(
-                    self.line_names, self._get_flow_hourly
-                )
-            )
-        return (
-            data_utils.argument_condition(line_name, self._get_flow)
-            if line_name is not None
-            else data_utils.argument_condition(self.line_names, self._get_flow)
-        )
-
-    def get_capacity(
-        self, line_name: str | list[str] | None = None
-    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
-        raise NotImplementedError(
-            "This method will be implemented later when basecode will be ready"
-        )
-
-    def get_transmission_fee(
-        self, line_name: str | list[str] | None = None
-    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
-        return (
-            data_utils.argument_condition(line_name, self._get_transmission_fee)
-            if line_name is not None
-            else data_utils.argument_condition(
-                self.line_names, self._get_transmission_fee
-            )
-        )
+# ZefirAnalytics
+# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+import numpy as np
+import pandas as pd
+from pyzefir.model.network import Network
+
+from zefir_analytics._engine.constants import YEARS_LABEL
+from zefir_analytics._engine.data_queries import utils as data_utils
+
+
+class LineParametersOverYearsQuery:
+    def __init__(
+        self,
+        network: Network,
+        line_results: dict[str, dict[str, pd.DataFrame]],
+        hour_sample: np.ndarray,
+        hourly_scale: float,
+    ) -> None:
+        self._network = network
+        self._line_results = line_results
+        self._hourly_scale = hourly_scale
+        self._hour_sample = hour_sample
+
+    @property
+    def line_names(self) -> list[str]:
+        return list(self._line_results["flow"].keys())
+
+    @staticmethod
+    def _get_yearly_summary(
+        df: pd.DataFrame, column_name: str, operation: str
+    ) -> pd.DataFrame:
+        df = df.agg(axis=0, func=operation).to_frame(column_name)
+        df.index.name = YEARS_LABEL
+        df.index = df.index.astype(int)
+        return df
+
+    def _get_flow(self, line_name: str) -> pd.DataFrame:
+        return (
+            self._get_yearly_summary(
+                self._line_results["flow"][line_name], "Total energy volume", "sum"
+            )
+            * self._hourly_scale
+        )
+
+    def _get_flow_hourly(self, line_name: str) -> pd.DataFrame:
+        df = self._line_results["flow"][line_name]
+        df.columns = df.columns.astype(int)
+        df = df.rename_axis(YEARS_LABEL, axis="columns")
+        return df.T.stack().to_frame("Total energy volume")
+
+    def _get_transmission_fee(self, line_name: str) -> pd.DataFrame:
+        df_flow = self._line_results["flow"][line_name]
+        if tf_name := self._network.lines[line_name].transmission_fee:
+            series_tf = (
+                self._network.transmission_fees[tf_name]
+                .fee.iloc[self._hour_sample]
+                .reset_index(drop=True)
+            )
+            df = df_flow.mul(series_tf.values[:None], axis=0)
+        else:
+            df = df_flow * 0.0
+        return (
+            self._get_yearly_summary(df, "Transmission fee total cost", "sum")
+            * self._hourly_scale
+        )
+
+    def get_flow(
+        self,
+        line_name: str | list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
+        if is_hours_resolution:
+            return (
+                data_utils.argument_condition(line_name, self._get_flow_hourly)
+                if line_name is not None
+                else data_utils.argument_condition(
+                    self.line_names, self._get_flow_hourly
+                )
+            )
+        return (
+            data_utils.argument_condition(line_name, self._get_flow)
+            if line_name is not None
+            else data_utils.argument_condition(self.line_names, self._get_flow)
+        )
+
+    def get_capacity(
+        self, line_name: str | list[str] | None = None
+    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
+        raise NotImplementedError(
+            "This method will be implemented later when basecode will be ready"
+        )
+
+    def get_transmission_fee(
+        self, line_name: str | list[str] | None = None
+    ) -> pd.DataFrame | dict[str, pd.DataFrame]:
+        return (
+            data_utils.argument_condition(line_name, self._get_transmission_fee)
+            if line_name is not None
+            else data_utils.argument_condition(
+                self.line_names, self._get_transmission_fee
+            )
+        )
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/source_parameters_over_years.py` & `zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/source_parameters_over_years.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,713 +1,939 @@
-# ZefirAnalytics
-# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-from collections import defaultdict
-from typing import Any, Literal
-
-import numpy as np
-import pandas as pd
-from pyzefir.model.network import Network
-
-from zefir_analytics._engine.constants import (
-    COST_TYPE_LABEL,
-    EMISSION_LABEL,
-    ENERGY_TYPE_LABEL,
-    FUEL_LABEL,
-    HOUR_LABEL,
-    NETWORK_ELEMENT_NAME,
-    NETWORK_ELEMENT_TYPE,
-    YEARS_LABEL,
-)
-
-source_parameter_levels = Literal["element", "type"]
-source_parameter_filter_types = Literal["bus", "stack", "aggr"]
-
-
-class SourceParametersOverYearsQuery:
-    def __init__(
-        self,
-        network: Network,
-        generator_results: dict[str, dict[str, pd.DataFrame]],
-        storage_results: dict[str, dict[str, pd.DataFrame]],
-        year_sample: pd.Series,
-        discount_rate: pd.Series,
-        hourly_scale: float,
-        hour_sample: np.ndarray,
-    ):
-        self._network = network
-        self._generator_results = generator_results
-        self._storage_results = storage_results
-        self._year_sample = year_sample
-        self._discount_rate = discount_rate
-        self._energy_source_type_mapping = self._create_energy_source_type_mapping()
-        (
-            self._generator_capacity_plus,
-            self._storage_capacity_plus,
-        ) = self._calculate_cap_plus()
-        self._hourly_scale = hourly_scale
-        self._hour_sample = hour_sample
-
-    def _create_energy_source_type_mapping(self) -> dict[str, set[str]]:
-        mapping = defaultdict(set)
-        for gen in self._network.generators.values():
-            mapping[gen.energy_source_type].add(gen.name)
-
-        for stor in self._network.storages.values():
-            mapping[stor.energy_source_type].add(stor.name)
-
-        return dict(mapping)
-
-    def _aggregate_energy_sources(
-        self,
-        energy_source_df: pd.DataFrame,
-        index_name: str,
-        level: source_parameter_levels,
-        column_name: str | None = None,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        level_name = NETWORK_ELEMENT_NAME
-        if level == "type":
-            energy_source_df = self._aggregate_by_type(
-                energy_source_df, self._energy_source_type_mapping
-            )
-            level_name = NETWORK_ELEMENT_TYPE
-
-        column_names = (
-            [level_name, column_name] if column_name is not None else level_name
-        )
-        energy_source_df = energy_source_df.rename_axis(
-            columns=column_names,
-            index=[HOUR_LABEL, index_name] if is_hours_resolution else index_name,
-        )
-
-        if filter_type is None and filter_names is not None:
-            filtered_columns = energy_source_df.columns.get_level_values(0).isin(
-                filter_names
-            )
-            energy_source_df = energy_source_df.loc[:, filtered_columns]
-
-        energy_source_df = energy_source_df.T.sort_index()
-
-        if is_hours_resolution:
-            return energy_source_df.stack(level=0)
-
-        energy_source_df.index = energy_source_df.index.set_levels(
-            energy_source_df.index.get_level_values(1).astype(int),
-            level=1,
-            verify_integrity=False,
-        )
-        return energy_source_df
-
-    @staticmethod
-    def _aggregate_by_type(
-        df: pd.DataFrame, mapping: dict[str, set[str]]
-    ) -> pd.DataFrame:
-        result_dfs = []
-        for gen_type, gen_names in mapping.items():
-            columns = list(gen_names.intersection(df.columns.get_level_values(level=0)))
-            if not columns:
-                continue
-
-            if isinstance(df.columns, pd.MultiIndex):
-                type_df = df[columns].groupby(level=1, axis=1).sum()
-                multiindex = pd.MultiIndex.from_tuples(
-                    [(gen_type, col) for col in type_df.columns]
-                )
-                type_df.columns = multiindex
-            else:
-                type_df = df[columns].sum(axis=1).to_frame(gen_type)
-            result_dfs.append(type_df)
-
-        if result_dfs:
-            return pd.concat(result_dfs, axis=1)
-        return pd.DataFrame()
-
-    @staticmethod
-    def _flatten_2d_list(data: list[list]) -> list:
-        return [ele for d in data for ele in d]
-
-    def _filter_elements(  # noqa: R901
-        self,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-    ) -> tuple[list[str], list[str]]:
-        generators = list(self._network.generators.keys())
-        storages = list(self._network.storages.keys())
-
-        if filter_type is None or filter_names is None:
-            return generators, storages
-
-        available_buses, available_stacks = filter_names, filter_names
-        if filter_type == "aggr":
-            available_stacks_2d = [
-                list(aggr.stack_base_fraction.keys())
-                for aggr in self._network.aggregated_consumers.values()
-                if aggr.name in filter_names
-            ]
-            available_stacks = self._flatten_2d_list(available_stacks_2d)
-        if filter_type in ["stack", "aggr"]:
-            available_buses_2d = [
-                list(stack.buses_out.values())
-                for stack in self._network.local_balancing_stacks.values()
-                if stack.name in available_stacks
-            ]
-            available_buses = self._flatten_2d_list(available_buses_2d)
-
-        generators = [
-            g
-            for g in generators
-            if self._network.generators[g].buses.intersection(available_buses)
-        ]
-        storages = [
-            s for s in storages if self._network.storages[s].bus in available_buses
-        ]
-
-        return generators, storages
-
-    def _get_generation_sum(
-        self, generators: list[str], storages: list[str], is_hours_resolution: bool
-    ) -> pd.DataFrame:
-        generator_dfs = self._generator_results["generation_per_energy_type"]
-        storage_dfs = self._storage_results["generation"]
-
-        generator_dfs = {
-            k: (
-                v.pivot(columns=ENERGY_TYPE_LABEL).stack()
-                if is_hours_resolution
-                else v.pivot(columns=ENERGY_TYPE_LABEL).stack().groupby(level=1).sum()
-            )
-            for k, v in generator_dfs.items()
-            if k in generators
-        }
-        storage_dfs = {
-            k: v if is_hours_resolution else v.sum()
-            for k, v in storage_dfs.items()
-            if k in storages
-        }
-
-        for storage_name, df in storage_dfs.items():
-            storage_type = self._network.storages[storage_name].energy_source_type
-            energy_type = self._network.storage_types[storage_type].energy_type
-            if is_hours_resolution:
-                df = df.set_index(df.index.map(lambda x: (x, energy_type)))
-                df.index.names = [HOUR_LABEL, ENERGY_TYPE_LABEL]
-            else:
-                df = df.to_frame().T
-                df.index = [energy_type]
-            storage_dfs[storage_name] = df
-
-        generator_generation_sum = pd.concat(generator_dfs, axis=1)
-        storage_generation_sum = pd.concat(storage_dfs, axis=1)
-        generation_sum_df = pd.concat(
-            [generator_generation_sum, storage_generation_sum], axis=1
-        )
-
-        return generation_sum_df * self._hourly_scale
-
-    def get_generation_sum(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        df = self._get_generation_sum(generators, storages, is_hours_resolution)
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=ENERGY_TYPE_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-            is_hours_resolution=is_hours_resolution,
-        )
-
-    def _get_dump_energy_sum(
-        self,
-        generators: list[str],
-        _storages: list[str],
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generator_dfs = self._generator_results["dump_energy_per_energy_type"]
-        generator_dfs = {
-            k: (
-                v.pivot(columns=ENERGY_TYPE_LABEL).stack()
-                if is_hours_resolution
-                else v.pivot(columns=ENERGY_TYPE_LABEL).stack().groupby(level=1).sum()
-            )
-            for k, v in generator_dfs.items()
-            if k in generators
-        }
-        generator_sum = pd.concat(generator_dfs, axis=1)
-        return generator_sum
-
-    def get_dump_energy_sum(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        df = (
-            self._get_dump_energy_sum(generators, storages, is_hours_resolution)
-            * self._hourly_scale
-        )
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=ENERGY_TYPE_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-            is_hours_resolution=is_hours_resolution,
-        )
-
-    def _get_load_sum(
-        self,
-        _generators: list[str],
-        storages: list[str],
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        storage_dfs = self._storage_results["load"]
-        storage_dfs = {
-            k: v if is_hours_resolution else v.sum()
-            for k, v in storage_dfs.items()
-            if k in storages
-        }
-        for storage_name in storage_dfs.keys():
-            storage_type = self._network.storages[storage_name].energy_source_type
-            energy_type = self._network.storage_types[storage_type].energy_type
-            if is_hours_resolution:
-                df = storage_dfs[storage_name]
-                df = df.set_index(df.index.map(lambda x: (x, energy_type)))
-                df.index.names = [HOUR_LABEL, ENERGY_TYPE_LABEL]
-            else:
-                df = storage_dfs[storage_name].to_frame().T
-                df.index = [energy_type]
-            storage_dfs[storage_name] = df
-        storage_sum = pd.concat(storage_dfs, axis=1)
-        return storage_sum
-
-    def get_load_sum(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        df = (
-            self._get_load_sum(generators, storages, is_hours_resolution)
-            * self._hourly_scale
-        )
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=ENERGY_TYPE_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-            is_hours_resolution=is_hours_resolution,
-        )
-
-    def _get_installed_capacity(
-        self, generators: list[str], storages: list[str]
-    ) -> pd.DataFrame:
-        generator_df = self._generator_results["capacity"]["capacity"]
-        storage_df = self._storage_results["capacity"]["capacity"]
-        generator_df = generator_df.loc[:, generator_df.columns.isin(generators)]
-        storage_df = storage_df.loc[:, storage_df.columns.isin(storages)]
-        return pd.concat([generator_df, storage_df], axis=1)
-
-    def get_installed_capacity(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        df = (
-            self._get_installed_capacity(generators, storages)
-            .stack()
-            .swaplevel()
-            .to_frame()
-            .T
-        )
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=ENERGY_TYPE_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-        )
-
-    def _get_generation_demand(
-        self,
-        generators: list[str],
-        _storages: list[str],
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generator_dfs = self._generator_results["generation"]
-        dfs = []
-        for generator, generation_df in generator_dfs.items():
-            if generator not in generators:
-                continue
-            gen_type_name = self._network.generators[generator].energy_source_type
-            conversion_rates = self._network.generator_types[
-                gen_type_name
-            ].conversion_rate
-            if not conversion_rates:
-                continue
-            dem_series_list = []
-            for en_type, conv_en_rate in conversion_rates.items():
-                conv_en_rate_resampled = conv_en_rate.iloc[
-                    self._hour_sample
-                ].reset_index(drop=True)
-                if is_hours_resolution:
-                    dem_series = generation_df.mul(
-                        conv_en_rate_resampled, axis=0
-                    ).dropna()
-                    dem_series.index = pd.MultiIndex.from_tuples(
-                        [(hour, en_type) for hour in dem_series.index],
-                        names=[HOUR_LABEL, ENERGY_TYPE_LABEL],
-                    )
-                else:
-                    dem_series = (
-                        generation_df.mul(conv_en_rate_resampled, axis=0).dropna().sum()
-                    )
-                    dem_series.name = en_type
-                dem_series_list.append(dem_series)
-            dem_df = pd.concat(dem_series_list)
-            if len(dem_df.shape) == 1:
-                dem_df = dem_df.to_frame()
-            multiindex = pd.MultiIndex.from_tuples(
-                [(generator, col) for col in dem_df.columns]
-            )
-            dem_df.columns = multiindex
-            if not is_hours_resolution:
-                dem_df = dem_df.stack().swaplevel().unstack()
-            dfs.append(dem_df)
-        return pd.concat(dfs, axis=1)
-
-    def get_generation_demand(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        df = (
-            self._get_generation_demand(generators, storages, is_hours_resolution)
-            * self._hourly_scale
-        )
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=ENERGY_TYPE_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-            is_hours_resolution=is_hours_resolution,
-        )
-
-    def _calculate_opex(
-        self, generators: list[str], storages: list[str]
-    ) -> pd.DataFrame:
-        generator_df = self._generator_results["capacity"]["capacity"]
-        storage_df = self._storage_results["capacity"]["capacity"]
-        generator_df = generator_df.loc[:, generator_df.columns.isin(generators)]
-        storage_df = storage_df.loc[:, storage_df.columns.isin(storages)]
-        for generator_name in generator_df.columns:
-            generator_type_name = self._network.generators[
-                generator_name
-            ].energy_source_type
-            opex = self._network.generator_types[generator_type_name].opex
-            generator_df.loc[:, generator_name] = (
-                (generator_df[generator_name] * opex[self._year_sample].values)
-                if self._year_sample is not None
-                else generator_df[generator_name] * opex.values
-            )
-        for storage_name in storage_df.columns:
-            storage_type_name = self._network.storages[storage_name].energy_source_type
-            opex = self._network.storage_types[storage_type_name].opex
-            storage_df.loc[:, storage_name] = (
-                (storage_df[storage_name] * opex[self._year_sample].values)
-                if self._year_sample is not None
-                else storage_df[storage_name] * opex.values
-            )
-        return pd.concat([generator_df, storage_df], axis=1)
-
-    def _calculate_cap_plus(self) -> tuple[pd.DataFrame, pd.DataFrame]:
-        gen_cap_plus_df = (
-            self._generator_results["capacity"]["capacity"].diff().fillna(0)
-        )
-        gen_cap_plus_df[gen_cap_plus_df[gen_cap_plus_df.columns] < 0] = 0
-        stor_cap_plus_df = (
-            self._storage_results["capacity"]["capacity"].diff().fillna(0)
-        )
-        stor_cap_plus_df[stor_cap_plus_df[stor_cap_plus_df.columns] < 0] = 0
-
-        for (
-            energy_source_type,
-            energy_sources,
-        ) in self._energy_source_type_mapping.items():
-            unit_list = list(energy_sources)
-            if energy_source_type in self._network.generator_types:
-                gen_type_build_time = self._network.generator_types[
-                    energy_source_type
-                ].build_time
-                gen_cap_plus_df[unit_list] = (
-                    gen_cap_plus_df[unit_list].shift(-gen_type_build_time).fillna(0)
-                )
-            else:
-                stor_type_build_time = self._network.storage_types[
-                    energy_source_type
-                ].build_time
-                stor_cap_plus_df[unit_list] = (
-                    stor_cap_plus_df[unit_list].shift(-stor_type_build_time).fillna(0)
-                )
-
-        return gen_cap_plus_df, stor_cap_plus_df
-
-    def _get_capex_opex(
-        self, generators: list[str], storages: list[str]
-    ) -> pd.DataFrame:
-        capex_df = self._generator_results["capex"]["capex"].join(
-            self._storage_results["capex"]["capex"]
-        )
-        opex_df = self._calculate_opex(generators, storages)
-        capex_df.columns = pd.MultiIndex.from_tuples(
-            [(col, "capex") for col in capex_df.columns]
-        )
-        opex_df.columns = pd.MultiIndex.from_tuples(
-            [(col, "opex") for col in opex_df.columns]
-        )
-        df = pd.concat([capex_df, opex_df], axis=1)
-        df = df.reindex(
-            columns=df.columns.get_level_values(0).sort_values().unique(), level=0
-        )
-        df = df.stack().swaplevel().unstack()
-        return df
-
-    def get_capex_opex(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        df = self._get_capex_opex(generators, storages)
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=COST_TYPE_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-        )
-
-    def _get_fuel_usage(
-        self,
-        generators: list[str],
-        _storages: list[str],
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generator_dfs = self._generator_results["generation"]
-        generator_dfs = {
-            k: v if is_hours_resolution else v.sum()
-            for k, v in generator_dfs.items()
-            if k in generators
-        }
-        dfs = []
-        for generator, generation_df in generator_dfs.items():
-            generator_type = self._network.generators[generator].energy_source_type
-            fuel_name = self._network.generator_types[generator_type].fuel
-            if fuel_name is None:
-                continue
-            energy_per_unit = self._network.fuels[fuel_name].energy_per_unit
-            df = generation_df / energy_per_unit
-            if is_hours_resolution:
-                df.columns = df.columns.astype(int)
-                df.columns = pd.MultiIndex.from_tuples(
-                    [(generator, col) for col in df.columns],
-                )
-                df.index = pd.MultiIndex.from_tuples(
-                    [(hour, fuel_name) for hour in df.index],
-                )
-                df = df * self._hourly_scale
-            else:
-                df = df.to_frame()
-                multiindex = pd.MultiIndex.from_tuples([(generator, fuel_name)])
-                df.columns = multiindex
-                df = df.stack().swaplevel().unstack() * self._hourly_scale
-            dfs.append(df)
-
-        return pd.concat(dfs, axis=1)
-
-    def get_fuel_usage(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        df = self._get_fuel_usage(generators, storages, is_hours_resolution)
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=FUEL_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-            is_hours_resolution=is_hours_resolution,
-        )
-
-    def get_emission(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-        is_hours_resolution: bool = False,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        fuel_usage_df = self._get_fuel_usage(generators, storages, is_hours_resolution)
-
-        fuels_emissions: dict[str, dict[str, float]] = {
-            fuel_name: {
-                emission_type: (
-                    fuel.emission[emission_type]
-                    if emission_type in fuel.emission
-                    else 0
-                )
-                for emission_type in self._network.emission_types
-            }
-            for fuel_name, fuel in self._network.fuels.items()
-        }
-
-        dfs: list[dict[str, Any]] = self._get_emission_dfs_dicts(
-            is_hours_resolution, fuel_usage_df, fuels_emissions
-        )
-        index_columns: list[str] | Literal["emission_type"] = (
-            ["hour", "emission_type"] if is_hours_resolution else "emission_type"
-        )
-
-        df = (
-            pd.DataFrame(dfs)
-            .set_index(index_columns)
-            .pivot(columns=["generator_name", "year"])
-            .droplevel(0, axis=1)
-        )
-
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=EMISSION_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-            is_hours_resolution=is_hours_resolution,
-        )
-
-    def _get_emission_dfs_dicts(
-        self,
-        is_hours_resolution: bool,
-        fuel_usage_df: pd.DataFrame,
-        fuels_emissions: dict[str, dict[str, float]],
-    ) -> list[dict[str, Any]]:
-        dfs: list[dict[str, Any]] = []
-        for generator_name in fuel_usage_df.columns.levels[0]:
-            generator_em_reduction = self._network.generator_types[
-                self._network.generators[generator_name].energy_source_type
-            ].emission_reduction
-            generator_fuel = self._network.generator_types[
-                self._network.generators[generator_name].energy_source_type
-            ].fuel
-
-            if is_hours_resolution:
-                dfs.extend(
-                    [
-                        {
-                            "emission_type": emission_type,
-                            "generator_name": generator_name,
-                            "year": year,
-                            "hour": hour,
-                            "value": (
-                                fuel_usage_df[generator_name].loc[
-                                    (hour, generator_fuel)
-                                ][year]
-                                * fuels_emissions[generator_fuel][emission_type]
-                                * (1 - generator_em_reduction[emission_type])
-                            ),
-                        }
-                        for emission_type in fuels_emissions[generator_fuel].keys()
-                        for year in self._year_sample
-                        for hour in fuel_usage_df.index.get_level_values(0)[
-                            fuel_usage_df.index.get_level_values(1) == generator_fuel
-                        ]
-                    ]
-                )
-
-            else:
-                dfs.extend(
-                    [
-                        {
-                            "emission_type": emission_type,
-                            "generator_name": generator_name,
-                            "year": year,
-                            "value": (
-                                fuel_usage_df[generator_name].loc[generator_fuel][
-                                    str(year)
-                                ]
-                                * fuels_emissions[generator_fuel][emission_type]
-                                * (1 - generator_em_reduction[emission_type])
-                            ),
-                        }
-                        for emission_type in fuels_emissions[generator_fuel].keys()
-                        for year in self._year_sample
-                    ]
-                )
-
-        return dfs
-
-    def get_fuel_cost(
-        self,
-        level: source_parameter_levels,
-        filter_type: source_parameter_filter_types | None = None,
-        filter_names: list[str] | None = None,
-    ) -> pd.DataFrame:
-        generators, storages = self._filter_elements(filter_type, filter_names)
-        df = self._get_fuel_usage(generators, storages)
-
-        for fuel_name in df.index:
-            fuel = self._network.fuels[fuel_name]
-            for year in self._year_sample:
-                df.loc[fuel.name, (slice(None), str(year))] *= fuel.cost[year]
-
-        return self._aggregate_energy_sources(
-            energy_source_df=df,
-            column_name=YEARS_LABEL,
-            index_name=FUEL_LABEL,
-            level=level,
-            filter_type=filter_type,
-            filter_names=filter_names,
-        )
+# ZefirAnalytics
+# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from collections import defaultdict
+from typing import Any, Iterable, Literal
+
+import numpy as np
+import pandas as pd
+from pyzefir.model.network import Network
+
+from zefir_analytics._engine.constants import (
+    COST_TYPE_LABEL,
+    EMISSION_LABEL,
+    ENERGY_TYPE_LABEL,
+    FUEL_LABEL,
+    HOUR_LABEL,
+    NETWORK_ELEMENT_NAME,
+    NETWORK_ELEMENT_TYPE,
+    YEARS_LABEL,
+)
+from zefir_analytics._engine.data_queries.utils import assign_multiindex
+
+source_parameter_levels = Literal["element", "type"]
+source_parameter_filter_types = Literal["bus", "stack", "aggr"]
+
+
+class SourceParametersOverYearsQuery:
+    def __init__(
+        self,
+        network: Network,
+        generator_results: dict[str, dict[str, pd.DataFrame]],
+        storage_results: dict[str, dict[str, pd.DataFrame]],
+        bus_results: dict[str, dict[str, pd.DataFrame]],
+        year_sample: pd.Series,
+        discount_rate: pd.Series,
+        hourly_scale: float,
+        hour_sample: np.ndarray,
+    ):
+        self._network = network
+        self._generator_results = generator_results
+        self._storage_results = storage_results
+        self._bus_results = bus_results
+        self._year_sample = year_sample
+        self._discount_rate = discount_rate
+        self._energy_source_type_mapping = self._create_energy_source_type_mapping()
+        (
+            self._generator_capacity_plus,
+            self._storage_capacity_plus,
+        ) = self._calculate_cap_plus()
+        self._hourly_scale = hourly_scale
+        self._hour_sample = hour_sample
+
+    def _get_generator_and_storage_from_set_of_buses(
+        self,
+        bus_set: set[str],
+    ) -> tuple[list[str], list[str]]:
+        generators = [
+            g.name
+            for g in self._network.generators.values()
+            if g.buses.intersection(bus_set)
+        ]
+        storages = [s.name for s in self._network.storages.values() if s.bus in bus_set]
+        return generators, storages
+
+    def _get_global_generators_and_storage(
+        self,
+    ) -> tuple[list[str], list[str]]:
+        all_buses_out = {
+            item
+            for stack in self._network.local_balancing_stacks.values()
+            for item in list(stack.buses_out.values())
+        }
+        all_global_buses = set(self._network.buses).difference(all_buses_out)
+        return self._get_generator_and_storage_from_set_of_buses(all_global_buses)
+
+    def _get_generator_results(
+        self,
+        results_group: str,
+        generators: list[str],
+        is_hours_resolution: bool,
+    ) -> pd.DataFrame:
+        generator_dfs = self._generator_results[results_group]
+        generator_dfs = {
+            gen_name: (
+                df.pivot(columns=ENERGY_TYPE_LABEL).stack()
+                if is_hours_resolution
+                else df.pivot(columns=ENERGY_TYPE_LABEL).stack().groupby(level=1).sum()
+            )
+            for gen_name, df in generator_dfs.items()
+            if gen_name in generators
+        }
+        return pd.concat(generator_dfs, axis=1)
+
+    def _get_storage_results(
+        self,
+        results_group: str,
+        storages: list[str],
+        is_hours_resolution: bool,
+    ) -> pd.DataFrame:
+        storage_dfs = self._storage_results[results_group]
+
+        storage_dfs = {
+            storage_name: df if is_hours_resolution else df.sum()
+            for storage_name, df in storage_dfs.items()
+            if storage_name in storages
+        }
+        for storage_name, df in storage_dfs.items():
+            storage_type = self._network.storages[storage_name].energy_source_type
+            energy_type = self._network.storage_types[storage_type].energy_type
+            if is_hours_resolution:
+                df = df.set_index(df.index.map(lambda x: (x, energy_type)))
+                df.index.names = [HOUR_LABEL, ENERGY_TYPE_LABEL]
+            else:
+                df = df.to_frame().T
+                df.index = [energy_type]
+            storage_dfs[storage_name] = df
+        return pd.concat(storage_dfs, axis=1).fillna(0.0)
+
+    def _create_energy_source_type_mapping(self) -> dict[str, set[str]]:
+        mapping = defaultdict(set)
+        for gen in self._network.generators.values():
+            mapping[gen.energy_source_type].add(gen.name)
+
+        for stor in self._network.storages.values():
+            mapping[stor.energy_source_type].add(stor.name)
+
+        return dict(mapping)
+
+    def _aggregate_energy_sources(
+        self,
+        energy_source_df: pd.DataFrame,
+        index_name: str,
+        level: source_parameter_levels,
+        column_name: str | None = None,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        level_name = NETWORK_ELEMENT_NAME
+        if level == "type":
+            energy_source_df = self._aggregate_by_type(
+                energy_source_df, self._energy_source_type_mapping
+            )
+            level_name = NETWORK_ELEMENT_TYPE
+
+        column_names = (
+            [level_name, column_name] if column_name is not None else level_name
+        )
+        energy_source_df = energy_source_df.rename_axis(
+            columns=column_names,
+            index=[HOUR_LABEL, index_name] if is_hours_resolution else index_name,
+        )
+
+        if filter_type is None and filter_names is not None:
+            filtered_columns = energy_source_df.columns.get_level_values(0).isin(
+                filter_names
+            )
+            energy_source_df = energy_source_df.loc[:, filtered_columns]
+
+        energy_source_df = energy_source_df.T.sort_index()
+
+        energy_source_df.index = energy_source_df.index.set_levels(
+            energy_source_df.index.get_level_values(1).astype(int),
+            level=1,
+            verify_integrity=False,
+        )
+        if is_hours_resolution:
+            return energy_source_df.stack(level=0)
+
+        return energy_source_df
+
+    @staticmethod
+    def _aggregate_by_type(
+        df: pd.DataFrame, mapping: dict[str, set[str]]
+    ) -> pd.DataFrame:
+        result_dfs = []
+        for gen_type, gen_names in mapping.items():
+            columns = list(gen_names.intersection(df.columns.get_level_values(level=0)))
+            if not columns:
+                continue
+
+            if isinstance(df.columns, pd.MultiIndex):
+                type_df = df[columns].groupby(level=1, axis=1).sum()
+                multiindex = pd.MultiIndex.from_tuples(
+                    [(gen_type, col) for col in type_df.columns]
+                )
+                type_df.columns = multiindex
+            else:
+                type_df = df[columns].sum(axis=1).to_frame(gen_type)
+            result_dfs.append(type_df)
+
+        if result_dfs:
+            return pd.concat(result_dfs, axis=1)
+        return pd.DataFrame()
+
+    @staticmethod
+    def _flatten_2d_list(data: list[list]) -> list:
+        return [ele for d in data for ele in d]
+
+    def _filter_elements(  # noqa: R901
+        self,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_bus_filter: bool = False,
+    ) -> tuple[list[str], ...]:
+        generators = list(self._network.generators.keys())
+        storages = list(self._network.storages.keys())
+
+        if filter_type is None or filter_names is None:
+            if is_bus_filter:
+                return generators, storages, list(self._network.buses.keys())
+            return generators, storages
+
+        available_buses, available_stacks = set(filter_names), set(filter_names)
+        if filter_type == "aggr":
+            available_stacks_2d: list[list[str]] = [
+                list(aggr.stack_base_fraction.keys())
+                for aggr in self._network.aggregated_consumers.values()
+                if aggr.name in filter_names
+            ]
+            available_stacks = set(self._flatten_2d_list(available_stacks_2d))
+        if filter_type in ["stack", "aggr"]:
+            available_buses_2d: list[list[str]] = [
+                list(stack.buses_out.values())
+                for stack in self._network.local_balancing_stacks.values()
+                if stack.name in available_stacks
+            ]
+            available_buses = set(self._flatten_2d_list(available_buses_2d))
+
+        generators, storages = self._get_generator_and_storage_from_set_of_buses(
+            available_buses
+        )
+        if is_bus_filter:
+            return generators, storages, list(available_buses)
+        return generators, storages
+
+    def _get_generation_sum(
+        self, generators: list[str], storages: list[str], is_hours_resolution: bool
+    ) -> pd.DataFrame:
+        generator_df = self._get_generator_results(
+            "generation_per_energy_type", generators, is_hours_resolution
+        )
+        storage_df = self._get_storage_results(
+            "generation", storages, is_hours_resolution
+        )
+        generation_sum_df = pd.concat([generator_df, storage_df], axis=1)
+
+        return generation_sum_df * self._hourly_scale
+
+    def get_generation_sum(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        generators, storages = self._filter_elements(filter_type, filter_names)
+        df = self._get_generation_sum(generators, storages, is_hours_resolution)
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=ENERGY_TYPE_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+            is_hours_resolution=is_hours_resolution,
+        )
+
+    def get_dump_energy_sum(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        generators, _ = self._filter_elements(filter_type, filter_names)
+        df = (
+            self._get_generator_results(
+                "dump_energy_per_energy_type", generators, is_hours_resolution
+            )
+            * self._hourly_scale
+        )
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=ENERGY_TYPE_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+            is_hours_resolution=is_hours_resolution,
+        )
+
+    def get_load_sum(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        _, storages = self._filter_elements(filter_type, filter_names)
+        df = (
+            self._get_storage_results("load", storages, is_hours_resolution)
+            * self._hourly_scale
+        )
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=ENERGY_TYPE_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+            is_hours_resolution=is_hours_resolution,
+        )
+
+    def _get_installed_capacity(
+        self, generators: list[str], storages: list[str]
+    ) -> pd.DataFrame:
+        generator_df = self._generator_results["capacity"]["capacity"]
+        storage_df = self._storage_results["capacity"]["capacity"]
+        generator_df = generator_df.loc[:, generator_df.columns.isin(generators)]
+        storage_df = storage_df.loc[:, storage_df.columns.isin(storages)]
+        return pd.concat([generator_df, storage_df], axis=1)
+
+    def get_installed_capacity(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+    ) -> pd.DataFrame:
+        generators, storages = self._filter_elements(filter_type, filter_names)
+        df = (
+            self._get_installed_capacity(generators, storages)
+            .stack()
+            .swaplevel()
+            .to_frame()
+            .T
+        )
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=ENERGY_TYPE_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+        )
+
+    def _get_generation_demand(
+        self,
+        generators: list[str],
+        _storages: list[str],
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        generator_dfs = self._generator_results["generation"]
+        dfs = []
+        for generator, generation_df in generator_dfs.items():
+            if generator not in generators:
+                continue
+            gen_type_name = self._network.generators[generator].energy_source_type
+            conversion_rates = self._network.generator_types[
+                gen_type_name
+            ].conversion_rate
+            if not conversion_rates:
+                continue
+            dem_series_list = []
+            for en_type, conv_en_rate in conversion_rates.items():
+                conv_en_rate_resampled = conv_en_rate.iloc[
+                    self._hour_sample
+                ].reset_index(drop=True)
+                if is_hours_resolution:
+                    dem_series = generation_df.mul(
+                        conv_en_rate_resampled, axis=0
+                    ).dropna()
+                    dem_series.index = pd.MultiIndex.from_tuples(
+                        [(hour, en_type) for hour in dem_series.index],
+                        names=[HOUR_LABEL, ENERGY_TYPE_LABEL],
+                    )
+                else:
+                    dem_series = (
+                        generation_df.mul(conv_en_rate_resampled, axis=0).dropna().sum()
+                    )
+                    dem_series.name = en_type
+                dem_series_list.append(dem_series)
+            dem_df = pd.concat(dem_series_list)
+            if len(dem_df.shape) == 1:
+                dem_df = dem_df.to_frame()
+            multiindex = pd.MultiIndex.from_tuples(
+                [(generator, col) for col in dem_df.columns]
+            )
+            dem_df.columns = multiindex
+            if not is_hours_resolution:
+                dem_df = dem_df.stack().swaplevel().unstack()
+            dfs.append(dem_df)
+        return pd.concat(dfs, axis=1)
+
+    def get_generation_demand(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        generators, storages = self._filter_elements(filter_type, filter_names)
+        df = (
+            self._get_generation_demand(generators, storages, is_hours_resolution)
+            * self._hourly_scale
+        )
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=ENERGY_TYPE_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+            is_hours_resolution=is_hours_resolution,
+        )
+
+    def _calculate_opex(
+        self,
+        generators: list[str],
+        storages: list[str],
+        cast_to_energy_source_type: bool = False,
+    ) -> pd.DataFrame:
+        generator_df = self._generator_results["capacity"]["capacity"]
+        storage_df = self._storage_results["capacity"]["capacity"]
+        generator_df = generator_df.loc[:, generator_df.columns.isin(generators)]
+        storage_df = storage_df.loc[:, storage_df.columns.isin(storages)]
+        for generator_name in generator_df.columns:
+            generator_type_name = self._network.generators[
+                generator_name
+            ].energy_source_type
+            opex = self._network.generator_types[generator_type_name].opex
+            generator_df.loc[:, generator_name] = (
+                (generator_df[generator_name] * opex[self._year_sample].values)
+                if self._year_sample is not None
+                else generator_df[generator_name] * opex.values
+            )
+        for storage_name in storage_df.columns:
+            storage_type_name = self._network.storages[storage_name].energy_source_type
+            opex = self._network.storage_types[storage_type_name].opex
+            storage_df.loc[:, storage_name] = (
+                (storage_df[storage_name] * opex[self._year_sample].values)
+                if self._year_sample is not None
+                else storage_df[storage_name] * opex.values
+            )
+        if cast_to_energy_source_type:
+            generator_df = self._aggregate_by_type(
+                generator_df, self._energy_source_type_mapping
+            )
+            storage_df = self._aggregate_by_type(
+                storage_df, self._energy_source_type_mapping
+            )
+
+        return pd.concat([generator_df, storage_df], axis=1)
+
+    def _calculate_cap_plus(self) -> tuple[pd.DataFrame, pd.DataFrame]:
+        gen_cap_plus_df = (
+            self._generator_results["capacity"]["capacity"].diff().fillna(0)
+        )
+        gen_cap_plus_df[gen_cap_plus_df[gen_cap_plus_df.columns] < 0] = 0
+        stor_cap_plus_df = (
+            self._storage_results["capacity"]["capacity"].diff().fillna(0)
+        )
+        stor_cap_plus_df[stor_cap_plus_df[stor_cap_plus_df.columns] < 0] = 0
+
+        for (
+            energy_source_type,
+            energy_sources,
+        ) in self._energy_source_type_mapping.items():
+            unit_list = list(energy_sources)
+            if energy_source_type in self._network.generator_types:
+                gen_type_build_time = self._network.generator_types[
+                    energy_source_type
+                ].build_time
+                gen_cap_plus_df[unit_list] = (
+                    gen_cap_plus_df[unit_list].shift(-gen_type_build_time).fillna(0)
+                )
+            else:
+                stor_type_build_time = self._network.storage_types[
+                    energy_source_type
+                ].build_time
+                stor_cap_plus_df[unit_list] = (
+                    stor_cap_plus_df[unit_list].shift(-stor_type_build_time).fillna(0)
+                )
+
+        return gen_cap_plus_df, stor_cap_plus_df
+
+    @staticmethod
+    def _format_capex_opex_dfs(
+        capex_df: pd.DataFrame, opex_df: pd.DataFrame
+    ) -> pd.DataFrame:
+        if capex_df.empty and opex_df.empty:
+            return pd.DataFrame()
+        capex_df = assign_multiindex(capex_df, "capex")
+        opex_df = assign_multiindex(opex_df, "opex")
+        df = pd.concat([capex_df, opex_df], axis=1)
+        df = df.reindex(
+            columns=df.columns.get_level_values(0).sort_values().unique(), level=0
+        )
+        df = df.stack().swaplevel().unstack()
+        return df
+
+    def _get_global_capex_opex(
+        self,
+        generators: list[str],
+        storages: list[str],
+    ) -> pd.DataFrame:
+        capex_df = self._generator_results["global_capex"]["global_capex"].join(
+            self._storage_results["global_capex"]["global_capex"]
+        )
+        capex_df = capex_df.loc[:, capex_df.columns.isin(generators + storages)]
+        opex_df = self._calculate_opex(generators, storages)
+        return self._format_capex_opex_dfs(capex_df, opex_df)
+
+    def _get_local_capex_opex(
+        self,
+        generators: list[str],
+        storages: list[str],
+        filter_type: Literal["aggr"] | None = None,
+        filter_names: list[str] | None = None,
+    ) -> pd.DataFrame:
+        if filter_type is not None and filter_names is not None:
+            generator_values = [
+                value
+                for key, value in self._generator_results["local_capex"].items()
+                if key in filter_names
+            ]
+            storage_values = [
+                value
+                for key, value in self._storage_results["local_capex"].items()
+                if key in filter_names
+            ]
+        else:
+            generator_values = list(self._generator_results["local_capex"].values())
+            storage_values = list(self._storage_results["local_capex"].values())
+
+        if not storage_values:
+            capex_df = pd.concat(generator_values, axis=0).groupby(level=0).sum()
+        else:
+            capex_df = (
+                pd.concat(generator_values, axis=0).groupby(level=0).sum()
+            ).join(pd.concat(storage_values, axis=0).groupby(level=0).sum())
+
+        opex_df = self._calculate_opex(
+            generators, storages, cast_to_energy_source_type=True
+        )
+        return self._format_capex_opex_dfs(capex_df, opex_df)
+
+    def get_global_capex_opex(
+        self,
+        level: source_parameter_levels,
+    ) -> pd.DataFrame:
+        generators, storages = self._get_global_generators_and_storage()
+        df = self._get_global_capex_opex(generators, storages)
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=COST_TYPE_LABEL,
+            level=level,
+            filter_type=None,
+            filter_names=None,
+        )
+
+    def get_local_capex_opex(
+        self,
+        filter_type: Literal["aggr"] | None = None,
+        filter_names: list[str] | None = None,
+    ) -> pd.DataFrame:
+        generators, storages = self._filter_elements(filter_type, filter_names)
+        global_generators, global_storages = self._get_global_generators_and_storage()
+        generators = list(set(generators) - set(global_generators))
+        storages = list(set(storages) - set(global_storages))
+        df = self._get_local_capex_opex(generators, storages, filter_type, filter_names)
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=COST_TYPE_LABEL,
+            level="element",  # element coz data is already in type but when level=type func cast element-> type
+            filter_type=filter_type,
+            filter_names=filter_names,
+        )
+
+    def _get_fuel_usage(
+        self,
+        generators: list[str],
+        _storages: list[str],
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        generator_dfs = self._generator_results["generation"]
+        generator_dfs = {
+            k: v if is_hours_resolution else v.sum()
+            for k, v in generator_dfs.items()
+            if k in generators
+        }
+        dfs = []
+        for generator, generation_df in generator_dfs.items():
+            generator_type = self._network.generators[generator].energy_source_type
+            fuel_name = self._network.generator_types[generator_type].fuel
+            if fuel_name is None:
+                continue
+            energy_per_unit = self._network.fuels[fuel_name].energy_per_unit
+            df = generation_df / energy_per_unit
+            if is_hours_resolution:
+                df.columns = df.columns.astype(int)
+                df.columns = pd.MultiIndex.from_tuples(
+                    [(generator, col) for col in df.columns],
+                )
+                df.index = pd.MultiIndex.from_tuples(
+                    [(hour, fuel_name) for hour in df.index],
+                )
+                df = df * self._hourly_scale
+            else:
+                df = df.to_frame()
+                multiindex = pd.MultiIndex.from_tuples([(generator, fuel_name)])
+                df.columns = multiindex
+                df = df.stack().swaplevel().unstack() * self._hourly_scale
+            dfs.append(df)
+
+        return pd.concat(dfs, axis=1)
+
+    def get_fuel_usage(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        generators, storages = self._filter_elements(filter_type, filter_names)
+        df = self._get_fuel_usage(generators, storages, is_hours_resolution)
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=FUEL_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+            is_hours_resolution=is_hours_resolution,
+        )
+
+    def get_emission(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        generators, storages = self._filter_elements(filter_type, filter_names)
+        fuel_usage_df = self._get_fuel_usage(generators, storages, is_hours_resolution)
+
+        fuels_emissions: dict[str, dict[str, float]] = {
+            fuel_name: {
+                emission_type: (
+                    fuel.emission[emission_type]
+                    if emission_type in fuel.emission
+                    else 0
+                )
+                for emission_type in self._network.emission_types
+            }
+            for fuel_name, fuel in self._network.fuels.items()
+        }
+
+        dfs: list[dict[str, Any]] = self._get_emission_dfs_dicts(
+            is_hours_resolution, fuel_usage_df, fuels_emissions
+        )
+        index_columns: list[str] | Literal["emission_type"] = (
+            ["hour", "emission_type"] if is_hours_resolution else "emission_type"
+        )
+
+        df = (
+            pd.DataFrame(dfs)
+            .set_index(index_columns)
+            .pivot(columns=["generator_name", "year"])
+            .droplevel(0, axis=1)
+        )
+
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=EMISSION_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+            is_hours_resolution=is_hours_resolution,
+        )
+
+    def _get_emission_dfs_dicts(
+        self,
+        is_hours_resolution: bool,
+        fuel_usage_df: pd.DataFrame,
+        fuels_emissions: dict[str, dict[str, float]],
+    ) -> list[dict[str, Any]]:
+        dfs: list[dict[str, Any]] = []
+        for generator_name in fuel_usage_df.columns.levels[0]:
+            generator_em_reduction = self._network.generator_types[
+                self._network.generators[generator_name].energy_source_type
+            ].emission_reduction
+            generator_fuel = self._network.generator_types[
+                self._network.generators[generator_name].energy_source_type
+            ].fuel
+
+            if is_hours_resolution:
+                dfs.extend(
+                    [
+                        {
+                            "emission_type": emission_type,
+                            "generator_name": generator_name,
+                            "year": year,
+                            "hour": hour,
+                            "value": (
+                                fuel_usage_df[generator_name].loc[
+                                    (hour, generator_fuel)
+                                ][year]
+                                * fuels_emissions[generator_fuel][emission_type]
+                                * (1 - generator_em_reduction[emission_type])
+                            ),
+                        }
+                        for emission_type in fuels_emissions[generator_fuel].keys()
+                        for year in self._year_sample
+                        for hour in fuel_usage_df.index.get_level_values(0)[
+                            fuel_usage_df.index.get_level_values(1) == generator_fuel
+                        ]
+                    ]
+                )
+
+            else:
+                dfs.extend(
+                    [
+                        {
+                            "emission_type": emission_type,
+                            "generator_name": generator_name,
+                            "year": year,
+                            "value": (
+                                fuel_usage_df[generator_name].loc[generator_fuel][
+                                    str(year)
+                                ]
+                                * fuels_emissions[generator_fuel][emission_type]
+                                * (1 - generator_em_reduction[emission_type])
+                            ),
+                        }
+                        for emission_type in fuels_emissions[generator_fuel].keys()
+                        for year in self._year_sample
+                    ]
+                )
+
+        return dfs
+
+    def get_fuel_cost(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+    ) -> pd.DataFrame:
+        generators, storages = self._filter_elements(filter_type, filter_names)
+        df = self._get_fuel_usage(generators, storages)
+
+        for fuel_name in df.index:
+            fuel = self._network.fuels[fuel_name]
+            for year in self._year_sample:
+                df.loc[fuel.name, (slice(None), str(year))] *= fuel.cost[year]
+
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=FUEL_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+        )
+
+    def _get_data_per_unit(self, techs: Iterable, keys: list[str]) -> pd.DataFrame:
+        df_dict = {
+            key: pd.concat(
+                [getattr(t, key).to_frame(name=t.name) for t in techs], axis=1
+            )
+            for key in keys
+        }
+        df_dict = {
+            key: v.iloc[self._year_sample].unstack() for key, v in df_dict.items()
+        }
+        return pd.concat(df_dict, axis=1).T
+
+    def get_costs_per_tech_type(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+    ) -> pd.DataFrame:
+        techs = list(self._network.generator_types.values()) + list(
+            self._network.storage_types.values()
+        )
+        df = self._get_data_per_unit(
+            techs=techs,
+            keys=["capex", "opex"],
+        )
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=COST_TYPE_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+        )
+
+    def get_fuel_cost_per_tech(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+    ) -> pd.DataFrame:
+        fuels = self._network.fuels.values()
+        df = self._get_data_per_unit(techs=fuels, keys=["cost"])
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=FUEL_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+        )
+
+    def get_fuel_availability_per_tech(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+    ) -> pd.DataFrame:
+        fuels = self._network.fuels.values()
+        df = self._get_data_per_unit(techs=fuels, keys=["availability"])
+        return self._aggregate_energy_sources(
+            energy_source_df=df,
+            column_name=YEARS_LABEL,
+            index_name=FUEL_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+        )
+
+    def get_ets_cost(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+    ) -> pd.DataFrame:
+        emissions_df = self.get_emission(level="element")
+        filtered_gens_with_ets = {
+            key: obj.emission_fee
+            for key, obj in self._network.generators.items()
+            if obj.emission_fee
+        }
+        for gen_name, ets_names in filtered_gens_with_ets.items():
+            if gen_name not in emissions_df.index.get_level_values(0):
+                continue
+            for ets_name in ets_names:
+                ets = self._network.emission_fees[ets_name]
+                emissions_df.loc[gen_name, ets.emission_type] = (
+                    emissions_df.loc[gen_name, ets.emission_type]
+                    .mul(ets.price)
+                    .dropna()
+                    .values
+                )
+
+        return self._aggregate_energy_sources(
+            energy_source_df=emissions_df.T,
+            column_name=YEARS_LABEL,
+            index_name=EMISSION_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+        )
+
+    def get_ens(
+        self,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        *_, buses = self._filter_elements(filter_type, filter_names, is_bus_filter=True)
+        ens_df = self._get_ens(is_hours_resolution, buses) * self._hourly_scale
+        return self._aggregate_energy_sources(
+            energy_source_df=ens_df,
+            column_name=YEARS_LABEL,
+            index_name=ENERGY_TYPE_LABEL,
+            level="element",
+            filter_type=filter_type,
+            filter_names=filter_names,
+            is_hours_resolution=is_hours_resolution,
+        )
+
+    def _get_ens(self, is_hours_resolution: bool, buses: list[str]) -> pd.DataFrame:
+        ens_dfs = self._bus_results["generation_ens"]
+        ens_dfs = {
+            bus_name: df if is_hours_resolution else df.sum()
+            for bus_name, df in ens_dfs.items()
+            if bus_name in buses
+        }
+        for bus_name, ens_df in ens_dfs.items():
+            energy_type = self._network.buses[bus_name].energy_type
+            if is_hours_resolution:
+                ens_df = ens_df.set_index(ens_df.index.map(lambda x: (x, energy_type)))
+                ens_df.index.names = [HOUR_LABEL, ENERGY_TYPE_LABEL]
+            else:
+                ens_df = ens_df.to_frame().T
+                ens_df.index = [energy_type]
+            ens_dfs[bus_name] = ens_df
+        return pd.concat(ens_dfs, axis=1).fillna(0.0)
+
+    def get_state_of_charge(
+        self,
+        level: source_parameter_levels,
+        filter_type: source_parameter_filter_types | None = None,
+        filter_names: list[str] | None = None,
+        is_hours_resolution: bool = False,
+    ) -> pd.DataFrame:
+        _, storages = self._filter_elements(filter_type, filter_names)
+        soc_df = (
+            self._get_storage_results("state_of_charge", storages, is_hours_resolution)
+            * self._hourly_scale
+        )
+        return self._aggregate_energy_sources(
+            energy_source_df=soc_df,
+            column_name=YEARS_LABEL,
+            index_name=ENERGY_TYPE_LABEL,
+            level=level,
+            filter_type=filter_type,
+            filter_names=filter_names,
+            is_hours_resolution=is_hours_resolution,
+        )
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics/_engine/data_queries/utils.py` & `zefir-analytics-0.4.13/zefir_analytics/_engine/data_queries/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,49 @@
-# ZefirAnalytics
-# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
-#
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Affero General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# This program is distributed in the hope that it will be useful,
-# but WITHOUT ANY WARRANTY; without even the implied warranty of
-# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-# GNU Affero General Public License for more details.
-#
-# You should have received a copy of the GNU Affero General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-from typing import Callable, TypeVar
-
-import pandas as pd
-
-T = TypeVar("T")
-
-
-def argument_condition(
-    name: str | list[str], function: Callable[[str], pd.DataFrame]
-) -> pd.DataFrame | dict[str, pd.DataFrame]:
-    if isinstance(name, str):
-        return function(name)
-    return {el_name: function(el_name) for el_name in name}
-
-
-def dict_filter(
-    dictionary: dict[str, T], keys: list[str] | str | None
-) -> dict[str, T] | T:
-    return (
-        dictionary
-        if keys is None
-        else (
-            dictionary[keys]
-            if isinstance(keys, str)
-            else {key: dictionary[key] for key in keys}
-        )
-    )
+# ZefirAnalytics
+# Copyright (C) 2023-2024 Narodowe Centrum Badań Jądrowych
+#
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Affero General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# This program is distributed in the hope that it will be useful,
+# but WITHOUT ANY WARRANTY; without even the implied warranty of
+# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+# GNU Affero General Public License for more details.
+#
+# You should have received a copy of the GNU Affero General Public License
+# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+from typing import Callable, TypeVar
+
+import pandas as pd
+
+T = TypeVar("T")
+
+
+def argument_condition(
+    name: str | list[str], function: Callable[[str], pd.DataFrame]
+) -> pd.DataFrame | dict[str, pd.DataFrame]:
+    if isinstance(name, str):
+        return function(name)
+    return {el_name: function(el_name) for el_name in name}
+
+
+def dict_filter(
+    dictionary: dict[str, T], keys: list[str] | str | None
+) -> dict[str, T] | T:
+    return (
+        dictionary
+        if keys is None
+        else (
+            dictionary[keys]
+            if isinstance(keys, str)
+            else {key: dictionary[key] for key in keys}
+        )
+    )
+
+
+def assign_multiindex(df: pd.DataFrame, label: str) -> pd.DataFrame:
+    if not df.empty:
+        df.columns = pd.MultiIndex.from_tuples([(col, label) for col in df.columns])
+    return df
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics.egg-info/PKG-INFO` & `zefir-analytics-0.4.13/zefir_analytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zefir-analytics
-Version: 0.4.1
+Version: 0.4.13
 Author-email: Narodowe Centrum Badań Jądrowych <office@idea.edu.pl>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -671,15 +671,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy~=1.24.2
 Requires-Dist: pandas==2.0.1
-Requires-Dist: pyzefir==0.4.1
+Requires-Dist: pyzefir
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest==7.4.4; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: black==24.2.0; extra == "dev"
 Requires-Dist: pytest-cov~=4.1.0; extra == "dev"
 Requires-Dist: pytest-mock~=3.11.1; extra == "dev"
@@ -731,27 +731,35 @@
 ```
 Remove temporary directories such as .venv, .mypy_cache, .pytest_cache etc.
 ```bash
 make clean
 ```
 ## Available methods in Zefir Engine objects
 * source_params:
-  * get_generation_sum
-  * get_dump_energy_sum
-  * get_load_sum
-  * get_installed_capacity
-  * get_generation_demand
-  * get_fuel_usage
   * get_capex_opex
+  * get_costs_per_tech_type
+  * get_dump_energy_sum
   * get_emission
+  * get_ets_cost
+  * get_fuel_availability_per_tech
+  * get_fuel_cost
+  * get_fuel_cost_per_tech
+  * get_fuel_usage
+  * get_generation_demand
+  * get_generation_sum
+  * get_installed_capacity
+  * get_load_sum
+  * get_var_costs
 * aggregated_consumer_params:
+  * get_aggregate_elements_type_attachments
+  * get_aggregate_parameters
   * get_fractions
   * get_n_consumers
-  * get_yearly_energy_usage
   * get_total_yearly_energy_usage
-  * get_fractions
+  * get_yearly_energy_usage
 * lbs_params:
-  * get_lbs_fraction
   * get_lbs_capacity
+  * get_lbs_fraction
 * line_params:
+  * get_capacity
   * get_flow
   * get_transmission_fee
```

### Comparing `zefir-analytics-0.4.1/zefir_analytics.egg-info/SOURCES.txt` & `zefir-analytics-0.4.13/zefir_analytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

