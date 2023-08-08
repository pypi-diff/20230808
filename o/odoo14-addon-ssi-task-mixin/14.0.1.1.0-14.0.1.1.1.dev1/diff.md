# Comparing `tmp/odoo14_addon_ssi_task_mixin-14.0.1.1.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 15389 bytes, number of entries: 11
--rw-r--r--  2.0 unx     1162 b- defN 23-Jul-24 05:39 odoo/addons/ssi_task_mixin/README.rst
--rw-r--r--  2.0 unx      181 b- defN 23-Jul-24 05:39 odoo/addons/ssi_task_mixin/__init__.py
--rw-r--r--  2.0 unx      542 b- defN 23-Jul-24 05:39 odoo/addons/ssi_task_mixin/__manifest__.py
--rw-r--r--  2.0 unx      185 b- defN 23-Jul-24 05:39 odoo/addons/ssi_task_mixin/models/__init__.py
--rw-r--r--  2.0 unx     7494 b- defN 23-Jul-24 05:39 odoo/addons/ssi_task_mixin/models/mixin_task.py
--rw-r--r--  2.0 unx     8619 b- defN 23-Jul-24 05:39 odoo/addons/ssi_task_mixin/static/description/icon.png
--rw-r--r--  2.0 unx     1730 b- defN 23-Jul-24 05:39 odoo/addons/ssi_task_mixin/templates/mixin_task_templates.xml
--rw-r--r--  2.0 unx     1746 b- defN 23-Jul-24 05:40 odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-24 05:40 odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Jul-24 05:40 odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1117 b- defN 23-Jul-24 05:40 odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/RECORD
-11 files, 22873 bytes uncompressed, 13427 bytes compressed:  41.3%
+Zip file size: 15431 bytes, number of entries: 11
+-rw-r--r--  2.0 unx     1158 b- defN 23-Aug-08 01:01 odoo/addons/ssi_task_mixin/README.rst
+-rw-r--r--  2.0 unx      181 b- defN 23-Aug-08 01:01 odoo/addons/ssi_task_mixin/__init__.py
+-rw-r--r--  2.0 unx      542 b- defN 23-Aug-08 01:01 odoo/addons/ssi_task_mixin/__manifest__.py
+-rw-r--r--  2.0 unx      185 b- defN 23-Aug-08 01:01 odoo/addons/ssi_task_mixin/models/__init__.py
+-rw-r--r--  2.0 unx     7494 b- defN 23-Aug-08 01:01 odoo/addons/ssi_task_mixin/models/mixin_task.py
+-rw-r--r--  2.0 unx     8619 b- defN 23-Aug-08 01:01 odoo/addons/ssi_task_mixin/static/description/icon.png
+-rw-r--r--  2.0 unx     1730 b- defN 23-Aug-08 01:01 odoo/addons/ssi_task_mixin/templates/mixin_task_templates.xml
+-rw-r--r--  2.0 unx     1738 b- defN 23-Aug-08 01:02 odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 01:02 odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-08 01:02 odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1137 b- defN 23-Aug-08 01:02 odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/RECORD
+11 files, 22881 bytes uncompressed, 13429 bytes compressed:  41.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: odoo/addons/ssi_task_mixin/static/description/icon.png
 Comment: 
 
 Filename: odoo/addons/ssi_task_mixin/templates/mixin_task_templates.xml
 Comment: 
 
-Filename: odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/METADATA
+Filename: odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/WHEEL
+Filename: odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/top_level.txt
+Filename: odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/RECORD
+Filename: odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/ssi_task_mixin/README.rst

```diff
@@ -1,10 +1,10 @@
-.. image:: https://img.shields.io/badge/licence-LGPL--3-blue.svg
-   :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
-   :alt: License: LGPL-3
+.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+   :alt: License: AGPL-3
 
 ==========
 Task Mixin
 ==========
 
 
 Installation
@@ -37,10 +37,10 @@
 * Andhitia Rama <andhitia.r@gmail.com>
 
 Maintainer
 ----------
 
 .. image:: https://simetri-sinergi.id/logo.png
    :alt: PT. Simetri Sinergi Indonesia
-   :target: https://simetri-sinergi.id.com
+   :target: https://simetri-sinergi.id
 
 This module is maintained by the PT. Simetri Sinergi Indonesia.
```

## odoo/addons/ssi_task_mixin/__init__.py

```diff
@@ -1,7 +1,7 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from . import (
     models,
 )
```

## odoo/addons/ssi_task_mixin/__manifest__.py

```diff
@@ -1,17 +1,17 @@
 # Copyright 2023 OpenSynergy Indonesia
 # Copyright 2023 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 {
     "name": "Task Mixin",
     "version": "14.0.1.1.0",
     "website": "https://simetri-sinergi.id",
     "author": "OpenSynergy Indonesia, PT. Simetri Sinergi Indonesia",
-    "license": "LGPL-3",
+    "license": "AGPL-3",
     "installable": True,
     "depends": [
         "ssi_task_timebox",
         "ssi_project_template",
     ],
     "data": [
         "templates/mixin_task_templates.xml",
```

## odoo/addons/ssi_task_mixin/models/__init__.py

```diff
@@ -1,7 +1,7 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from . import (
     mixin_task,
 )
```

## odoo/addons/ssi_task_mixin/models/mixin_task.py

```diff
@@ -1,10 +1,10 @@
 # Copyright 2022 OpenSynergy Indonesia
 # Copyright 2022 PT. Simetri Sinergi Indonesia
-# License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl).
+# License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl).
 
 from lxml import etree
 
 from odoo import api, fields, models
 
 
 class MixinTask(models.AbstractModel):
```

## odoo/addons/ssi_task_mixin/templates/mixin_task_templates.xml

### odoo/addons/ssi_task_mixin/templates/mixin_task_templates.xml

```diff
@@ -1,11 +1,11 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!-- Copyright 2022 OpenSynergy Indonesia
      Copyright 2022 PT. Simetri Sinergi Indonesia
-     License LGPL-3.0 or later (http://www.gnu.org/licenses/lgpl). -->
+     License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl). -->
 <odoo>
   <template id="task_mixin_template">
     <page name="task" string="Related Task(s)">
       <group name="task" colspan="4" col="2">
         <field name="need_task"/>
         <field name="total_task"/>
         <field name="task_draft_count"/>
```

## Comparing `odoo14_addon_ssi_task_mixin-14.0.1.1.0.dist-info/METADATA` & `odoo14_addon_ssi_task_mixin-14.0.1.1.1.dev1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 Metadata-Version: 2.1
 Name: odoo14-addon-ssi-task-mixin
-Version: 14.0.1.1.0
+Version: 14.0.1.1.1.dev1
 Summary: Task Mixin
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
 Requires-Dist: odoo14-addon-ssi-project-template
 Requires-Dist: odoo14-addon-ssi-task-timebox
 Requires-Dist: odoo (<14.1dev,>=14.0a)
 
-.. image:: https://img.shields.io/badge/licence-LGPL--3-blue.svg
-   :target: http://www.gnu.org/licenses/lgpl-3.0-standalone.html
-   :alt: License: LGPL-3
+.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+   :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+   :alt: License: AGPL-3
 
 ==========
 Task Mixin
 ==========
 
 
 Installation
@@ -54,12 +54,12 @@
 * Andhitia Rama <andhitia.r@gmail.com>
 
 Maintainer
 ----------
 
 .. image:: https://simetri-sinergi.id/logo.png
    :alt: PT. Simetri Sinergi Indonesia
-   :target: https://simetri-sinergi.id.com
+   :target: https://simetri-sinergi.id
 
 This module is maintained by the PT. Simetri Sinergi Indonesia.
```

