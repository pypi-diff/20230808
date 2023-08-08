# Comparing `tmp/odoo12-addon-sm_donation_crm-12.0.0.0.1.tar.gz` & `tmp/odoo12_addon_sm_donation_crm-12.0.0.0.1.99.dev1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo12-addon-sm_donation_crm-12.0.0.0.1.tar", last modified: Tue Aug  8 15:22:40 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

