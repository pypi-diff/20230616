# Comparing `tmp/jaaql-monitor-1.2.64.tar.gz` & `tmp/jaaql-monitor-1.2.67.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.64.tar", last modified: Fri Jun  2 01:45:35 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.67.tar", last modified: Fri Jun 16 15:01:19 2023, max compression
```

## Comparing `jaaql-monitor-1.2.64.tar` & `jaaql-monitor-1.2.67.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 01:45:35.131842 jaaql-monitor-1.2.64/
--rw-rw-rw-   0        0        0    17736 2022-07-13 13:12:08.000000 jaaql-monitor-1.2.64/LICENSE.txt
--rw-rw-rw-   0        0        0     1475 2023-06-02 01:45:35.131842 jaaql-monitor-1.2.64/PKG-INFO
--rw-rw-rw-   0        0        0     1050 2023-04-25 20:11:51.000000 jaaql-monitor-1.2.64/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 01:45:35.127843 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1475 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-02 01:45:35.000000 jaaql-monitor-1.2.64/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-02 01:45:35.130842 jaaql-monitor-1.2.64/monitor/
--rw-rw-rw-   0        0        0        0 2023-04-25 20:19:29.000000 jaaql-monitor-1.2.64/monitor/__init__.py
--rw-rw-rw-   0        0        0    29060 2023-06-02 01:44:22.000000 jaaql-monitor-1.2.64/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-06-02 01:45:21.000000 jaaql-monitor-1.2.64/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-06-02 01:45:35.131842 jaaql-monitor-1.2.64/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-02 12:48:45.000000 jaaql-monitor-1.2.64/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-16 15:01:19.133139 jaaql-monitor-1.2.67/
+-rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.67/LICENSE.txt
+-rw-rw-rw-   0        0        0     1454 2023-06-16 15:01:19.133139 jaaql-monitor-1.2.67/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.67/README.md
+drwxrwxrwx   0        0        0        0 2023-06-16 15:01:19.133139 jaaql-monitor-1.2.67/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1454 2023-06-16 15:01:19.000000 jaaql-monitor-1.2.67/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-16 15:01:19.000000 jaaql-monitor-1.2.67/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-16 15:01:19.000000 jaaql-monitor-1.2.67/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-16 15:01:19.000000 jaaql-monitor-1.2.67/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-16 15:01:19.000000 jaaql-monitor-1.2.67/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-16 15:01:19.133139 jaaql-monitor-1.2.67/monitor/
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.67/monitor/__init__.py
+-rw-rw-rw-   0        0        0    31356 2023-06-16 14:59:07.000000 jaaql-monitor-1.2.67/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-06-16 15:01:11.000000 jaaql-monitor-1.2.67/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-06-16 15:01:19.133139 jaaql-monitor-1.2.67/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.67/setup.py
```

### Comparing `jaaql-monitor-1.2.64/LICENSE.txt` & `jaaql-monitor-1.2.67/LICENSE.txt`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,388 +1,388 @@
-“Commons Clause” License Condition v1.0
-
-The Software is provided to you by the Licensor under the License, as defined below, subject to the following condition.
-
-Without limiting other conditions in the License, the grant of rights under the License will not include, and the License does not grant to you, the right to Sell the Software.
-
-For purposes of the foregoing, “Sell” means practicing any or all of the rights granted to you under the License to provide to third parties, for a fee or other consideration (including without limitation fees for hosting or consulting/ support services related to the Software), a product or service whose value derives, entirely or substantially, from the functionality of the Software. Any license notice or attribution required by the License must also include this Commons Clause License Condition notice.
-
-Software: JAAQL-monitor
-
-License: Mozilla Public License Version 2.0 with Commons Clause
-
-Licensor: Software Quality Measurement and Improvement bv
-
-
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
-  defined by the Mozilla Public License, v. 2.0.
+“Commons Clause” License Condition v1.0
+
+The Software is provided to you by the Licensor under the License, as defined below, subject to the following condition.
+
+Without limiting other conditions in the License, the grant of rights under the License will not include, and the License does not grant to you, the right to Sell the Software.
+
+For purposes of the foregoing, “Sell” means practicing any or all of the rights granted to you under the License to provide to third parties, for a fee or other consideration (including without limitation fees for hosting or consulting/ support services related to the Software), a product or service whose value derives, entirely or substantially, from the functionality of the Software. Any license notice or attribution required by the License must also include this Commons Clause License Condition notice.
+
+Software: JAAQL-monitor
+
+License: Mozilla Public License Version 2.0 with Commons Clause
+
+Licensor: Software Quality Measurement and Improvement bv
+
+
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
+  defined by the Mozilla Public License, v. 2.0.
```

### Comparing `jaaql-monitor-1.2.64/PKG-INFO` & `jaaql-monitor-1.2.67/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.64
+Version: 1.2.67
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Usage
 JAAQL Monitor can be called as such
 
     jaaql_monitor.exe creds_file
@@ -32,8 +31,7 @@
 # Building
 To build you will need to have a python environment (3.8) setup locally. Building will produce a windows executable (the latest executable is in the repo if you require it). If you are on linux you can create an executable as well but you need to install python to do that so you might as well just use the python script. To build please run the commands below
 
     pyinstaller -F main.py
 
 # Running locally
 Please install requirements.txt. Using python 3.11
-
```

### Comparing `jaaql-monitor-1.2.64/README.md` & `jaaql-monitor-1.2.67/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-# Usage
-JAAQL Monitor can be called as such
-
-    jaaql_monitor.exe creds_file
-    
-Where creds_file is a file of the format
-
-    jaaql_url
-    username
-    password
-
-And as an example
-
-    jaaql.io
-    superjaaql
-    passw0rd
-
-Then it will accept input over standard input. Scripts can be separated via \p and \g. \p Will print everything in the standard input so far (since the last \g) and \g will submit everything in the standard input so far to jaaql (since the last \g). So \p\g will print and submit to jaaql. Any errors which we receive will be output on stdin and stderr
-
-# Building
-To build you will need to have a python environment (3.8) setup locally. Building will produce a windows executable (the latest executable is in the repo if you require it). If you are on linux you can create an executable as well but you need to install python to do that so you might as well just use the python script. To build please run the commands below
-
-    pyinstaller -F main.py
-
-# Running locally
+# Usage
+JAAQL Monitor can be called as such
+
+    jaaql_monitor.exe creds_file
+    
+Where creds_file is a file of the format
+
+    jaaql_url
+    username
+    password
+
+And as an example
+
+    jaaql.io
+    superjaaql
+    passw0rd
+
+Then it will accept input over standard input. Scripts can be separated via \p and \g. \p Will print everything in the standard input so far (since the last \g) and \g will submit everything in the standard input so far to jaaql (since the last \g). So \p\g will print and submit to jaaql. Any errors which we receive will be output on stdin and stderr
+
+# Building
+To build you will need to have a python environment (3.8) setup locally. Building will produce a windows executable (the latest executable is in the repo if you require it). If you are on linux you can create an executable as well but you need to install python to do that so you might as well just use the python script. To build please run the commands below
+
+    pyinstaller -F main.py
+
+# Running locally
 Please install requirements.txt. Using python 3.11
```

### Comparing `jaaql-monitor-1.2.64/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.67/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.64
+Version: 1.2.67
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Usage
 JAAQL Monitor can be called as such
 
     jaaql_monitor.exe creds_file
@@ -32,8 +31,7 @@
 # Building
 To build you will need to have a python environment (3.8) setup locally. Building will produce a windows executable (the latest executable is in the repo if you require it). If you are on linux you can create an executable as well but you need to install python to do that so you might as well just use the python script. To build please run the commands below
 
     pyinstaller -F main.py
 
 # Running locally
 Please install requirements.txt. Using python 3.11
-
```

### Comparing `jaaql-monitor-1.2.64/monitor/main.py` & `jaaql-monitor-1.2.67/monitor/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,697 +1,730 @@
-from monitor.version import print_version
-import sys
-import requests
-from sys import exit
-from getpass import getpass
-from inspect import getframeinfo, stack
-from datetime import datetime
-from base64 import urlsafe_b64encode as b64e, urlsafe_b64decode as b64d
-import os
-
-HEADER__security_bypass = "Authentication-Token-Bypass"
-HEADER__security_bypass_jaaql = "Authentication-Token-Bypass-Jaaql"
-HEADER__security = "Authentication-Token"
-MARKER__bypass = "bypass "
-MARKER__jaaql_bypass = "jaaql_bypass "
-
-ENDPOINT__oauth = "/oauth/token"
-ENDPOINT__submit = "/submit"
-ENDPOINT__attach = "/accounts"
-ENDPOINT__dispatchers = "/internal/dispatchers"
-ENDPOINT__wipe = "/internal/clean"
-ENDPOINT__freeze = "/internal/freeze"
-ENDPOINT__defrost = "/internal/defrost"
-
-COMMAND__initialiser = "\\"
-COMMAND__reset_short = "\\r"
-COMMAND__reset = "\\reset"
-COMMAND__go_short = "\g"
-COMMAND__go = "\go"
-COMMAND__print_short = "\p"
-COMMAND__print = "\print"
-COMMAND__wipe_dbms = "\wipe dbms"
-COMMAND__switch_jaaql_account_to = "\switch jaaql account to "
-COMMAND__connect_to_database = "\connect to database "
-COMMAND__register_jaaql_account_with = "\\register jaaql account with "
-COMMAND__attach_email_account = "\\attach email account "
-COMMAND__quit_short = "\q"
-COMMAND__quit = "\quit"
-COMMAND__freeze_instance = "\\freeze instance"
-COMMAND__defrost_instance = "\defrost instance"
-
-CONNECT_FOR_CREATEDB = " for createdb"
-
-DEFAULT_CONNECTION = "default"
-DEFAULT_EMAIL_ACCOUNT = "default"
-
-LINE_LENGTH_MAX = 115
-ROWS_MAX = 25
-
-METHOD__post = "POST"
-METHOD__get = "GET"
-
-ARGS__encoded_config = ['--encoded-config']
-ARGS__config = ['-c', '--config']
-ARGS__folder_config = ['-f', '--folder-config']
-ARGS__input_file = ['-i', '--input-file']
-ARGS__parameter = ['-p', '--parameter']
-ARGS__single_query = ['-s', '--single-query']
-ARGS__environment = ['-e', '--environment-file']
-
-
-class JAAQLMonitorException(Exception):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-
-class EOFMarker:
-    pass
-
-
-class ConnectionInfo:
-    def __init__(self, host, username, password, database, override_url = None):
-        self.host = host
-        self.username = username
-        self.password = password
-        self.database = database
-        self.oauth_token = None
-        self.override_url = override_url
-
-    def get_port(self):
-        return int(self.host.split(":")[1])
-
-    def get_host(self):
-        return self.host.split(":")[0]
-
-    def get_http_url(self):
-        if self.override_url is not None:
-            return self.override_url
-
-        formatted = self.host
-        if not formatted.startswith("http"):
-            url_input = "https://www." + formatted
-            if not url_input.endswith("/api"):
-                url_input += "/api"
-        if formatted.startswith("http") and ":6060" not in formatted and not formatted.endswith("/api"):
-            formatted += "/api"
-        return formatted
-
-
-class State:
-    def __init__(self):
-        self.was_go = False
-        self.fetched_query = ""
-        self.fetched_stdin = None
-        self.connections = {}
-        self.connection_info = {}
-        self._current_connection = None
-        self.fetched_database = None
-        self.is_verbose = False
-        self.single_query = False
-        self.is_debugging = False
-        self.file_name = None
-        self.cur_file_line = 0
-        self.file_lines = []
-        self.override_url = None
-        self.parameters = {}
-
-        self.do_exit = True
-
-        self.database_override = None
-        self.is_transactional = True
-
-    def set_current_connection(self, connection: ConnectionInfo):
-        self._current_connection = connection
-        self.database_override = None
-        self.is_transactional = True
-
-    def is_script(self):
-        return self.file_name is not None
-
-    def get_current_connection(self) -> ConnectionInfo:
-        if self._current_connection is None:
-            print_error(self, "There is no selected connection. Please supply a default connection or switch to a connection first")
-
-        return self._current_connection
-
-    def log(self, msg):
-        if self.is_verbose:
-            print(str(msg))
-
-    def _fetch_oauth_token_for_current_connection(self):
-        conn = self.get_current_connection()
-        try:
-            oauth_res = requests.post(conn.get_http_url() + ENDPOINT__oauth, json={
-                "username": conn.username,
-                "password": conn.password
-            })
-
-            if oauth_res.status_code != 200:
-                print_error(self, "Invalid credentials: response code " + str(oauth_res.status_code) + " content: " + oauth_res.text)
-                return None
-
-            conn.oauth_token = {HEADER__security: oauth_res.json()}
-        except requests.exceptions.RequestException:
-            print_error(self, "Could not connect to JAAQL running on " + conn.host + "\nPlease make sure that JAAQL is running and accessible")
-
-    def time_delta_ms(self, start_time: datetime, end_time: datetime) -> int:
-        return int(round((end_time - start_time).total_seconds() * 1000))
-
-    def request_handler(self, method, endpoint, send_json=None, handle_error: bool = True):
-        conn = self.get_current_connection()
-        if conn.oauth_token is None:
-            if conn.password.startswith(MARKER__bypass):
-                conn.oauth_token = {HEADER__security_bypass: conn.password.split(MARKER__bypass)[1]}
-            elif conn.password.startswith(MARKER__jaaql_bypass):
-                conn.oauth_token = {HEADER__security_bypass_jaaql: conn.password.split(MARKER__jaaql_bypass)[1]}
-            else:
-                self._fetch_oauth_token_for_current_connection()
-
-        start_time = datetime.now()
-        res = requests.request(method, conn.get_http_url() + endpoint, json=send_json, headers=conn.oauth_token)
-
-        if res.status_code == 401:
-            self.log("Refreshing oauth token")
-            self._fetch_oauth_token_for_current_connection()
-            start_time = datetime.now()
-            res = requests.request(method, conn.get_http_url() + endpoint, json=send_json, headers=conn.oauth_token)
-
-        self.log("Request took " + str(self.time_delta_ms(start_time, datetime.now())) + "ms")
-
-        if res.status_code == 200:
-            format_query_output(self, res.json())
-        else:
-            if handle_error:
-                if endpoint == ENDPOINT__submit:
-                    submit_error(self, res.text)
-                else:
-                    print_error(self, res.text)
-
-        return res
-
-
-def split_by_lines(split_str, gap=1):
-    split_str = split_str.split("".join(["\r\n"] * gap))
-    if len(split_str) == 1:
-        split_str = split_str[0].split("".join(["\n"] * gap))
-    return [s for s in split_str if len(s.strip()) != 0]
-
-
-def get_connection_info(state: State, connection_name: str = None, file_name: str = None):
-    if connection_name and connection_name in state.connection_info:
-        return state.connection_info[connection_name]
-    elif connection_name and connection_name in state.connections:
-        file_name = state.connections[connection_name]
-
-    if file_name is None and connection_name is None:
-        print_error(state, "Error in the python script. A connection is being fetched without a name or file")
-    elif file_name is None:
-        print_error(state, "No named connection: '" + connection_name + "'")
-
-    try:
-        config = open(file_name, "r").read()
-        config = split_by_lines(config)
-        host = config[0].strip()
-        username = config[1].strip()
-        password = config[2].strip()
-        database = None
-        if len(config) > 3:
-            database = config[3].strip()
-            if len(database) == 0:
-                database = None
-            else:
-                state.log("Found database '" + database + "'")
-
-        state.log("Successfully loaded config")
-
-        ci = ConnectionInfo(host, username, password, database, state.override_url)
-
-        if connection_name:
-            state.connection_info[connection_name] = ci
-
-        return ci
-    except FileNotFoundError:
-        if connection_name is None:
-            print_error(state, "Could not find credentials file located at '" + file_name + "', using working directory " + os.getcwd())
-        else:
-            print_error(state, "Could not find named credentials file '" + connection_name + "' located at '" + file_name +
-                        "', using working directory " + os.getcwd())
-
-
-def format_output_row(data, max_length, data_types, breaches):
-    builder = ""
-    for col, the_length, data_type, did_breach in zip(data, max_length, data_types, breaches):
-        col_str = str(col) if col is not None else "null"
-        builder += "|"
-        spacing = "".join([" "] * max(the_length - len(col_str), 0))
-        if did_breach and len(col_str) > the_length:
-            col_str = col_str[0:min(the_length, len(col_str)) - 3]
-            col_str += "..."
-        else:
-            col_str = col_str[0:min(the_length, len(col_str))]
-        if data_type == str:
-            builder += col_str + spacing
-        else:
-            builder += spacing + col_str
-    builder += "|"
-    return builder
-
-
-def format_output_divider(max_length):
-    builder = ""
-
-    for x in max_length:
-        builder += "+"
-        builder += "".join(["-"] * x)
-
-    builder += "+"
-    return builder
-
-
-def format_query_output(state, json_output):
-    if "rows" not in json_output:
-        return None
-    str_num_rows = "(" + str(len(json_output["rows"])) + " " + ("row" if len(json_output["rows"]) == 1 else "rows") + ")"
-
-    if len(json_output["rows"]) > 50:
-        state.log(str_num_rows)
-
-    max_length = []
-    types = []
-    first_pass = True
-    for row in json_output["rows"]:
-        for col, col_idx in zip(row, range(len(row))):
-            col_str = str(col)
-            if first_pass:
-                max_length.append(len(col_str))
-                types.append(type(col))
-            elif len(col_str) > max_length[col_idx]:
-                max_length[col_idx] = len(col_str)
-        first_pass = False
-
-    breaches = [False] * len(max_length)
-
-    while sum(max_length) + len(max_length) > LINE_LENGTH_MAX:
-        max_idx = 0
-        max_len = 0
-        for cur_len, col_idx in zip(max_length, range(len(max_length))):
-            if cur_len > max_len:
-                max_len = cur_len
-                max_idx = col_idx
-        breaches[max_idx] = True
-        max_length[max_idx] -= 1
-
-    if first_pass:
-        for col in json_output["columns"]:
-            max_length.append(len(col))
-
-    state.log(format_output_divider(max_length))
-    state.log(format_output_row(json_output["columns"], max_length, [str] * len(json_output["columns"]), [False] * len(max_length)))
-    state.log(format_output_divider(max_length))
-
-    if len(json_output["rows"]) > ROWS_MAX and not state.file_name:
-        json_output["rows"] = json_output["rows"][0:ROWS_MAX]
-        json_output["rows"].append(["..." for _ in json_output["columns"]])
-
-    for row in json_output["rows"]:
-        state.log(format_output_row(row, max_length, types, breaches))
-
-    if len(json_output["rows"]) != 0:
-        state.log(format_output_divider(max_length))
-
-    state.log(str_num_rows)
-
-
-def handle_login(state, jaaql_url: str = None):
-    load_file = False
-    username = None
-    password = None
-    if not jaaql_url:
-        jaaql_url = input("Jaaql Url: ")
-    elif jaaql_url.startswith("file "):
-        return get_connection_info(state, file_name=jaaql_url.split("file ")[1])
-
-    if not load_file:
-        username = input("Username: ").strip()
-        password = getpass(prompt='Password: ', stream=None)
-
-    return ConnectionInfo(jaaql_url, username, password, None, state.override_url)
-
-
-def dump_buffer(state, start: str = "\n\n"):
-    return ("%sBuffer [" % start) + str(len(state.fetched_query.strip())) + "]:\n" + state.fetched_query.strip() + "\n\n"
-
-
-def get_message(state, err, line_offset, buffer, additional_line_message: str = ""):
-    caller = getframeinfo(stack()[1][0])
-    file_message = ""
-    if state.file_name is not None:
-        file_message = "Error on " + additional_line_message + "line %d of file '%s':\n\n" % (state.cur_file_line - line_offset, state.file_name)
-    debug_message = " [%s:%d]" % (caller.filename, caller.lineno)
-    if not state.is_script() or not state.is_debugging:
-        debug_message = ""
-    buffer = "\n" + buffer
-    if not state.is_script():
-        buffer = ""
-
-    print(file_message + err + debug_message + buffer, file=sys.stderr)
-    if state.is_script():
-        if state.do_exit:
-            exit(1)
-        else:
-            raise JAAQLMonitorException(file_message + err + debug_message + buffer)
-
-
-def submit_error(state, err, line_offset: int = 0):
-    divided_lines = [line for line in [err_line.strip() for err_line in err.split("\n")]]
-    lines_with_line_number = [line for line in divided_lines if line.startswith("LINE ")]
-    marker_lines = [line for line in [err_line for err_line in err.split("\n")] if line.strip() == "^"]
-
-    print_buffer = dump_buffer(state, "")
-    if len(lines_with_line_number) != 0:
-        line_err_num = int(lines_with_line_number[0].split("LINE ")[1].split(":")[0])
-        state.cur_file_line = line_err_num
-        buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
-        start_line_num = max(0, line_err_num - 10) + 1
-        end_line_num = min(line_err_num, len(buffer_lines)) + 1
-        buffer_lines = buffer_lines[start_line_num - 1:end_line_num - 1]
-
-        marker_line = marker_lines[0]
-        marker_line = marker_line[lines_with_line_number[0].index(":"):]
-        marker_line = "     " + marker_line
-
-        err = "\n".join(err.replace("\r\n", "\n").split("\n")[:-4])
-
-        buffer_lines = [str(start_line_num + idx).rjust(5, '0') + "> " +
-                        (line + "\n" + marker_line + "\n" + err if start_line_num + idx == line_err_num else line)
-                        for idx, line in zip(range(len(buffer_lines)), buffer_lines)]
-
-        err = "\\<b>" + err + "\\</b>\n\n" + "\n".join(buffer_lines)
-        err = err + "\n\n"
-    get_message(state, err, line_offset, print_buffer)
-
-
-def print_error(state, err, line_offset: int = 0):
-    get_message(state, err, line_offset, dump_buffer(state, ""))
-
-
-def freeze_defrost_instance(state: State, freeze: bool):
-    endpoint = ENDPOINT__freeze if freeze else ENDPOINT__defrost
-    verb = "freezing" if freeze else "defrosting"
-    res = state.request_handler(METHOD__post, endpoint, handle_error=False)
-
-    if res.status_code != 200:
-        print_error(state, "Error " + verb + " jaaql box, received status code %d and message:\n\n\t%s" % (res.status_code, res.text))
-
-
-def wipe_jaaql_box(state: State):
-    res = state.request_handler(METHOD__post, ENDPOINT__wipe, handle_error=False)
-
-    if res.status_code != 200:
-        print_error(state, "Error wiping jaaql box, received status code %d and message:\n\n\t%s" % (res.status_code, res.text))
-
-
-def attach_email_account(state, application: str, dispatcher_name: str, credentials_name: str, connection_info: ConnectionInfo):
-    res = state.request_handler(METHOD__post, ENDPOINT__dispatchers, send_json={
-        "application": application,
-        "name": dispatcher_name,
-        "url": connection_info.get_host(),
-        "port": connection_info.get_port(),
-        "username": connection_info.username,
-        "password": connection_info.password
-    }, handle_error=False)
-
-    if res.status_code != 200:
-        print_error(state, "Error attaching email account '%s' to dispatcher '%s', received status code %d and message:\n\n\t%s" %
-                    (credentials_name, dispatcher_name, res.status_code, res.text))
-
-
-def register_jaaql_account(state, credentials_name: str, connection_info: ConnectionInfo):
-    res = state.request_handler(METHOD__post, ENDPOINT__attach, send_json={
-        "username": connection_info.username,
-        "password": connection_info.password,
-        "attach_as": connection_info.username
-    }, handle_error=False)
-
-    if res.status_code != 200:
-        print_error(state, "Error registering jaaql account '%s' with username '%s', received status code %d and message:\n\n\t%s" %
-                    (credentials_name, connection_info.username, res.status_code, res.text))
-
-
-def on_go(state):
-    for parameter, value in state.parameters.items():
-        state.fetched_query = state.fetched_query.replace("{{" + parameter + "}}", value)
-
-    send_json = {"query": state.fetched_query}
-    cur_conn = state.get_current_connection()
-    if cur_conn.database is not None:
-        send_json["database"] = cur_conn.database
-    if state.database_override is not None:
-        send_json["database"] = state.database_override
-    if not state.is_transactional:
-        send_json["autocommit"] = True
-
-    state.request_handler(METHOD__post, ENDPOINT__submit, send_json=send_json)
-
-    state.fetched_query = ""
-
-
-def parse_user_printing_any_errors(state, potential_user, allow_spaces: bool = False):
-    if " " in potential_user and not allow_spaces:
-        print_error(state, "Expected user without spaces, instead found spaces in user: '" + potential_user + "'")
-    if not potential_user.startswith("@"):
-        print_error(state, "Malformatted user, expected user to start with @")
-
-    return potential_user.split("@")[1].split(" ")[0]
-
-
-def deal_with_input(state: State, file_content: str = None):
-    if len(state.connections) == 0 and state.is_script():
-        print_error(state, "Must supply credentials file as argument in script mode")
-    if len(state.connections) != 0 and state.connections.get(DEFAULT_CONNECTION):
-        state.set_current_connection(get_connection_info(state, DEFAULT_CONNECTION))  # Preloads the default connection
-    elif not state.is_script():
-        print(state, "Type jaaql url or \"file [config_file_location]\"")
-        state.set_current_connection(handle_login(state, input("LOGIN>").strip()))
-
-    if state.is_script():
-        try:
-            if file_content:
-                state.file_lines = [line + "\n" for line in file_content.replace("\r\n", "\n").split("\n")]
-            else:
-                state.file_lines = open(state.file_name, "r").readlines()
-            state.file_lines.append(EOFMarker())  # Ignore warning. We can have multiple types. This is python
-        except FileNotFoundError as ex:
-            print_error(state, "Could not load file for processing '" + state.file_name + "'")
-        except Exception as ex:
-            print_error(state, "Unhandled exception whilst processing file '" + state.file_name + "' " + str(ex))
-
-    while True:
-        fetched_line = None
-        try:
-            if len(state.file_lines) != 0:
-                fetched_line = state.file_lines[0]
-                state.cur_file_line += 1
-                state.file_lines = state.file_lines[1:]
-                if isinstance(fetched_line, EOFMarker):
-                    raise EOFError()
-        except EOFError:
-            break
-
-        if fetched_line.startswith(COMMAND__initialiser):
-            fetched_line = fetched_line.strip()  # Ignore the line terminator e.g. \r\n
-            if fetched_line == COMMAND__go or fetched_line == COMMAND__go_short:
-                on_go(state)
-            elif fetched_line == COMMAND__reset or fetched_line == COMMAND__reset_short:
-                state.fetched_query = ""
-            elif fetched_line == COMMAND__print or fetched_line == COMMAND__print_short:
-                dump_buffer(state)
-            elif fetched_line == COMMAND__freeze_instance:
-                freeze_defrost_instance(state, freeze=True)
-            elif fetched_line == COMMAND__defrost_instance:
-                freeze_defrost_instance(state, freeze=False)
-            elif len(state.fetched_query.strip()) != 0:
-                print_error(state, "Tried to execute the command '" + fetched_line + "' but buffer was non empty.")
-            elif fetched_line == COMMAND__wipe_dbms:
-                wipe_jaaql_box(state)
-            elif fetched_line.startswith(COMMAND__switch_jaaql_account_to):
-                candidate_connection_name = fetched_line.split(COMMAND__switch_jaaql_account_to)[1]
-                connection_name = parse_user_printing_any_errors(state, candidate_connection_name)
-                state.set_current_connection(get_connection_info(state, connection_name=connection_name))
-            elif fetched_line.startswith(COMMAND__connect_to_database):
-                candidate_database = fetched_line.split(COMMAND__connect_to_database)[1].split(" ")[0]
-                if fetched_line.endswith(CONNECT_FOR_CREATEDB):
-                    state.is_transactional = False
-
-                state.database_override = candidate_database.split(CONNECT_FOR_CREATEDB)[0]
-            elif fetched_line.startswith(COMMAND__register_jaaql_account_with):
-                candidate_connection_name = fetched_line.split(COMMAND__register_jaaql_account_with)[1]
-                connection_name = parse_user_printing_any_errors(state, candidate_connection_name)
-
-                register_jaaql_account(state, connection_name, get_connection_info(state, connection_name=connection_name))
-            elif fetched_line.startswith(COMMAND__attach_email_account):
-                candidate_connection_name = fetched_line.split(COMMAND__attach_email_account)[1]
-                connection_name = parse_user_printing_any_errors(state, candidate_connection_name, allow_spaces=True)
-                if " to " not in candidate_connection_name:
-                    print_error(state, "Expected token 'to' after dispatcher credentials file e.g. " +
-                                COMMAND__attach_email_account + "@dispatcher to app.dispatcher_name")
-                if candidate_connection_name.endswith(" to "):
-                    print_error(state, "Expected fully qualified dispatcher after ' to ' e.g. " +
-                                COMMAND__attach_email_account + "@dispatcher to app.dispatcher_name")
-                dispatcher_fqn = candidate_connection_name.split(" to ")[1]
-                dispatcher_fqn_split = dispatcher_fqn.split(".")
-                if len(dispatcher_fqn_split) != 2:
-                    print_error(state, "Badly formatted dispatcher name. Must be of the format 'app.dispatcher_name'. Received '%s'" % dispatcher_fqn)
-
-                attach_email_account(state, dispatcher_fqn_split[0], dispatcher_fqn_split[1], connection_name,
-                                     get_connection_info(state, connection_name=connection_name))
-            elif fetched_line == COMMAND__quit or fetched_line == COMMAND__quit_short:
-                break
-            else:
-                print_error(state, "Unrecognised command '" + fetched_line + "'")
-        else:
-            if len(state.fetched_query.strip()) != 0 or len(fetched_line.strip()) != 0:
-                state.fetched_query += fetched_line  # Do not pre-append things with empty lines
-
-            if fetched_line.strip().endswith(COMMAND__go_short):
-                state.fetched_query = state.fetched_query[:-(len(COMMAND__go_short) + 1)]
-                on_go(state)
-
-    if len(state.fetched_query) != 0:
-        if state.single_query:
-            on_go(state)
-        else:
-            print_error(state, "Attempting to quit with non-empty buffer. Please submit with \\g or clear with \\r")
-
-
-def initialise_from_args(args, file_name: str = None, file_content: str = None, do_exit: bool = True, override_url: str = None):
-    state = State()
-    state.do_exit = do_exit
-
-    if file_name is None:
-        file_name = [idx for arg, idx in zip(args, range(len(args))) if arg in ARGS__input_file]
-        if len(file_name) != 0:
-            state.file_name = args[file_name[0] + 1]
-    else:
-        state.file_name = file_name
-
-    state.override_url = override_url
-
-    state.is_verbose = len([arg for arg in args if arg in ['-v', '--verbose']]) != 0
-    state.is_debugging = len([arg for arg in args if arg in ['-d', '--debugging']]) != 0
-    state.single_query = len([arg for arg in args if arg in ARGS__single_query]) != 0
-
-    if state.is_verbose:
-        print_version()
-
-    for arg, arg_idx in zip(args, range(len(args))):
-        if arg not in ARGS__parameter:
-            continue
-
-        if arg_idx == len(args) - 1:
-            print_error(state, "The parameter flag is the last argument. You need to supply a parameter name")
-
-        if arg_idx == len(args) - 2:
-            print_error(state, "The parameter name is the last argument. You need to supply a parameter value")
-
-        parameter_name = args[arg_idx + 1]
-        parameter_value = args[arg_idx + 2]
-
-        if parameter_name in state.parameters:
-            print_error(state, "The parameter '" + parameter_name + "' has already been supplied")
-
-        state.parameters[parameter_name] = parameter_value
-
-    for arg, arg_idx in zip(args, range(len(args))):
-        if arg not in ARGS__environment:
-            continue
-
-        if arg_idx == len(args) - 1:
-            print_error(state, "The environment flag is the last argument. You need to supply a file")
-
-        parameter_file = args[arg_idx + 1]
-
-        for line in open(parameter_file, "r").readlines():
-            state.parameters[line.split("=")[0]] = "=".join(line.split("=")[1:])
-
-    for arg, arg_idx in zip(args, range(len(args))):
-        if arg not in ARGS__folder_config:
-            continue
-
-        if arg_idx == len(args) - 1:
-            print_error(state, "The folder config flag is the last argument. You need to supply a file")
-
-        configuration_folder = args[arg_idx + 1]
-
-        for config_file in os.listdir(configuration_folder):
-            full_file_name = os.path.join(configuration_folder, config_file)
-            if config_file.endswith(".email-credentials.txt"):
-                configuration_name = config_file[0:-len(".email.credentials.txt")]
-            elif config_file.endswith(".credentials.txt"):
-                configuration_name = config_file[0:-len(".credentials.txt")]
-            else:
-                raise JAAQLMonitorException("Unrecognised file extension for file " + full_file_name)
-
-            if configuration_name in state.connections:
-                print_error(state, "The configuration with name '" + configuration_name + "' already exists")
-
-            state.connections[configuration_name] = full_file_name
-
-    for arg, arg_idx in zip(args, range(len(args))):
-        if arg not in ARGS__encoded_config and arg not in ARGS__config:
-            continue
-
-        if arg_idx == len(args) - 1:
-            print_error(state, "The config flag is the last argument. You need to supply a file")
-
-        configuration_name = args[arg_idx + 1]
-        candidate_content_or_file_name = None
-        if arg_idx < len(args) - 2:
-            candidate_content_or_file_name = args[arg_idx + 2]
-
-        # The following branch of logic will use the supplied configuration name as the file name and set the configuration name to default
-        if candidate_content_or_file_name is None or candidate_content_or_file_name.startswith("<") or candidate_content_or_file_name.startswith("-"):
-            candidate_content_or_file_name = configuration_name
-            configuration_name = DEFAULT_CONNECTION
-
-        if configuration_name in state.connections:
-            print_error(state, "The configuration with name '" + configuration_name + "' already exists")
-
-        state.connections[configuration_name] = candidate_content_or_file_name
-
-        if arg in ARGS__encoded_config:
-            content_split = candidate_content_or_file_name.split(":")
-
-            db = None
-            if len(content_split) == 4:
-                db = b64d(content_split[3]).decode()
-
-            state.connection_info[configuration_name] = ConnectionInfo(b64d(content_split[0]).decode(), b64d(content_split[1]).decode(),
-                                                                       b64d(content_split[2]).decode(), db, state.override_url)
-
-    deal_with_input(state, file_content)
-
-
-def initialise(file_name: str, file_content: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]],
-               override_url: str):
-    args = [ARGS__single_query[0]]
-
-    for config in configs:
-        args.append(ARGS__config[0])
-        args.append(config[0])
-        args.append(config[1])
-
-    for encoded_config in encoded_configs:
-        args.append(ARGS__encoded_config[0])
-        args.append(encoded_config[0])
-        db_part = ""
-        if encoded_config[4]:
-            db_part = ":" + b64e(encoded_config[4].encode()).decode()
-        args.append(b64e(encoded_config[1].encode()).decode() + ":" + b64e(encoded_config[2].encode()).decode() + ":" +
-                    b64e(encoded_config[3].encode()).decode() + db_part)
-
-    initialise_from_args(args, file_name, file_content, False, override_url)
-
-
-if __name__ == "__main__":
-    initialise_from_args(sys.argv[1:])
+import traceback
+from json import JSONDecodeError
+
+from monitor.version import print_version
+import sys
+import requests
+from sys import exit
+from getpass import getpass
+from inspect import getframeinfo, stack
+from datetime import datetime
+from base64 import urlsafe_b64encode as b64e, urlsafe_b64decode as b64d
+import os
+import json
+
+HEADER__security_bypass = "Authentication-Token-Bypass"
+HEADER__security_bypass_jaaql = "Authentication-Token-Bypass-Jaaql"
+HEADER__security = "Authentication-Token"
+MARKER__bypass = "bypass "
+MARKER__jaaql_bypass = "jaaql_bypass "
+
+ENDPOINT__oauth = "/oauth/token"
+ENDPOINT__submit = "/submit"
+ENDPOINT__attach = "/accounts"
+ENDPOINT__dispatchers = "/internal/dispatchers"
+ENDPOINT__wipe = "/internal/clean"
+ENDPOINT__freeze = "/internal/freeze"
+ENDPOINT__defrost = "/internal/defrost"
+
+COMMAND__initialiser = "\\"
+COMMAND__reset_short = "\\r"
+COMMAND__reset = "\\reset"
+COMMAND__go_short = "\\g"
+COMMAND__go = "\\go"
+COMMAND__print_short = "\\p"
+COMMAND__print = "\\print"
+COMMAND__wipe_dbms = "\\wipe dbms"
+COMMAND__switch_jaaql_account_to = "\\switch jaaql account to "
+COMMAND__connect_to_database = "\\connect to database "
+COMMAND__register_jaaql_account_with = "\\register jaaql account with "
+COMMAND__attach_email_account = "\\attach email account "
+COMMAND__quit_short = "\\q"
+COMMAND__quit = "\\quit"
+COMMAND__freeze_instance = "\\freeze instance"
+COMMAND__defrost_instance = "\\defrost instance"
+COMMAND__with_parameters = "WITH PARAMETERS {"
+
+CONNECT_FOR_CREATEDB = " for createdb"
+
+DEFAULT_CONNECTION = "default"
+DEFAULT_EMAIL_ACCOUNT = "default"
+
+LINE_LENGTH_MAX = 115
+ROWS_MAX = 25
+
+METHOD__post = "POST"
+METHOD__get = "GET"
+
+ARGS__encoded_config = ['--encoded-config']
+ARGS__config = ['-c', '--config']
+ARGS__folder_config = ['-f', '--folder-config']
+ARGS__input_file = ['-i', '--input-file']
+ARGS__parameter = ['-p', '--parameter']
+ARGS__single_query = ['-s', '--single-query']
+ARGS__environment = ['-e', '--environment-file']
+
+
+class JAAQLMonitorException(Exception):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+
+class EOFMarker:
+    pass
+
+
+class ConnectionInfo:
+    def __init__(self, host, username, password, database, override_url=None):
+        self.host = host
+        self.username = username
+        self.password = password
+        self.database = database
+        self.oauth_token = None
+        self.override_url = override_url
+
+    def get_port(self):
+        return int(self.host.split(":")[1])
+
+    def get_host(self):
+        return self.host.split(":")[0]
+
+    def get_http_url(self):
+        if self.override_url is not None:
+            return self.override_url
+
+        formatted = self.host
+        if not formatted.startswith("http"):
+            url_input = "https://www." + formatted
+            if not url_input.endswith("/api"):
+                url_input += "/api"
+        if formatted.startswith("http") and ":6060" not in formatted and not formatted.endswith("/api"):
+            formatted += "/api"
+        return formatted
+
+
+class State:
+    def __init__(self):
+        self.was_go = False
+        self.fetched_query = ""
+        self.fetched_stdin = None
+        self.connections = {}
+        self.connection_info = {}
+        self._current_connection = None
+        self.fetched_database = None
+        self.is_verbose = False
+        self.single_query = False
+        self.is_debugging = False
+        self.file_name = None
+        self.cur_file_line = 0
+        self.file_lines = []
+        self.override_url = None
+        self.parameters = {}
+        self.query_parameters = None
+        self.reading_parameters = False
+
+        self.do_exit = True
+
+        self.database_override = None
+        self.is_transactional = True
+
+    def set_current_connection(self, connection: ConnectionInfo):
+        self._current_connection = connection
+        self.database_override = None
+        self.is_transactional = True
+
+    def is_script(self):
+        return self.file_name is not None
+
+    def get_current_connection(self) -> ConnectionInfo:
+        if self._current_connection is None:
+            print_error(self, "There is no selected connection. Please supply a default connection or switch to a connection first")
+
+        return self._current_connection
+
+    def log(self, msg):
+        if self.is_verbose:
+            print(str(msg))
+
+    def _fetch_oauth_token_for_current_connection(self):
+        conn = self.get_current_connection()
+        try:
+            oauth_res = requests.post(conn.get_http_url() + ENDPOINT__oauth, json={
+                "username": conn.username,
+                "password": conn.password
+            })
+
+            if oauth_res.status_code != 200:
+                print_error(self, "Invalid credentials: response code " + str(oauth_res.status_code) + " content: " + oauth_res.text +
+                            " for username '" + conn.username + "'")
+                return None
+
+            conn.oauth_token = {HEADER__security: oauth_res.json()}
+        except requests.exceptions.RequestException:
+            print_error(self, "Could not connect to JAAQL running on " + conn.host + "\nPlease make sure that JAAQL is running and accessible")
+
+    def time_delta_ms(self, start_time: datetime, end_time: datetime) -> int:
+        return int(round((end_time - start_time).total_seconds() * 1000))
+
+    def request_handler(self, method, endpoint, send_json=None, handle_error: bool = True):
+        conn = self.get_current_connection()
+        if conn.oauth_token is None:
+            if conn.password.startswith(MARKER__bypass):
+                conn.oauth_token = {HEADER__security_bypass: conn.password.split(MARKER__bypass)[1]}
+            elif conn.password.startswith(MARKER__jaaql_bypass):
+                conn.oauth_token = {HEADER__security_bypass_jaaql: conn.password.split(MARKER__jaaql_bypass)[1]}
+            else:
+                self._fetch_oauth_token_for_current_connection()
+
+        start_time = datetime.now()
+        res = requests.request(method, conn.get_http_url() + endpoint, json=send_json, headers=conn.oauth_token)
+
+        if res.status_code == 401:
+            self.log("Refreshing oauth token")
+            self._fetch_oauth_token_for_current_connection()
+            start_time = datetime.now()
+            res = requests.request(method, conn.get_http_url() + endpoint, json=send_json, headers=conn.oauth_token)
+
+        self.log("Request took " + str(self.time_delta_ms(start_time, datetime.now())) + "ms")
+
+        if res.status_code == 200:
+            format_query_output(self, res.json())
+        else:
+            if handle_error:
+                if endpoint == ENDPOINT__submit:
+                    submit_error(self, res.text)
+                else:
+                    print_error(self, res.text)
+
+        return res
+
+
+def split_by_lines(split_str, gap=1):
+    split_str = split_str.split("".join(["\r\n"] * gap))
+    if len(split_str) == 1:
+        split_str = split_str[0].split("".join(["\n"] * gap))
+    return [s for s in split_str if len(s.strip()) != 0]
+
+
+def get_connection_info(state: State, connection_name: str = None, file_name: str = None):
+    if connection_name and connection_name in state.connection_info:
+        return state.connection_info[connection_name]
+    elif connection_name and connection_name in state.connections:
+        file_name = state.connections[connection_name]
+
+    if file_name is None and connection_name is None:
+        print_error(state, "Error in the python script. A connection is being fetched without a name or file")
+    elif file_name is None:
+        print_error(state, "No named connection: '" + connection_name + "'")
+
+    try:
+        config = open(file_name, "r").read()
+        config = split_by_lines(config)
+        host = config[0].strip()
+        username = config[1].strip()
+        password = config[2].strip()
+        database = None
+        if len(config) > 3:
+            database = config[3].strip()
+            if len(database) == 0:
+                database = None
+            else:
+                state.log("Found database '" + database + "'")
+
+        state.log("Successfully loaded config")
+
+        ci = ConnectionInfo(host, username, password, database, state.override_url)
+
+        if connection_name:
+            state.connection_info[connection_name] = ci
+
+        return ci
+    except FileNotFoundError:
+        if connection_name is None:
+            print_error(state, "Could not find credentials file located at '" + file_name + "', using working directory " + os.getcwd())
+        else:
+            print_error(state, "Could not find named credentials file '" + connection_name + "' located at '" + file_name +
+                        "', using working directory " + os.getcwd())
+    except Exception:
+        traceback.print_exc()
+        print_error(state, "Could not load the credential file '" + connection_name + "'. Is the file formatted correctly?")
+
+
+def format_output_row(data, max_length, data_types, breaches):
+    builder = ""
+    for col, the_length, data_type, did_breach in zip(data, max_length, data_types, breaches):
+        col_str = str(col) if col is not None else "null"
+        builder += "|"
+        spacing = "".join([" "] * max(the_length - len(col_str), 0))
+        if did_breach and len(col_str) > the_length:
+            col_str = col_str[0:min(the_length, len(col_str)) - 3]
+            col_str += "..."
+        else:
+            col_str = col_str[0:min(the_length, len(col_str))]
+        if data_type == str:
+            builder += col_str + spacing
+        else:
+            builder += spacing + col_str
+    builder += "|"
+    return builder
+
+
+def format_output_divider(max_length):
+    builder = ""
+
+    for x in max_length:
+        builder += "+"
+        builder += "".join(["-"] * x)
+
+    builder += "+"
+    return builder
+
+
+def format_query_output(state, json_output):
+    if "rows" not in json_output:
+        return None
+    str_num_rows = "(" + str(len(json_output["rows"])) + " " + ("row" if len(json_output["rows"]) == 1 else "rows") + ")"
+
+    if len(json_output["rows"]) > 50:
+        state.log(str_num_rows)
+
+    max_length = []
+    types = []
+    first_pass = True
+    for row in json_output["rows"]:
+        for col, col_idx in zip(row, range(len(row))):
+            col_str = str(col)
+            if first_pass:
+                max_length.append(len(col_str))
+                types.append(type(col))
+            elif len(col_str) > max_length[col_idx]:
+                max_length[col_idx] = len(col_str)
+        first_pass = False
+
+    breaches = [False] * len(max_length)
+
+    while sum(max_length) + len(max_length) > LINE_LENGTH_MAX:
+        max_idx = 0
+        max_len = 0
+        for cur_len, col_idx in zip(max_length, range(len(max_length))):
+            if cur_len > max_len:
+                max_len = cur_len
+                max_idx = col_idx
+        breaches[max_idx] = True
+        max_length[max_idx] -= 1
+
+    if first_pass:
+        for col in json_output["columns"]:
+            max_length.append(len(col))
+
+    state.log(format_output_divider(max_length))
+    state.log(format_output_row(json_output["columns"], max_length, [str] * len(json_output["columns"]), [False] * len(max_length)))
+    state.log(format_output_divider(max_length))
+
+    if len(json_output["rows"]) > ROWS_MAX and not state.file_name:
+        json_output["rows"] = json_output["rows"][0:ROWS_MAX]
+        json_output["rows"].append(["..." for _ in json_output["columns"]])
+
+    for row in json_output["rows"]:
+        state.log(format_output_row(row, max_length, types, breaches))
+
+    if len(json_output["rows"]) != 0:
+        state.log(format_output_divider(max_length))
+
+    state.log(str_num_rows)
+
+
+def handle_login(state, jaaql_url: str = None):
+    load_file = False
+    username = None
+    password = None
+    if not jaaql_url:
+        jaaql_url = input("Jaaql Url: ")
+    elif jaaql_url.startswith("file "):
+        return get_connection_info(state, file_name=jaaql_url.split("file ")[1])
+
+    if not load_file:
+        username = input("Username: ").strip()
+        password = getpass(prompt='Password: ', stream=None)
+
+    return ConnectionInfo(jaaql_url, username, password, None, state.override_url)
+
+
+def dump_buffer(state, start: str = "\n\n"):
+    return ("%sBuffer [" % start) + str(len(state.fetched_query.strip())) + "]:\n" + state.fetched_query.strip() + "\n\n"
+
+
+def get_message(state, err, line_offset, buffer, additional_line_message: str = ""):
+    caller = getframeinfo(stack()[1][0])
+    file_message = ""
+    if state.file_name is not None:
+        file_message = "Error on " + additional_line_message + "line %d of file '%s':\n\n" % (state.cur_file_line - line_offset, state.file_name)
+    debug_message = " [%s:%d]" % (caller.filename, caller.lineno)
+    if not state.is_script() or not state.is_debugging:
+        debug_message = ""
+    buffer = "\n" + buffer
+    if not state.is_script():
+        buffer = ""
+
+    print(file_message + err + debug_message + buffer, file=sys.stderr)
+    if state.is_script():
+        if state.do_exit:
+            exit(1)
+        else:
+            raise JAAQLMonitorException(file_message + err + debug_message + buffer)
+
+
+def submit_error(state, err, line_offset: int = 0):
+    divided_lines = [line for line in [err_line.strip() for err_line in err.split("\n")]]
+    lines_with_line_number = [line for line in divided_lines if line.startswith("LINE ")]
+    marker_lines = [line for line in [err_line for err_line in err.split("\n")] if line.strip() == "^"]
+
+    print_buffer = dump_buffer(state, "")
+    if len(lines_with_line_number) != 0:
+        line_err_num = int(lines_with_line_number[0].split("LINE ")[1].split(":")[0])
+        state.cur_file_line = line_err_num
+        buffer_lines = state.fetched_query.strip().replace("\r\n", "\n").split("\n")
+        start_line_num = max(0, line_err_num - 10) + 1
+        end_line_num = min(line_err_num, len(buffer_lines)) + 1
+        buffer_lines = buffer_lines[start_line_num - 1:end_line_num - 1]
+
+        marker_line = marker_lines[0]
+        marker_line = marker_line[lines_with_line_number[0].index(":"):]
+        marker_line = "     " + marker_line
+
+        err = "\n".join(err.replace("\r\n", "\n").split("\n")[:-4])
+
+        buffer_lines = [str(start_line_num + idx).rjust(5, '0') + "> " +
+                        (line + "\n" + marker_line + "\n" + err if start_line_num + idx == line_err_num else line)
+                        for idx, line in zip(range(len(buffer_lines)), buffer_lines)]
+
+        err = "\\<b>" + err + "\\</b>\n\n" + "\n".join(buffer_lines)
+        err = err + "\n\n"
+    get_message(state, err, line_offset, print_buffer)
+
+
+def print_error(state, err, line_offset: int = 0):
+    get_message(state, err, line_offset, dump_buffer(state, ""))
+
+
+def freeze_defrost_instance(state: State, freeze: bool):
+    endpoint = ENDPOINT__freeze if freeze else ENDPOINT__defrost
+    verb = "freezing" if freeze else "defrosting"
+    res = state.request_handler(METHOD__post, endpoint, handle_error=False)
+
+    if res.status_code != 200:
+        print_error(state, "Error " + verb + " jaaql box, received status code %d and message:\n\n\t%s" % (res.status_code, res.text))
+
+
+def wipe_jaaql_box(state: State):
+    res = state.request_handler(METHOD__post, ENDPOINT__wipe, handle_error=False)
+
+    if res.status_code != 200:
+        print_error(state, "Error wiping jaaql box, received status code %d and message:\n\n\t%s" % (res.status_code, res.text))
+
+
+def attach_email_account(state, application: str, dispatcher_name: str, credentials_name: str, connection_info: ConnectionInfo):
+    res = state.request_handler(METHOD__post, ENDPOINT__dispatchers, send_json={
+        "application": application,
+        "name": dispatcher_name,
+        "url": connection_info.get_host(),
+        "port": connection_info.get_port(),
+        "username": connection_info.username,
+        "password": connection_info.password
+    }, handle_error=False)
+
+    if res.status_code != 200:
+        print_error(state, "Error attaching email account '%s' to dispatcher '%s', received status code %d and message:\n\n\t%s" %
+                    (credentials_name, dispatcher_name, res.status_code, res.text))
+
+
+def register_jaaql_account(state, credentials_name: str, connection_info: ConnectionInfo):
+    res = state.request_handler(METHOD__post, ENDPOINT__attach, send_json={
+        "username": connection_info.username,
+        "password": connection_info.password,
+        "attach_as": connection_info.username
+    }, handle_error=False)
+
+    if res.status_code != 200:
+        print_error(state, "Error registering jaaql account '%s' with username '%s', received status code %d and message:\n\n\t%s" %
+                    (credentials_name, connection_info.username, res.status_code, res.text))
+
+
+def on_go(state):
+    for parameter, value in state.parameters.items():
+        state.fetched_query = state.fetched_query.replace("{{" + parameter + "}}", value)
+
+    send_json = {"query": state.fetched_query}
+    if state.query_parameters is not None:
+        try:
+            send_json["parameters"] = json.loads(state.query_parameters)
+        except JSONDecodeError as ex:
+            print_error(state, "You have messed up your parameters: " + str(ex))
+    cur_conn = state.get_current_connection()
+    if cur_conn.database is not None:
+        send_json["database"] = cur_conn.database
+    if state.database_override is not None:
+        send_json["database"] = state.database_override
+    if not state.is_transactional:
+        send_json["autocommit"] = True
+
+    state.request_handler(METHOD__post, ENDPOINT__submit, send_json=send_json)
+
+    state.fetched_query = ""
+    state.query_parameters = None
+
+
+def parse_user_printing_any_errors(state, potential_user, allow_spaces: bool = False):
+    if " " in potential_user and not allow_spaces:
+        print_error(state, "Expected user without spaces, instead found spaces in user: '" + potential_user + "'")
+    if not potential_user.startswith("@"):
+        print_error(state, "Malformatted user, expected user to start with @")
+
+    return potential_user.split("@")[1].split(" ")[0]
+
+
+def deal_with_input(state: State, file_content: str = None):
+    if len(state.connections) == 0 and state.is_script():
+        print_error(state, "Must supply credentials file as argument in script mode")
+    if len(state.connections) != 0 and state.connections.get(DEFAULT_CONNECTION):
+        state.set_current_connection(get_connection_info(state, DEFAULT_CONNECTION))  # Preloads the default connection
+    elif not state.is_script():
+        print(state, "Type jaaql url or \"file [config_file_location]\"")
+        state.set_current_connection(handle_login(state, input("LOGIN>").strip()))
+
+    if state.is_script():
+        try:
+            if file_content:
+                state.file_lines = [line + "\n" for line in file_content.replace("\r\n", "\n").split("\n")]
+            else:
+                state.file_lines = open(state.file_name, "r").readlines()
+            state.file_lines.append(EOFMarker())  # Ignore warning. We can have multiple types. This is python
+        except FileNotFoundError:
+            print_error(state, "Could not load file for processing '" + state.file_name + "'")
+        except Exception as ex:
+            print_error(state, "Unhandled exception whilst processing file '" + state.file_name + "' " + str(ex))
+
+    while True:
+        fetched_line = None
+        try:
+            if len(state.file_lines) != 0:
+                fetched_line = state.file_lines[0]
+                state.cur_file_line += 1
+                state.file_lines = state.file_lines[1:]
+                if isinstance(fetched_line, EOFMarker):
+                    raise EOFError()
+        except EOFError:
+            break
+
+        if fetched_line.startswith(COMMAND__initialiser) or fetched_line.startswith(COMMAND__with_parameters):
+            fetched_line = fetched_line.strip()  # Ignore the line terminator e.g. \r\n
+            if fetched_line == COMMAND__go or fetched_line == COMMAND__go_short:
+                on_go(state)
+            elif fetched_line == COMMAND__reset or fetched_line == COMMAND__reset_short:
+                state.fetched_query = ""
+            elif fetched_line == COMMAND__print or fetched_line == COMMAND__print_short:
+                dump_buffer(state)
+            elif fetched_line == COMMAND__freeze_instance:
+                freeze_defrost_instance(state, freeze=True)
+            elif fetched_line == COMMAND__defrost_instance:
+                freeze_defrost_instance(state, freeze=False)
+            elif len(state.fetched_query.strip()) != 0:
+                print_error(state, "Tried to execute the command '" + fetched_line + "' but buffer was non empty.")
+            elif fetched_line == COMMAND__wipe_dbms:
+                wipe_jaaql_box(state)
+            elif fetched_line.startswith(COMMAND__with_parameters):
+                if fetched_line.strip().endswith("}"):
+                    state.query_parameters = fetched_line[len(COMMAND__with_parameters)-1:]
+                else:
+                    state.query_parameters = "{"
+                    state.reading_parameters = True
+            elif fetched_line.startswith(COMMAND__switch_jaaql_account_to):
+                candidate_connection_name = fetched_line.split(COMMAND__switch_jaaql_account_to)[1]
+                connection_name = parse_user_printing_any_errors(state, candidate_connection_name)
+                state.set_current_connection(get_connection_info(state, connection_name=connection_name))
+            elif fetched_line.startswith(COMMAND__connect_to_database):
+                candidate_database = fetched_line.split(COMMAND__connect_to_database)[1].split(" ")[0]
+                if fetched_line.endswith(CONNECT_FOR_CREATEDB):
+                    state.is_transactional = False
+
+                state.database_override = candidate_database.split(CONNECT_FOR_CREATEDB)[0]
+            elif fetched_line.startswith(COMMAND__register_jaaql_account_with):
+                candidate_connection_name = fetched_line.split(COMMAND__register_jaaql_account_with)[1]
+                connection_name = parse_user_printing_any_errors(state, candidate_connection_name)
+
+                register_jaaql_account(state, connection_name, get_connection_info(state, connection_name=connection_name))
+            elif fetched_line.startswith(COMMAND__attach_email_account):
+                candidate_connection_name = fetched_line.split(COMMAND__attach_email_account)[1]
+                connection_name = parse_user_printing_any_errors(state, candidate_connection_name, allow_spaces=True)
+                if " to " not in candidate_connection_name:
+                    print_error(state, "Expected token 'to' after dispatcher credentials file e.g. " +
+                                COMMAND__attach_email_account + "@dispatcher to app.dispatcher_name")
+                if candidate_connection_name.endswith(" to "):
+                    print_error(state, "Expected fully qualified dispatcher after ' to ' e.g. " +
+                                COMMAND__attach_email_account + "@dispatcher to app.dispatcher_name")
+                dispatcher_fqn = candidate_connection_name.split(" to ")[1]
+                dispatcher_fqn_split = dispatcher_fqn.split(".")
+                if len(dispatcher_fqn_split) != 2:
+                    print_error(state, "Badly formatted dispatcher name. Must be of the format 'app.dispatcher_name'. Received '%s'" % dispatcher_fqn)
+
+                attach_email_account(state, dispatcher_fqn_split[0], dispatcher_fqn_split[1], connection_name,
+                                     get_connection_info(state, connection_name=connection_name))
+            elif fetched_line == COMMAND__quit or fetched_line == COMMAND__quit_short:
+                break
+            else:
+                print_error(state, "Unrecognised command '" + fetched_line + "'")
+        else:
+            if state.reading_parameters:
+                state.query_parameters += fetched_line
+                if fetched_line.strip().startswith("}"):
+                    state.reading_parameters = False
+            else:
+                if len(state.fetched_query.strip()) != 0 or len(fetched_line.strip()) != 0:
+                    state.fetched_query += fetched_line  # Do not pre-append things with empty lines
+
+            if fetched_line.strip().endswith(COMMAND__go_short):
+                if state.reading_parameters:
+                    state.query_parameters = state.query_parameters[:-(len(COMMAND__go_short) + 1)]
+                    state.reading_parameters = False
+                else:
+                    state.fetched_query = state.fetched_query[:-(len(COMMAND__go_short) + 1)]
+
+                on_go(state)
+
+    if len(state.fetched_query) != 0:
+        if state.single_query:
+            on_go(state)
+        else:
+            print_error(state, "Attempting to quit with non-empty buffer. Please submit with \\g or clear with \\r")
+
+
+def initialise_from_args(args, file_name: str = None, file_content: str = None, do_exit: bool = True, override_url: str = None):
+    state = State()
+    state.do_exit = do_exit
+
+    if file_name is None:
+        file_name = [idx for arg, idx in zip(args, range(len(args))) if arg in ARGS__input_file]
+        if len(file_name) != 0:
+            state.file_name = args[file_name[0] + 1]
+    else:
+        state.file_name = file_name
+
+    state.override_url = override_url
+
+    state.is_verbose = len([arg for arg in args if arg in ['-v', '--verbose']]) != 0
+    state.is_debugging = len([arg for arg in args if arg in ['-d', '--debugging']]) != 0
+    state.single_query = len([arg for arg in args if arg in ARGS__single_query]) != 0
+
+    if state.is_verbose:
+        print_version()
+
+    for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__parameter:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The parameter flag is the last argument. You need to supply a parameter name")
+
+        if arg_idx == len(args) - 2:
+            print_error(state, "The parameter name is the last argument. You need to supply a parameter value")
+
+        parameter_name = args[arg_idx + 1]
+        parameter_value = args[arg_idx + 2]
+
+        if parameter_name in state.parameters:
+            print_error(state, "The parameter '" + parameter_name + "' has already been supplied")
+
+        state.parameters[parameter_name] = parameter_value
+
+    for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__environment:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The environment flag is the last argument. You need to supply a file")
+
+        parameter_file = args[arg_idx + 1]
+
+        for line in open(parameter_file, "r").readlines():
+            state.parameters[line.split("=")[0]] = "=".join(line.split("=")[1:])
+
+    for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__folder_config:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The folder config flag is the last argument. You need to supply a file")
+
+        configuration_folder = args[arg_idx + 1]
+
+        for config_file in os.listdir(configuration_folder):
+            full_file_name = os.path.join(configuration_folder, config_file)
+            if config_file.endswith(".email-credentials.txt"):
+                configuration_name = config_file[0:-len(".email-credentials.txt")]
+            elif config_file.endswith(".credentials.txt"):
+                configuration_name = config_file[0:-len(".credentials.txt")]
+            else:
+                raise JAAQLMonitorException("Unrecognised file extension for file " + full_file_name)
+
+            if configuration_name in state.connections:
+                print_error(state, "The configuration with name '" + configuration_name + "' already exists")
+
+            state.connections[configuration_name] = full_file_name
+
+    for arg, arg_idx in zip(args, range(len(args))):
+        if arg not in ARGS__encoded_config and arg not in ARGS__config:
+            continue
+
+        if arg_idx == len(args) - 1:
+            print_error(state, "The config flag is the last argument. You need to supply a file")
+
+        configuration_name = args[arg_idx + 1]
+        candidate_content_or_file_name = None
+        if arg_idx < len(args) - 2:
+            candidate_content_or_file_name = args[arg_idx + 2]
+
+        # The following branch of logic will use the supplied configuration name as the file name and set the configuration name to default
+        if candidate_content_or_file_name is None or candidate_content_or_file_name.startswith("<") or candidate_content_or_file_name.startswith("-"):
+            candidate_content_or_file_name = configuration_name
+            configuration_name = DEFAULT_CONNECTION
+
+        if configuration_name in state.connections:
+            print_error(state, "The configuration with name '" + configuration_name + "' already exists")
+
+        state.connections[configuration_name] = candidate_content_or_file_name
+
+        if arg in ARGS__encoded_config:
+            content_split = candidate_content_or_file_name.split(":")
+
+            db = None
+            if len(content_split) == 4:
+                db = b64d(content_split[3]).decode()
+
+            state.connection_info[configuration_name] = ConnectionInfo(b64d(content_split[0]).decode(), b64d(content_split[1]).decode(),
+                                                                       b64d(content_split[2]).decode(), db, state.override_url)
+
+    deal_with_input(state, file_content)
+
+
+def initialise(file_name: str, file_content: str, configs: list[[str, str]], encoded_configs: list[[str, str, str, str, str | None]],
+               override_url: str):
+    args = [ARGS__single_query[0]]
+
+    for config in configs:
+        args.append(ARGS__config[0])
+        args.append(config[0])
+        args.append(config[1])
+
+    for encoded_config in encoded_configs:
+        args.append(ARGS__encoded_config[0])
+        args.append(encoded_config[0])
+        db_part = ""
+        if encoded_config[4]:
+            db_part = ":" + b64e(encoded_config[4].encode()).decode()
+        args.append(b64e(encoded_config[1].encode()).decode() + ":" + b64e(encoded_config[2].encode()).decode() + ":" +
+                    b64e(encoded_config[3].encode()).decode() + db_part)
+
+    initialise_from_args(args, file_name, file_content, False, override_url)
+
+
+if __name__ == "__main__":
+    initialise_from_args(sys.argv[1:])
```

### Comparing `jaaql-monitor-1.2.64/setup.py` & `jaaql-monitor-1.2.67/setup.py`

 * *Files identical despite different names*

