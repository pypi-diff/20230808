# Comparing `tmp/cloudwash-1.1.3.tar.gz` & `tmp/cloudwash-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudwash-1.1.3.tar", last modified: Wed Jan 25 14:04:42 2023, max compression
+gzip compressed data, was "cloudwash-1.1.4.tar", last modified: Tue Aug  8 08:20:02 2023, max compression
```

## Comparing `cloudwash-1.1.3.tar` & `cloudwash-1.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 14:04:42.158119 cloudwash-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-01-25 14:02:50.000000 cloudwash-1.1.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 14:04:42.154119 cloudwash-1.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-01-25 14:02:50.000000 cloudwash-1.1.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 14:04:42.154119 cloudwash-1.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-01-25 14:02:50.000000 cloudwash-1.1.3/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-01-25 14:02:50.000000 cloudwash-1.1.3/.github/workflows/new_release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-01-25 14:02:50.000000 cloudwash-1.1.3/.github/workflows/pull_request.yml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-01-25 14:02:50.000000 cloudwash-1.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-01-25 14:02:50.000000 cloudwash-1.1.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-01-25 14:02:50.000000 cloudwash-1.1.3/Dockerfile.dev
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-25 14:02:50.000000 cloudwash-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-01-25 14:04:42.158119 cloudwash-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-01-25 14:02:50.000000 cloudwash-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 14:04:42.158119 cloudwash-1.1.3/cloudwash/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 14:04:42.158119 cloudwash-1.1.3/cloudwash/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/providers/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/providers/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/providers/gce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 14:04:42.158119 cloudwash-1.1.3/cloudwash.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-01-25 14:04:42.000000 cloudwash-1.1.3/cloudwash.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-01-25 14:04:42.000000 cloudwash-1.1.3/cloudwash.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 14:04:42.000000 cloudwash-1.1.3/cloudwash.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-01-25 14:04:42.000000 cloudwash-1.1.3/cloudwash.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-01-25 14:04:42.000000 cloudwash-1.1.3/cloudwash.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-01-25 14:04:42.000000 cloudwash-1.1.3/cloudwash.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-01-25 14:02:50.000000 cloudwash-1.1.3/cloudwash_openshift_buildconfig.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 14:04:42.158119 cloudwash-1.1.3/conf/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-01-25 14:02:50.000000 cloudwash-1.1.3/conf/aws.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-01-25 14:02:50.000000 cloudwash-1.1.3/conf/azure.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-01-25 14:02:50.000000 cloudwash-1.1.3/conf/gce.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-01-25 14:02:50.000000 cloudwash-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-01-25 14:02:50.000000 cloudwash-1.1.3/settings.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-01-25 14:04:42.158119 cloudwash-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-01-25 14:02:50.000000 cloudwash-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:20:02.570555 cloudwash-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-08 08:17:25.000000 cloudwash-1.1.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:20:02.562555 cloudwash-1.1.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-08 08:17:25.000000 cloudwash-1.1.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:20:02.562555 cloudwash-1.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-08-08 08:17:25.000000 cloudwash-1.1.4/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-08-08 08:17:25.000000 cloudwash-1.1.4/.github/workflows/new_release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-08-08 08:17:25.000000 cloudwash-1.1.4/.github/workflows/pull_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-08 08:17:25.000000 cloudwash-1.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-08-08 08:17:25.000000 cloudwash-1.1.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-08 08:17:25.000000 cloudwash-1.1.4/Dockerfile.dev
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-08 08:17:25.000000 cloudwash-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-08 08:20:02.570555 cloudwash-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-08-08 08:17:25.000000 cloudwash-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:20:02.566555 cloudwash-1.1.4/cloudwash/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:20:02.566555 cloudwash-1.1.4/cloudwash/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6529 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/providers/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8467 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/providers/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/providers/gce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:20:02.566555 cloudwash-1.1.4/cloudwash.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-08 08:20:02.000000 cloudwash-1.1.4/cloudwash.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-08-08 08:20:02.000000 cloudwash-1.1.4/cloudwash.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 08:20:02.000000 cloudwash-1.1.4/cloudwash.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 08:20:02.000000 cloudwash-1.1.4/cloudwash.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-08 08:20:02.000000 cloudwash-1.1.4/cloudwash.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-08 08:20:02.000000 cloudwash-1.1.4/cloudwash.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-08-08 08:17:25.000000 cloudwash-1.1.4/cloudwash_openshift_buildconfig.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 08:20:02.570555 cloudwash-1.1.4/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-08-08 08:17:25.000000 cloudwash-1.1.4/conf/aws.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-08-08 08:17:25.000000 cloudwash-1.1.4/conf/azure.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-08 08:17:25.000000 cloudwash-1.1.4/conf/gce.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-08 08:17:25.000000 cloudwash-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-08-08 08:17:25.000000 cloudwash-1.1.4/settings.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-08 08:20:02.570555 cloudwash-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 08:17:25.000000 cloudwash-1.1.4/setup.py
```

### Comparing `cloudwash-1.1.3/.github/dependabot.yml` & `cloudwash-1.1.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/.github/workflows/codeql-analysis.yml` & `cloudwash-1.1.4/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/.github/workflows/new_release.yml` & `cloudwash-1.1.4/.github/workflows/new_release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
   release_to_pypi:
     needs: codechecks
     name: PyPi Release
     runs-on: ubuntu-latest
 
     steps:
       - name: Checkout
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
 
       - name: Set Up Python3
         uses: actions/setup-python@v4
         with:
           python-version: 3.11
 
       - name: Setup and Build
@@ -68,15 +68,15 @@
           pip uninstall -y pycurl
           pip install --compile --no-cache-dir pycurl
           pip install .[setup]
           python setup.py sdist bdist_wheel
           python -m twine check dist/*
 
       - name: Release to PyPi
-        uses: pypa/gh-action-pypi-publish@v1.6.4
+        uses: pypa/gh-action-pypi-publish@v1.8.5
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
           skip_existing: true
 
   cloudwash_container:
     needs: release_to_pypi
@@ -97,13 +97,13 @@
         uses: docker/login-action@v2
         with:
           registry: 'quay.io'
           username: ${{ secrets.QUAY_USERNAME }}
           password: ${{ secrets.QUAY_TOKEN }}
 
       - name: Build and push image to Quay
-        uses: docker/build-push-action@v3
+        uses: docker/build-push-action@v4
         with:
           context: .
           file: ./Dockerfile.dev
           push: true
           tags: quay.io/redhatqe/cloudwash:latest,quay.io/redhatqe/cloudwash:v${{ github.ref_name }}
```

### Comparing `cloudwash-1.1.3/.github/workflows/pull_request.yml` & `cloudwash-1.1.4/.github/workflows/pull_request.yml`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/Dockerfile.dev` & `cloudwash-1.1.4/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/LICENSE` & `cloudwash-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/PKG-INFO` & `cloudwash-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudwash
-Version: 1.1.3
+Version: 1.1.4
 Summary: The cloud resources cleanup utility
 Home-page: https://github.com/RedHatQE/cloudwash
 Author: Jitendra Yejare
 Author-email: jyejare@redhat.com
 License: Apache license
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `cloudwash-1.1.3/README.md` & `cloudwash-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/cloudwash/cli.py` & `cloudwash-1.1.4/cloudwash/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,48 +63,58 @@
     validate_provider(ctx.command.name)
     is_dry_run = ctx.parent.params["dry"]
     gceCleanup(vms=vms, discs=discs, nics=nics, _all=_all, dry_run=is_dry_run)
 
 
 @cleanup_providers.command(help="Cleanup Azure provider")
 @common_options
+@click.option("--images", is_flag=True, help="Remove only images from the provider")
 @click.option("--pips", is_flag=True, help="Remove only PiPs from the provider")
 @click.option(
     "--all_rg",
     "_all_rg",
     is_flag=True,
     help="Remove resource group only if all resources are older than SLA",
 )
 @click.pass_context
-def azure(ctx, vms, discs, nics, pips, _all, _all_rg):
+def azure(ctx, vms, discs, nics, images, pips, _all, _all_rg):
     # Validate Azure Settings
     validate_provider(ctx.command.name)
     is_dry_run = ctx.parent.params["dry"]
     azureCleanup(
         vms=vms,
         discs=discs,
         nics=nics,
+        images=images,
         pips=pips,
         _all=_all,
         _all_rg=_all_rg,
         dry_run=is_dry_run,
     )
 
 
 @cleanup_providers.command(help="Cleanup Amazon provider")
 @common_options
+@click.option("--images", is_flag=True, help="Remove only images from the provider")
 @click.option("--pips", is_flag=True, help="Remove only Public IPs from the provider")
 @click.option("--stacks", is_flag=True, help="Remove only CloudFormations from the provider")
 @click.pass_context
-def aws(ctx, vms, discs, nics, pips, stacks, _all):
+def aws(ctx, vms, discs, nics, images, pips, stacks, _all):
     # Validate Amazon Settings
     validate_provider(ctx.command.name)
     is_dry_run = ctx.parent.params["dry"]
     awsCleanup(
-        vms=vms, discs=discs, nics=nics, pips=pips, stacks=stacks, _all=_all, dry_run=is_dry_run
+        vms=vms,
+        discs=discs,
+        nics=nics,
+        images=images,
+        pips=pips,
+        stacks=stacks,
+        _all=_all,
+        dry_run=is_dry_run,
     )
 
 
 @cleanup_providers.command(help="Cleanup VMWare provider")
 @common_options
 @click.pass_context
 def vmware(ctx, vms, discs, nics, _all):
```

### Comparing `cloudwash-1.1.3/cloudwash/client.py` & `cloudwash-1.1.4/cloudwash/client.py`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/cloudwash/config.py` & `cloudwash-1.1.4/cloudwash/config.py`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/cloudwash/providers/aws.py` & `cloudwash-1.1.4/cloudwash/providers/aws.py`

 * *Files 20% similar despite different names*

```diff
@@ -49,14 +49,35 @@
             def dry_discs():
                 rdiscs = []
                 if settings.aws.criteria.disc.unassigned:
                     rdiscs = aws_client.get_all_unattached_volumes()
                     [dry_data["DISCS"]["delete"].append(ddisc["VolumeId"]) for ddisc in rdiscs]
                 return rdiscs
 
+            def dry_images():
+                rimages = []
+                if settings.aws.criteria.image.unassigned:
+                    rimages = aws_client.list_templates(executable_by_me=False, owned_by_me=True)
+                    free_images = aws_client.list_free_images(
+                        image_list=[image.raw.image_id for image in rimages]
+                    )
+                    remove_images = [
+                        image
+                        for image in free_images
+                        if image not in settings.aws.exceptions.images
+                    ]
+                    if settings.aws.criteria.image.delete_image:
+                        remove_images = [
+                            image
+                            for image in remove_images
+                            if image.startswith(settings.aws.criteria.image.delete_image)
+                        ]
+                    dry_data["IMAGES"]["delete"].extend(remove_images)
+                return remove_images
+
             def dry_pips():
                 rpips = []
                 if settings.aws.criteria.public_ip.unassigned:
                     rpips = aws_client.get_all_disassociated_addresses()
                     [dry_data["PIPS"]["delete"].append(dpip["AllocationId"]) for dpip in rpips]
                 return rpips
 
@@ -102,14 +123,20 @@
                     aws_client.remove_all_unused_nics()
                     logger.info(f"Removed NICs: \n{rnics}")
             if kwargs["discs"] or kwargs["_all"]:
                 rdiscs = dry_discs()
                 if not is_dry_run and rdiscs:
                     aws_client.remove_all_unused_volumes()
                     logger.info(f"Removed Discs: \n{rdiscs}")
+            if kwargs["images"] or kwargs["_all"]:
+                rimages = dry_images()
+                if not is_dry_run and rimages:
+                    aws_client.delete_images(image_list=rimages)
+                    logger.info(f"Removed Images: \n{rimages}")
+
             if kwargs["pips"] or kwargs["_all"]:
                 rpips = dry_pips()
                 if not is_dry_run and rpips:
                     aws_client.remove_all_unused_ips()
                     logger.info(f"Removed PIPs: \n{rpips}")
             if kwargs["stacks"] or kwargs["_all"]:
                 rstacks = dry_stacks()
```

### Comparing `cloudwash-1.1.3/cloudwash/providers/azure.py` & `cloudwash-1.1.4/cloudwash/providers/azure.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 _vms["delete"].append(vm.name)
     return _vms
 
 
 def cleanup(**kwargs):
     is_dry_run = kwargs["dry_run"]
 
-    data = ['VMS', 'NICS', 'DISCS', 'PIPS', 'RESOURCES']
+    data = ['VMS', 'NICS', 'DISCS', 'IMAGES', 'PIPS', 'RESOURCES']
     regions = settings.azure.auth.regions
     groups = settings.azure.auth.resource_groups
 
     if "all" in regions:
         # non-existent RG can be chosen for query
         # as it's never accessed and is only stored within wrapper
         with compute_client("azure", azure_region="us-west", resource_group="foo") as azure_client:
@@ -93,14 +93,36 @@
                 def dry_resources(hours_old=None):
                     dry_data["RESOURCES"]["delete"] = azure_client.list_resources_from_hours_old(
                         hours_old=hours_old
                         or (settings.azure.criteria.resource_group.resources_sla_minutes / 60)
                     )
                     return dry_data["RESOURCES"]["delete"]
 
+                def dry_images():
+                    remove_images = []
+                    if settings.azure.criteria.image.unassigned:
+                        images_list = azure_client.list_compute_images_by_resource_group(
+                            free_images=True
+                        )
+                        image_names = [image.name for image in images_list]
+                        # Filter out the images not to be removed.
+                        remove_images = [
+                            image
+                            for image in image_names
+                            if image not in settings.azure.exceptions.images
+                        ]
+                        if settings.azure.criteria.image.delete_image:
+                            remove_images = [
+                                image
+                                for image in remove_images
+                                if image.startswith(settings.azure.criteria.image.delete_image)
+                            ]
+                        dry_data["IMAGES"]["delete"].extend(remove_images)
+                    return remove_images
+
                 # Remove / Stop VMs
                 def remove_vms(avms):
                     # Remove VMs
                     [azure_client.get_vm(vm_name).delete() for vm_name in avms["delete"]]
                     # Stop VMs
                     [azure_client.get_vm(vm_name).stop() for vm_name in avms["stop"]]
 
@@ -125,14 +147,20 @@
                         azure_client.remove_discs_by_search()
                         logger.info(f"Removed Discs: \n{rdiscs}")
                 if kwargs["pips"] or kwargs["_all"]:
                     rpips = dry_pips()
                     if not is_dry_run and rpips:
                         azure_client.remove_pips_by_search()
                         logger.info(f"Removed PIPs: \n{rpips}")
+                if kwargs["images"] or kwargs["_all"]:
+                    rimages = dry_images()
+                    if not is_dry_run and rimages:
+                        azure_client.delete_compute_image_by_resource_group(image_list=rimages)
+                        logger.info(f"Removed Images: \n{rimages}")
+
                 if kwargs["_all_rg"]:
                     sla_time = settings.azure.criteria.resource_group.resources_sla_minutes
 
                     # Exception list has priority
                     if group in settings.azure.exceptions.group.rg_list:
                         continue
```

### Comparing `cloudwash-1.1.3/cloudwash/providers/gce.py` & `cloudwash-1.1.4/cloudwash/providers/gce.py`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/cloudwash/utils.py` & `cloudwash-1.1.4/cloudwash/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 _vms_dict = {"VMS": {"delete": [], "stop": [], "skip": []}}
 dry_data = {
     "NICS": {"delete": []},
     "DISCS": {"delete": []},
     "PIPS": {"delete": []},
     "RESOURCES": {"delete": []},
     "STACKS": {"delete": []},
+    "IMAGES": {"delete": []},
 }
 dry_data.update(_vms_dict)
 
 
 def echo_dry(dry_data=None) -> None:
     """Prints and Logs the per resource cleanup data on STDOUT and logfile
 
@@ -25,26 +26,29 @@
     """
     logger.info("\n=========== DRY SUMMARY ============\n")
     deletable_vms = dry_data["VMS"]["delete"]
     stopable_vms = dry_data["VMS"]["stop"]
     skipped_vms = dry_data["VMS"]["skip"]
     deletable_discs = dry_data["DISCS"]["delete"]
     deletable_nics = dry_data["NICS"]["delete"]
+    deletable_images = dry_data["IMAGES"]["delete"]
     deletable_pips = dry_data["PIPS"]["delete"] if "PIPS" in dry_data else None
     deletable_resources = dry_data["RESOURCES"]["delete"]
     deletable_stacks = dry_data["STACKS"]["delete"] if "STACKS" in dry_data else None
     if deletable_vms or stopable_vms or skipped_vms:
         logger.info(
             f"VMs:\n\tDeletable: {deletable_vms}\n\tStoppable: {stopable_vms}\n\t"
             f"Skip: {skipped_vms}"
         )
     if deletable_discs:
         logger.info(f"DISCs:\n\tDeletable: {deletable_discs}")
     if deletable_nics:
         logger.info(f"NICs:\n\tDeletable: {deletable_nics}")
+    if deletable_images:
+        logger.info(f"IMAGES:\n\tDeletable: {deletable_images}")
     if deletable_pips:
         logger.info(f"PIPs:\n\tDeletable: {deletable_pips}")
     if deletable_resources:
         logger.info(f"RESOURCEs:\n\tDeletable: {deletable_resources}")
     if deletable_stacks:
         logger.info(f"STACKs:\n\tDeletable: {deletable_stacks}")
     if not any(
@@ -52,14 +56,15 @@
             deletable_vms,
             stopable_vms,
             deletable_discs,
             deletable_nics,
             deletable_pips,
             deletable_resources,
             deletable_stacks,
+            deletable_images,
         ]
     ):
         logger.info("\nNo resources are eligible for cleanup!")
     logger.info("\n====================================\n")
 
 
 def total_running_time(vm_obj) -> namedtuple:
```

### Comparing `cloudwash-1.1.3/cloudwash.egg-info/PKG-INFO` & `cloudwash-1.1.4/cloudwash.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudwash
-Version: 1.1.3
+Version: 1.1.4
 Summary: The cloud resources cleanup utility
 Home-page: https://github.com/RedHatQE/cloudwash
 Author: Jitendra Yejare
 Author-email: jyejare@redhat.com
 License: Apache license
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `cloudwash-1.1.3/cloudwash.egg-info/SOURCES.txt` & `cloudwash-1.1.4/cloudwash.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/cloudwash_openshift_buildconfig.yaml` & `cloudwash-1.1.4/cloudwash_openshift_buildconfig.yaml`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/conf/aws.yaml.template` & `cloudwash-1.1.4/conf/aws.yaml.template`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,19 @@
             DELETE_VM: 'test'
             # Number of minutes the deletable VM should be allowed to live, e.g 120 minutes = 2 Hours
             SLA_MINUTES: 120
         DISC:
             UNASSIGNED: True
         NIC:
             UNASSIGNED: True
+        IMAGE:
+            # Image name starts with
+            DELETE_IMAGE:
+
+            UNASSIGNED: True
         PUBLIC_IP:
             UNASSIGNED: True
         STACKS:
             # The CloudFormation to be deleted with prepend string, e.g stack name that starts with 'test'
             DELETE_STACK: 'test'
             # Number of minutes the deletable CloudFormation should be allowed to live, e.g 120 minutes = 2 Hours
             SLA_MINUTES: 120
@@ -26,7 +31,8 @@
             # VM names that would be skipped from cleanup
             VM_LIST: []
             # VMs that would be stopped from current running state
             STOP_LIST: []
         STACKS:
             # CloudFormations names that would be skipped from cleanup
             STACK_LIST: []
+        IMAGES: []
```

### Comparing `cloudwash-1.1.3/conf/azure.yaml.template` & `cloudwash-1.1.4/conf/azure.yaml.template`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,19 @@
             DELETE_VM: 'test'
             # Number of minutes the deletable VM should be allowed to live, e.g 120 minutes = 2 Hours
             SLA_MINUTES: 120
         DISC:
             UNASSIGNED: True
         NIC:
             UNASSIGNED: True
+        IMAGE:
+            # Image name starts with
+            DELETE_IMAGE:
+
+            UNASSIGNED: True
         PUBLIC_IP:
             UNASSIGNED: True
         RESOURCE_GROUP:
             # Select AND to match all criteria or OR to match any one of them
             LOGIC: AND
             # Group to be deleted with prepend string, e.g. resource group name that starts with 'test'
             DELETE_GROUP:
@@ -32,7 +37,8 @@
             # VM names that would be skipped from cleanup
             VM_LIST: []
             # VMs that would be stopped from current running state
             STOP_LIST: []
         GROUP:
             # Resource groups that would be skipped from cleanup
             RG_LIST: []
+        IMAGES: []
```

### Comparing `cloudwash-1.1.3/conf/gce.yaml.template` & `cloudwash-1.1.4/conf/gce.yaml.template`

 * *Files identical despite different names*

### Comparing `cloudwash-1.1.3/settings.yaml.template` & `cloudwash-1.1.4/settings.yaml.template`

 * *Files 10% similar despite different names*

```diff
@@ -39,14 +39,19 @@
             DELETE_VM: 'test'
             # Number of minutes the deletable VM should be allowed to live, e.g 120 minutes = 2 Hours
             SLA_MINUTES: 120
         DISC:
             UNASSIGNED: True
         NIC:
             UNASSIGNED: True
+        IMAGE:
+            # Image name starts with
+            DELETE_IMAGE:
+
+            UNASSIGNED: True
         PUBLIC_IP:
             UNASSIGNED: True
         RESOURCE_GROUP:
             # Select AND to match all criteria or OR to match any one of them
             LOGIC: AND
             # Group to be deleted with prepend string, e.g. resource group name that starts with 'test'
             DELETE_GROUP:
@@ -57,14 +62,15 @@
             # VM names that would be skipped from cleanup
             VM_LIST: []
             # VMs that would be stopped from current running state
             STOP_LIST: []
         GROUP:
             # Resource groups that would be skipped from cleanup
             RG_LIST: []
+        IMAGES: []
 
 AWS:
     AUTH:
         ACCESS_KEY:
         SECRET_KEY:
         # Multiple regions can be added like ["ap-south-1", "us-west-2", "us-west-1"] or ["all"] for all regions
         REGIONS: []
@@ -74,14 +80,20 @@
             DELETE_VM: 'test'
             # Number of minutes the deletable VM should be allowed to live, e.g 120 minutes = 2 Hours
             SLA_MINUTES: 120
         DISC:
             UNASSIGNED: True
         NIC:
             UNASSIGNED: True
+        # Image name starts with
+        IMAGE:
+            # Image name starts with
+            DELETE_IMAGE:
+
+            UNASSIGNED: True
         PUBLIC_IP:
             UNASSIGNED: True
         STACKS:
             # The CloudFormation to be deleted with prepend string, e.g stack name that starts with 'test'
             DELETE_STACK: 'test'
             # Number of minutes the deletable CloudFormation should be allowed to live, e.g 120 minutes = 2 Hours
             SLA_MINUTES: 120
@@ -90,7 +102,8 @@
             # VM names that would be skipped from cleanup
             VM_LIST: []
             # VMs that would be stopped from current running state
             STOP_LIST: []
         STACKS:
             # CloudFormations names that would be skipped from cleanup
             STACK_LIST: []
+        IMAGES: []
```

### Comparing `cloudwash-1.1.3/setup.cfg` & `cloudwash-1.1.4/setup.cfg`

 * *Files identical despite different names*

