# Comparing `tmp/yc_aws_wrapper-0.0.0.tar.gz` & `tmp/yc_aws_wrapper-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yc_aws_wrapper-0.0.0.tar", last modified: Fri May 17 14:37:27 2024, max compression
+gzip compressed data, was "yc_aws_wrapper-0.0.1.tar", last modified: Wed May 22 14:53:22 2024, max compression
```

## Comparing `yc_aws_wrapper-0.0.0.tar` & `yc_aws_wrapper-0.0.1.tar`

### file list

```diff
@@ -1,14 +1,28 @@
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-17 14:37:27.246275 yc_aws_wrapper-0.0.0/
--rw-r--r--   0 macuser    (502) staff       (20)     1226 2023-08-25 10:40:36.000000 yc_aws_wrapper-0.0.0/COPYRIGHT
--rw-r--r--   0 macuser    (502) staff       (20)    34520 2023-08-25 10:40:36.000000 yc_aws_wrapper-0.0.0/LICENSE
--rw-r--r--   0 macuser    (502) staff       (20)       53 2023-08-25 10:40:36.000000 yc_aws_wrapper-0.0.0/MANIFEST.in
--rw-r--r--   0 macuser    (502) staff       (20)     1104 2024-05-17 14:37:27.246083 yc_aws_wrapper-0.0.0/PKG-INFO
--rw-r--r--   0 macuser    (502) staff       (20)       11 2024-05-17 14:19:55.000000 yc_aws_wrapper-0.0.0/README.md
--rw-r--r--   0 macuser    (502) staff       (20)       38 2024-05-17 14:37:27.246317 yc_aws_wrapper-0.0.0/setup.cfg
--rw-r--r--   0 macuser    (502) staff       (20)     3082 2024-05-17 14:21:23.000000 yc_aws_wrapper-0.0.0/setup.py
-drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-17 14:37:27.245910 yc_aws_wrapper-0.0.0/yc_aws_wrapper.egg-info/
--rw-r--r--   0 macuser    (502) staff       (20)     1104 2024-05-17 14:37:27.000000 yc_aws_wrapper-0.0.0/yc_aws_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 macuser    (502) staff       (20)      237 2024-05-17 14:37:27.000000 yc_aws_wrapper-0.0.0/yc_aws_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-17 14:37:27.000000 yc_aws_wrapper-0.0.0/yc_aws_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-17 14:37:27.000000 yc_aws_wrapper-0.0.0/yc_aws_wrapper.egg-info/not-zip-safe
--rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-17 14:37:27.000000 yc_aws_wrapper-0.0.0/yc_aws_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.649551 yc_aws_wrapper-0.0.1/
+-rw-r--r--   0 macuser    (502) staff       (20)     1226 2023-08-25 10:40:36.000000 yc_aws_wrapper-0.0.1/COPYRIGHT
+-rw-r--r--   0 macuser    (502) staff       (20)    35149 2024-05-20 12:22:26.000000 yc_aws_wrapper-0.0.1/LICENSE
+-rw-r--r--   0 macuser    (502) staff       (20)       52 2024-05-20 12:46:04.000000 yc_aws_wrapper-0.0.1/MANIFEST.in
+-rw-r--r--   0 macuser    (502) staff       (20)     2118 2024-05-22 14:53:22.649328 yc_aws_wrapper-0.0.1/PKG-INFO
+-rw-r--r--   0 macuser    (502) staff       (20)      780 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/README.md
+-rw-r--r--   0 macuser    (502) staff       (20)       38 2024-05-22 14:53:22.649587 yc_aws_wrapper-0.0.1/setup.cfg
+-rw-r--r--   0 macuser    (502) staff       (20)     3713 2024-05-22 14:52:38.000000 yc_aws_wrapper-0.0.1/setup.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.646514 yc_aws_wrapper-0.0.1/tests/
+-rw-r--r--   0 macuser    (502) staff       (20)     1842 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/tests/test_s3.py
+-rw-r--r--   0 macuser    (502) staff       (20)     1907 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/tests/test_sqs.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.647147 yc_aws_wrapper-0.0.1/yc_aws_wrapper/
+-rw-r--r--   0 macuser    (502) staff       (20)     1966 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/__about__.py
+-rw-r--r--   0 macuser    (502) staff       (20)     1703 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/__init__.py
+-rw-r--r--   0 macuser    (502) staff       (20)     2230 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/base.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.648294 yc_aws_wrapper-0.0.1/yc_aws_wrapper/kinesis/
+-rw-r--r--   0 macuser    (502) staff       (20)      600 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/kinesis/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.648536 yc_aws_wrapper-0.0.1/yc_aws_wrapper/s3/
+-rw-r--r--   0 macuser    (502) staff       (20)     1306 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/s3/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.648776 yc_aws_wrapper-0.0.1/yc_aws_wrapper/sqs/
+-rw-r--r--   0 macuser    (502) staff       (20)     2578 2024-05-22 14:07:05.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper/sqs/__init__.py
+drwxr-xr-x   0 macuser    (502) staff       (20)        0 2024-05-22 14:53:22.649065 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/
+-rw-r--r--   0 macuser    (502) staff       (20)     2118 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 macuser    (502) staff       (20)      483 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 macuser    (502) staff       (20)        1 2024-05-22 13:53:56.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/not-zip-safe
+-rw-r--r--   0 macuser    (502) staff       (20)       31 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/requires.txt
+-rw-r--r--   0 macuser    (502) staff       (20)       15 2024-05-22 14:53:22.000000 yc_aws_wrapper-0.0.1/yc_aws_wrapper.egg-info/top_level.txt
```

### Comparing `yc_aws_wrapper-0.0.0/COPYRIGHT` & `yc_aws_wrapper-0.0.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `yc_aws_wrapper-0.0.0/LICENSE` & `yc_aws_wrapper-0.0.1/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,70 +1,82 @@
-                    GNU AFFERO GENERAL PUBLIC LICENSE
-                       Version 3, 19 November 2007
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
-  The GNU Affero General Public License is a free, copyleft license for
-software and other kinds of works, specifically designed to ensure
-cooperation with the community in the case of network server software.
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
 
   The licenses for most software and other practical works are designed
 to take away your freedom to share and change the works.  By contrast,
-our General Public Licenses are intended to guarantee your freedom to
+the GNU General Public License is intended to guarantee your freedom to
 share and change all versions of a program--to make sure it remains free
-software for all its users.
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
 
   When we speak of free software, we are referring to freedom, not
 price.  Our General Public Licenses are designed to make sure that you
 have the freedom to distribute copies of free software (and charge for
 them if you wish), that you receive source code or can get it if you
 want it, that you can change the software or use pieces of it in new
 free programs, and that you know you can do these things.
 
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
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
 
   The precise terms and conditions for copying, distribution and
 modification follow.
 
                        TERMS AND CONDITIONS
 
   0. Definitions.
 
-  "This License" refers to version 3 of the GNU Affero General Public License.
+  "This License" refers to version 3 of the GNU General Public License.
 
   "Copyright" also means copyright-like laws that apply to other kinds of
 works, such as semiconductor masks.
 
   "The Program" refers to any copyrightable work licensed under this
 License.  Each licensee is addressed as "you".  "Licensees" and
 "recipients" may be individuals or organizations.
@@ -533,53 +545,43 @@
 covered work so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you may
 not convey it at all.  For example, if you agree to terms that obligate you
 to collect a royalty for further conveying from those to whom you convey
 the Program, the only way you could satisfy both those terms and this
 License would be to refrain entirely from conveying the Program.
 
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
+  13. Use with the GNU Affero General Public License.
 
   Notwithstanding any other provision of this License, you have
 permission to link or combine any covered work with a work licensed
-under version 3 of the GNU General Public License into a single
+under version 3 of the GNU Affero General Public License into a single
 combined work, and to convey the resulting work.  The terms of this
 License will continue to apply to the part which is the covered work,
-but the work with which it is combined will remain governed by version
-3 of the GNU General Public License.
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
 
   14. Revised Versions of this License.
 
   The Free Software Foundation may publish revised and/or new versions of
-the GNU Affero General Public License from time to time.  Such new versions
-will be similar in spirit to the present version, but may differ in detail to
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
 address new problems or concerns.
 
   Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU Affero General
+Program specifies that a certain numbered version of the GNU General
 Public License "or any later version" applies to it, you have the
 option of following the terms and conditions either of that numbered
 version or of any later version published by the Free Software
 Foundation.  If the Program does not specify a version number of the
-GNU Affero General Public License, you may choose any version ever published
+GNU General Public License, you may choose any version ever published
 by the Free Software Foundation.
 
   If the Program specifies that a proxy can decide which future
-versions of the GNU Affero General Public License can be used, that proxy's
+versions of the GNU General Public License can be used, that proxy's
 public statement of acceptance of a version permanently authorizes you
 to choose that version for the Program.
 
   Later license versions may give you additional or different
 permissions.  However, no additional obligations are imposed on any
 author or copyright holder as a result of your choosing to follow a
 later version.
@@ -629,33 +631,44 @@
 state the exclusion of warranty; and each file should have at least
 the "copyright" line and a pointer to where the full notice is found.
 
     <one line to give the program's name and a brief idea of what it does.>
     Copyright (C) <year>  <name of author>
 
     This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU Affero General Public License as published by
+    it under the terms of the GNU General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU Affero General Public License for more details.
+    GNU General Public License for more details.
 
-    You should have received a copy of the GNU Affero General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
-  If your software can interact with users remotely through a computer
-network, you should also make sure that it provides a way for users to
-get its source.  For example, if your program is a web application, its
-interface could display a "Source" link that leads users to an archive
-of the code.  There are many ways you could offer source, and different
-solutions will be better for different programs; see section 13 for the
-specific requirements.
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU AGPL, see
-<http://www.gnu.org/licenses/>.
+For more information on this, and how to apply and follow the GNU GPL, see
+<https://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `yc_aws_wrapper-0.0.0/setup.py` & `yc_aws_wrapper-0.0.1/yc_aws_wrapper/__about__.py`

 * *Files 25% similar despite different names*

```diff
@@ -24,57 +24,26 @@
 #  See the GNU Affero General Public License Version 3 for more details.
 #
 #  You should have received a copy of the GNU Affero General Public license along
 #  with this program. If not, see <http://www.gnu.org/licenses/agpl-3.0.en.html>.
 #
 #####################################################################################
 
-from __future__ import absolute_import
-import os
-from setuptools import setup, find_packages
-
-
-base_dir = os.path.dirname(__file__)
-about = {}
-if base_dir:
-    os.chdir(base_dir)
-with open(os.path.join(base_dir, "__about__.py")) as f:
-    exec(f.read(), about)
-
-with open(os.path.join(base_dir, "README.md")) as f:
-    long_description = f.read()
-
-
-setup(
-    name=about["__title__"],
-    version=about["__version__"],
-    description=about["__summary__"],
-    long_description=long_description,
-    license=about["__license__"],
-    url=about["__uri__"],
-    author=about["__author__"],
-    author_email=about["__email__"],
-    platforms=('Any'),
-    install_requires=[],
-    packages=find_packages(),
-    include_package_data=True,
-    data_files=[('.', ['LICENSE', 'COPYRIGHT'])],
-    zip_safe=False,
-    classifiers=[
-        "License :: OSI Approved :: GNU Affero General Public License v3",
-        "Development Status :: 1 - Planning",
-        "Environment :: No Input/Output (Daemon)",
-        "Environment :: Console",
-        "Intended Audience :: Developers",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
-        "Topic :: Internet",
-        "Topic :: Communications",
-        "Topic :: Database",
-        "Topic :: Software Development :: Libraries",
-        "Topic :: Software Development :: Libraries :: Application Frameworks",
-        "Topic :: System :: Networking"
-    ],
-    keywords='WAMP crossbar beanstalkd boom'
-)
+__all__ = [
+    "__title__",
+    "__summary__",
+    "__uri__",
+    "__version__",
+    "__author__",
+    "__email__",
+    "__license__",
+    "__copyright__"
+]
+
+__title__ = "yc-aws-wrapper"
+__summary__ = "yc-aws-wrapper."
+__uri__ = "https://github.com/mcode-cc/python-yandex-cloud-sdk-wrapper/"
+__version__ = "0.0.1"
+__author__ = "MCode GmbH"
+__email__ = "python-yandex-cloud-sdk-wrapper@mcode.cc"
+__license__ = "GNU AFFERO GENERAL PUBLIC LICENSE Version 3, 29 June 2007"
+__copyright__ = "2021 %s" % __author__
```

