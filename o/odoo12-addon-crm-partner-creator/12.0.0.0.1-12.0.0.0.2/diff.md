# Comparing `tmp/odoo12_addon_crm_partner_creator-12.0.0.0.1-py3-none-any.whl.zip` & `tmp/odoo12_addon_crm_partner_creator-12.0.0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 5882 bytes, number of entries: 12
--rw-r--r--  2.0 unx       46 b- defN 23-Apr-19 15:51 odoo/addons/crm_partner_creator/__init__.py
--rw-r--r--  2.0 unx      615 b- defN 23-Apr-19 16:23 odoo/addons/crm_partner_creator/__manifest__.py
--rw-r--r--  2.0 unx       89 b- defN 23-Apr-19 15:51 odoo/addons/crm_partner_creator/models/__init__.py
--rw-r--r--  2.0 unx     5024 b- defN 23-Apr-19 15:51 odoo/addons/crm_partner_creator/models/crm_lead.py
--rw-r--r--  2.0 unx      400 b- defN 23-Apr-19 15:51 odoo/addons/crm_partner_creator/models/crm_partner_creator_config.py
--rw-r--r--  2.0 unx      180 b- defN 23-Apr-19 15:51 odoo/addons/crm_partner_creator/security/ir.model.access.csv
--rw-r--r--  2.0 unx      964 b- defN 23-Apr-19 15:51 odoo/addons/crm_partner_creator/views/crm_lead.xml
--rw-r--r--  2.0 unx     1630 b- defN 23-Apr-19 15:51 odoo/addons/crm_partner_creator/views/crm_partner_creator_config.xml
--rw-r--r--  2.0 unx      517 b- defN 23-Apr-19 16:29 odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-19 16:29 odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Apr-19 16:29 odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1300 b- defN 23-Apr-19 16:29 odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/RECORD
-12 files, 10862 bytes uncompressed, 3580 bytes compressed:  67.0%
+Zip file size: 5895 bytes, number of entries: 12
+-rw-r--r--  2.0 unx       46 b- defN 23-Aug-08 17:25 odoo/addons/crm_partner_creator/__init__.py
+-rw-r--r--  2.0 unx      615 b- defN 23-Aug-08 17:25 odoo/addons/crm_partner_creator/__manifest__.py
+-rw-r--r--  2.0 unx       89 b- defN 23-Aug-08 17:25 odoo/addons/crm_partner_creator/models/__init__.py
+-rw-r--r--  2.0 unx     5034 b- defN 23-Aug-08 17:26 odoo/addons/crm_partner_creator/models/crm_lead.py
+-rw-r--r--  2.0 unx      400 b- defN 23-Aug-08 17:25 odoo/addons/crm_partner_creator/models/crm_partner_creator_config.py
+-rw-r--r--  2.0 unx      180 b- defN 23-Aug-08 17:25 odoo/addons/crm_partner_creator/security/ir.model.access.csv
+-rw-r--r--  2.0 unx      964 b- defN 23-Aug-08 17:25 odoo/addons/crm_partner_creator/views/crm_lead.xml
+-rw-r--r--  2.0 unx     1630 b- defN 23-Aug-08 17:25 odoo/addons/crm_partner_creator/views/crm_partner_creator_config.xml
+-rw-r--r--  2.0 unx      517 b- defN 23-Aug-08 17:26 odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-08 17:26 odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Aug-08 17:26 odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1300 b- defN 23-Aug-08 17:26 odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/RECORD
+12 files, 10872 bytes uncompressed, 3593 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: odoo/addons/crm_partner_creator/views/crm_lead.xml
 Comment: 
 
 Filename: odoo/addons/crm_partner_creator/views/crm_partner_creator_config.xml
 Comment: 
 
-Filename: odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/METADATA
+Filename: odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/WHEEL
+Filename: odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/top_level.txt
+Filename: odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/RECORD
+Filename: odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/crm_partner_creator/__manifest__.py

```diff
@@ -6,15 +6,15 @@
         Create new partner from crm lead metadata
     """,
 
     'author': "Coopdevs Treball SCCL",
     'website': "https://git.coopdevs.org/coopdevs/odoo/odoo-addons/enhancements/enhancements-crm",
 
     'category': 'crm',
-    'version': '12.0.0.0.1',
+    'version': '12.0.0.0.2',
 
     # any module necessary for this one to work correctly
     'depends': ['base', 'crm_metadata', 'crm_sale_order_line'],
 
     # always loaded
     'data': [
         'security/ir.model.access.csv',
```

## odoo/addons/crm_partner_creator/models/crm_lead.py

```diff
@@ -71,19 +71,19 @@
 
     def _validate_partner_creation(self):
         if not self.partner_creator_config_id:
             raise exceptions.ValidationError(
                 _("Partner creator must be defined")
             )
         # TODO: Move to new module "crm_cooperator_partner_creator"
-        if self.subscription_request_id:
-            raise exceptions.ValidationError(
-                _("Can't create partner on lead \
-                with subcription request defined.")
-            )
+#         if self.subscription_request_id:
+#             raise exceptions.ValidationError(
+#                 _("Can't create partner on lead \
+#                 with subcription request defined.")
+#             )
 
     def _search_partner_from_config(self, config_json):
         if not self.partner_id:
             search_data = self._get_partner_search_data(
                 config_json
             )
             if search_data:
```

## Comparing `odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/METADATA` & `odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo12-addon-crm-partner-creator
-Version: 12.0.0.0.1
+Version: 12.0.0.0.2
 Summary: Create new partner from crm lead metadata
 Home-page: https://git.coopdevs.org/coopdevs/odoo/odoo-addons/enhancements/enhancements-crm
 Author: Coopdevs Treball SCCL
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 12.0
 Requires-Python: >=3.5
```

## Comparing `odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/RECORD` & `odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 odoo/addons/crm_partner_creator/__init__.py,sha256=Ax4qLxdb9ATk05MF7cSQ0BdpYCpGVYFy9n4U4zODf9o,46
-odoo/addons/crm_partner_creator/__manifest__.py,sha256=vHZBamnpXrjSEbvrO1-uH5vjmPdDY0fMQqcdS9io1E4,615
+odoo/addons/crm_partner_creator/__manifest__.py,sha256=8ppMGrRB0Jqk1f4zx3rqz8fT8Tt9D088K98r_TyzosM,615
 odoo/addons/crm_partner_creator/models/__init__.py,sha256=_EKOulW5fMkDjz5AanuHlVqbjRad4VUTri7zZt4skyY,89
-odoo/addons/crm_partner_creator/models/crm_lead.py,sha256=GKogvIgxisNJuh1XeWGRermjU5ReUptfRM1VP2N2g5Y,5024
+odoo/addons/crm_partner_creator/models/crm_lead.py,sha256=gumPxK_zWdAsmCXVvrUi9Omaw8RfRheJPmi5Qt7Oiuc,5034
 odoo/addons/crm_partner_creator/models/crm_partner_creator_config.py,sha256=py5iS_YDpjMDDhQ0tk5dK7wXpGSCIzwKv6qbhwiqSf0,400
 odoo/addons/crm_partner_creator/security/ir.model.access.csv,sha256=l66PSbsGFaRmicIqLB_LgIaxGoMSVNLN0MehLMGosiU,180
 odoo/addons/crm_partner_creator/views/crm_lead.xml,sha256=YaYBWZzIme3G2ri0jAiMSudqhxGYTig-hA4giueT61U,964
 odoo/addons/crm_partner_creator/views/crm_partner_creator_config.xml,sha256=0wclhSeouY-S0bevC3jXqU4Qzfy5X5sLKoYvbHEUx5c,1630
-odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/METADATA,sha256=F9x5xhlXegwBnr5QQ1shyKnd7r1ntq6oMrpKVW75GKA,517
-odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo12_addon_crm_partner_creator-12.0.0.0.1.dist-info/RECORD,,
+odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/METADATA,sha256=fmSsZvUPQ--sGdFXOoOzhBHvgu7mRfYS1DzqlD6_r10,517
+odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo12_addon_crm_partner_creator-12.0.0.0.2.dist-info/RECORD,,
```

