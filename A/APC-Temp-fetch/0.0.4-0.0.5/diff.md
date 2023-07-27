# Comparing `tmp/APC-Temp-fetch-0.0.4.tar.gz` & `tmp/apc_temp_fetch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "APC-Temp-fetch-0.0.4.tar", last modified: Wed Jul 19 22:20:33 2023, max compression
+gzip compressed data, was "apc_temp_fetch-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `APC-Temp-fetch-0.0.4.tar` & `apc_temp_fetch-0.0.5.tar`

### file list

```diff
@@ -1,27 +1,14 @@
-drwxr-xr-x   0 fogti     (1000) fogti     (1000)        0 2023-07-19 22:20:33.548119 APC-Temp-fetch-0.0.4/
--rw-r--r--   0 fogti     (1000) fogti     (1000)    11358 2021-11-23 11:00:47.000000 APC-Temp-fetch-0.0.4/LICENSE.txt
--rw-r--r--   0 fogti     (1000) fogti     (1000)       36 2022-03-25 21:25:42.000000 APC-Temp-fetch-0.0.4/MANIFEST.in
--rw-r--r--   0 fogti     (1000) fogti     (1000)     3717 2023-07-19 22:20:33.548119 APC-Temp-fetch-0.0.4/PKG-INFO
--rw-r--r--   0 fogti     (1000) fogti     (1000)     3230 2023-07-19 22:18:26.000000 APC-Temp-fetch-0.0.4/README.md
--rw-r--r--   0 fogti     (1000) fogti     (1000)      805 2023-07-19 22:20:33.548119 APC-Temp-fetch-0.0.4/setup.cfg
--rw-r--r--   0 fogti     (1000) fogti     (1000)       37 2021-11-23 11:19:36.000000 APC-Temp-fetch-0.0.4/setup.py
-drwxr-xr-x   0 fogti     (1000) fogti     (1000)        0 2023-07-19 22:20:33.543119 APC-Temp-fetch-0.0.4/src/
-drwxr-xr-x   0 fogti     (1000) fogti     (1000)        0 2023-07-19 22:20:33.546119 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/
--rw-r--r--   0 fogti     (1000) fogti     (1000)      324 2023-07-19 21:36:07.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/__init__.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)     2017 2022-03-25 16:27:46.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/base.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)     3150 2023-07-19 19:43:41.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/cli.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)     1383 2023-07-19 22:15:16.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/cs121.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)     1443 2022-03-25 20:41:47.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/cs141.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)     2639 2023-07-19 21:30:07.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/frmnc.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)     1346 2023-07-19 21:30:44.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/frmnc666.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)     3057 2023-07-19 21:27:58.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/gden_nt07.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)      493 2021-11-24 23:24:20.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/old.py
--rw-r--r--   0 fogti     (1000) fogti     (1000)        0 2021-11-24 14:24:48.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/py.typed
-drwxr-xr-x   0 fogti     (1000) fogti     (1000)        0 2023-07-19 22:20:33.547119 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch.egg-info/
--rw-r--r--   0 fogti     (1000) fogti     (1000)     3717 2023-07-19 22:20:33.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch.egg-info/PKG-INFO
--rw-r--r--   0 fogti     (1000) fogti     (1000)      632 2023-07-19 22:20:33.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch.egg-info/SOURCES.txt
--rw-r--r--   0 fogti     (1000) fogti     (1000)        1 2023-07-19 22:20:33.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch.egg-info/dependency_links.txt
--rw-r--r--   0 fogti     (1000) fogti     (1000)      102 2023-07-19 22:20:33.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch.egg-info/entry_points.txt
--rw-r--r--   0 fogti     (1000) fogti     (1000)        1 2023-07-19 19:41:03.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch.egg-info/not-zip-safe
--rw-r--r--   0 fogti     (1000) fogti     (1000)        9 2023-07-19 22:20:33.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch.egg-info/requires.txt
--rw-r--r--   0 fogti     (1000) fogti     (1000)       15 2023-07-19 22:20:33.000000 APC-Temp-fetch-0.0.4/src/APC_Temp_fetch.egg-info/top_level.txt
+-rw-r--r--   0        0        0     9161 2023-07-20 12:44:31.164749 apc_temp_fetch-0.0.5/LICENSE
+-rw-r--r--   0        0        0     3230 2023-07-19 22:18:26.341626 apc_temp_fetch-0.0.5/README.md
+-rw-r--r--   0        0        0      825 2023-07-27 12:14:40.903265 apc_temp_fetch-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      324 2023-07-27 11:42:23.454936 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/__init__.py
+-rw-r--r--   0        0        0     2017 2022-03-25 16:27:46.596593 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/base.py
+-rw-r--r--   0        0        0     3150 2023-07-19 19:43:41.327909 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/cli.py
+-rw-r--r--   0        0        0     1383 2023-07-19 22:15:16.317435 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/cs121.py
+-rw-r--r--   0        0        0     1443 2022-03-25 20:41:47.095024 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/cs141.py
+-rw-r--r--   0        0        0     2639 2023-07-19 21:30:07.147413 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/frmnc.py
+-rw-r--r--   0        0        0     1346 2023-07-19 21:30:44.786707 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/frmnc666.py
+-rw-r--r--   0        0        0     3057 2023-07-19 21:27:58.339893 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/gden_nt07.py
+-rw-r--r--   0        0        0      493 2021-11-24 23:24:20.248813 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/old.py
+-rw-r--r--   0        0        0        0 2021-11-24 14:24:48.644272 apc_temp_fetch-0.0.5/src/APC_Temp_fetch/py.typed
+-rw-r--r--   0        0        0     3656 1970-01-01 00:00:00.000000 apc_temp_fetch-0.0.5/PKG-INFO
```

### Comparing `APC-Temp-fetch-0.0.4/LICENSE.txt` & `apc_temp_fetch-0.0.5/LICENSE`

 * *Files 19% similar despite different names*

```diff
@@ -1,202 +1,68 @@
+Apache License
+Version 2.0, January 2004
+http://www.apache.org/licenses/
 
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
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+"License" shall mean the terms and conditions for use, reproduction, and distribution as defined by Sections 1 through 9 of this document.
+
+"Licensor" shall mean the copyright owner or entity authorized by the copyright owner that is granting the License.
+
+"Legal Entity" shall mean the union of the acting entity and all other entities that control, are controlled by, or are under common control with that entity. For the purposes of this definition, "control" means (i) the power, direct or indirect, to cause the direction or management of such entity, whether by contract or otherwise, or (ii) ownership of fifty percent (50%) or more of the outstanding shares, or (iii) beneficial ownership of such entity.
+
+"You" (or "Your") shall mean an individual or Legal Entity exercising permissions granted by this License.
+
+"Source" form shall mean the preferred form for making modifications, including but not limited to software source code, documentation source, and configuration files.
+
+"Object" form shall mean any form resulting from mechanical transformation or translation of a Source form, including but not limited to compiled object code, generated documentation, and conversions to other media types.
+
+"Work" shall mean the work of authorship, whether in Source or Object form, made available under the License, as indicated by a copyright notice that is included in or attached to the work (an example is provided in the Appendix below).
+
+"Derivative Works" shall mean any work, whether in Source or Object form, that is based on (or derived from) the Work and for which the editorial revisions, annotations, elaborations, or other modifications represent, as a whole, an original work of authorship. For the purposes of this License, Derivative Works shall not include works that remain separable from, or merely link (or bind by name) to the interfaces of, the Work and Derivative Works thereof.
+
+"Contribution" shall mean any work of authorship, including the original version of the Work and any modifications or additions to that Work or Derivative Works thereof, that is intentionally submitted to Licensor for inclusion in the Work by the copyright owner or by an individual or Legal Entity authorized to submit on behalf of the copyright owner. For the purposes of this definition, "submitted" means any form of electronic, verbal, or written communication sent to the Licensor or its representatives, including but not limited to communication on electronic mailing lists, source code control systems, and issue tracking systems that are managed by, or on behalf of, the Licensor for the purpose of discussing and improving the Work, but excluding communication that is conspicuously marked or otherwise designated in writing by the copyright owner as "Not a Contribution."
+
+"Contributor" shall mean Licensor and any individual or Legal Entity on behalf of whom a Contribution has been received by Licensor and subsequently incorporated within the Work.
+
+2. Grant of Copyright License.
+
+Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable copyright license to reproduce, prepare Derivative Works of, publicly display, publicly perform, sublicense, and distribute the Work and such Derivative Works in Source or Object form.
+
+3. Grant of Patent License.
+
+Subject to the terms and conditions of this License, each Contributor hereby grants to You a perpetual, worldwide, non-exclusive, no-charge, royalty-free, irrevocable (except as stated in this section) patent license to make, have made, use, offer to sell, sell, import, and otherwise transfer the Work, where such license applies only to those patent claims licensable by such Contributor that are necessarily infringed by their Contribution(s) alone or by combination of their Contribution(s) with the Work to which such Contribution(s) was submitted. If You institute patent litigation against any entity (including a cross-claim or counterclaim in a lawsuit) alleging that the Work or a Contribution incorporated within the Work constitutes direct or contributory patent infringement, then any patent licenses granted to You under this License for that Work shall terminate as of the date such litigation is filed.
+
+4. Redistribution.
+
+You may reproduce and distribute copies of the Work or Derivative Works thereof in any medium, with or without modifications, and in Source or Object form, provided that You meet the following conditions:
+
+    You must give any other recipients of the Work or Derivative Works a copy of this License; and
+    You must cause any modified files to carry prominent notices stating that You changed the files; and
+    You must retain, in the Source form of any Derivative Works that You distribute, all copyright, patent, trademark, and attribution notices from the Source form of the Work, excluding those notices that do not pertain to any part of the Derivative Works; and
+    If the Work includes a "NOTICE" text file as part of its distribution, then any Derivative Works that You distribute must include a readable copy of the attribution notices contained within such NOTICE file, excluding those notices that do not pertain to any part of the Derivative Works, in at least one of the following places: within a NOTICE text file distributed as part of the Derivative Works; within the Source form or documentation, if provided along with the Derivative Works; or, within a display generated by the Derivative Works, if and wherever such third-party notices normally appear. The contents of the NOTICE file are for informational purposes only and do not modify the License. You may add Your own attribution notices within Derivative Works that You distribute, alongside or as an addendum to the NOTICE text from the Work, provided that such additional attribution notices cannot be construed as modifying the License.
+
+You may add Your own copyright statement to Your modifications and may provide additional or different license terms and conditions for use, reproduction, or distribution of Your modifications, or for any such Derivative Works as a whole, provided Your use, reproduction, and distribution of the Work otherwise complies with the conditions stated in this License.
+
+5. Submission of Contributions.
+
+Unless You explicitly state otherwise, any Contribution intentionally submitted for inclusion in the Work by You to the Licensor shall be under the terms and conditions of this License, without any additional terms or conditions. Notwithstanding the above, nothing herein shall supersede or modify the terms of any separate license agreement you may have executed with Licensor regarding such Contributions.
+
+6. Trademarks.
+
+This License does not grant permission to use the trade names, trademarks, service marks, or product names of the Licensor, except as required for reasonable and customary use in describing the origin of the Work and reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty.
+
+Unless required by applicable law or agreed to in writing, Licensor provides the Work (and each Contributor provides its Contributions) on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied, including, without limitation, any warranties or conditions of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A PARTICULAR PURPOSE. You are solely responsible for determining the appropriateness of using or redistributing the Work and assume any risks associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability.
+
+In no event and under no legal theory, whether in tort (including negligence), contract, or otherwise, unless required by applicable law (such as deliberate and grossly negligent acts) or agreed to in writing, shall any Contributor be liable to You for damages, including any direct, indirect, special, incidental, or consequential damages of any character arising as a result of this License or out of the use or inability to use the Work (including but not limited to damages for loss of goodwill, work stoppage, computer failure or malfunction, or any and all other commercial damages or losses), even if such Contributor has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability.
+
+While redistributing the Work or Derivative Works thereof, You may choose to offer, and charge a fee for, acceptance of support, warranty, indemnity, or other liability obligations and/or rights consistent with this License. However, in accepting such obligations, You may act only on Your own behalf and on Your sole responsibility, not on behalf of any other Contributor, and only if You agree to indemnify, defend, and hold each Contributor harmless for any liability incurred by, or claims asserted against, such Contributor by reason of your accepting any such warranty or additional liability.
+
+END OF TERMS AND CONDITIONS
```

### Comparing `APC-Temp-fetch-0.0.4/PKG-INFO` & `apc_temp_fetch-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 Metadata-Version: 2.1
 Name: APC-Temp-fetch
-Version: 0.0.4
+Version: 0.0.5
 Summary: APC/Schneider UPS current temperature fetchers
-Home-page: https://github.com/YZITE/APC_Temp_fetch
-Author: Alain Zscheile
-Author-email: fogti+atf@ytrizja.de
-License: Apache-2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
+Author-email: Alain Zscheile <fogti+atf@ytrizja.de>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE.txt
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Dist: requests >=2.0
+Project-URL: Home, https://github.com/YZITE/APC_Temp_fetch
 
 # APC_Temp_fetch
 
 This python package provides an unified interface to several UPS
 network adapters with different firmware versions. It does not
 support guessing which interface to use; that wasn't necessary yet.
 
@@ -59,7 +56,8 @@
 If required, `--proxy <proxy_url>` can be added to the entry point command line
 to contact all API endpoints through the specified proxy.
 Note that this might require `pip3 install 'requests[socks]'` or
 on Gentoo `USE="socks5" emerge -v dev-python/requests` to work with SOCKS proxies.
 
 When using the python API, proxies can be specified in the `ApcKind.__init__(_, rqa)`
 `rqa` parameter (see Requests documentation, or the source code in `cli.py`)
+
```

### Comparing `APC-Temp-fetch-0.0.4/README.md` & `apc_temp_fetch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/base.py` & `apc_temp_fetch-0.0.5/src/APC_Temp_fetch/base.py`

 * *Files identical despite different names*

### Comparing `APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/cli.py` & `apc_temp_fetch-0.0.5/src/APC_Temp_fetch/cli.py`

 * *Files identical despite different names*

### Comparing `APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/cs121.py` & `apc_temp_fetch-0.0.5/src/APC_Temp_fetch/cs121.py`

 * *Files identical despite different names*

### Comparing `APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/cs141.py` & `apc_temp_fetch-0.0.5/src/APC_Temp_fetch/cs141.py`

 * *Files identical despite different names*

### Comparing `APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/frmnc.py` & `apc_temp_fetch-0.0.5/src/APC_Temp_fetch/frmnc.py`

 * *Files identical despite different names*

### Comparing `APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/frmnc666.py` & `apc_temp_fetch-0.0.5/src/APC_Temp_fetch/frmnc666.py`

 * *Files identical despite different names*

### Comparing `APC-Temp-fetch-0.0.4/src/APC_Temp_fetch/gden_nt07.py` & `apc_temp_fetch-0.0.5/src/APC_Temp_fetch/gden_nt07.py`

 * *Files identical despite different names*

