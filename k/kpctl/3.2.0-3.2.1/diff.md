# Comparing `tmp/kpctl-3.2.0.tar.gz` & `tmp/kpctl-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpctl-3.2.0.tar", last modified: Mon Nov 14 10:22:49 2022, max compression
+gzip compressed data, was "kpctl-3.2.1.tar", max compression
```

## Comparing `kpctl-3.2.0.tar` & `kpctl-3.2.1.tar`

### file list

```diff
@@ -1,31 +1,19 @@
-drwxrwxr-x   0 tstephen  (1000) tstephen  (1000)        0 2022-11-14 10:22:49.994463 kpctl-3.2.0/
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)    11358 2022-07-07 18:16:28.000000 kpctl-3.2.0/LICENSE
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)       36 2022-07-07 18:16:28.000000 kpctl-3.2.0/MANIFEST.in
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)     1375 2022-11-14 10:22:49.994463 kpctl-3.2.0/PKG-INFO
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)      811 2022-11-14 08:45:58.000000 kpctl-3.2.0/README.md
-drwxrwxr-x   0 tstephen  (1000) tstephen  (1000)        0 2022-11-14 10:22:49.994463 kpctl-3.2.0/kpctl/
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)      809 2022-11-14 10:19:31.000000 kpctl-3.2.0/kpctl/__init__.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)     6908 2022-11-14 10:16:45.000000 kpctl-3.2.0/kpctl/__main__.py
-drwxrwxr-x   0 tstephen  (1000) tstephen  (1000)        0 2022-11-14 10:22:49.994463 kpctl-3.2.0/kpctl/bpmn/
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)        0 2022-11-14 08:40:20.000000 kpctl-3.2.0/kpctl/bpmn/__init__.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)     4175 2022-11-14 09:56:22.000000 kpctl-3.2.0/kpctl/bpmn/bpmn_documenter.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)    13426 2022-11-14 09:56:45.000000 kpctl-3.2.0/kpctl/bpmn/bpmn_editor.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)     5313 2022-11-14 10:04:22.000000 kpctl-3.2.0/kpctl/bpmn/bpmn_validator.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)     3910 2022-11-14 10:09:55.000000 kpctl-3.2.0/kpctl/configurator.py
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)     2489 2022-11-04 18:55:08.000000 kpctl-3.2.0/kpctl/constants.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)     1362 2022-11-04 18:55:08.000000 kpctl-3.2.0/kpctl/exceptions.py
-drwxrwxr-x   0 tstephen  (1000) tstephen  (1000)        0 2022-11-14 10:22:49.994463 kpctl-3.2.0/kpctl/exec/
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)        0 2022-11-14 08:40:51.000000 kpctl-3.2.0/kpctl/exec/__init__.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)     4423 2022-11-14 10:07:11.000000 kpctl-3.2.0/kpctl/exec/curl.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)    11626 2022-11-14 10:04:35.000000 kpctl-3.2.0/kpctl/exec/deployer.py
--rwxrwxr-x   0 tstephen  (1000) tstephen  (1000)     1907 2022-11-14 09:51:43.000000 kpctl-3.2.0/kpctl/local_cache.py
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)     1861 2022-11-04 18:55:08.000000 kpctl-3.2.0/kpctl/xml_support.py
-drwxrwxr-x   0 tstephen  (1000) tstephen  (1000)        0 2022-11-14 10:22:49.994463 kpctl-3.2.0/kpctl.egg-info/
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)     1375 2022-11-14 10:22:49.000000 kpctl-3.2.0/kpctl.egg-info/PKG-INFO
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)      526 2022-11-14 10:22:49.000000 kpctl-3.2.0/kpctl.egg-info/SOURCES.txt
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)        1 2022-11-14 10:22:49.000000 kpctl-3.2.0/kpctl.egg-info/dependency_links.txt
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)       47 2022-11-14 10:22:49.000000 kpctl-3.2.0/kpctl.egg-info/entry_points.txt
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)       45 2022-11-14 10:22:49.000000 kpctl-3.2.0/kpctl.egg-info/requires.txt
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)        6 2022-11-14 10:22:49.000000 kpctl-3.2.0/kpctl.egg-info/top_level.txt
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)       38 2022-11-14 10:22:49.994463 kpctl-3.2.0/setup.cfg
--rw-rw-r--   0 tstephen  (1000) tstephen  (1000)     1155 2022-11-14 10:19:12.000000 kpctl-3.2.0/setup.py
+-rw-r--r--   0        0        0    11358 2022-07-07 18:16:28.071920 kpctl-3.2.1/LICENSE
+-rw-r--r--   0        0        0      811 2023-06-14 22:52:33.885892 kpctl-3.2.1/README.md
+-rwxr-xr-x   0        0        0      808 2023-04-17 19:18:12.272703 kpctl-3.2.1/kpctl/__init__.py
+-rwxr-xr-x   0        0        0     7108 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-14 10:29:17.897510 kpctl-3.2.1/kpctl/bpmn/__init__.py
+-rwxr-xr-x   0        0        0     4206 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/bpmn/bpmn_documenter.py
+-rwxr-xr-x   0        0        0    13097 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/bpmn/bpmn_editor.py
+-rwxr-xr-x   0        0        0     5304 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/bpmn/bpmn_validator.py
+-rw-r--r--   0        0        0     1548 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/color_log_formatter.py
+-rwxr-xr-x   0        0        0     3781 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/configurator.py
+-rw-r--r--   0        0        0     2489 2022-11-04 18:55:08.133767 kpctl-3.2.1/kpctl/constants.py
+-rwxr-xr-x   0        0        0     1362 2022-11-04 18:55:08.133767 kpctl-3.2.1/kpctl/exceptions.py
+-rw-r--r--   0        0        0        0 2022-11-14 10:29:17.901510 kpctl-3.2.1/kpctl/exec/__init__.py
+-rwxr-xr-x   0        0        0     4001 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/exec/curl.py
+-rwxr-xr-x   0        0        0    10825 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/exec/deployer.py
+-rwxr-xr-x   0        0        0     1851 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/local_cache.py
+-rw-r--r--   0        0        0     1918 2023-08-08 12:21:21.149373 kpctl-3.2.1/kpctl/xml_support.py
+-rw-r--r--   0        0        0      558 2023-08-08 17:15:13.269710 kpctl-3.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1680 1970-01-01 00:00:00.000000 kpctl-3.2.1/PKG-INFO
```

### Comparing `kpctl-3.2.0/LICENSE` & `kpctl-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kpctl-3.2.0/README.md` & `kpctl-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `kpctl-3.2.0/kpctl/__init__.py` & `kpctl-3.2.1/kpctl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,9 +12,8 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations under
 #  the License.
 #
 ###############################################################################
-
 __version__ = '3.2.0'
```

### Comparing `kpctl-3.2.0/kpctl/__main__.py` & `kpctl-3.2.1/kpctl/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,40 +16,41 @@
 #
 # Command line client for managing process application lifecycle.
 #
 ###############################################################################
 import argparse
 from colorama import Fore, Back, Style
 from getpass import getpass
+import logging
 import sys
 
 import kpctl
 from kpctl.bpmn.bpmn_documenter import BpmDocumenter
 from kpctl.bpmn.bpmn_editor import BpmnEditor
 from kpctl.bpmn.bpmn_validator import BpmnValidator
 from kpctl.exec.curl import Curl
 from kpctl.configurator import Configurator
 from kpctl.exec.deployer import BpmDeployer
 from kpctl.exceptions import KpException
 from kpctl.local_cache import cache
 
+from kpctl.color_log_formatter import ColorFormatter
+
 def help(parser):
     print('{} {}'.format(kpctl.__name__, kpctl.__version__))
     parser.print_help()
 
 def main():
     '''Main entry point to kpctl'''
 
     parser = argparse.ArgumentParser(prog="kpctl", add_help=False)
     parser.add_argument("-f", "--force", help="overwrite existing files",
         action="store_true")
     parser.add_argument("-v", "--verbose", help="increase output verbosity",
-        action="store_true")
-    parser.add_argument("-X", "--debug", help="extra verbose output for debugging",
-        action="store_true")
+        type=int, default=logging.WARNING, required=False)
     subparser = parser.add_subparsers(dest="cmd")
 
     subparser.add_parser('cache', help='cache resources used elsewhere')
 
     validate_parser = subparser.add_parser('validate', help='validate (esp. bpmn)')
     validate_parser.add_argument("input", help="source file or folder")
 
@@ -104,14 +105,21 @@
 
     subparser.add_parser('help', help='show this help')
 
     # custom help message
     parser._positionals.title = "commands"
 
     args = parser.parse_args()
+
+    # create console handler with coloured output
+    ch = logging.StreamHandler()
+    ch.setLevel(args.verbose)
+    ch.setFormatter(ColorFormatter())
+    logging.basicConfig(level=args.verbose, handlers=[ ch ])
+
     configurator = Configurator(args)
     documenter = BpmDocumenter(args)
     validator = BpmnValidator(args)
     editor = BpmnEditor(args)
     deployer = BpmDeployer(args, configurator, validator)
     curl = Curl(args, configurator)
```

### Comparing `kpctl-3.2.0/kpctl/bpmn/bpmn_documenter.py` & `kpctl-3.2.1/kpctl/bpmn/bpmn_documenter.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,84 +13,83 @@
 #  License for the specific language governing permissions and limitations under
 #  the License.
 #
 # Command line client for managing process application lifecycle.
 #
 ###############################################################################
 from cairosvg import svg2png
+import logging
 import lxml.etree as ET
 import os
 import requests
 from kpctl.constants import NS
 
 from kpctl.xml_support import write_pretty_xml
 
 XSLT_PROC_RENDERER = 'http://modeler.knowprocess.com/xslt/bpmn2svg.xslt'
 
 class BpmDocumenter():
     def __init__(self, options):
         self.options = options
 
     def document(self, input_):
-        if self.options.verbose:
-            print('generating documentation...')
+        logging.info('generating documentation...')
 
         if input_.endswith('.bpmn'):
-            self.generate_proc_image(input_)
+            self.generate_proc_images(input_)
         elif input_.endswith('.form'):
             self.generate_form_image(input_)
         else:
             for root, dirs, files in os.walk(input_):
                 for file in files:
                     if file.endswith('.bpmn'):
-                        self.generate_proc_image(root+'/'+file)
+                        self.generate_proc_images(root+'/'+file)
                     elif file.endswith('.form'):
                         self.generate_form_image(root+'/'+file)
 
-        if self.options.verbose:
-            print('...done')
+        logging.info('...done')
 
     def generate_form_image(self, form_file):
-        if self.options.verbose:
-            print('  generating image for ...'+form_file)
-            print('  ...not yet implemented...')
-
-    def generate_proc_image(self, bpmn_file):
-        if self.options.verbose:
-            print('  generating image for ...'+bpmn_file)
+        logging.warning(f'  generating image for {form_file} not yet implemented.')
+
+    def generate_proc_image(self, bpmn_file, dom, diag_id, diag_count, cur_diag_pos, lang=None):
+        logging.info(f'  generating image for {bpmn_file}')
 
-        dom = ET.parse(bpmn_file)
         res = requests.get(XSLT_PROC_RENDERER)
         xslt = ET.fromstring(res.content)
         transform = ET.XSLT(xslt)
+        if lang == None:
+            newdom = transform(dom, diagramId=ET.XSLT.strparam(diag_id))
+        else:
+            newdom = transform(dom, diagramId=ET.XSLT.strparam(diag_id),
+                                lang=ET.XSLT.strparam(lang))
+        if diag_count == 1:
+            write_pretty_xml(f'{bpmn_file}.svg', newdom)
+        else:
+            write_pretty_xml(f'{bpmn_file}.{cur_diag_pos}.svg', newdom)
+        try:
+            lang_suffix = '' if lang == None else f'.{lang}'
+            if diag_count == 1:
+                svg2png(bytestring=ET.tostring(newdom, encoding='unicode'), write_to=f'{bpmn_file}{lang_suffix}.png')
+            else:
+                svg2png(bytestring=ET.tostring(newdom, encoding='unicode'), write_to=f'{bpmn_file}{lang_suffix}.{cur_diag_pos}.png')
+        except KeyError as e:
+            logging.error(f'  ... unable to render { diag_id} from {bpmn_file} in {lang} translation, cause is {e} ', exc_info=True)
+        except Exception as e:
+            logging.error(f'  ... unable to render {diag_id} from {bpmn_file}, optional language is {lang}, cause is {e} ', exc_info=True)
+
+    def generate_proc_images(self, bpmn_file):
+        logging.info(f'  generating image for {bpmn_file}')
+
+        dom = ET.parse(bpmn_file)
         diags = dom.findall('//bpmndi:BPMNDiagram', NS)
         for count, diag in enumerate(diags):
-            if self.options.verbose:
-                print('found diag {}'.format(diag.get('id')))
-            newdom = transform(dom, diagramId=ET.XSLT.strparam(diag.get('id')))
-            #newdom = transform(dom)
-            write_pretty_xml(bpmn_file+'.'+str(count+1)+'.svg', newdom)
-            try:
-                svg2png(bytestring=ET.tostring(newdom, encoding='unicode'), write_to=bpmn_file+'.png')
-            except Exception as e:
-                print('  ... unable to create png of the process: {}'.format(e))
+            logging.info(f'found diag {diag.get("id")}')
+            self.generate_proc_image(bpmn_file, dom, diag.get('id'), len(diags), count+1)
 
             # now generate language variants
-            try:
-                langs = dom.findall('//i18n:translation[@xml:lang]', NS)
-                langs = set(map(lambda x : x.get('{http://www.w3.org/XML/1998/namespace}lang'), langs))
-                if (len(langs)>0):
-                    if self.options.verbose:
-                        print('  detected the following languages: "{}"'.format(langs))
-                    for l in langs:
-                        if self.options.verbose:
-                            print("    generating localised '%s' image ..." % l)
-                        newdom = transform(dom, diagramId=ET.XSLT.strparam(diag.get('id')),
-                                           lang=ET.XSLT.strparam(l))
-                        write_pretty_xml(bpmn_file+'.'+str(count+1)+'.'+l+'.svg', newdom)
-                        svg2png(bytestring=ET.tostring(newdom, encoding='unicode'), write_to=bpmn_file+'.'+l+'.png')
-                else:
-                    if self.options.verbose:
-                        print('  ... no translations found to document')
-            except KeyError as e:
-                if self.options.verbose:
-                    print('  ... unable to render translations: {} '.format(e))
+            langs = dom.findall('//i18n:translation[@xml:lang]', NS)
+            langs = set(map(lambda x : x.get('{http://www.w3.org/XML/1998/namespace}lang'), langs))
+            logging.idebug(f'  detected the following languages: "{langs}"')
+            for l in langs:
+                logging.info("    generating localised '{l}' image ...")
+                self.generate_proc_image(bpmn_file, dom, diag.get('id'), len(diags), count+1, l)
```

### Comparing `kpctl-3.2.0/kpctl/bpmn/bpmn_editor.py` & `kpctl-3.2.1/kpctl/bpmn/bpmn_editor.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #  the License.
 #
 # Command line client for managing process application lifecycle.
 #
 ###############################################################################
 import colorama
 from colorama import Fore, Style
+import logging
 import lxml.etree as ET
 import os
 
 from kpctl.constants import APP_NAME, NS
 import kpctl
 from kpctl.xml_support import local_tag, write_pretty_xml
 
@@ -35,16 +36,15 @@
         else:
             for root, dirs, files in os.walk(input_):
                 for file_ in files:
                     if file_.endswith('.bpmn'):
                         self.describe_from_file(id_, root+'/'+file_)
 
     def describe_from_file(self, id_, bpmn_file):
-        if self.options.verbose:
-            print('describing {} within {} ...'.format(id_, bpmn_file))
+        logging.info(f'describing {id_} within {bpmn_file} ...')
         colorama.init()
 
         dom = ET.parse(bpmn_file)
         objs = dom.findall("//*[@id='{}']".format(id_), NS)
         for obj in objs:
             ltag = local_tag(obj)
             print('  {}{}{}:{} {}'.format(Style.BRIGHT, Fore.GREEN,
@@ -133,16 +133,15 @@
         else:
             for root, dirs, files in os.walk(input_):
                 for file_ in files:
                     if file_.endswith('.bpmn'):
                         self.get_from_file(type_, root+'/'+file_)
 
     def get_from_file(self, type_, bpmn_file):
-        if self.options.verbose:
-            print('finding {} within {} ...'.format(type_, bpmn_file))
+        logging.info(f'finding {type_} within {bpmn_file} ...')
         colorama.init()
 
         dom = ET.parse(bpmn_file)
         objs = dom.findall('//{}'.format((type_, 'bpmn:'+type_) [type_.find(':')==-1]), NS)
         for obj in objs:
             print('  {}{}{}: {}'.format(Fore.GREEN, obj.attrib['id'],
                                         Style.RESET_ALL,
@@ -154,25 +153,23 @@
         else:
             for root, dirs, files in os.walk(input_):
                 for file_ in files:
                     if file_.endswith('.bpmn'):
                         self.set_in_file(id_, target, value, root+'/'+file_)
 
     def set_in_file(self, id_, target, value, bpmn_file):
-        if self.options.verbose:
-            print('setting {} of {} to {} ...'.format(target, id_, value))
+        logging.info(f'setting {target} of {id_} to {value} ...')
 
         dom = ET.parse(bpmn_file)
         obj = dom.find("//*[@id='{}']".format(id_), NS)
 
-        if (target.find(':') > -1):
+        if target.find(':') > -1:
             target = '{'+NS[target[0:target.find(':')]]+'}'+target[target.find(':')+1:]
-        if (obj == None):
-            if self.options.verbose:
-                print('  object not found')
+        if obj == None:
+            logging.warning('  object not found')
         else:
             obj.set(target, value)
             self.write_kp_bpmn(bpmn_file, dom)
 
             # add any missing implementation extensions
             if target == 'implementation' and value == 'kp:http':
                 self.set_ext_if_missing(id_, 'requestMethod', 'GET', bpmn_file)
@@ -189,29 +186,28 @@
                 self.set_ext_if_missing(id_, 'decisionTaskThrowErrorOnNoHits', 'false', bpmn_file)
 
     def set_ext_if_missing(self, id_, target, value, bpmn_file):
         dom = ET.parse(bpmn_file)
         obj = dom.find("//*[@id='{}']/bpmn:extensionElements/*[@name='{}']".format(id_, target), NS)
         if (obj is None):
             self.set_ext(id_, target, value, bpmn_file)
-        elif self.options.verbose:
-            print('  {} already has {} extension, skipping set'.format(id_, target))
+        else:
+            logging.warning(f'  {id_} already has {target} extension, skipping set')
 
     def set_ext(self, id_, target, value, input_):
         if input_.endswith('.bpmn'):
             self.set_ext_in_file(id_, target, value, input_)
         else:
             for root, dirs, files in os.walk(input_):
                 for file_ in files:
                     if file_.endswith('.bpmn'):
                         self.set_ext_in_file(id_, target, value, root+'/'+file_)
 
     def set_ext_in_file(self, id_, target, value, bpmn_file):
-        if self.options.verbose:
-            print('set extension {} of {} to {} ...'.format(target, id_, value))
+        logging.info(f'set extension {target} of {id_} to {value} ...')
 
         dom = ET.parse(bpmn_file)
         obj = dom.find("//*[@id='{}']/bpmn:extensionElements/*[@name='{}']".format(id_, target), NS)
         if (obj is None):
             exts = dom.find("//*[@id='{}']/bpmn:extensionElements".format(id_), NS)
             ext = ET.SubElement(exts, ('{%s}field' % NS['kp']))
             ext.set('name', target)
@@ -237,33 +233,30 @@
         else:
             for root, dirs, files in os.walk(input_):
                 for file_ in files:
                     if file_.endswith('.bpmn'):
                         self.set_res_in_file(id_, value, root+'/'+file_)
 
     def set_res_in_file(self, id_, value, bpmn_file):
-        if self.options.verbose:
-            print('set resource of {} to {} ...'.format(id_, value))
+        logging.info(f'set resource of {id_} to {value} ...')
 
         dom = ET.parse(bpmn_file)
         obj = dom.find("//*[@id='{}']/bpmn:potentialOwner".format(id_), NS)
         if (obj is None):
-            if self.options.verbose:
-                print('  creating new potentialOwner {} ...'.format(value))
+            logging.info(f'  creating new potentialOwner {value} ...')
             task = dom.find("//*[@id='{}']".format(id_), NS)
             po = ET.SubElement(task, ('{%s}potentialOwner' % NS['bpmn']))
             resExpr = ET.SubElement(po, ('{%s}resourceAssignmentExpression' % NS['bpmn']))
             expr = ET.SubElement(resExpr, ('{%s}formalExpression' % NS['bpmn']))
             expr.text = value
             resExpr.append(expr)
             po.append(resExpr)
             task.append(po)
         else:
-            if self.options.verbose:
-                print('  updating existing potentialOwner to {} ...'.format(value))
+            logging.info(f'  updating existing potentialOwner to {value} ...')
             dom.find("//*[@id='{}']/bpmn:potentialOwner//bpmn:formalExpression".format(id_), NS).text = value
         self.write_kp_bpmn(bpmn_file, dom)
 
     def write_kp_bpmn(self, path, dom):
         dom.getroot().set('exporter', APP_NAME)
         dom.getroot().set('exporterVersion', kpctl.__version__)
         write_pretty_xml(path, dom)
```

### Comparing `kpctl-3.2.0/kpctl/bpmn/bpmn_validator.py` & `kpctl-3.2.1/kpctl/bpmn/bpmn_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #  the License.
 #
 # Command line client for managing process application lifecycle.
 #
 ###############################################################################
 import colorama
 from colorama import Fore, Style
+import logging
 import lxml.etree as ET
 import os
 
 from kpctl.constants import NS
 from kpctl.exceptions import Error, KpException
 from kpctl.local_cache import CACHE_DIR, cache
 from kpctl.xml_support import transform
@@ -32,62 +33,63 @@
 
 class BpmnValidator():
     def __init__(self, options):
         self.options = options
 
     def validate(self, input_):
         cache(self.options)
-        if self.options.verbose:
-            print('validating...')
+        logging.info('validating...')
 
         if input_.endswith('.bpmn'):
             self.validate_bpmn(input_)
         else:
             proc_ids = []
             for root, dirs, files in os.walk(input_):
                 for file_ in files:
                     if file_.endswith('.bpmn') and not(file_.endswith('.kp.bpmn')):
                         self.validate_bpmn(root+'/'+file_)
                         dom = ET.parse(root+'/'+file_)
                         for proc in dom.findall('//bpmn:process[@isExecutable="true"]', NS):
                             proc_id = proc.attrib['id']
                             if proc_ids.count(proc_id):
-                                print('ERROR: More than one file contains process with id %s' % (proc_id))
+                                logging.error(f'More than one file contains process with id {proc_id}')
                                 raise KpException(Error.IMPL_DUPE_ID)
                             else:
                                 proc_ids.append(proc_id)
 
-        if self.options.verbose:
-            print('...done')
+        logging.info('...done')
 
     def validate_bpmn(self, bpmn_file):
-        if self.options.verbose:
-            print('  validating ...'+bpmn_file)
+        logging.info(f'  validating ...{bpmn_file}')
         colorama.init()
 
         try:
             issues = self.validate_xsd(bpmn_file)
             if issues[0:5] == 'ERROR':
                 print(issues)
 
             issues += str(transform(XSLT_VALIDATOR, bpmn_file, self.options))
             issues += str(transform(XSLT_EXT_VALIDATOR, bpmn_file, self.options))
 
             issueArr = issues.split('\n')
             errs = list(filter(lambda issue: issue[0:5] == 'ERROR', issueArr))
-            print('\n'.join(errs).replace('ERROR',Fore.RED + 'ERROR' + Style.RESET_ALL))
+            for err in errs:
+                logging.error(err.replace('ERROR: ', ''))
             warns = list(filter(lambda issue: issue[1:5] == 'WARN', issueArr))
-            print('\n'.join(warns).replace('WARN',Fore.YELLOW + 'WARN' + Style.RESET_ALL))
+            for warning in warns:
+                logging.warning(warning.replace('WARN: ', '').strip())
             infos = list(filter(lambda issue: issue[1:5] == 'INFO', issueArr))
+            logging.debug(f'found {len(infos)} information messages')
             debugs = list(filter(lambda issue: issue[0:5] == 'DEBUG', issueArr))
+            logging.debug(f'found {len(debugs)} debug messages')
 
-            if self.options.verbose:
-                print('\n'.join(infos).replace('INFO',Fore.GREEN+ 'INFO' + Style.RESET_ALL))
-            if self.options.debug:
-                print('\n'.join(debugs).replace('DEBUG',Fore.GREEN+ 'DEBUG' + Style.RESET_ALL))
+            for info in infos:
+                logging.info(info.replace('INFO: ', ''))
+            for debug in debugs:
+                logging.debug(debug.replace('DEBUG: ', ''))
             print('\n  %s %s schema valid and has %d errors, %d warnings and %d messages.'
                 % (bpmn_file, ('is' if 'is schema valid' in issueArr[0] else 'is not'),
                     len(errs), len(warns), len(infos)))
             if len(errs) > 0:
                 raise KpException(Error.DEPLOYMENT_INVALID)
         except ET.XMLSyntaxError as e:
             issue = "ERROR: file '%s' is not well-formed XML, individual issues follow:\n" % (bpmn_file)
```

### Comparing `kpctl-3.2.0/kpctl/configurator.py` & `kpctl-3.2.1/kpctl/configurator.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 #  the License.
 #
 # Command line client for managing process application lifecycle.
 #
 ###############################################################################
 import configparser
 from configparser import ConfigParser
+import logging
 import os
 from pathlib import Path
 
 from kpctl.exceptions import Error, KpException
 
 class Configurator():
     CFG_DIR_DEFAULT=Path.home().joinpath('.config')
@@ -49,47 +50,43 @@
         self.options = options
 
     def read_config(self, key):
         """Read the local configuration"""
 
         cfg_file = self.CFG_FILE
         try:
-            if self.options.verbose:
-                print('CONFIG DIR > ', os.environ['XDG_CONFIG_HOME'])
+            logging.info(f'CONFIG DIR > {os.environ["XDG_CONFIG_HOME"]}')
             cfg_file = Path.joinpath(os.environ['XDG_CONFIG_HOME'], self.CFG_FILE)
         except KeyError:
-            if self.options.verbose:
-                print('$XDG_CONFIG_HOME not set, fall back to ~/.config/')
+            logging.info(f'$XDG_CONFIG_HOME not set, fall back to ~/.config/')
             if not(os.path.isdir(self.CFG_DIR_DEFAULT)):
                 os.mkdir(self.CFG_DIR_DEFAULT)
             cfg_file = Path.joinpath(self.CFG_DIR_DEFAULT, self.CFG_FILE)
 
         if cfg_file.is_file():
-            if self.options.verbose:
-                print('reading configuration [{}]'.format(key))
+            logging.info(f'reading configuration [{key}]')
             config = ConfigParser()
             try:
                 config.read(str(cfg_file))
 
                 self.auth_type = config.get(key, 'auth_type')
                 self.auth_url = config.get(key, 'auth_url') if 'auth_url' in config[key] else ''
                 self.client_id = config.get(key, 'client_id') if 'client_id' in config[key] else ''
                 self.client_secret = config.get(key, 'client_secret') if 'client_secret' in config[key] else ''
                 self.username = config.get(key, 'username')
                 self.password = config.get(key, 'password')
                 self.url = config.get(key, 'url')
-                if self.options.verbose:
-                    print('... authentication type: {} ...'.format(self.auth_type))
-                    print('... credentials {}:**** ...'.format(self.username))
+                logging.info(f'... authentication type: {self.auth_type} ...')
+                logging.into(f'... credentials {self.username}:**** ...')
             except configparser.NoSectionError as e:
-                print("ERROR: No section named '{}' in config file".format(key))
+                logging.error(f"  ... No section named '{key}' in config file", exc_info=True)
                 raise KpException(Error.DEPLOY_BAD_CONFIG)
             except configparser.NoOptionError as e:
-                print("ERROR: reading section named '{}' in config file, detail: {}".format(key, e))
+                logging.error(f"  ... reading section named '{key}' in config file", exc_info=True)
                 raise KpException(Error.DEPLOY_BAD_CONFIG)
         else:
-            print('no config file {} found, initialising a default...'.format(self.CFG_FILE))
+            logging.warning(f'no config file {self.CFG_FILE} found, initialising a default...')
             file = open(cfg_file, 'w')
             file.write(self.CFG_TEMPLATE)
             file.close()
             os.chmod(cfg_file, 0o600)
             raise KpException(Error.DEPLOY_BAD_CONFIG)
```

### Comparing `kpctl-3.2.0/kpctl/constants.py` & `kpctl-3.2.1/kpctl/constants.py`

 * *Files identical despite different names*

### Comparing `kpctl-3.2.0/kpctl/exceptions.py` & `kpctl-3.2.1/kpctl/exceptions.py`

 * *Files identical despite different names*

### Comparing `kpctl-3.2.0/kpctl/exec/deployer.py` & `kpctl-3.2.1/kpctl/exec/deployer.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #  License for the specific language governing permissions and limitations under
 #  the License.
 #
 # Command line client for managing process application lifecycle.
 #
 ###############################################################################
 import glob
+import logging
 import lxml.etree as ET
 import os
 from os.path import basename
 from os.path import exists
 import requests
 from requests.auth import HTTPBasicAuth
 from zipfile import ZipFile
@@ -108,62 +109,53 @@
 
     def __init__(self, options, configurator, validator):
         self.options = options
         self.configurator = configurator
         self.validator = validator
 
     def deploy(self, app, target):
-        if self.options.verbose:
-            print('deploying {} to {} ...'.format(app, target))
+        logging.info(f'deploying {app} to {target} ...')
 
         if not app.endswith('bar') and not app.endswith('zip'):
-            if self.options.verbose:
-                print('... cannot deploy \''+app+'\', must be .bar or .zip')
+            logging.info(f'... cannot deploy {app}, must be .bar or .zip')
             raise KpException(Error.DEPLOY_UNSUPPORTED_APP)
 
         self.configurator.read_config(target)
         if self.configurator.auth_type == 'Basic':
             r = requests.post(self.get_deployment_api(self.configurator.url), data={'file':app},
                 files={'file': open(app, 'rb')},
                 auth = HTTPBasicAuth(self.configurator.username, self.configurator.password))
             if r.status_code <= 400:
-                if self.options.verbose:
-                    print('...done, status: '+str(r.status_code))
+                logging.info(f'...done, status: '+str(r.status_code))
             else:
-                if self.options.verbose:
-                    print('...error: '+str(r.status_code))
+                logging.info(f'...error: '+str(r.status_code))
                 raise KpException(Error.DEPLOY_FAILED)
         else:
-            if self.options.verbose:
-                print('... unsupported authentication type {}'.format(self.configurator.auth_type))
+            logging.info(f'... unsupported authentication type {self.configurator.auth_type}')
             raise KpException(Error.DEPLOY_UNSUPPORTED_AUTH_TYPE)
 
     def generate_app(self, root):
         appPath = '%s/%s.app' % (root, root)
         if exists(appPath) and not(self.options.force):
-            if self.options.verbose:
-                print("  ... app '%s' already exists, --force to overwrite" % appPath)
+            logging.warning(f"  ... app '{appPath}' already exists, --force to overwrite")
         else:
             count = 0
             for filename in glob.glob(root+"/*.app"):
-                if self.options.verbose:
-                    print("  ... found '%s', not generating another app descriptor" % filename)
+                logging.info(f"  ... found '%s', not generating another app descriptor" % filename)
                 count += 1
 
             if count == 0:
-                if self.options.verbose:
-                    print('  generating app at %s ...' % root)
+                logging.info(f'  generating app at %s ...' % root)
                 file = open(appPath, 'w')
                 key = root[0:1].upper() + root[1:]
                 file.write(TEMPLATE_APP_DESCRIPTOR % (key, key))
                 file.close()
 
     def generate_forms(self, bpmn_file):
-        if self.options.verbose:
-            print('  generating forms for ...'+bpmn_file)
+        logging.info(f'  generating forms for ...'+bpmn_file)
 
         dom = ET.parse(bpmn_file)
         for startEvent in dom.findall('//bpmn:startEvent', NS):
             self.generate_form(bpmn_file, dom, startEvent)
         for userTask in dom.findall('//bpmn:userTask', NS):
             self.generate_form(bpmn_file, dom, userTask)
 
@@ -171,109 +163,95 @@
         name = bpmn_obj.get('name')
         formKey = bpmn_obj.get('{http://knowprocess.com/bpmn}formKey')
         if formKey == None:
             formKey = bpmn_obj.get('{http://flowable.org/bpmn}formKey')
         formPath = '%s/%s.form' % (bpmn_file[:bpmn_file.rfind('/')], formKey)
 
         if formKey == None:
-            if self.options.verbose:
-                print("  ... found %s '%s', but it has no formKey"
-                    % (local_tag(bpmn_obj), name))
+            logging.warning(f"  ... found {local_tag(bpmn_obj)} '{name}', but it has no formKey")
         elif exists(formPath) and not(self.options.force):
-            if self.options.verbose:
-                print("  ... found %s '%s', but form already exists with key '%s' --force to overwrite"
-                    % (local_tag(bpmn_obj), name, formKey))
+            logging.warning(f"  ... found {local_tag(bpmn_obj)} '{name}', but form already exists with key '{formKey}' --force to overwrite")
         else:
             print("  ... generating stub form '%s'" % formKey)
             fields = ''
             data_inputs = dom.findall('//bpmn:process/bpmn:ioSpecification/bpmn:dataInput', NS) if (local_tag(bpmn_obj) == 'startEvent') else dom.findall('//*[@id="{}"]//bpmn:dataInput'.format(bpmn_obj.get('id')), NS)
             for count, data_input in enumerate(data_inputs):
                 fields += TEMPLATE_FORM_FIELD % (camel_case(data_input.get('name')),
                                                 data_input.get('name'))
                 if (count+1 < len(data_inputs)):
                     fields += ','
             file = open(formPath, 'w')
             file.write(TEMPLATE_FORM % (formKey, formKey if name == None else name, fields))
             file.close()
 
     def generate_proc_executable(self, bpmn_file):
-        if self.options.verbose:
-            print('  generating executable process for %s ...' % bpmn_file)
+        logging.info(f'  generating executable process for %s ...' % bpmn_file)
 
         fileStart = int(bpmn_file.rfind('/'))+1
         implPath = '%s/%s.kp.bpmn' % (bpmn_file[:fileStart], bpmn_file[fileStart:bpmn_file.rfind('.')]) if fileStart > 0 else ('%s.kp.bpmn' % bpmn_file[:bpmn_file.rfind('.')])
         if exists(implPath):
-            if self.options.verbose:
-                print("  ... overwriting executable process '%s' ..." % (implPath))
+            logging.warning(f"  ... overwriting executable process '{implPath}' ...")
 
         dom = ET.parse(bpmn_file)
         res = requests.get(XSLT_PROC_ENHANCER)
         xslt = ET.fromstring(res.content)
         transform = ET.XSLT(xslt)
         write_pretty_xml(implPath, transform(dom, unsupportedTasksToUserTask=ET.XSLT.strparam('false')))
 
     def get_deployment_api(self, target):
-        if self.options.verbose:
-            print('deploying to {}{}...'.format(target, self.DEPLOYMENT_API))
+        logging.info(f'deploying to {target}{self.DEPLOYMENT_API}...')
 
         return target+self.DEPLOYMENT_API
 
     def implement(self, input_):
-        if self.options.verbose:
-            print('generating implementation hints...')
+        logging.info(f'generating implementation hints...')
 
         if input_.endswith('.bpmn'):
             self.generate_forms(input_)
             if not input_.endswith('.kp.bpmn'):
                 self.generate_proc_executable(input_)
         else:
             for root, dirs, files in os.walk(input_):
                 self.generate_app(root)
                 for file_ in files:
                     if file_.endswith('.bpmn'):
                         self.generate_forms(root+'/'+file_)
                         if not file_.endswith('.kp.bpmn'):
                             self.generate_proc_executable(root+'/'+file_)
 
-        if self.options.verbose:
-            print('...done')
+        logging.info(f'...done')
 
     def is_executable(self, file_name):
         if (file_name.endswith('kp.bpmn')):
             dom = ET.parse(file_name)
             return dom.findall('//bpmn:process[@isExecutable="true"]', NS)
         else:
             exts_inc = tuple(['app', 'form', 'md', 'txt'])
             return file_name.endswith(exts_inc)
 
     # Zip the files from given directory that matches the filter
     def zipFilesInDir(self, dirName, zipFileName, filter):
         zipFileName = zipFileName if zipFileName.endswith('.zip') else zipFileName+'.zip'
-        if self.options.verbose:
-            print('packaging {} from {} ...'.format(zipFileName, dirName))
+        logging.info(f'packaging {zipFileName} from {dirName} ...')
         # create a ZipFile object
         with ZipFile(zipFileName, 'w') as zipObj:
             # Iterate over all the files in directory
             for folderName, subfolders, filenames in os.walk(dirName):
                 for filename in filenames:
                     if filter(filename):
                         # create complete filepath of file in directory
                         filePath = os.path.join(folderName, filename)
-                        # Add file to zip
-                        if self.options.verbose:
-                            print('  adding: {}'.format(filePath))
+                        logging.info(f'  adding: {filePath}')
                         zipObj.write(filePath, basename(filePath))
 
     def package(self, dir_name, file_name):
 
         self.validator.validate(dir_name)
         self.implement(dir_name)
 
         if file_name == None or len(file_name) == 0:
             file_name = dir_name[:(len(dir_name)-1)] if dir_name.endswith('/') else dir_name
-            if self.options.verbose:
-                print('defaulted file_name to {}'.format(file_name))
+            logging.info(f'defaulted file_name to {file_name}')
 
         self.zipFilesInDir(dir_name, file_name, lambda name : self.is_executable(os.path.join(dir_name, name)))
 
-        if self.options.verbose:
-            print('...done')
+        logging.info(f'...done')
```

### Comparing `kpctl-3.2.0/kpctl/local_cache.py` & `kpctl-3.2.1/kpctl/local_cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,42 +12,40 @@
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations under
 #  the License.
 #
 # Command line client for managing process application lifecycle.
 #
 ###############################################################################
+import logging
 import os
 from os.path import exists
 from os import mkdir
 import requests
 
 from kpctl.constants import XSD_BPMN, XSD_BPMNDI, XSD_DC, XSD_DI, XSD_SEMANTIC
 
 CACHE_DIR = os.path.expanduser('~') + '/.kp'
 
 def cache(options):
-    if options.verbose:
-        print('caching external resources...')
+    logging.info('caching external resources...')
 
     if not(exists(CACHE_DIR)):
         mkdir(CACHE_DIR, 0o755)
         if not(exists(CACHE_DIR + '/xsd')):
             mkdir(CACHE_DIR + '/xsd', 0o755)
 
     cache_file(XSD_BPMN, CACHE_DIR + '/xsd/BPMN20.xsd', options)
     cache_file(XSD_BPMNDI, CACHE_DIR + '/xsd/BPMNDI.xsd', options)
     cache_file(XSD_DC, CACHE_DIR + '/xsd/DC.xsd', options)
     cache_file(XSD_DI, CACHE_DIR + '/xsd/DI.xsd', options)
     cache_file(XSD_SEMANTIC, CACHE_DIR + '/xsd/Semantic.xsd', options)
 
-    if options.verbose:
-        print('... done.')
+    logging.info('... done.')
 
 def cache_file(url, file_path, options):
     if not(exists(file_path)):
-        if options.verbose:
-            print('...%s...' % (file_path))
+        logging.info(f'...{file_path}...')
 
         file = open(file_path, 'wb')
         file.write(requests.get(url).content)
         file.close()
```

### Comparing `kpctl-3.2.0/kpctl/xml_support.py` & `kpctl-3.2.1/kpctl/xml_support.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,31 +12,31 @@
 #  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #  License for the specific language governing permissions and limitations under
 #  the License.
 #
 # Command line client for managing process application lifecycle.
 #
 ###############################################################################
-
+import logging
 import lxml.etree as ET
 import requests
 from xml.dom.minidom import parseString
 
 def local_tag(obj):
     return (obj.tag[obj.tag.find('}')+1:], obj.tag) [obj.tag.find('}')==-1]
 
 def transform(xsl_file, xml_file, options):
     dom = ET.parse(xml_file)
     res = requests.get(xsl_file)
     xslt = ET.fromstring(res.content)
     try:
       transform = ET.XSLT(xslt)
     except Exception as e:
-      print(e)
-    if options.debug:
+      logging.error(f'e', exc_info=True)
+    if options.verbose < logging.INFO:
       return transform(dom, verbosity="0")
     else:
       # collect all (v=1) and let decide calling func decide what to report
       return transform(dom, verbosity="1")
 
 def write_pretty_xml(path, dom):
     # despite many examples of parsing pretty_print=True to ET.tostring
```

