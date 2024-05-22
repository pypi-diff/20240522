# Comparing `tmp/termsaver-0.6.tar.gz` & `tmp/termsaver-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "termsaver-0.6.tar", last modified: Fri Apr 21 00:44:25 2023, max compression
+gzip compressed data, was "termsaver-0.7.tar", last modified: Wed May 22 21:00:41 2024, max compression
```

## Comparing `termsaver-0.6.tar` & `termsaver-0.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0    11609 2023-02-06 15:23:26.427148 termsaver-0.6/LICENSE
--rw-r--r--   0        0        0     7934 2023-02-08 01:13:09.696063 termsaver-0.6/README.md
--rw-r--r--   0        0        0      750 2023-04-21 00:44:25.645660 termsaver-0.6/pyproject.toml
--rw-r--r--   0        0        0    11248 2023-04-21 00:05:45.797612 termsaver-0.6/termsaver/__init__.py
--rw-r--r--   0        0        0       80 2023-02-08 01:47:38.876905 termsaver-0.6/termsaver/__main__.py
--rw-r--r--   0        0        0  2046847 2023-02-08 01:13:09.713067 termsaver-0.6/termsaver/data/sw1.txt
--rw-r--r--   0        0        0     1682 2023-02-08 01:13:09.699063 termsaver-0.6/termsaver/termsaverlib/__init__.py
--rw-r--r--   0        0        0     8477 2023-02-08 01:13:09.700063 termsaver-0.6/termsaver/termsaverlib/common.py
--rw-r--r--   0        0        0     3647 2023-02-08 01:13:09.700063 termsaver-0.6/termsaver/termsaverlib/constants.py
--rw-r--r--   0        0        0     5889 2023-02-08 01:13:09.702064 termsaver-0.6/termsaver/termsaverlib/exception.py
--rw-r--r--   0        0        0     1211 2023-02-08 01:13:09.701063 termsaver-0.6/termsaver/termsaverlib/helper/__init__.py
--rw-r--r--   0        0        0     1397 2023-02-08 01:13:09.702064 termsaver-0.6/termsaver/termsaverlib/helper/smartformatter.py
--rw-r--r--   0        0        0     1375 2023-02-08 01:13:09.701063 termsaver-0.6/termsaver/termsaverlib/helper/utilities.py
--rw-r--r--   0        0        0     1985 2023-02-08 01:13:09.702064 termsaver-0.6/termsaver/termsaverlib/i18n.py
--rw-r--r--   0        0        0     4614 2023-04-21 00:05:00.093614 termsaver-0.6/termsaver/termsaverlib/plugins/__init__.py
--rw-r--r--   0        0        0     2994 2023-02-08 01:13:09.704063 termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/constants.py
--rw-r--r--   0        0        0     1064 2023-02-08 01:13:09.703064 termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/__init__.py
--rw-r--r--   0        0        0     2077 2023-02-08 01:13:09.703064 termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/base/__init__.py
--rw-r--r--   0        0        0     3012 2023-02-08 01:13:09.703064 termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/eps.py
--rw-r--r--   0        0        0     4100 2023-02-13 17:17:10.128732 termsaver-0.6/termsaver/termsaverlib/screen/__init__.py
--rw-r--r--   0        0        0     4101 2023-02-08 01:13:09.705063 termsaver-0.6/termsaver/termsaverlib/screen/asciiartfarts.py
--rw-r--r--   0        0        0    12567 2023-04-21 00:05:45.795615 termsaver-0.6/termsaver/termsaverlib/screen/base/__init__.py
--rw-r--r--   0        0        0    13235 2023-02-08 01:13:09.704063 termsaver-0.6/termsaver/termsaverlib/screen/base/filereader.py
--rw-r--r--   0        0        0     9617 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/base/rssfeed.py
--rw-r--r--   0        0        0     5945 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/base/urlfetcher.py
--rw-r--r--   0        0        0    14623 2023-04-21 00:05:45.794614 termsaver-0.6/termsaver/termsaverlib/screen/clock.py
--rw-r--r--   0        0        0    53820 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/clocknumber for tremsaver.xlsm
--rw-r--r--   0        0        0     2608 2023-02-08 01:13:09.705063 termsaver-0.6/termsaver/termsaverlib/screen/helper/__init__.py
--rw-r--r--   0        0        0     4134 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/helper/imageconverter.py
--rw-r--r--   0        0        0    12002 2023-04-21 00:05:45.796613 termsaver-0.6/termsaver/termsaverlib/screen/helper/position.py
--rw-r--r--   0        0        0     4081 2023-02-08 01:13:09.706063 termsaver-0.6/termsaver/termsaverlib/screen/helper/typing.py
--rw-r--r--   0        0        0     7322 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/helper/urlfetcher.py
--rw-r--r--   0        0        0     7204 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/helper/xmlreader.py
--rw-r--r--   0        0        0    16945 2023-02-08 01:13:09.707063 termsaver-0.6/termsaver/termsaverlib/screen/img2ascii.py
--rw-r--r--   0        0        0     4643 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/jokes4all.py
--rw-r--r--   0        0        0    13137 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/matrix.py
--rw-r--r--   0        0        0     4642 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/programmer.py
--rw-r--r--   0        0        0     4694 2023-02-08 01:13:09.708063 termsaver-0.6/termsaver/termsaverlib/screen/quotes4all.py
--rw-r--r--   0        0        0     6242 2023-02-08 01:13:09.709064 termsaver-0.6/termsaver/termsaverlib/screen/randtxt.py
--rw-r--r--   0        0        0     4629 2023-02-08 01:13:09.711067 termsaver-0.6/termsaver/termsaverlib/screen/rfc.py
--rw-r--r--   0        0        0     4217 2023-02-08 01:13:09.711067 termsaver-0.6/termsaver/termsaverlib/screen/rssfeed.py
--rw-r--r--   0        0        0     4725 2023-02-08 01:13:09.711067 termsaver-0.6/termsaver/termsaverlib/screen/starwars.py
--rw-r--r--   0        0        0    15328 2023-02-08 01:13:09.711067 termsaver-0.6/termsaver/termsaverlib/screen/sysmon.py
--rw-r--r--   0        0        0     3307 2023-02-08 01:13:09.709064 termsaver-0.6/termsaver/termsaverlib/screen/urlfetcher.py
--rw-r--r--   0        0        0     3987 2023-02-08 01:13:09.710066 termsaver-0.6/termsaver/termsaverlib/screen/wttr.py
--rw-r--r--   0        0        0       20 2023-02-06 15:23:26.441441 termsaver-0.6/tests/empty-for-tests/testfile.txt
--rw-r--r--   0        0        0    12237 2023-02-08 01:13:09.710066 termsaver-0.6/tests/screentests.py
--rw-r--r--   0        0        0     6540 2023-02-08 01:13:09.710066 termsaver-0.6/tests/test.py
--rw-r--r--   0        0        0     8188 1970-01-01 00:00:00.000000 termsaver-0.6/PKG-INFO
+-rw-r--r--   0        0        0    11818 2024-05-22 20:19:57.589258 termsaver-0.7/LICENSE
+-rw-r--r--   0        0        0     7934 2024-05-22 20:19:57.590263 termsaver-0.7/README.md
+-rw-r--r--   0        0        0      751 2024-05-22 21:00:41.875922 termsaver-0.7/pyproject.toml
+-rw-r--r--   0        0        0    11248 2024-05-22 20:19:57.599260 termsaver-0.7/termsaver/__init__.py
+-rw-r--r--   0        0        0       80 2024-05-22 20:19:57.599260 termsaver-0.7/termsaver/__main__.py
+-rw-r--r--   0        0        0  2046847 2024-05-22 20:19:57.605268 termsaver-0.7/termsaver/data/sw1.txt
+-rw-r--r--   0        0        0     1682 2024-05-22 20:19:57.606267 termsaver-0.7/termsaver/termsaverlib/__init__.py
+-rw-r--r--   0        0        0     8477 2024-05-22 20:19:57.606267 termsaver-0.7/termsaver/termsaverlib/common.py
+-rw-r--r--   0        0        0     3647 2024-05-22 20:19:57.606267 termsaver-0.7/termsaver/termsaverlib/constants.py
+-rw-r--r--   0        0        0     5889 2024-05-22 20:19:57.607266 termsaver-0.7/termsaver/termsaverlib/exception.py
+-rw-r--r--   0        0        0     1211 2024-05-22 20:19:57.608267 termsaver-0.7/termsaver/termsaverlib/helper/__init__.py
+-rw-r--r--   0        0        0     1397 2024-05-22 20:19:57.608267 termsaver-0.7/termsaver/termsaverlib/helper/smartformatter.py
+-rw-r--r--   0        0        0     1375 2024-05-22 20:19:57.608267 termsaver-0.7/termsaver/termsaverlib/helper/utilities.py
+-rw-r--r--   0        0        0     1985 2024-05-22 20:19:57.608267 termsaver-0.7/termsaver/termsaverlib/i18n.py
+-rw-r--r--   0        0        0     4614 2024-05-22 20:19:57.609268 termsaver-0.7/termsaver/termsaverlib/plugins/__init__.py
+-rw-r--r--   0        0        0     2994 2024-05-22 20:19:57.609268 termsaver-0.7/termsaver/termsaverlib/plugins/exampleplugin/constants.py
+-rw-r--r--   0        0        0     1064 2024-05-22 20:19:57.609268 termsaver-0.7/termsaver/termsaverlib/plugins/exampleplugin/screen/__init__.py
+-rw-r--r--   0        0        0     2077 2024-05-22 20:19:57.610268 termsaver-0.7/termsaver/termsaverlib/plugins/exampleplugin/screen/base/__init__.py
+-rw-r--r--   0        0        0     3012 2024-05-22 20:19:57.610268 termsaver-0.7/termsaver/termsaverlib/plugins/exampleplugin/screen/eps.py
+-rw-r--r--   0        0        0     4100 2024-05-22 20:19:57.610268 termsaver-0.7/termsaver/termsaverlib/screen/__init__.py
+-rw-r--r--   0        0        0     4101 2024-05-22 20:19:57.611269 termsaver-0.7/termsaver/termsaverlib/screen/asciiartfarts.py
+-rw-r--r--   0        0        0    12567 2024-05-22 20:19:57.611269 termsaver-0.7/termsaver/termsaverlib/screen/base/__init__.py
+-rw-r--r--   0        0        0    13235 2024-05-22 20:19:57.611269 termsaver-0.7/termsaver/termsaverlib/screen/base/filereader.py
+-rw-r--r--   0        0        0     9617 2024-05-22 20:19:57.612268 termsaver-0.7/termsaver/termsaverlib/screen/base/rssfeed.py
+-rw-r--r--   0        0        0     5945 2024-05-22 20:19:57.612268 termsaver-0.7/termsaver/termsaverlib/screen/base/urlfetcher.py
+-rw-r--r--   0        0        0    14623 2024-05-22 20:19:57.612268 termsaver-0.7/termsaver/termsaverlib/screen/clock.py
+-rw-r--r--   0        0        0    53820 2024-05-22 20:19:57.613268 termsaver-0.7/termsaver/termsaverlib/screen/clocknumber for tremsaver.xlsm
+-rw-r--r--   0        0        0     2608 2024-05-22 20:19:57.613268 termsaver-0.7/termsaver/termsaverlib/screen/helper/__init__.py
+-rw-r--r--   0        0        0     4134 2024-05-22 20:19:57.613268 termsaver-0.7/termsaver/termsaverlib/screen/helper/imageconverter.py
+-rw-r--r--   0        0        0    12002 2024-05-22 20:19:57.614267 termsaver-0.7/termsaver/termsaverlib/screen/helper/position.py
+-rw-r--r--   0        0        0     4081 2024-05-22 20:19:57.614267 termsaver-0.7/termsaver/termsaverlib/screen/helper/typing.py
+-rw-r--r--   0        0        0     7322 2024-05-22 20:19:57.615264 termsaver-0.7/termsaver/termsaverlib/screen/helper/urlfetcher.py
+-rw-r--r--   0        0        0     7204 2024-05-22 20:19:57.615264 termsaver-0.7/termsaver/termsaverlib/screen/helper/xmlreader.py
+-rw-r--r--   0        0        0    16945 2024-05-22 20:19:57.615264 termsaver-0.7/termsaver/termsaverlib/screen/img2ascii.py
+-rw-r--r--   0        0        0     4643 2024-05-22 20:19:57.615264 termsaver-0.7/termsaver/termsaverlib/screen/jokes4all.py
+-rw-r--r--   0        0        0    13142 2024-05-22 20:50:30.112582 termsaver-0.7/termsaver/termsaverlib/screen/matrix.py
+-rw-r--r--   0        0        0     4642 2024-05-22 20:19:57.616370 termsaver-0.7/termsaver/termsaverlib/screen/programmer.py
+-rw-r--r--   0        0        0     4694 2024-05-22 20:19:57.616370 termsaver-0.7/termsaver/termsaverlib/screen/quotes4all.py
+-rw-r--r--   0        0        0     6242 2024-05-22 20:19:57.616370 termsaver-0.7/termsaver/termsaverlib/screen/randtxt.py
+-rw-r--r--   0        0        0     4629 2024-05-22 20:19:57.616370 termsaver-0.7/termsaver/termsaverlib/screen/rfc.py
+-rw-r--r--   0        0        0     4217 2024-05-22 20:19:57.617275 termsaver-0.7/termsaver/termsaverlib/screen/rssfeed.py
+-rw-r--r--   0        0        0     4725 2024-05-22 20:19:57.617275 termsaver-0.7/termsaver/termsaverlib/screen/starwars.py
+-rw-r--r--   0        0        0    15328 2024-05-22 20:19:57.617275 termsaver-0.7/termsaver/termsaverlib/screen/sysmon.py
+-rw-r--r--   0        0        0     3307 2024-05-22 20:19:57.617275 termsaver-0.7/termsaver/termsaverlib/screen/urlfetcher.py
+-rw-r--r--   0        0        0     3987 2024-05-22 20:19:57.617275 termsaver-0.7/termsaver/termsaverlib/screen/wttr.py
+-rw-r--r--   0        0        0       20 2024-05-22 20:19:57.618270 termsaver-0.7/tests/empty-for-tests/testfile.txt
+-rw-r--r--   0        0        0    12237 2024-05-22 20:19:57.618270 termsaver-0.7/tests/screentests.py
+-rw-r--r--   0        0        0     6540 2024-05-22 20:19:57.618270 termsaver-0.7/tests/test.py
+-rw-r--r--   0        0        0     8189 1970-01-01 00:00:00.000000 termsaver-0.7/PKG-INFO
```

### Comparing `termsaver-0.6/LICENSE` & `termsaver-0.7/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,209 +1,209 @@
-
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
-
-
-THIRD-PARTY DEPENDENCIES
-========================
-Convenience copies of some third-party dependencies are distributed with
-Apache Cassandra as Java jar files in lib/. Licensing information for
-these files can be found in the lib/licenses directory.
+
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
+
+
+THIRD-PARTY DEPENDENCIES
+========================
+Convenience copies of some third-party dependencies are distributed with
+Apache Cassandra as Java jar files in lib/. Licensing information for
+these files can be found in the lib/licenses directory.
```

### Comparing `termsaver-0.6/README.md` & `termsaver-0.7/README.md`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/pyproject.toml` & `termsaver-0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.pdm]
 
 [project]
 name = "termsaver"
-version = "0.6"
+version = "0.7"
 description = "Simple text-based terminal screensaver."
 keywords = [
     "command-line",
     "terminal",
     "screensaver",
 ]
 readme = "README.md"
 authors = [
     { name = "Bruno Braga", email = "bruno@brunobraga.net" },
 ]
 maintainers = [
     { name = "Eddie Dover", email = "ed@eddiedover.dev" },
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.12"
 dependencies = [
     "pillow",
     "requests",
 ]
 
 [project.license]
 text = "Apache License v2"
```

### Comparing `termsaver-0.6/termsaver/__init__.py` & `termsaver-0.7/termsaver/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/data/sw1.txt` & `termsaver-0.7/termsaver/data/sw1.txt`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/__init__.py` & `termsaver-0.7/termsaver/termsaverlib/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/common.py` & `termsaver-0.7/termsaver/termsaverlib/common.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/constants.py` & `termsaver-0.7/termsaver/termsaverlib/constants.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/exception.py` & `termsaver-0.7/termsaver/termsaverlib/exception.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/helper/__init__.py` & `termsaver-0.7/termsaver/termsaverlib/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/helper/smartformatter.py` & `termsaver-0.7/termsaver/termsaverlib/helper/smartformatter.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/helper/utilities.py` & `termsaver-0.7/termsaver/termsaverlib/helper/utilities.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/i18n.py` & `termsaver-0.7/termsaver/termsaverlib/i18n.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/plugins/__init__.py` & `termsaver-0.7/termsaver/termsaverlib/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/constants.py` & `termsaver-0.7/termsaver/termsaverlib/plugins/exampleplugin/constants.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/__init__.py` & `termsaver-0.7/termsaver/termsaverlib/plugins/exampleplugin/screen/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/base/__init__.py` & `termsaver-0.7/termsaver/termsaverlib/plugins/exampleplugin/screen/base/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/plugins/exampleplugin/screen/eps.py` & `termsaver-0.7/termsaver/termsaverlib/plugins/exampleplugin/screen/eps.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/__init__.py` & `termsaver-0.7/termsaver/termsaverlib/screen/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/asciiartfarts.py` & `termsaver-0.7/termsaver/termsaverlib/screen/asciiartfarts.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/base/__init__.py` & `termsaver-0.7/termsaver/termsaverlib/screen/base/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/base/filereader.py` & `termsaver-0.7/termsaver/termsaverlib/screen/base/filereader.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/base/rssfeed.py` & `termsaver-0.7/termsaver/termsaverlib/screen/base/rssfeed.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/base/urlfetcher.py` & `termsaver-0.7/termsaver/termsaverlib/screen/base/urlfetcher.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/clock.py` & `termsaver-0.7/termsaver/termsaverlib/screen/clock.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/clocknumber for tremsaver.xlsm` & `termsaver-0.7/termsaver/termsaverlib/screen/clocknumber for tremsaver.xlsm`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/helper/__init__.py` & `termsaver-0.7/termsaver/termsaverlib/screen/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/helper/imageconverter.py` & `termsaver-0.7/termsaver/termsaverlib/screen/helper/imageconverter.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/helper/position.py` & `termsaver-0.7/termsaver/termsaverlib/screen/helper/position.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/helper/typing.py` & `termsaver-0.7/termsaver/termsaverlib/screen/helper/typing.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/helper/urlfetcher.py` & `termsaver-0.7/termsaver/termsaverlib/screen/helper/urlfetcher.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/helper/xmlreader.py` & `termsaver-0.7/termsaver/termsaverlib/screen/helper/xmlreader.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/img2ascii.py` & `termsaver-0.7/termsaver/termsaverlib/screen/img2ascii.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/jokes4all.py` & `termsaver-0.7/termsaver/termsaverlib/screen/jokes4all.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/matrix.py` & `termsaver-0.7/termsaver/termsaverlib/screen/matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,16 +322,16 @@
         """
         creates a randomized list of characters to be used in the `screen_map`.
         """
         result = []
         while(len(result) == 0):
             bt = [self.space for __ in range(0, 
                     min((self.geometry['y'], random.randint(0, 
-                        self.geometry['y'] * 20 / (self.granularity * \
-                            self.proportion)))))]
+                        int(self.geometry['y'] * 20 / (self.granularity * \
+                            self.proportion))))))]
             cl = [self.digmap[random.randint(0, len(self.digmap)) - 1] \
                   for __ in range(0, random.randint(0, 
                       self.geometry['y'] - len(bt)))]
             result = bt
             result.extend(cl)
         return result
```

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/programmer.py` & `termsaver-0.7/termsaver/termsaverlib/screen/programmer.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/quotes4all.py` & `termsaver-0.7/termsaver/termsaverlib/screen/quotes4all.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/randtxt.py` & `termsaver-0.7/termsaver/termsaverlib/screen/randtxt.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/rfc.py` & `termsaver-0.7/termsaver/termsaverlib/screen/rfc.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/rssfeed.py` & `termsaver-0.7/termsaver/termsaverlib/screen/rssfeed.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/starwars.py` & `termsaver-0.7/termsaver/termsaverlib/screen/starwars.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/sysmon.py` & `termsaver-0.7/termsaver/termsaverlib/screen/sysmon.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/urlfetcher.py` & `termsaver-0.7/termsaver/termsaverlib/screen/urlfetcher.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/termsaver/termsaverlib/screen/wttr.py` & `termsaver-0.7/termsaver/termsaverlib/screen/wttr.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/tests/screentests.py` & `termsaver-0.7/tests/screentests.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/tests/test.py` & `termsaver-0.7/tests/test.py`

 * *Files identical despite different names*

### Comparing `termsaver-0.6/PKG-INFO` & `termsaver-0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: termsaver
-Version: 0.6
+Version: 0.7
 Summary: Simple text-based terminal screensaver.
-Keywords: command-line terminal screensaver
+Keywords: command-line,terminal,screensaver
 Author-Email: Bruno Braga <bruno@brunobraga.net>
 Maintainer-Email: Eddie Dover <ed@eddiedover.dev>
 License: Apache License v2
 Project-URL: Homepage, https://www.github.com/brunobraga/termsaver
 Project-URL: Bug tracker, https://github.com/brunobraga/termsaver/issues
-Requires-Python: >=3.6
+Requires-Python: >=3.12
 Requires-Dist: pillow
 Requires-Dist: requests
 Description-Content-Type: text/markdown
 
 <!-- 
 ###############################################################################
 #
```

