# Comparing `tmp/odoo14_addon_ssi_project_code-14.0.1.1.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_project_code-14.0.1.1.1.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 53346 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1185 b- defN 23-Jul-24 05:39 odoo/addons/ssi_project_code/README.rst
--rw-r--r--  2.0 unx      180 b- defN 23-Jul-24 05:39 odoo/addons/ssi_project_code/__init__.py
--rw-r--r--  2.0 unx      503 b- defN 23-Jul-24 05:39 odoo/addons/ssi_project_code/__manifest__.py
--rw-r--r--  2.0 unx      189 b- defN 23-Jul-24 05:39 odoo/addons/ssi_project_code/models/__init__.py
--rw-r--r--  2.0 unx     1471 b- defN 23-Jul-24 05:39 odoo/addons/ssi_project_code/models/project_project.py
--rw-r--r--  2.0 unx    48333 b- defN 23-Jul-24 05:39 odoo/addons/ssi_project_code/static/description/icon.png
--rw-r--r--  2.0 unx      716 b- defN 23-Jul-24 05:39 odoo/addons/ssi_project_code/views/project_project_views.xml
--rw-r--r--  2.0 unx     1719 b- defN 23-Jul-24 05:40 odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 05:40 odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-24 05:40 odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1141 b- defN 23-Jul-24 05:40 odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/RECORD
-11 files, 55534 bytes uncompressed, 51336 bytes compressed:  7.6%
+Zip file size: 53378 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1181 b- defN 23-Aug-08 01:01 odoo/addons/ssi_project_code/README.rst
+-rw-r--r--  2.0 unx      180 b- defN 23-Aug-08 01:01 odoo/addons/ssi_project_code/__init__.py
+-rw-r--r--  2.0 unx      503 b- defN 23-Aug-08 01:01 odoo/addons/ssi_project_code/__manifest__.py
+-rw-r--r--  2.0 unx      189 b- defN 23-Aug-08 01:01 odoo/addons/ssi_project_code/models/__init__.py
+-rw-r--r--  2.0 unx     1471 b- defN 23-Aug-08 01:01 odoo/addons/ssi_project_code/models/project_project.py
+-rw-r--r--  2.0 unx    48333 b- defN 23-Aug-08 01:01 odoo/addons/ssi_project_code/static/description/icon.png
+-rw-r--r--  2.0 unx      716 b- defN 23-Aug-08 01:01 odoo/addons/ssi_project_code/views/project_project_views.xml
+-rw-r--r--  2.0 unx     1711 b- defN 23-Aug-08 01:03 odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 01:03 odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-08 01:03 odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1161 b- defN 23-Aug-08 01:03 odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/RECORD
+11 files, 55542 bytes uncompressed, 51328 bytes compressed:  7.6%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_project_code/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_project_code/views/project_project_views.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_project_code/README.rst

```diff
@@ -1,10 +1,10 @@
-.. image:: https://img.shields.io/badge/licence-LGPL--3-blue.svg
-   :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
-   :alt: License: LGPL-3
+.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+   :alt: License: AGPL-3
 
 ============
 Project Code
 ============
 
 
 Installation
@@ -37,10 +37,10 @@
 * Michael Viriyananda <viriyananda.michael@gmail.com>
 
 Maintainer
 ----------
 
 .. image:: https://simetri-sinergi.id/logo.png
    :alt: PT. Simetri Sinergi Indonesia
-   :target: https://simetri-sinergi.id.com
+   :target: https://simetri-sinergi.id
 
 This module is maintained by the PT. Simetri Sinergi Indonesia.
```

## odoo/addons/ssi_project_code/__init__.py

```diff
@@ -1,6 +1,6 @@
 # Copyright 2023 OpenSynergy Indonesia
 # Copyright 2023 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 from . import (
     models,
 )
```

## odoo/addons/ssi_project_code/__manifest__.py

```diff
@@ -1,16 +1,16 @@
 # Copyright 2023 OpenSynergy Indonesia
 # Copyright 2023 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 {
     "name": "Project Code",
     "version": "14.0.1.1.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
-    "license": "LGPL-3",
+    "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_project",
     ],
     "data": [
         "views/project_project_views.xml",
     ],
```

## odoo/addons/ssi_project_code/models/__init__.py

```diff
@@ -1,6 +1,6 @@
 # Copyright 2023 OpenSynergy Indonesia
 # Copyright 2023 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 from . import (
     project_project,
 )
```

## odoo/addons/ssi_project_code/models/project_project.py

```diff
@@ -1,10 +1,10 @@
 # Copyright 2023 OpenSynergy Indonesia
 # Copyright 2023 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 from odoo import _, api, fields, models
 from odoo.osv import expression
 
 
 class ProjectProject(models.Model):
     _inherit = "project.project"
```

## odoo/addons/ssi_project_code/views/project_project_views.xml

### odoo/addons/ssi_project_code/views/project_project_views.xml

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- Copyright 2023 OpenSynergy Indonesia
      Copyright 2023 PT. Simetri Sinergi Indonesia
-     License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl). -->
+     License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl). -->
 <odoo>
   <record id="project_project_view_form" model="ir.ui.view">
     <field name="name">project.project form</field>
     <field name="model">project.project</field>
     <field name="inherit_id" ref="project.edit_project"/>
     <field name="mode">extension</field>
     <field name="arch" type="xml">
```

## Comparing `odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/METADATA` & `odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-project-code
-Version: 14.0.1.1.0
+Version: 14.0.1.1.1.dev1
 Summary: Project Code
 Home-page: https://simetri-sinergi.id
 Author: OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia
-License: LGPL-3
+License: AGPL-3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Requires-Python: >=3.6
 Requires-Dist: odoo14-addon-ssi-project
 Requires-Dist: odoo (<14.1dev,>=14.0a)
 
-.. image:: https://img.shields.io/badge/licence-LGPL--3-blue.svg
-   :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
-   :alt: License: LGPL-3
+.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+   :alt: License: AGPL-3
 
 ============
 Project Code
 ============
 
 
 Installation
@@ -53,12 +53,12 @@
 * Michael Viriyananda <viriyananda.michael@gmail.com>
 
 Maintainer
 ----------
 
 .. image:: https://simetri-sinergi.id/logo.png
    :alt: PT. Simetri Sinergi Indonesia
-   :target: https://simetri-sinergi.id.com
+   :target: https://simetri-sinergi.id
 
 This module is maintained by the PT. Simetri Sinergi Indonesia.
```

## Comparing `odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/RECORD` & `odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-odoo/addons/ssi_project_code/README.rst,sha256=X1NB3CgUi2L_FTyqy4YQmwSF9_xDAT5PlNKi1cNjVkM,1185
-odoo/addons/ssi_project_code/__init__.py,sha256=Fa3RlqVGaZ5BNTMGtrlYO2v-HvTwO0OEB-mR7VqP2rQ,180
-odoo/addons/ssi_project_code/__manifest__.py,sha256=D7duVtrMbVxt9Sn6p2jLKB6khnpgKTVaDQJRgYrKUJc,503
-odoo/addons/ssi_project_code/models/__init__.py,sha256=soIIqBW4WaiOBykDuCqIE1fnnWN6VQOgQP5_NOfBcQg,189
-odoo/addons/ssi_project_code/models/project_project.py,sha256=ZgguFU0y_YyS8yoJsc6L2jcJpkopUbfKna5j2RKBYuI,1471
+odoo/addons/ssi_project_code/README.rst,sha256=nPEFn_llZb-q_y0REUyGapKCftP9JCjim8sGP20HAAQ,1181
+odoo/addons/ssi_project_code/__init__.py,sha256=3RrAUm6syewJ2K0Dc03UHMZKejAWRTQXaEgQ8cyN77I,180
+odoo/addons/ssi_project_code/__manifest__.py,sha256=kcN4DiDouUU7eecEgFHLzZOAm2x_rqDmbKw15gvvkCo,503
+odoo/addons/ssi_project_code/models/__init__.py,sha256=y4bAQuddoI4QoQXIcqisiQ3vupEqz_hPPHh-mgHE7I8,189
+odoo/addons/ssi_project_code/models/project_project.py,sha256=mmFK1hRyO2yZlaWIuc7x3dmRWP7QUsmIjIxIpYizB5s,1471
 odoo/addons/ssi_project_code/static/description/icon.png,sha256=lNGJOSg4cMRfwPTfFKVT6d5B2N1N83iVpEEN1blqu1I,48333
-odoo/addons/ssi_project_code/views/project_project_views.xml,sha256=TFXP07Y28NP4i78lH2-cY2Nmxzo8TWKEWm3mW4QUmkc,716
-odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/METADATA,sha256=ewbQt84iIogLAaHXk3XTPtgPtXD6fhvQEg6Cge36LVE,1719
-odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_ssi_project_code-14.0.1.1.0.dist-info/RECORD,,
+odoo/addons/ssi_project_code/views/project_project_views.xml,sha256=uCmdgyrzXyOLi6xBfgXEsbJ2OC15un1FaDGehceSqfQ,716
+odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/METADATA,sha256=YPRiSfD_5gRbrtnF6xifYDbD2ErkfpItBvAu830SY7w,1711
+odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_ssi_project_code-14.0.1.1.1.dev1.dist-info/RECORD,,
```

