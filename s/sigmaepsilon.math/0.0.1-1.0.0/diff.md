# Comparing `tmp/sigmaepsilon.math-0.0.1.tar.gz` & `tmp/sigmaepsilon.math-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon.math-0.0.1.tar", last modified: Wed Jul 12 16:40:02 2023, max compression
+gzip compressed data, was "sigmaepsilon.math-1.0.0.tar", last modified: Tue Aug  8 16:19:54 2023, max compression
```

## Comparing `sigmaepsilon.math-0.0.1.tar` & `sigmaepsilon.math-1.0.0.tar`

### file list

```diff
@@ -1,405 +1,138 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.185185 sigmaepsilon.math-0.0.1/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.117185 sigmaepsilon.math-0.0.1/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6009 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3084 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.gitignore
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.117185 sigmaepsilon.math-0.0.1/.math-pub/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.137185 sigmaepsilon.math-0.0.1/.math-pub/Scripts/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18934 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/Activate.ps1
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2225 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/activate
--rw-r--r--   0 circleci  (1001) circleci  (1002)      961 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/activate.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      292 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/copy_sphinxgallery.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108424 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/coverage-3.8.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108424 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/coverage.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108424 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/coverage3.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      347 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/deactivate.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106377 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/docutils.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108425 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/f2py.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108423 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/flake8.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108428 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/hypothesis.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106385 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/ipython.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106385 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/ipython3.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108414 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/isympy.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106374 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jsonschema.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106396 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-dejavu.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106372 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-execute.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106384 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-kernel.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106422 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-kernelspec.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106380 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-migrate.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106382 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-nbconvert.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106401 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-run.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106385 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-troubleshoot.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106413 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter-trust.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106380 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/jupyter.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106381 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/markdown-it.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106393 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/myst-anchors.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106409 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/myst-docutils-demo.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106397 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/myst-docutils-html.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106399 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/myst-docutils-html5.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106399 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/myst-docutils-latex.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106407 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/myst-docutils-pseudoxml.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106395 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/myst-docutils-xml.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106399 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/myst-inv.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106405 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/normalizer.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/numba
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108430 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pip.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108430 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pip3.10.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108430 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pip3.8.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108430 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pip3.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108430 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/py.test.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106383 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pybabel.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106392 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pybtex-convert.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106391 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pybtex-format.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106375 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pybtex.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108421 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pycodestyle.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108420 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pyflakes.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106376 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pygmentize.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108430 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pytest.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   537776 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/python.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   711168 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/python_d.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   536752 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pythonw.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   710144 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pythonw_d.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27255 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pywin32_postinstall.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3721 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/pywin32_testall.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2html.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2html4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1114 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2html5.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2latex.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2man.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      835 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2odt.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1773 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2odt_prepstyles.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2pseudoxml.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      690 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2s5.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      926 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2xetex.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      655 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rst2xml.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/rstpep2html.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106377 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/sphinx-apidoc.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106391 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/sphinx-autogen.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106376 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/sphinx-build.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106381 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/sphinx-quickstart.exe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      423 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/sphx_glr_python_to_jupyter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108417 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/Scripts/wheel.exe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/etc/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/etc/jupyter/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/etc/jupyter/nbconfig/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.137185 sigmaepsilon.math-0.0.1/.math-pub/etc/jupyter/nbconfig/notebook.d/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/etc/jupyter/nbconfig/notebook.d/jupyterlab-plotly.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/pyvenv.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.137185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1763 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/LICENSE.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.137185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.137185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/3d_drawing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/3d_drawing/README.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      934 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/3d_drawing/mayavi2_spring.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1149 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/3d_drawing/plot_basic.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      185 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/README.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.141185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       22 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/README.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1346746 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/WormNet.v3.benchmark.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2335 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/hartford_drug.edgelist
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4119 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_beam_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2126 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_betweenness_centrality.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2678 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_blockmodel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3496 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_circuits.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1194 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_davis_club.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2253 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_dedensification.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2477 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_girvan_newman.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5996 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_iterated_dynamical_systems.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_krackhardt_centrality.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      901 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_maximum_independent_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2444 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_parallel_betweenness.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1039 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_rcm.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3082 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_snap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6474 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/algorithms/plot_subgraphs.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.141185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/basic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/basic/README.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/basic/plot_properties.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      525 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/basic/plot_read_write.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1240 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/basic/plot_simple_graph.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.145185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/README.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   100224 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/chess_masters_WCC.pgn.bz2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20317 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/knuth_miles.txt.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)      621 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_center_node.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4579 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_chess_masters.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2139 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_custom_node_icons.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1556 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_degree.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1115 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_directed.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_edge_colormap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      910 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_ego_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_eigenvalues.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1054 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_four_grids.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_house_with_colors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4103 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_knuth_miles.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1243 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_labels_and_colors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      993 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_multipartite_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      288 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_node_colormap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2172 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_rainbow_coloring.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      938 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_random_geometric_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1228 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_sampson.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      753 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_selfloops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      252 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_simple_path.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1592 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_spectral_grid.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1301 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_tsp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1964 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_unix_email.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/plot_weighted_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/drawing/unix_email.mbox
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.149185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/README.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1011 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_dag_layout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      806 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_degree_sequence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_erdos_renyi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_expected_degree_sequence.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1171 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_football.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      494 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_karate_club.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2966 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_morse_trie.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1393 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_mst.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2901 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_napoleon_russian_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2126 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_roget.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1952 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_triad_types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2681 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/plot_words.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15758 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/roget_dat.txt.gz
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33695 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/graph/words_dat.txt.gz
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.149185 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/subclass/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       18 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/subclass/README.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6023 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/subclass/plot_antigraph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/doc/networkx-3.1/examples/subclass/plot_printgraph.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/kernels/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.149185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/kernels/python3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      193 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/kernels/python3/kernel.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1084 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/kernels/python3/logo-32x32.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2180 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/kernels/python3/logo-64x64.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9605 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/kernels/python3/logo-svg.svg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.149185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2732 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.153185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2643 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/133.5342d9bec93d5de59ad2.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8311 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)  3586208 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/478.247fddac0148cc4e151b.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1110 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/478.247fddac0148cc4e151b.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    70520 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2360 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/657.d89469e0b1d5bb171fde.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14766 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7706 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/remoteEntry.f294278414d0a929e4ae.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5802 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.157185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      199 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/install.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3508 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.157185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7753 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3889 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/static/style.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2452 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/labextensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.157185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/asciidoc/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/asciidoc/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2298 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/asciidoc/index.asciidoc.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.157185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/base/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/base/cell_id_anchor.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      231 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/base/celltags.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/base/display_priority.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1250 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/base/jupyter_widgets.html.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1188 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/base/mathjax.html.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6265 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/base/null.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.157185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/basic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/basic/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)       39 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/basic/index.html.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.157185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/classic/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8261 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/classic/base.html.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      243 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/classic/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2581 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/classic/index.html.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.157185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/classic/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   265101 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/classic/static/style.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.157185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/compatibility/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      133 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/compatibility/display_priority.tpl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/compatibility/full.tpl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.161185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9816 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/base.html.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      217 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4172 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/index.html.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3507 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/mermaidjs.html.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.161185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   581722 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/static/index.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16733 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/static/theme-dark.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15637 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/lab/static/theme-light.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.161185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9739 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/base.tex.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      126 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1643 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/display_priority.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2782 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/document_contents.tex.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      496 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/index.tex.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5544 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/null.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      909 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/report.tex.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1989 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/style_bw_ipython.tex.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      479 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/style_bw_python.tex.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2587 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/style_ipython.tex.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8233 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/style_jupyter.tex.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      794 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/latex/style_python.tex.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.161185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/markdown/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/markdown/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2028 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/markdown/index.md.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.165185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/python/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       78 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/python/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)      472 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/python/index.py.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.165185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/reveal/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      872 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/reveal/base.html.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      402 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/reveal/cellslidedata.j2
--rw-r--r--   0 circleci  (1001) circleci  (1002)      337 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/reveal/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5539 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/reveal/index.html.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.165185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/reveal/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2374 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/reveal/static/custom_reveal.css
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.165185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/rst/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/rst/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2838 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/rst/index.rst.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.165185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/script/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/script/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)       84 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/script/script.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.165185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/webpdf/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/webpdf/conf.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)       36 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbconvert/templates/webpdf/index.pdf.j2
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbextensions/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.169185 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbextensions/jupyterlab-plotly/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbextensions/jupyterlab-plotly/extension.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)  3674328 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbextensions/jupyterlab-plotly/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/jupyter/nbextensions/jupyterlab-plotly/index.js.LICENSE.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.113185 sigmaepsilon.math-0.0.1/.math-pub/share/man/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.169185 sigmaepsilon.math-0.0.1/.math-pub/share/man/man1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2058 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/man/man1/ipython.1
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6659 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.math-pub/share/man/man1/isympy.1
--rw-r--r--   0 circleci  (1001) circleci  (1002)      782 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/.readthedocs.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7343 2023-07-12 16:40:02.185185 sigmaepsilon.math-0.0.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5069 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.169185 sigmaepsilon.math-0.0.1/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      361 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.169185 sigmaepsilon.math-0.0.1/docs/source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/README_link.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.169185 sigmaepsilon.math-0.0.1/docs/source/_static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    86941 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/_static/linalgR3.pdf
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.173185 sigmaepsilon.math-0.0.1/docs/source/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/api/api_approx.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/api/api_function.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/api/api_ga.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/api/api_graph.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2018 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/api/api_linalg.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1764 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/api/api_lp.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6279 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/doc_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.173185 sigmaepsilon.math-0.0.1/docs/source/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    51843 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/examples/lagrange_1d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   104780 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/examples/mls.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/examples_gallery.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      317 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/index.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.173185 sigmaepsilon.math-0.0.1/docs/source/notebooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11968 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/algebra.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    53115 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/approx1d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6490 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/function.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21090 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/genetic.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    67750 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/graph.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      680 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/grid.edgelist
--rw-r--r--   0 circleci  (1001) circleci  (1002)    66838 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/lpp.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    53052 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/moving_least_squares.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3062 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/test_dcm.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26425 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/test_frame.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10476 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/test_vector.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15458 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/testdata.out
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8195 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/notebooks/vector_algebra.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/references.bib
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.173185 sigmaepsilon.math-0.0.1/docs/source/theory/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/theory/theory_linalg.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/docs/source/user_guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1621 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/requirements-dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/requirements-test.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-07-12 16:40:02.185185 sigmaepsilon.math-0.0.1/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.117185 sigmaepsilon.math-0.0.1/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.117185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.177185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.177185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/approx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/approx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/approx/func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7230 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/approx/lagrange.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9900 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/approx/mls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5627 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/arraysetops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1303 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/decorate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/downloads.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.177185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2530 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/constraint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9160 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3849 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/metafunction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2884 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/relation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/testfunction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/hist.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.181185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6305 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/abstract.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25701 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frame.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.181185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8015 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/frontal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2131 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/frutils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7447 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/path.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10580 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/proc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1605 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/imap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14816 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8006 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/solve.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.181185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/sparse/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/sparse/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10065 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/sparse/csr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10331 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/sparse/jaggedarray.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/sparse/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10476 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/tensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1026 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/testing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/tr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29761 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6798 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/vector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4373 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/logical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3821 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/numint.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.181185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5918 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/bga.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14513 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/ga.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31630 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/lp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.181185 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/topology/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/topology/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5512 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/topology/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13236 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.173185 sigmaepsilon.math-0.0.1/src/sigmaepsilon.math.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7343 2023-07-12 16:40:01.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon.math.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16694 2023-07-12 16:40:02.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon.math.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-07-12 16:40:01.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon.math.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      441 2023-07-12 16:40:01.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon.math.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-07-12 16:40:01.000000 sigmaepsilon.math-0.0.1/src/sigmaepsilon.math.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.181185 sigmaepsilon.math-0.0.1/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:40:02.185185 sigmaepsilon.math-0.0.1/tests/linalg/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/linalg/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32342 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/linalg/test_linalg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3629 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/linalg/test_tensor2x3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3058 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/linalg/test_tensor4x3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1173 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/test_approx.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4324 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/test_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2098 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/test_ga.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/test_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3699 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/test_logical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7631 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/test_lpp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/test_numint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3847 2023-07-12 16:39:25.000000 sigmaepsilon.math-0.0.1/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.227022 sigmaepsilon.math-1.0.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.211021 sigmaepsilon.math-1.0.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6009 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3094 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      782 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7533 2023-08-08 16:19:54.227022 sigmaepsilon.math-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5259 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.211021 sigmaepsilon.math-1.0.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      361 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.215021 sigmaepsilon.math-1.0.0/docs/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/README_link.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.215021 sigmaepsilon.math-1.0.0/docs/source/_static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    86941 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/_static/linalgR3.pdf
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.215021 sigmaepsilon.math-1.0.0/docs/source/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      107 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/api/api_approx.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      374 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/api/api_function.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      761 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/api/api_ga.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      142 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/api/api_graph.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2083 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/api/api_linalg.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1764 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/api/api_lp.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      196 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6279 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/doc_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.215021 sigmaepsilon.math-1.0.0/docs/source/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    51843 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/examples/lagrange_1d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   104780 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/examples/mls.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/examples_gallery.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      317 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/index.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.219021 sigmaepsilon.math-1.0.0/docs/source/notebooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11968 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/algebra.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    53115 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/approx1d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6490 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/function.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21090 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/genetic.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    67750 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/graph.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      680 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/grid.edgelist
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    66838 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/lpp.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    53052 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/moving_least_squares.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3062 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/test_dcm.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26425 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/test_frame.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10476 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/test_vector.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15458 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/testdata.out
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8195 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/notebooks/vector_algebra.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      975 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/references.bib
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.219021 sigmaepsilon.math-1.0.0/docs/source/theory/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/theory/theory_linalg.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/docs/source/user_guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1621 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/requirements-dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/requirements-test.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-08 16:19:54.227022 sigmaepsilon.math-1.0.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.211021 sigmaepsilon.math-1.0.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.211021 sigmaepsilon.math-1.0.0/src/sigmaepsilon/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.219021 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      266 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.219021 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/approx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/approx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/approx/func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7230 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/approx/lagrange.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9900 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/approx/mls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5627 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/arraysetops.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1303 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/decorate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/downloads.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.219021 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2530 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/constraint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9160 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3849 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/metafunction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2884 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/relation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/testfunction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/hist.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.223021 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      129 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6305 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/abstract.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25726 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frame.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.223021 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8015 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/frontal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2131 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/frutils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7447 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/path.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10580 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/proc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1605 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/imap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3337 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14816 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8006 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/solve.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.223021 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/sparse/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/sparse/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10065 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/sparse/csr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10331 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/sparse/jaggedarray.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/sparse/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10496 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/tensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1026 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/testing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/tr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29808 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6798 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/vector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4373 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3821 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/numint.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.223021 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5914 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/bga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14511 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/ga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31630 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/lp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.227022 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/topology/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/topology/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5512 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/topology/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13236 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.219021 sigmaepsilon.math-1.0.0/src/sigmaepsilon.math.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7533 2023-08-08 16:19:54.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon.math.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3840 2023-08-08 16:19:54.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon.math.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 16:19:54.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon.math.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      450 2023-08-08 16:19:54.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon.math.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-08-08 16:19:54.000000 sigmaepsilon.math-1.0.0/src/sigmaepsilon.math.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.227022 sigmaepsilon.math-1.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:54.227022 sigmaepsilon.math-1.0.0/tests/linalg/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/linalg/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1143 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/linalg/test_inverse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32053 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/linalg/test_linalg.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1254 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/linalg/test_logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1766 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/linalg/test_rank.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3629 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/linalg/test_tensor2x3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3058 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/linalg/test_tensor4x3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1173 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/test_approx.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4324 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/test_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2098 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/test_ga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      580 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/test_graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3699 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/test_logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7631 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/test_lpp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      669 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/test_numint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3847 2023-08-08 16:19:19.000000 sigmaepsilon.math-1.0.0/tests/test_utils.py
```

### Comparing `sigmaepsilon.math-0.0.1/.circleci/config.yml` & `sigmaepsilon.math-1.0.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/.gitignore` & `sigmaepsilon.math-1.0.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 # SageMath parsed files
 *.sage.py
 
 # Environments
 .env
 .venv
 .math
+.math-pub
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
 # Spyder project settings
```

### Comparing `sigmaepsilon.math-0.0.1/.readthedocs.yaml` & `sigmaepsilon.math-1.0.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/LICENSE` & `sigmaepsilon.math-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/PKG-INFO` & `sigmaepsilon.math-1.0.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.math
-Version: 0.0.1
+Version: 1.0.0
 Summary: A Python Library for Applied Mathematics in Physical Sciences.
 Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 License: MIT License
         
         Copyright (c) 2023 SigmaEpsilon
         
@@ -73,99 +73,69 @@
 
 > **Note**
 > Be aware, that the library uses JIT-compilation through Numba, and as a result,
 > first calls to these functions may take longer, but it pays off big time in the long run.
 
 ## **Documentation**
 
-The [documentation](https://sigmaepsilonmath.readthedocs.io/en/latest/) is hosted on ReadTheDocs.
+The [documentation](https://sigmaepsilonmath.readthedocs.io/en/latest/) is hosted on ReadTheDocs. You can find examples there.
 
 ## **Installation**
 
-`sigmaepsilon.math` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
+sigmaepsilon.math can be installed from PyPI using `pip` on Python >= 3.7:
 
 ```console
 >>> pip install sigmaepsilon.math
 ```
 
 or chechkout with the following command using GitHub CLI
 
 ```console
 gh repo clone sigma-epsilon/sigmaepsilon.math
 ```
 
 and install from source by typing
 
 ```console
->>> python install setup.py
+>>> pip install .
 ```
 
-## **Motivating Examples**
+If you want to run the tests, you can install the package along with the necessary optional dependencies like this
 
-### Linear Algebra
-
-Define a reference frame $\mathbf{B}$ relative to the frame $\mathbf{A}$:
-
-```python
->>> from sigmaepsilon.math.linalg import ReferenceFrame, Vector, Tensor
->>> A = ReferenceFrame(name='A', axes=np.eye(3))
->>> B = A.orient_new('Body', [0, 0, 90*np.pi/180], 'XYZ', name='B')
+```console
+>>> pip install ".[test]"
 ```
 
-Get the *DCM matrix* of the transformation between two frames:
-
-```python
->>> B.dcm(target=A)
-```
+### Development mode
 
-Define a vector $\mathbf{v}$ in frame $\mathbf{A}$ and show the components of it in frame $\mathbf{B}$:
+If you are a developer and want to install the library in development mode, the suggested way is by using this command:
 
-```python
->>> v = Vector([0.0, 1.0, 0.0], frame=A)
->>> v.show(B)
+```console
+>>> pip install "-e .[test, dev]"
 ```
 
-Define the same vector in frame $\mathbf{B}$:
+## How to contribute?
 
-```python
->>> v = Vector(v.show(B), frame=B)
->>> v.show(A)
-```
+Contributions are currently expected in any the following ways:
 
-### Linear Programming
+* finding bugs
+  If you run into trouble when using the library and you think it is a bug, feel free to raise an issue.
+* feedback
+  All kinds of ideas are welcome. For instance if you feel like something is still shady (after reading the user guide), we want to know. Be gentle though, the development of the library is financially not supported yet.
+* feature requests
+  Tell us what you think is missing (with realistic expectations).
+* examples
+  If you've done something with the library and you think that it would make for a good example, get in touch with the developers and we will happily inlude it in the documention.
+* sharing is caring
+  If you like the library, share it with your friends or colleagues so they can like it too.
 
-Solve the following Linear Programming Problem (LPP) with one unique solution:
+## Acknowledgements
 
-```python
->>> from sigmaepsilon.math.optimize import LinearProgrammingProblem as LPP
->>> from sigmaepsilon.math.function import Function, Equality
->>> import sympy as sy
->>> variables = ['x1', 'x2', 'x3', 'x4']
->>> x1, x2, x3, x4 = syms = sy.symbols(variables, positive=True)
->>> obj1 = Function(3*x1 + 9*x3 + x2 + x4, variables=syms)
->>> eq11 = Equality(x1 + 2*x3 + x4 - 4, variables=syms)
->>> eq12 = Equality(x2 + x3 - x4 - 2, variables=syms)
->>> problem = LPP(cost=obj1, constraints=[eq11, eq12], variables=syms)
->>> problem.solve()['x']
-array([0., 6., 0., 4.])
-```
+Although `sigmaepsilon.math` heavily builds on `NumPy`, `Scipy`, `Numba` and `Awkward` and it also has functionality related to `networkx` and other third party libraries. Whithout these libraries the concept of writing performant, yet elegant Python code would be much more difficult.
 
-### NonLinear Programming
+**A lot of the packages mentioned on this document here and the introduction have a citable research paper. If you use them in your work through sigmaepsilon.mesh, take a moment to check out their documentations and cite their papers.**
 
-Find the minimizer of the Rosenbrock function:
-
-```python
->>> from sigmaepsilon.math.optimize import BinaryGeneticAlgorithm
->>>
->>> def Rosenbrock(x):
-...     a, b = 1, 100
-...     return (a-x[0])**2 + b*(x[1]-x[0]**2)**2
->>>
->>> ranges = [[-10, 10], [-10, 10]]
->>> BGA = BinaryGeneticAlgorithm(Rosenbrock, ranges, length=12, nPop=200)
->>> BGA.solve()
-...
-```
+Also, funding of these libraries is partly based on the size of the community they are able to support. If what you are doing strongly relies on these libraries, don't forget to press the :star: button to show your support.
 
 ## **License**
 
-This package is licensed under the MIT license.
+This package is licensed under the [MIT license](https://opensource.org/license/mit/).
```

### Comparing `sigmaepsilon.math-0.0.1/docs/Makefile` & `sigmaepsilon.math-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/make.bat` & `sigmaepsilon.math-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/_static/linalgR3.pdf` & `sigmaepsilon.math-1.0.0/docs/source/_static/linalgR3.pdf`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/api/api_ga.rst` & `sigmaepsilon.math-1.0.0/docs/source/api/api_ga.rst`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/api/api_linalg.rst` & `sigmaepsilon.math-1.0.0/docs/source/api/api_linalg.rst`

 * *Files 6% similar despite different names*

```diff
@@ -65,9 +65,12 @@
 
 .. autoclass:: sigmaepsilon.math.linalg.Tensor4
     :members:
 
 Routines
 ========
 
+.. automodule:: sigmaepsilon.math.linalg.logical
+    :members: 
+
 .. automodule:: sigmaepsilon.math.linalg.utils
     :members:
```

### Comparing `sigmaepsilon.math-0.0.1/docs/source/api/api_lp.rst` & `sigmaepsilon.math-1.0.0/docs/source/api/api_lp.rst`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/conf.py` & `sigmaepsilon.math-1.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/doc_utils.py` & `sigmaepsilon.math-1.0.0/docs/source/doc_utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/examples/lagrange_1d.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/examples/lagrange_1d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/examples/mls.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/examples/mls.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/algebra.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/algebra.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/approx1d.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/approx1d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/function.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/function.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/genetic.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/genetic.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/graph.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/graph.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/grid.edgelist` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/grid.edgelist`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/lpp.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/lpp.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/moving_least_squares.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/moving_least_squares.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/test_dcm.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/test_dcm.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/test_frame.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/test_frame.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/test_vector.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/test_vector.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/testdata.out` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/testdata.out`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/notebooks/vector_algebra.ipynb` & `sigmaepsilon.math-1.0.0/docs/source/notebooks/vector_algebra.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/references.bib` & `sigmaepsilon.math-1.0.0/docs/source/references.bib`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/docs/source/theory/theory_linalg.rst` & `sigmaepsilon.math-1.0.0/docs/source/theory/theory_linalg.rst`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/pyproject.toml` & `sigmaepsilon.math-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools-scm",
     "wheel>=0.38.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigmaepsilon.math"
-version = "0.0.1"
+version = "1.0.0"
 description = "A Python Library for Applied Mathematics in Physical Sciences."
 classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/approx/func.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/approx/func.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/approx/lagrange.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/approx/lagrange.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/approx/mls.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/approx/mls.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/arraysetops.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/arraysetops.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/decorate.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/decorate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/downloads.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/downloads.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/constraint.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/constraint.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/function.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/function.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/functions.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/functions.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/metafunction.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/metafunction.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/relation.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/relation.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/function/testfunction.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/function/testfunction.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/hist.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/hist.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/abstract.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/abstract.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frame.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 
 import numpy as np
 from numpy import ndarray
 
 from sigmaepsilon.core.typing import issequence
 
 from .utils import (
-    is_rectangular_frame,
-    is_orthonormal_frame,
-    is_normal_frame,
     normalize_frame,
     Gram,
     dual_frame,
     transpose_axes,
     show_frame,
     rotation_matrix,
 )
+from .logical import (
+    is_rectangular_frame,
+    is_orthonormal_frame,
+    is_normal_frame,
+)
 from ..utils import repeat
 from .meta import FrameLike, TensorLike, ArrayWrapper
 
 
 __all__ = ["ReferenceFrame", "RectangularFrame", "CartesianFrame"]
```

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/frontal.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/frontal.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/frutils.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/frutils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/path.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/path.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/postproc.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/postproc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/proc.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/proc.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/frontal/topo.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/frontal/topo.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/meta.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/meta.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/solve.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/solve.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/sparse/csr.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/sparse/csr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/sparse/jaggedarray.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/sparse/jaggedarray.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/sparse/utils.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/sparse/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/tensor.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 from sigmaepsilon.core.alphabet import latinrange
 
 from .frame import ReferenceFrame as Frame
 from .abstract import AbstractTensor
 from .tr import _tr_tensors2, _tr_tensors4x3
 from .exceptions import TensorShapeMismatchError
-from .utils import is_hermitian, transpose_axes
+from .utils import transpose_axes
+from .logical import is_hermitian
 
 __all__ = [
     "Tensor",
     "Tensor2",
     "Tensor4",
     "Tensor2x3",
     "Tensor4x3",
```

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/testing.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/testing.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/tr.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/utils.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,33 +8,26 @@
 import sympy as sy
 from sympy import symbols, Matrix
 from sympy.physics.vector import ReferenceFrame as SymPyFrame
 
 from sigmaepsilon.core.alphabet import latinrange
 
 from .meta import TensorLike, ArrayWrapper, FrameLike
-from .exceptions import LinalgOperationInputError, LinalgMissingInputError
+from .exceptions import LinalgOperationInputError, LinalgMissingInputError, LinalgError
 
 __cache = True
 
 
 __all__ = [
     "permutation_tensor",
     "dot",
     "cross",
-    "is_rectangular_frame",
-    "is_normal_frame",
-    "is_orthonormal_frame",
-    "is_independent_frame",
-    "is_hermitian",
     "normalize_frame",
     "Gram",
     "dual_frame",
-    "is_pos_def",
-    "is_pos_semidef",
     "random_pos_semidef_matrix",
     "random_posdef_matrix",
     "inv_sym_3x3",
     "vpath",
     "det3x3",
     "det2x2",
     "inv2x2",
@@ -50,14 +43,17 @@
     "norm2d",
     "linspace",
     "linspace1d",
     "inv",
     "show_vector",
     "show_frame",
     "rotation_matrix",
+    "generalized_left_inverse",
+    "generalized_right_inverse",
+    "generalized_inverse",
 ]
 
 
 def rotation_matrix(
     rot_type: str, amounts: Iterable, rot_order: Union[str, int] = ""
 ) -> ndarray:
     """
@@ -150,33 +146,33 @@
     coincides with NumPy when all inputs are arrays and generalizes when they are not,
     but all inputs must be either all arrays or all tensors of some kind. The operation for
     tensors of order 1 and 2 have dedicated implementations, for higher order tensors
     it generalizes to tensor contraction along specified axes.
 
     Parameters
     ----------
-    a: TensorLike or ArrayLike
+    a: :class:`~sigmaepsilon.math.linalg.meta.TensorLike` or ArrayLike
        A tensor or an array.
-    b: TensorLike or ArrayLike
+    b: :class:`~sigmaepsilon.math.linalg.meta.TensorLike` or ArrayLike
        A tensor or an array.
     out: ArrayLike, Optional
         Output argument. This must have the exact kind that would be returned if it was
         not used. See `numpy.dot` for the details. Only if all inputs are ArrayLike.
         Default is None.
-    frame: FrameLike, Optinal
+    frame: FrameLike, Optional
         The target frame of the output. Only if all inputs are TensorLike. If not specified,
         the returned tensor migh be returned in an arbitrary frame, depending on the inputs.
         Default is None.
     axes: tuple or list, Optional
         The indices along which contraction happens if any of the input tensors have a rank
         higher than 2. Default is None.
 
     Returns
     -------
-    TensorLike or numpy.ndarray or scalar
+    :class:`~sigmaepsilon.math.linalg.meta.TensorLike` or numpy.ndarray or scalar
         An array or a tensor, depending on the inputs.
 
     Notes
     -----
     For general tensors, the current implementation has an upper limit considering the rank
     of the input tensors. The sum of the ranks of the input tensors plus the sum of contraction
     indices must be at most 26.
@@ -262,30 +258,30 @@
     tensor. The behaviour coincides with NumPy when all inputs are arrays and generalizes
     when they are not, but all inputs must be either all arrays or all tensors of some kind.
 
     Parameters
     ----------
     *args : Tuple, Optional
         Positional arguments forwarded to NumPy, if all input objects are arrays.
-    a: TensorLike or ArrayLike
+    a: :class:`~sigmaepsilon.math.linalg.meta.TensorLike` or ArrayLike
         A tensor or an array.
-    b: TensorLike or ArrayLike
+    b: :class:`~sigmaepsilon.math.linalg.meta.TensorLike` or ArrayLike
         A tensor or an array.
     frame: FrameLike, Optional
         The target frame of the output. Only if all inputs are TensorLike. If not specified,
         the returned tensor migh be returned in an arbitrary frame, depending on the inputs.
         Default is None.
     **kwargs: dict, Optional
         Keyword arguments forwarded to `numpy.cross`. As of NumPy version '1.22.4', there
         are no keyword arguments for `numpy.cross`, this is to assure compliance with
         all future versions of numpy.
 
     Returns
     -------
-    numpy.ndarray or TensorLike
+    numpy.ndarray or :class:`~sigmaepsilon.math.linalg.meta.TensorLike`
         An 1d or 2d array, or an 1d or 2d tensor, depending on the inputs.
 
     References
     ----------
     https://mathworld.wolfram.com/CrossProduct.html
 
     Examples
@@ -558,75 +554,14 @@
         indices = tuple(range(len(shape)))
         data_indices = indices[:-2]
         tensor_indices = indices[len(shape) - 2 :]
         indices = data_indices + tensor_indices[::-1]
         return np.transpose(arr, indices)
 
 
-def is_rectangular_frame(axes: ndarray) -> bool:
-    """
-    Returns True if a frame is Cartesian.
-
-    Parameters
-    ----------
-    axes: numpy.ndarray
-        A matrix where the i-th row is the i-th basis vector.
-    """
-    assert len(axes.shape) == 2, "Input is not a matrix!"
-    assert axes.shape[0] == axes.shape[1], "Input is not a square matrix!"
-    agram = np.abs(axes @ axes.T)
-    return np.isclose(np.trace(agram), np.sum(agram))
-
-
-def is_normal_frame(axes: ndarray) -> bool:
-    """
-    Returns True if a frame is normal, meaning, that it's base vectors
-    are all of unit length.
-
-    Parameters
-    ----------
-    axes: numpy.ndarray
-        A matrix where the i-th row is the i-th basis vector.
-    """
-    return np.allclose(np.linalg.norm(axes, axis=1), 1.0)
-
-
-def is_orthonormal_frame(axes: ndarray) -> bool:
-    """
-    Returns True if a frame is orthonormal.
-
-    Parameters
-    ----------
-    axes: numpy.ndarray
-        A matrix where the i-th row is the i-th basis vector.
-    """
-    return is_rectangular_frame(axes) and is_normal_frame(axes)
-
-
-def is_independent_frame(axes: ndarray, tol: float = 0) -> bool:
-    """
-    Returns True if a the base vectors of a frame are linearly independent.
-
-    Parameters
-    ----------
-    axes: numpy.ndarray
-        A matrix where the i-th row is the i-th basis vector.
-    """
-    return np.linalg.det(Gram(axes)) > tol
-
-
-def is_hermitian(arr: ndarray) -> bool:
-    """
-    Returns True if the input is a hermitian array.
-    """
-    shp = arr.shape
-    s0 = shp[0]
-    return all([s == s0 for s in shp[1:]])
-
-
 def normalize_frame(axes: ndarray) -> ndarray:
     """
     Returns the frame with normalized base vectors.
 
     Parameters
     ----------
     axes: numpy.ndarray
@@ -655,28 +590,14 @@
     ----------
     axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
     return transpose_axes(np.linalg.inv(axes))
 
 
-def is_pos_def(arr) -> bool:
-    """
-    Returns True if the input is positive definite.
-    """
-    return np.all(np.linalg.eigvals(arr) > 0)
-
-
-def is_pos_semidef(arr) -> bool:
-    """
-    Returns True if the input is positive semi definite.
-    """
-    return np.all(np.linalg.eigvals(arr) >= 0)
-
-
 def random_pos_semidef_matrix(N) -> ndarray:
     """
     Returns a random positive semidefinite matrix of shape (N, N).
 
     Example
     -------
     >>> from sigmaepsilon.math.linalg import random_pos_semidef_matrix, is_pos_semidef
@@ -950,7 +871,61 @@
 @njit(nogil=True, parallel=True, cache=__cache)
 def linspace1d(start, stop, N) -> ndarray:
     res = np.zeros(N)
     di = (stop - start) / (N - 1)
     for i in prange(N):
         res[i] = start + i * di
     return res
+
+
+def generalized_left_inverse(matrix: ndarray) -> ndarray:
+    """Returns the generalized left inverse
+
+    .. math::
+        :nowrap:
+
+        \\begin{equation}
+            \left( \mathbf{A}^{T} \mathbf{A} \\right)^{-1} \mathbf{A}^{T}
+        \\end{equation}
+
+    """
+    return np.linalg.inv(matrix.T @ matrix) @ matrix.T
+
+
+def generalized_right_inverse(matrix: ndarray) -> ndarray:
+    """Returns the generalized right inverse
+
+    .. math::
+        :nowrap:
+
+        \\begin{equation}
+            \mathbf{A}^{T} \left( \mathbf{A} \mathbf{A}^{T} \\right)^{-1}
+        \\end{equation}
+
+    """
+    return matrix.T @ np.linalg.inv(matrix @ matrix.T)
+
+
+def generalized_inverse(matrix: ndarray) -> ndarray:
+    """
+    Returns the generalized inverse of the input matrix, in any of the following
+    cases:
+    1) The matrix is square and has full rank. In this case the returned matrix
+    is the usual inverse.
+    2) The matrix has more columns than rows and has full row rank. In this case
+    the generalized right inverse is returned.
+    3) The matrix has more rows than columns and has full column rank. In this case
+    the generalized left inverse is returned.
+    """
+    if not len(matrix.shape) == 2:
+        raise LinalgOperationInputError("The input must be a matrix")
+
+    num_rows, num_columns = matrix.shape
+    rank = np.linalg.matrix_rank(matrix)
+    if (num_rows == num_columns) and rank == num_columns == num_rows:
+        return np.linalg.inv(matrix)
+    elif (num_rows > num_columns) and rank == num_columns:
+        return generalized_left_inverse(matrix)
+    elif (num_rows < num_columns) and rank == num_rows:
+        return generalized_right_inverse(matrix)
+    else:
+        raise LinalgError("The matrix has no inverse")
```

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/linalg/vector.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/linalg/vector.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/logical.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/logical.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/numint.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/numint.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/bga.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/bga.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         Chromosome length (string length). Default is 5.
     p_c: float, Optional
         Probability of crossover, 0 <= p_c <= 1. Default is 1.
     p_m: float, Optional
         Probability of mutation, 0 <= p_m <= 1. Default is 0.2.
     nPop: int, Optional
         Number of members in the population. Default is 100.
-    elitism: float or integer, Optional
+    elitism: float or int, Optional
         Value to control elitism. Default is 1.
 
     Examples
     --------
     Find the minimizer of the Rosenbrock function.
     The exact value of the solution is x = [1.0, 1.0].
```

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/ga.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/ga.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     A data class for members of a population.
     """
 
     phenotype: List[float] = Field(default_factory=list)
     genotype: List[int] = Field(default_factory=list)
     fittness: float
     age: int = Field(default=0)
-    _index: int = Field(default=-1)
+    index: int = Field(default=-1)
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, Genom):
             return False
         return np.all(self.genotype == other.genotype)
 
     def __hash__(self):
@@ -310,15 +310,15 @@
         """
         fittness = self.fittness
         index = np.argmin(fittness)
         return Genom(
             phenotype=self.phenotypes[index],
             genotype=self.genotypes[index],
             fittness=fittness[index],
-            _index=index,
+            index=index,
         )
 
     def celebrate(self, genom: Genom) -> None:
         """
         Celebration of the winner. Curretly this means that the beast candidate is added
         to a history to keep track of the improvements across evolutions.
         """
```

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/optimize/lp.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/optimize/lp.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/topology/graph.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/topology/graph.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon/math/utils.py` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon/math/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/src/sigmaepsilon.math.egg-info/PKG-INFO` & `sigmaepsilon.math-1.0.0/src/sigmaepsilon.math.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.math
-Version: 0.0.1
+Version: 1.0.0
 Summary: A Python Library for Applied Mathematics in Physical Sciences.
 Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 License: MIT License
         
         Copyright (c) 2023 SigmaEpsilon
         
@@ -73,99 +73,69 @@
 
 > **Note**
 > Be aware, that the library uses JIT-compilation through Numba, and as a result,
 > first calls to these functions may take longer, but it pays off big time in the long run.
 
 ## **Documentation**
 
-The [documentation](https://sigmaepsilonmath.readthedocs.io/en/latest/) is hosted on ReadTheDocs.
+The [documentation](https://sigmaepsilonmath.readthedocs.io/en/latest/) is hosted on ReadTheDocs. You can find examples there.
 
 ## **Installation**
 
-`sigmaepsilon.math` can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
+sigmaepsilon.math can be installed from PyPI using `pip` on Python >= 3.7:
 
 ```console
 >>> pip install sigmaepsilon.math
 ```
 
 or chechkout with the following command using GitHub CLI
 
 ```console
 gh repo clone sigma-epsilon/sigmaepsilon.math
 ```
 
 and install from source by typing
 
 ```console
->>> python install setup.py
+>>> pip install .
 ```
 
-## **Motivating Examples**
+If you want to run the tests, you can install the package along with the necessary optional dependencies like this
 
-### Linear Algebra
-
-Define a reference frame $\mathbf{B}$ relative to the frame $\mathbf{A}$:
-
-```python
->>> from sigmaepsilon.math.linalg import ReferenceFrame, Vector, Tensor
->>> A = ReferenceFrame(name='A', axes=np.eye(3))
->>> B = A.orient_new('Body', [0, 0, 90*np.pi/180], 'XYZ', name='B')
+```console
+>>> pip install ".[test]"
 ```
 
-Get the *DCM matrix* of the transformation between two frames:
-
-```python
->>> B.dcm(target=A)
-```
+### Development mode
 
-Define a vector $\mathbf{v}$ in frame $\mathbf{A}$ and show the components of it in frame $\mathbf{B}$:
+If you are a developer and want to install the library in development mode, the suggested way is by using this command:
 
-```python
->>> v = Vector([0.0, 1.0, 0.0], frame=A)
->>> v.show(B)
+```console
+>>> pip install "-e .[test, dev]"
 ```
 
-Define the same vector in frame $\mathbf{B}$:
+## How to contribute?
 
-```python
->>> v = Vector(v.show(B), frame=B)
->>> v.show(A)
-```
+Contributions are currently expected in any the following ways:
 
-### Linear Programming
+* finding bugs
+  If you run into trouble when using the library and you think it is a bug, feel free to raise an issue.
+* feedback
+  All kinds of ideas are welcome. For instance if you feel like something is still shady (after reading the user guide), we want to know. Be gentle though, the development of the library is financially not supported yet.
+* feature requests
+  Tell us what you think is missing (with realistic expectations).
+* examples
+  If you've done something with the library and you think that it would make for a good example, get in touch with the developers and we will happily inlude it in the documention.
+* sharing is caring
+  If you like the library, share it with your friends or colleagues so they can like it too.
 
-Solve the following Linear Programming Problem (LPP) with one unique solution:
+## Acknowledgements
 
-```python
->>> from sigmaepsilon.math.optimize import LinearProgrammingProblem as LPP
->>> from sigmaepsilon.math.function import Function, Equality
->>> import sympy as sy
->>> variables = ['x1', 'x2', 'x3', 'x4']
->>> x1, x2, x3, x4 = syms = sy.symbols(variables, positive=True)
->>> obj1 = Function(3*x1 + 9*x3 + x2 + x4, variables=syms)
->>> eq11 = Equality(x1 + 2*x3 + x4 - 4, variables=syms)
->>> eq12 = Equality(x2 + x3 - x4 - 2, variables=syms)
->>> problem = LPP(cost=obj1, constraints=[eq11, eq12], variables=syms)
->>> problem.solve()['x']
-array([0., 6., 0., 4.])
-```
+Although `sigmaepsilon.math` heavily builds on `NumPy`, `Scipy`, `Numba` and `Awkward` and it also has functionality related to `networkx` and other third party libraries. Whithout these libraries the concept of writing performant, yet elegant Python code would be much more difficult.
 
-### NonLinear Programming
+**A lot of the packages mentioned on this document here and the introduction have a citable research paper. If you use them in your work through sigmaepsilon.mesh, take a moment to check out their documentations and cite their papers.**
 
-Find the minimizer of the Rosenbrock function:
-
-```python
->>> from sigmaepsilon.math.optimize import BinaryGeneticAlgorithm
->>>
->>> def Rosenbrock(x):
-...     a, b = 1, 100
-...     return (a-x[0])**2 + b*(x[1]-x[0]**2)**2
->>>
->>> ranges = [[-10, 10], [-10, 10]]
->>> BGA = BinaryGeneticAlgorithm(Rosenbrock, ranges, length=12, nPop=200)
->>> BGA.solve()
-...
-```
+Also, funding of these libraries is partly based on the size of the community they are able to support. If what you are doing strongly relies on these libraries, don't forget to press the :star: button to show your support.
 
 ## **License**
 
-This package is licensed under the MIT license.
+This package is licensed under the [MIT license](https://opensource.org/license/mit/).
```

### Comparing `sigmaepsilon.math-0.0.1/tests/linalg/test_linalg.py` & `sigmaepsilon.math-1.0.0/tests/linalg/test_linalg.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from numpy import vstack
 from scipy.sparse import csr_matrix as csr_scipy
 from numba import njit
 import sympy as sy
 
 from sigmaepsilon.math.linalg.testing import LinalgTestCase
 
-from sigmaepsilon.math.linalg.utils import random_pos_semidef_matrix, random_posdef_matrix
+from sigmaepsilon.math.linalg.utils import (
+    random_pos_semidef_matrix,
+    random_posdef_matrix,
+)
 from sigmaepsilon.math.logical import ispossemidef, isposdef
 from sigmaepsilon.math.linalg import (
     ReferenceFrame,
     RectangularFrame,
     CartesianFrame,
     ArrayWrapper,
     Vector,
@@ -852,40 +855,34 @@
 
 class TestPosDef(LinalgTestCase):
     def test_random_pos_semidef(self, N=5):
         """
         Tests the creation of random, positive semidefinite matrices.
         """
         self.assertTrue(ispossemidef(random_pos_semidef_matrix(N)))
-        self.assertTrue(lautils.is_pos_semidef(random_pos_semidef_matrix(N)))
 
     def test_random_posdef(self, N=2):
         """
         Tests the creation of random, positive definite matrices.
         """
         self.assertTrue(isposdef(random_posdef_matrix(N)))
-        self.assertTrue(lautils.is_pos_def(random_posdef_matrix(N)))
 
 
 class TestUtils(LinalgTestCase):
     def test_behaviour(self):
         """
         Tests performed to boost coverage and assert basic responeses.
         """
         A = np.eye(3)
         a1, a2 = np.array([1.0, 0, 0]), np.array([2.0, 0, 0])
 
         # functions related to frames
         lautils.Gram(A)
         lautils.normalize_frame(A)
         lautils.dual_frame(A)
-        lautils.is_independent_frame(A)
-        lautils.is_orthonormal_frame(A)
-        lautils.is_normal_frame(A)
-        lautils.is_rectangular_frame(A)
 
         # miscellanous operations
         lautils.vpath(a1, a2, 3)
         lautils.linsolve(A, a1)
         lautils.inv(A)
         lautils.matmul(A, A)
         lautils.matmulw(A, A, 1)
```

### Comparing `sigmaepsilon.math-0.0.1/tests/linalg/test_tensor2x3.py` & `sigmaepsilon.math-1.0.0/tests/linalg/test_tensor2x3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/linalg/test_tensor4x3.py` & `sigmaepsilon.math-1.0.0/tests/linalg/test_tensor4x3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/test_approx.py` & `sigmaepsilon.math-1.0.0/tests/test_approx.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/test_function.py` & `sigmaepsilon.math-1.0.0/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/test_ga.py` & `sigmaepsilon.math-1.0.0/tests/test_ga.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/test_graph.py` & `sigmaepsilon.math-1.0.0/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/test_logical.py` & `sigmaepsilon.math-1.0.0/tests/test_logical.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/test_lpp.py` & `sigmaepsilon.math-1.0.0/tests/test_lpp.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/test_numint.py` & `sigmaepsilon.math-1.0.0/tests/test_numint.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.math-0.0.1/tests/test_utils.py` & `sigmaepsilon.math-1.0.0/tests/test_utils.py`

 * *Files identical despite different names*

