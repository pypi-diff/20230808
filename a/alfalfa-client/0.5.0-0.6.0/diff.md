# Comparing `tmp/alfalfa_client-0.5.0.tar.gz` & `tmp/alfalfa_client-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfalfa_client-0.5.0.tar", max compression
+gzip compressed data, was "alfalfa_client-0.6.0.tar", max compression
```

## Comparing `alfalfa_client-0.5.0.tar` & `alfalfa_client-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1679 2022-03-30 21:50:10.989022 alfalfa_client-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     2086 2022-04-14 19:13:14.031011 alfalfa_client-0.5.0/README.md
--rw-r--r--   0        0        0     1900 2023-02-16 20:39:48.627142 alfalfa_client-0.5.0/alfalfa_client/__init__.py
--rw-r--r--   0        0        0    12035 2023-03-27 19:02:33.406759 alfalfa_client-0.5.0/alfalfa_client/alfalfa_client.py
--rw-r--r--   0        0        0     6226 2022-03-30 21:50:10.990747 alfalfa_client-0.5.0/alfalfa_client/historian.py
--rw-r--r--   0        0        0     4959 2023-03-27 19:02:33.407337 alfalfa_client-0.5.0/alfalfa_client/lib.py
--rw-r--r--   0        0        0      869 2023-03-20 14:41:46.640316 alfalfa_client-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 alfalfa_client-0.5.0/setup.py
--rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 alfalfa_client-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1679 2022-03-30 21:50:10.989022 alfalfa_client-0.6.0/LICENSE.txt
+-rw-r--r--   0        0        0     2086 2022-04-14 19:13:14.031011 alfalfa_client-0.6.0/README.md
+-rw-r--r--   0        0        0     1935 2023-08-08 15:52:01.621656 alfalfa_client-0.6.0/alfalfa_client/__init__.py
+-rw-r--r--   0        0        0    12239 2023-08-08 15:52:01.622678 alfalfa_client-0.6.0/alfalfa_client/alfalfa_client.py
+-rw-r--r--   0        0        0     6261 2023-08-08 15:52:01.624385 alfalfa_client-0.6.0/alfalfa_client/historian.py
+-rw-r--r--   0        0        0     4993 2023-08-08 15:52:01.625680 alfalfa_client-0.6.0/alfalfa_client/lib.py
+-rw-r--r--   0        0        0      881 2023-08-08 15:52:01.635655 alfalfa_client-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2872 1970-01-01 00:00:00.000000 alfalfa_client-0.6.0/setup.py
+-rw-r--r--   0        0        0     2809 1970-01-01 00:00:00.000000 alfalfa_client-0.6.0/PKG-INFO
```

### Comparing `alfalfa_client-0.5.0/LICENSE.txt` & `alfalfa_client-0.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alfalfa_client-0.5.0/README.md` & `alfalfa_client-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `alfalfa_client-0.5.0/alfalfa_client/__init__.py` & `alfalfa_client-0.6.0/alfalfa_client/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-"""
-****************************************************************************************************
-:copyright (c) 2008-2021 URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
-
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met:
-
-Redistributions of source code must retain the above copyright notice, this list of conditions
-and the following disclaimer.
-
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials provided with the
-distribution.
-
-Neither the name of the copyright holder nor the names of its contributors may be used to endorse
-or promote products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
-IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
-IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-****************************************************************************************************
-"""
+# ****************************************************************************************************
+# :copyright (c) 2008-2021 URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
+
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted
+# provided that the following conditions are met:
+
+# Redistributions of source code must retain the above copyright notice, this list of conditions
+# and the following disclaimer.
+
+# Redistributions in binary form must reproduce the above copyright notice, this list of conditions
+# and the following disclaimer in the documentation and/or other materials provided with the
+# distribution.
+
+# Neither the name of the copyright holder nor the names of its contributors may be used to endorse
+# or promote products derived from this software without specific prior written permission.
+
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
+# IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
+# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+# DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
+# IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+# OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# ****************************************************************************************************
+
 
 import pkg_resources
 
 from alfalfa_client.alfalfa_client import AlfalfaClient
 
 __version__ = pkg_resources.get_distribution('alfalfa-client').version
```

### Comparing `alfalfa_client-0.5.0/alfalfa_client/alfalfa_client.py` & `alfalfa_client-0.6.0/alfalfa_client/alfalfa_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""
-****************************************************************************************************
-:copyright (c) 2008-2021 URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
-
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met:
-
-Redistributions of source code must retain the above copyright notice, this list of conditions
-and the following disclaimer.
-
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials provided with the
-distribution.
-
-Neither the name of the copyright holder nor the names of its contributors may be used to endorse
-or promote products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
-IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
-IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-****************************************************************************************************
-"""
+# ****************************************************************************************************
+# :copyright (c) 2008-2021 URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
+
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted
+# provided that the following conditions are met:
+
+# Redistributions of source code must retain the above copyright notice, this list of conditions
+# and the following disclaimer.
+
+# Redistributions in binary form must reproduce the above copyright notice, this list of conditions
+# and the following disclaimer in the documentation and/or other materials provided with the
+# distribution.
+
+# Neither the name of the copyright holder nor the names of its contributors may be used to endorse
+# or promote products derived from this software without specific prior written permission.
+
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
+# IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
+# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+# DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
+# IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+# OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# ****************************************************************************************************
 
 import json
 import os
 from collections import OrderedDict
 from datetime import datetime
 from numbers import Number
 from time import sleep, time
@@ -50,22 +48,23 @@
 )
 
 ModelID = str
 SiteID = str
 
 
 class AlfalfaClient:
+    """AlfalfaClient is a wrapper for the Alfalfa REST API"""
 
     def __init__(self, host: str = 'http://localhost', api_version: str = 'v2'):
         """Create a new alfalfa client instance
 
         :param host: url for host of alfalfa web server
         :param api_version: version of alfalfa api to use (probably don't change this)
         """
-        self.host = host.lstrip('/')
+        self.host = host.rstrip('/')
         self.haystack_filter = self.host + '/haystack/read?filter='
         self.haystack_json_header = {
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         self.host = host
@@ -279,15 +278,18 @@
 
         :param site_id: id of site
         :returns: dictionary of output names and values"""
         response = self._request(f"sites/{site_id}/points/outputs", method="GET")
         response_body = response.json()
         outputs = {}
         for point in response_body["data"]:
-            outputs[point["name"]] = point["value"]
+            if "value" in point.keys():
+                outputs[point["name"]] = point["value"]
+            else:
+                outputs[point["name"]] = None
 
         return outputs
 
     @parallelize
     def get_sim_time(self, site_id: Union[SiteID, List[SiteID]]) -> datetime:
         """Get sim_time of site
```

### Comparing `alfalfa_client-0.5.0/alfalfa_client/historian.py` & `alfalfa_client-0.6.0/alfalfa_client/historian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
-"""
-****************************************************************************************************
-:copyright (c) 2008-2021 URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
-
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met:
-
-Redistributions of source code must retain the above copyright notice, this list of conditions
-and the following disclaimer.
-
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials provided with the
-distribution.
-
-Neither the name of the copyright holder nor the names of its contributors may be used to endorse
-or promote products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
-IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
-IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-****************************************************************************************************
-"""
+# ****************************************************************************************************
+# :copyright (c) 2008-2021 URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
+
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted
+# provided that the following conditions are met:
+
+# Redistributions of source code must retain the above copyright notice, this list of conditions
+# and the following disclaimer.
+
+# Redistributions in binary form must reproduce the above copyright notice, this list of conditions
+# and the following disclaimer in the documentation and/or other materials provided with the
+# distribution.
+
+# Neither the name of the copyright holder nor the names of its contributors may be used to endorse
+# or promote products derived from this software without specific prior written permission.
+
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
+# IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
+# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+# DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
+# IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+# OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# ****************************************************************************************************
+
 
 # Credit: Nicholas Long
 
 import os
 
 import pandas as pd
```

### Comparing `alfalfa_client-0.5.0/alfalfa_client/lib.py` & `alfalfa_client-0.6.0/alfalfa_client/lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-"""
-****************************************************************************************************
-:copyright (c) 2008-2021 URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
-
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without modification, are permitted
-provided that the following conditions are met:
-
-Redistributions of source code must retain the above copyright notice, this list of conditions
-and the following disclaimer.
-
-Redistributions in binary form must reproduce the above copyright notice, this list of conditions
-and the following disclaimer in the documentation and/or other materials provided with the
-distribution.
-
-Neither the name of the copyright holder nor the names of its contributors may be used to endorse
-or promote products derived from this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
-IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
-CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
-DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
-IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-****************************************************************************************************
-"""
+# ****************************************************************************************************
+# :copyright (c) 2008-2021 URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
+
+# All rights reserved.
+
+# Redistribution and use in source and binary forms, with or without modification, are permitted
+# provided that the following conditions are met:
+
+# Redistributions of source code must retain the above copyright notice, this list of conditions
+# and the following disclaimer.
+
+# Redistributions in binary form must reproduce the above copyright notice, this list of conditions
+# and the following disclaimer in the documentation and/or other materials provided with the
+# distribution.
+
+# Neither the name of the copyright holder nor the names of its contributors may be used to endorse
+# or promote products derived from this software without specific prior written permission.
+
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR
+# IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND
+# FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
+# CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+# DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
+# DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER
+# IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
+# OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+# ****************************************************************************************************
 
 import concurrent.futures
 import functools
 import shutil
 import tempfile
 from functools import partial
 from os import PathLike, path
```

### Comparing `alfalfa_client-0.5.0/pyproject.toml` & `alfalfa_client-0.6.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "alfalfa-client"
-version = "0.5.0"
+version = "0.6.0"
 description = "A standalone client for the NREL Alfalfa application"
 authors = [
     'Kyle Benne <kyle.benne@nrel.gov>',
     'Brian Ball <brian.ball@nrel.gov>',
     'Cory Mosiman <cory.mosiman@nrel.gov>',
     'Nicholas Long <nicholas.long@nrel.gov>',
     'Willy Bernal <willy.bernalheredia@nrel.gov>',
     'Yanfei Li <yanfei.li@nrel.gov>',
     'Tobias Shapinsky <tobias.shapinsky@nrel.gov>'
 ]
 readme = 'README.md'
 license = 'LICENSE.txt'
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = ">=3.8"
 
 hszinc = "~1.3"
 importlib-metadata = "~6.0"
 pandas = "~1.5"
 requests-toolbelt = "~0.10"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "~2.21"
 pytest = "~7.2"
 tox = "~4.1"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.21.2"
+sphinx = "^6.1.3"
+
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `alfalfa_client-0.5.0/setup.py` & `alfalfa_client-0.6.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 ['hszinc>=1.3,<1.4',
  'importlib-metadata>=6.0,<6.1',
  'pandas>=1.5,<1.6',
  'requests-toolbelt>=0.10,<0.11']
 
 setup_kwargs = {
     'name': 'alfalfa-client',
-    'version': '0.5.0',
+    'version': '0.6.0',
     'description': 'A standalone client for the NREL Alfalfa application',
     'long_description': '# Alfalfa Client\n\nThe purpose of this repository is to provide a standalone client for use with the Alfalfa application. It additionally includes a Historian to quickly/easily enable saving of results from Alfalfa simulations.\n\n# Usage\n\nThis repo is packaged and hosted on [PyPI here](https://pypi.org/project/alfalfa-client/).\n\n```bash\npip install alfalfa-client\n```\n\n```python\nimport alfalfa_client.alfalfa_client as ac\nimport alfalfa_client.historian as ah\n\nclient = ac.AlfalfaClient\nhistorian = ah.Historian\n```\n\n# Setup and Testing\n\nThis repository is setup to use:\n\n- [pyenv](https://github.com/pyenv/pyenv#installation) for managing python versions\n- [poetry](https://python-poetry.org/docs/#installation) for managing environment\n- [pre-commit](https://pre-commit.com/#install) for managing code styling\n- tox for running tests in isolated build environments. See the expected python versions in [tox.ini](./tox.ini)\n\nAssuming poetry is installed and the necessary python versions are installed, the following should exit cleanly:\n\n```bash\ngit clone https://github.com/NREL/alfalfa-client.git\ncd alfalfa-client\npoetry run tox\n```\n\nThis may take some time resolving on the initial run, but subsequent runs should be faster.\n\nSee [this gist](https://gist.github.com/corymosiman12/26fb682df2d36b5c9155f344eccbe404) for additional info.\n\n# History\n\n- The implemented client is previously referred to as Boptest, from the alfalfa/client/boptest.py implementation. It has been ported as a standalone package for easier usage across projects.\n\n# Releasing\n\n1. Merge all branches into develop, make sure tests pass\n1. Update the version (assume version is 0.1.2): `poetry version 0.1.2`\n1. Update the version test file (i.e. my-repo/tests/test_version.py) to match the above version\n1. Make sure tests pass: `poetry run tox`\n1. Merge develop into main (previously, master), make sure tests pass\n1. Create a tag: `git tag 0.1.2`\n1. Build: `poetry build`\n1. Publish `poetry publish` (this will push to pypi)\n1. Create a new release on the Github repository using the tag and link to PyPI\n',
     'author': 'Kyle Benne',
     'author_email': 'kyle.benne@nrel.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+    'python_requires': '>=3.8',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `alfalfa_client-0.5.0/PKG-INFO` & `alfalfa_client-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: alfalfa-client
-Version: 0.5.0
+Version: 0.6.0
 Summary: A standalone client for the NREL Alfalfa application
 License: LICENSE.txt
 Author: Kyle Benne
 Author-email: kyle.benne@nrel.gov
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: hszinc (>=1.3,<1.4)
 Requires-Dist: importlib-metadata (>=6.0,<6.1)
 Requires-Dist: pandas (>=1.5,<1.6)
 Requires-Dist: requests-toolbelt (>=0.10,<0.11)
 Description-Content-Type: text/markdown
 
 # Alfalfa Client
```

