# Comparing `tmp/sigmaepsilon.mesh-0.0.3.tar.gz` & `tmp/sigmaepsilon.mesh-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmaepsilon.mesh-0.0.3.tar", last modified: Sun Aug  6 17:04:15 2023, max compression
+gzip compressed data, was "sigmaepsilon.mesh-1.0.0.tar", last modified: Tue Aug  8 21:30:21 2023, max compression
```

## Comparing `sigmaepsilon.mesh-0.0.3.tar` & `sigmaepsilon.mesh-1.0.0.tar`

### file list

```diff
@@ -1,192 +1,204 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.079240 sigmaepsilon.mesh-0.0.3/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.027239 sigmaepsilon.mesh-0.0.3/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6009 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/.readthedocs.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9081 2023-08-06 17:04:15.079240 sigmaepsilon.mesh-0.0.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6779 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.027239 sigmaepsilon.mesh-0.0.3/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/make.bat
--rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.031239 sigmaepsilon.mesh-0.0.3/docs/source/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/README_link.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.035240 sigmaepsilon.mesh-0.0.3/docs/source/_static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/logo.PNG
--rw-r--r--   0 circleci  (1001) circleci  (1002)    57097 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot1.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   131843 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot2.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   179580 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot3.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61611 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot4.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91565 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot4a.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    89629 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot5.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    88428 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot6.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   181162 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/plot7.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    50423 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_1.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    47062 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_2.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   132201 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_3.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106791 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_4.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)   132473 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_5.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.035240 sigmaepsilon.mesh-0.0.3/docs/source/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1064 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_cells.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_db.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_recipes.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_space.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_topo.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api/api_utils.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      180 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/api.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/doc_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.047240 sigmaepsilon.mesh-0.0.3/docs/source/examples/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   167698 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/compound1.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   273863 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/compound2.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   112067 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/compound3.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   613748 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/cube.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   420021 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/cylinder.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   353852 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/disc.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   186760 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/grids2d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   250977 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/grids3d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   610460 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/import_file.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   325635 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/import_gmsh.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   319837 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/import_pyvista.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1260616 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/joint_cube.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   110806 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/lighting.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   253615 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/shape_functions_1d.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   259081 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples/trigridQ4.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/examples_gallery.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/logo.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.051240 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   949800 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/data.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   757783 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/grids.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   162584 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/io.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8001 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_analysis.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   135639 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_composition.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25963 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_structure.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   812456 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/plotting.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14480 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/points_and_pointclouds.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11679 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/shape_function_generation.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)   383025 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/trafo_geom.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/notebooks/trafo_topo.ipynb
--rw-r--r--   0 circleci  (1001) circleci  (1002)      979 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/references.bib
--rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/refs.bib
--rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/docs/source/user_guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/logo.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/requirements-dev.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/requirements-test.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-06 17:04:15.079240 sigmaepsilon.mesh-0.0.3/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.023239 sigmaepsilon.mesh-0.0.3/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.023239 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.063240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      985 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/abcdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/akwrap.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3327 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43719 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cell.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14433 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/celldata.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.063240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      704 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4088 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2438 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1503 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/l2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1343 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/l3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1581 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2001 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1532 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/t3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2086 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/t6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2117 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1362 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2458 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/w18.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1663 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/w6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3796 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/downloads.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/extrude.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21752 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/grid.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/helpers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.067240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/inp2stl.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/line.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/linedata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/mesh1d.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8279 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/pointdata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    83934 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polydata.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polygon.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2617 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polyhedron.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1040 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/pop.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13752 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/recipes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14608 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/section.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.067240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7879 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/frame.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2736 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/point.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19474 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/pointcloud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tetmesh.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1947 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tetrahedralize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2350 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4895 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/topoarray.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/triang.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6450 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/trimesh.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.067240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.071240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3252 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/gauss.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32014 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/h27.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7165 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/h8.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/l2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/l3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2398 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/q4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4756 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/q9.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/t3.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2646 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/t6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/tet10.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/tet4.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4507 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1396 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/w18.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/w6.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      706 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/colors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4734 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/knn.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/locate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11071 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/space.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4568 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/tet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5482 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topodata.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.075240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29528 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20845 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/tr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16702 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/tri.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30106 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/voxelize.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3206 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/vtkcelltypes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1886 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/vtkutils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.055240 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9081 2023-08-06 17:04:14.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5490 2023-08-06 17:04:15.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-06 17:04:14.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      699 2023-08-06 17:04:14.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-08-06 17:04:14.000000 sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.075240 sigmaepsilon.mesh-0.0.3/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:04:15.079240 sigmaepsilon.mesh-0.0.3/tests/cells/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2016 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/test_cells.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3696 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/test_hex.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1261 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/test_lines.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2014 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/cells/test_tet.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_colors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_compound.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_geom.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_io.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6097 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_linalg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_mesh_anal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_meshing.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_pointcloud.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2100 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_recipes.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4082 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_topo_tr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2392 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tests/test_tri.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-08-06 17:03:29.000000 sigmaepsilon.mesh-0.0.3/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.978172 sigmaepsilon.mesh-1.0.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.930172 sigmaepsilon.mesh-1.0.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6009 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1903 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      822 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8920 2023-08-08 21:30:21.978172 sigmaepsilon.mesh-1.0.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6618 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.930172 sigmaepsilon.mesh-1.0.0/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      769 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/make.bat
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      322 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.934172 sigmaepsilon.mesh-1.0.0/docs/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/README_link.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.938172 sigmaepsilon.mesh-1.0.0/docs/source/_static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/logo.PNG
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    57097 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/plot1.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   131843 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/plot2.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   179580 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/plot3.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61611 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/plot4.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91565 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/plot4a.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    89629 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/plot5.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    88428 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/plot6.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   181162 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/plot7.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    50423 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_1.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    47062 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_2.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   132201 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_3.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106791 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_4.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   132473 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_5.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.938172 sigmaepsilon.mesh-1.0.0/docs/source/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/api/api_cells.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1141 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/api/api_db.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      127 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/api/api_interpolator.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      311 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/api/api_recipes.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      282 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/api/api_space.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       87 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/api/api_topo.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      464 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/api/api_utils.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      206 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/api.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6367 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1001 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/doc_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.946172 sigmaepsilon.mesh-1.0.0/docs/source/examples/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   167698 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/compound1.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   273863 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/compound2.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   112067 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/compound3.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   613748 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/cube.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   420021 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/cylinder.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   353852 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/disc.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   186760 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/grids2d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   250977 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/grids3d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   610460 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/import_file.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   325635 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/import_gmsh.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   319837 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/import_pyvista.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1260616 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/joint_cube.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   110806 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/lighting.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   253615 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/shape_functions_1d.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   259081 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples/trigridQ4.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      467 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/examples_gallery.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      321 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/logo.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.954172 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   949800 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/data.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   757783 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/grids.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9276 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/interpolation.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   162584 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/io.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8001 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/mesh_analysis.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   135639 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/mesh_composition.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25963 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/mesh_structure.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   812456 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/plotting.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14480 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/points_and_pointclouds.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11679 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/shape_function_generation.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   383025 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/trafo_geom.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/notebooks/trafo_topo.ipynb
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      979 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/references.bib
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/refs.bib
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      379 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/docs/source/user_guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   140483 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/logo.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1696 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/requirements-dev.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/requirements-test.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      165 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-08 21:30:21.978172 sigmaepsilon.mesh-1.0.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.926172 sigmaepsilon.mesh-1.0.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.926172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.962172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      985 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/abcdata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7429 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/akwrap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3327 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14433 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/celldata.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.962172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.966172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27635 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/cell.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7148 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/cell1d.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3776 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/cell2d.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8968 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/cell3d.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6334 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/interpolator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      480 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/line.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3185 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/polygon.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2621 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/polyhedron.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4093 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/h27.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2443 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/h8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/l2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1348 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/l3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1586 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/q4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2006 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/q9.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1537 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/t3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2091 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/t6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2122 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/tet10.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1367 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/tet4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2463 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/w18.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1668 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/w6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1067 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3796 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/downloads.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.966172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/errors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1234 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/errors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2196 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/extrude.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21752 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/grid.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       45 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/helpers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.966172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/io/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/io/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11440 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/io/inp2stl.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2322 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/io/io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2807 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/linedata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1761 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/mesh1d.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8279 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/pointdata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    83945 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/polydata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1040 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/pop.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13752 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/recipes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14608 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/section.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.966172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/space/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/space/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7879 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/space/frame.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2736 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/space/point.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19474 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/space/pointcloud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      841 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/tetmesh.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1947 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/tetrahedralize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2350 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/tile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4895 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/topoarray.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8210 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/triang.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6450 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/trimesh.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.970173 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.974172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32014 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/h27.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7165 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/h8.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      312 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/interpolator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1438 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/l2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      204 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/l3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3572 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/numint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2398 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/q4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4756 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/q9.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/t3.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2646 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/t6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/tet10.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2506 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/tet4.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4507 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1396 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/w18.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      994 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/w6.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      706 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/colors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4734 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/knn.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/locate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11071 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/space.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4568 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/tet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5482 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/topodata.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.974172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/topology/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/topology/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29528 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/topology/topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20845 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/topology/tr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16702 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/tri.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30106 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1074 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/voxelize.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3206 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/vtkcelltypes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1886 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/vtkutils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.954172 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8920 2023-08-08 21:30:21.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5961 2023-08-08 21:30:21.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-08 21:30:21.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      633 2023-08-08 21:30:21.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-08-08 21:30:21.000000 sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.974172 sigmaepsilon.mesh-1.0.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:30:21.978172 sigmaepsilon.mesh-1.0.0/tests/cells/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/cells/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1977 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/cells/test_cells.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3696 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/cells/test_hex.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3240 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/cells/test_interpolator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1261 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/cells/test_lines.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2014 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/cells/test_tet.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_colors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1709 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_compound.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4456 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_geom.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3350 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_io.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6097 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_linalg.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1014 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_mesh_anal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_meshing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1352 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_pointcloud.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2100 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_recipes.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      424 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4082 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_topo_tr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2392 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tests/test_tri.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      367 2023-08-08 21:29:33.000000 sigmaepsilon.mesh-1.0.0/tox.ini
```

### Comparing `sigmaepsilon.mesh-0.0.3/.circleci/config.yml` & `sigmaepsilon.mesh-1.0.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/.gitignore` & `sigmaepsilon.mesh-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/.readthedocs.yaml` & `sigmaepsilon.mesh-1.0.0/.readthedocs.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -24,11 +24,10 @@
 #    - pdf
 
 # Optionally declare the Python requirements required to build your docs
 python:
    install:
    - requirements: requirements.txt
    - requirements: requirements-dev.txt
-   - requirements: requirements-devops.txt
    - requirements: docs/requirements.txt
    - method: pip
      path: .
```

### Comparing `sigmaepsilon.mesh-0.0.3/LICENSE` & `sigmaepsilon.mesh-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/PKG-INFO` & `sigmaepsilon.mesh-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.mesh
-Version: 0.0.3
+Version: 1.0.0
 Summary: A Python package to build, manipulate and analyze polygonal meshes.
 Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 License: MIT License
         
         Copyright (c) 2021 SigmaEpsilon
         
@@ -51,44 +51,42 @@
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main)
 [![Documentation Status](https://readthedocs.org/projects/sigmaepsilonmesh/badge/?version=latest)](https://sigmaepsilonmesh.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://badge.fury.io/py/sigmaepsilon.mesh.svg)](https://pypi.org/project/sigmaepsilon.mesh)
 [![Python 3.7‒3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-> **Warning** sigmaepsilon.mesh is in the early stages of it's lifetime, and some concepts may change in the future. If you seek long-term stability, wait until version 1.0, which is planned to be released if the core concepts all seem to sit and the documentation covers all major concepts.
-
 The [sigmaepsilon.mesh](https://sigmaepsilon.mesh.readthedocs.io/en/latest/) library aims to provide the tools to build and analyse poligonal meshes with complex topologies. Meshes can be built like a dictionary, using arbitarily nested layouts and then be translated to other formats including [VTK](https://vtk.org/) and [PyVista](https://docs.pyvista.org/). For plotting, there is also support for [K3D](http://k3d-jupyter.org/), [Matplotlib](https://matplotlib.org/) and [Plotly](https://plotly.com/python/).
 
 The data model is built around [Awkward](https://awkward-array.org/doc/main/), which makes it possible to attach nested, variable-sized data to the points or the cells in a mesh, also providing interfaces to other popular libraries like [Pandas](https://vtk.org/) or [PyArrow](https://arrow.apache.org/docs/python/index.html). Implementations are fast as implementations rely on the vector math capabilities of [NumPy](https://numpy.org/doc/stable/index.html), while other computationally sensitive calculations are JIT-compiled using [Numba](https://numba.pydata.org/).
 
 Here and there we also use [NetworkX](https://networkx.org/documentation/stable/index.html#), [SciPy](https://scipy.org/), [SymPy](https://www.sympy.org/en/index.html) and [scikit-learn](https://scikit-learn.org/stable/).
 
 > **Note** Implementation of the performance critical parts of the library rely on the JIT-compilation capabilities of Numba. This means that the library performs well even for large scale problems, on the expense of a longer first call.
 
 ## Highlights
 
-- Classes to handle points, pointclouds, reference frames and jagged topologies.
-- Array-like mesh composition with a Numba-jittable database model. Join or split meshes, attach numerical data and save to and load from disk.
-- Simplified and preconfigured plotting facility using PyVista.
-- Grid generation in 1, 2 and 3 dimensions for arbitrarily structured Lagrangian cells.
-- A mechanism for all sorts of geometrical and topological transformations.
-- A customizable nodal distribution mechanism to effortlessly pass around data between points and cells.
-- Generation of *Pseudo Peripheral Nodes*, *Rooted Level Structures* and *Adjancency Matrices* for arbitrary polygonal meshes.
-- Symbolic shape function generation for arbitrarily structured Lagrangian cells in 1, 2 and 3 dimensions.
-- Connections to popular third party libraries.
+* Classes to handle points, pointclouds, reference frames and jagged topologies.
+* Array-like mesh composition with a Numba-jittable database model. Join or split meshes, attach numerical data and save to and load from disk.
+* Simplified and preconfigured plotting facility using PyVista.
+* Grid generation in 1, 2 and 3 dimensions for arbitrarily structured Lagrangian cells.
+* A mechanism for all sorts of geometrical and topological transformations.
+* A customizable nodal distribution mechanism to effortlessly pass around data between points and cells.
+* Generation of *Pseudo Peripheral Nodes*, *Rooted Level Structures* and *Adjancency Matrices* for arbitrary polygonal meshes.
+* Symbolic shape function generation for arbitrarily structured Lagrangian cells in 1, 2 and 3 dimensions with an extendible interpolation and extrapolation mechanism.
+* Connections to popular third party libraries like `networkx`, `pandas`, `vtk`, `PyVista` and others.
 
 ## Projects using sigmaepsilon.mesh
 
-- [SigmaEpsilon](https://github.com/dewloosh/SigmaEpsilon) - A Python library for computational solid mechanics.
-- [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
+* [SigmaEpsilon.Solid](https://github.com/sigma-epsilon/sigmaepsilon.solid) - A Python library for computational solid mechanics.
+* [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
 
 ## Documentation
 
-The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
+The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set of examples, and API Reference.
 
 ## Installation
 
 sigmaepsilon.mesh can be installed from PyPI using `pip` on Python >= 3.7:
 
 ```console
 >>> pip install sigmaepsilon.mesh
@@ -120,23 +118,23 @@
 >>> pip install "-e .[test, dev]"
 ```
 
 ## How to contribute?
 
 Contributions are currently expected in any the following ways:
 
-- finding bugs
+* finding bugs
   If you run into trouble when using the library and you think it is a bug, feel free to raise an issue.
-- feedback
+* feedback
   All kinds of ideas are welcome. For instance if you feel like something is still shady (after reading the user guide), we want to know. Be gentle though, the development of the library is financially not supported yet.
-- feature requests
+* feature requests
   Tell us what you think is missing (with realistic expectations).
-- examples
+* examples
   If you've done something with the library and you think that it would make for a good example, get in touch with the developers and we will happily inlude it in the documention.
-- sharing is caring
+* sharing is caring
   If you like the library, share it with your friends or colleagues so they can like it too.
 
 ## Acknowledgements
 
 Although `sigmaepsilon.mesh` works without `VTK` or `PyVista` being installed, it is highly influenced by these libraries and works best with them around. Also shout-out for the developers of `NumPy`, `Scipy`, `Numba`, `Awkward` and all the third-party libraries involved in the project. Whithout these libraries the concept of writing performant, yet elegant Python code would be much more difficult.
 
 **A lot of the packages mentioned on this document here and the introduction have a citable research paper. If you use them in your work through sigmaepsilon.mesh, take a moment to check out their documentations and cite their papers.**
```

### Comparing `sigmaepsilon.mesh-0.0.3/README.md` & `sigmaepsilon.mesh-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,44 +5,42 @@
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main)
 [![Documentation Status](https://readthedocs.org/projects/sigmaepsilonmesh/badge/?version=latest)](https://sigmaepsilonmesh.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://badge.fury.io/py/sigmaepsilon.mesh.svg)](https://pypi.org/project/sigmaepsilon.mesh)
 [![Python 3.7‒3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-> **Warning** sigmaepsilon.mesh is in the early stages of it's lifetime, and some concepts may change in the future. If you seek long-term stability, wait until version 1.0, which is planned to be released if the core concepts all seem to sit and the documentation covers all major concepts.
-
 The [sigmaepsilon.mesh](https://sigmaepsilon.mesh.readthedocs.io/en/latest/) library aims to provide the tools to build and analyse poligonal meshes with complex topologies. Meshes can be built like a dictionary, using arbitarily nested layouts and then be translated to other formats including [VTK](https://vtk.org/) and [PyVista](https://docs.pyvista.org/). For plotting, there is also support for [K3D](http://k3d-jupyter.org/), [Matplotlib](https://matplotlib.org/) and [Plotly](https://plotly.com/python/).
 
 The data model is built around [Awkward](https://awkward-array.org/doc/main/), which makes it possible to attach nested, variable-sized data to the points or the cells in a mesh, also providing interfaces to other popular libraries like [Pandas](https://vtk.org/) or [PyArrow](https://arrow.apache.org/docs/python/index.html). Implementations are fast as implementations rely on the vector math capabilities of [NumPy](https://numpy.org/doc/stable/index.html), while other computationally sensitive calculations are JIT-compiled using [Numba](https://numba.pydata.org/).
 
 Here and there we also use [NetworkX](https://networkx.org/documentation/stable/index.html#), [SciPy](https://scipy.org/), [SymPy](https://www.sympy.org/en/index.html) and [scikit-learn](https://scikit-learn.org/stable/).
 
 > **Note** Implementation of the performance critical parts of the library rely on the JIT-compilation capabilities of Numba. This means that the library performs well even for large scale problems, on the expense of a longer first call.
 
 ## Highlights
 
-- Classes to handle points, pointclouds, reference frames and jagged topologies.
-- Array-like mesh composition with a Numba-jittable database model. Join or split meshes, attach numerical data and save to and load from disk.
-- Simplified and preconfigured plotting facility using PyVista.
-- Grid generation in 1, 2 and 3 dimensions for arbitrarily structured Lagrangian cells.
-- A mechanism for all sorts of geometrical and topological transformations.
-- A customizable nodal distribution mechanism to effortlessly pass around data between points and cells.
-- Generation of *Pseudo Peripheral Nodes*, *Rooted Level Structures* and *Adjancency Matrices* for arbitrary polygonal meshes.
-- Symbolic shape function generation for arbitrarily structured Lagrangian cells in 1, 2 and 3 dimensions.
-- Connections to popular third party libraries.
+* Classes to handle points, pointclouds, reference frames and jagged topologies.
+* Array-like mesh composition with a Numba-jittable database model. Join or split meshes, attach numerical data and save to and load from disk.
+* Simplified and preconfigured plotting facility using PyVista.
+* Grid generation in 1, 2 and 3 dimensions for arbitrarily structured Lagrangian cells.
+* A mechanism for all sorts of geometrical and topological transformations.
+* A customizable nodal distribution mechanism to effortlessly pass around data between points and cells.
+* Generation of *Pseudo Peripheral Nodes*, *Rooted Level Structures* and *Adjancency Matrices* for arbitrary polygonal meshes.
+* Symbolic shape function generation for arbitrarily structured Lagrangian cells in 1, 2 and 3 dimensions with an extendible interpolation and extrapolation mechanism.
+* Connections to popular third party libraries like `networkx`, `pandas`, `vtk`, `PyVista` and others.
 
 ## Projects using sigmaepsilon.mesh
 
-- [SigmaEpsilon](https://github.com/dewloosh/SigmaEpsilon) - A Python library for computational solid mechanics.
-- [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
+* [SigmaEpsilon.Solid](https://github.com/sigma-epsilon/sigmaepsilon.solid) - A Python library for computational solid mechanics.
+* [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
 
 ## Documentation
 
-The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
+The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set of examples, and API Reference.
 
 ## Installation
 
 sigmaepsilon.mesh can be installed from PyPI using `pip` on Python >= 3.7:
 
 ```console
 >>> pip install sigmaepsilon.mesh
@@ -74,23 +72,23 @@
 >>> pip install "-e .[test, dev]"
 ```
 
 ## How to contribute?
 
 Contributions are currently expected in any the following ways:
 
-- finding bugs
+* finding bugs
   If you run into trouble when using the library and you think it is a bug, feel free to raise an issue.
-- feedback
+* feedback
   All kinds of ideas are welcome. For instance if you feel like something is still shady (after reading the user guide), we want to know. Be gentle though, the development of the library is financially not supported yet.
-- feature requests
+* feature requests
   Tell us what you think is missing (with realistic expectations).
-- examples
+* examples
   If you've done something with the library and you think that it would make for a good example, get in touch with the developers and we will happily inlude it in the documention.
-- sharing is caring
+* sharing is caring
   If you like the library, share it with your friends or colleagues so they can like it too.
 
 ## Acknowledgements
 
 Although `sigmaepsilon.mesh` works without `VTK` or `PyVista` being installed, it is highly influenced by these libraries and works best with them around. Also shout-out for the developers of `NumPy`, `Scipy`, `Numba`, `Awkward` and all the third-party libraries involved in the project. Whithout these libraries the concept of writing performant, yet elegant Python code would be much more difficult.
 
 **A lot of the packages mentioned on this document here and the introduction have a citable research paper. If you use them in your work through sigmaepsilon.mesh, take a moment to check out their documentations and cite their papers.**
```

### Comparing `sigmaepsilon.mesh-0.0.3/docs/Makefile` & `sigmaepsilon.mesh-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/make.bat` & `sigmaepsilon.mesh-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/logo.PNG` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/logo.PNG`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot1.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/plot1.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot2.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/plot2.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot3.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/plot3.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot4.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/plot4.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot4a.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/plot4a.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot5.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/plot5.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot6.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/plot6.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/plot7.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/plot7.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_1.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_1.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_2.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_2.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_3.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_3.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_4.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_4.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/_static/readme_5.png` & `sigmaepsilon.mesh-1.0.0/docs/source/_static/readme_5.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/api/api_cells.rst` & `sigmaepsilon.mesh-1.0.0/docs/source/api/api_cells.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,33 @@
 
 This document summarizes the classes denoted to store and handle data about polygonal cells
 in 1, 2 or 3 dimensions.
 
 Base Classes
 ------------
 
-.. automodule:: sigmaepsilon.mesh.cell
+.. automodule:: sigmaepsilon.mesh.cells.base.cell
     :members:
 
-.. automodule:: sigmaepsilon.mesh.line
+.. automodule:: sigmaepsilon.mesh.cells.base.cell1d
+    :members:
+
+.. automodule:: sigmaepsilon.mesh.cells.base.cell2d
+    :members:
+
+.. automodule:: sigmaepsilon.mesh.cells.base.cell3d
+    :members:
+
+.. automodule:: sigmaepsilon.mesh.cells.base.line
     :members: 
 
-.. automodule:: sigmaepsilon.mesh.polygon
+.. automodule:: sigmaepsilon.mesh.cells.base.polygon
     :members: 
 
-.. automodule:: sigmaepsilon.mesh.polyhedron
+.. automodule:: sigmaepsilon.mesh.cells.base.polyhedron
     :members: 
 
 Lagrange Cells
 --------------
 
 .. autoclass:: sigmaepsilon.mesh.cells.l2.L2
     :members:
```

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/api/api_db.rst` & `sigmaepsilon.mesh-1.0.0/docs/source/api/api_db.rst`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/conf.py` & `sigmaepsilon.mesh-1.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/doc_utils.py` & `sigmaepsilon.mesh-1.0.0/docs/source/doc_utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/compound1.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/compound1.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/compound2.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/compound2.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/compound3.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/compound3.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/cube.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/cube.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/cylinder.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/cylinder.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/disc.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/disc.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/grids2d.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/grids2d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/grids3d.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/grids3d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/import_file.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/import_file.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/import_gmsh.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/import_gmsh.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/import_pyvista.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/import_pyvista.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/joint_cube.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/joint_cube.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/lighting.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/lighting.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/shape_functions_1d.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/shape_functions_1d.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/examples/trigridQ4.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/examples/trigridQ4.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/logo.png` & `sigmaepsilon.mesh-1.0.0/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/data.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/data.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/grids.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/grids.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/io.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/io.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_analysis.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/mesh_analysis.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_composition.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/mesh_composition.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/mesh_structure.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/mesh_structure.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/plotting.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/points_and_pointclouds.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/points_and_pointclouds.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/shape_function_generation.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/shape_function_generation.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/trafo_geom.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/trafo_geom.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/notebooks/trafo_topo.ipynb` & `sigmaepsilon.mesh-1.0.0/docs/source/notebooks/trafo_topo.ipynb`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/docs/source/references.bib` & `sigmaepsilon.mesh-1.0.0/docs/source/references.bib`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/logo.png` & `sigmaepsilon.mesh-1.0.0/logo.png`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/pyproject.toml` & `sigmaepsilon.mesh-1.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools-scm",
     "wheel>=0.38.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sigmaepsilon.mesh"
-version = "0.0.3"
+version = "1.0.0"
 description = "A Python package to build, manipulate and analyze polygonal meshes."
 classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/__init__.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/__init__.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/abcdata.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/abcdata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/akwrap.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/akwrap.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/base.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/base.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cell.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/cell.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,35 @@
 from typing import Union, MutableMapping, Iterable, Tuple, List, Callable
 
 import numpy as np
 from numpy import ndarray
 from sympy import Matrix, lambdify
 
 from sigmaepsilon.math import atleast1d, atleast2d, ascont
-from sigmaepsilon.math.utils import to_range_1d
 from sigmaepsilon.math.linalg import ReferenceFrame as FrameLike
 
 from sigmaepsilon.mesh.space import PointCloud, CartesianFrame
-from .celldata import CellData
-from .utils.utils import (
+from ...celldata import CellData
+from ...utils.utils import (
     jacobian_matrix_bulk,
     jacobian_matrix_bulk_1d,
     jacobian_det_bulk_1d,
     points_of_cells,
     pcoords_to_coords,
-    pcoords_to_coords_1d,
-    cells_coords,
-    lengths_of_lines,
     global_shape_function_derivatives,
 )
-from .utils.cells.utils import (
+from ...utils.cells.utils import (
     _loc_to_glob_bulk_,
-    _find_first_hits_,
-    _find_first_hits_knn_,
-    _ntet_to_loc_bulk_,
 )
-from .utils.tri import area_tri_bulk, _pip_tri_bulk_
-from .utils.tet import (
-    vol_tet_bulk,
-    _pip_tet_bulk_knn_,
-    _pip_tet_bulk_,
-    _glob_to_nat_tet_bulk_,
-    _glob_to_nat_tet_bulk_knn_,
-    __pip_tet_bulk__,
-)
-from .utils.space import index_of_closest_point
-from .vtkutils import mesh_to_UnstructuredGrid as mesh_to_vtk
-from .utils.topology.topo import detach_mesh_bulk, rewire
-from .utils.topology import transform_topology
-from .utils.tri import triangulate_cell_coords
-from .utils import cell_center, cell_center_2d, cell_centers_bulk
-from .utils.knn import k_nearest_neighbours
-from .topoarray import TopologyArray
-from .space import CartesianFrame
-from .triang import triangulate
-from .config import __haspyvista__
-
-if __haspyvista__:
-    import pyvista as pv
+from ...utils.topology.topo import detach_mesh_bulk, rewire
+from ...utils import cell_center, cell_centers_bulk
+from ...topoarray import TopologyArray
+from ...space import CartesianFrame
+from .interpolator import LagrangianCellInterpolator
+from ...config import __haspyvista__
 
 MapLike = Union[ndarray, MutableMapping]
 
 
 class PolyCell(CellData):
     """
     A subclass of :class:`sigmaepsilon.mesh.celldata.CellData` as a base class
@@ -81,15 +57,15 @@
         Ought to return local coordinates of the master element.
 
         Returns
         -------
         numpy.ndarray
         """
         raise NotImplementedError
-    
+
     @classmethod
     def master_coordinates(cls) -> ndarray:
         """
         Returns the coordinates of the master element.
 
         Returns
         -------
@@ -136,27 +112,27 @@
         ----------
         return_symbolic: bool, Optional
             If True, the function returns symbolic expressions of shape functions
             and their derivatives. Default is True.
         update: bool, Optional
             If True, class methods are updated with the generated versions.
             Default is True.
-        
+
         Notes
         -----
         Some cells are equipped with functions to evaluate shape functions a-priori,
         other classes rely on symbolic generation of these functions. In the latter case,
         this function is automatically invoked runtime, there is no need to manually
         trigger it.
-        
+
         Example
         -------
         >>> from sigmaepsilon.mesh.cells import H8
         >>> shp, dshp, shpf, shpmf, dshpf = H8.generate_class_functions()
-        
+
         Here `shp` and `dshp` are simbolic matrices for shape functions and
         their first derivatives, `shpf`, `shpmf` and `dshpf` are functions for
         fast evaluation of shape function values, the shape function matrix and
         shape function derivatives, respectively.
         """
         nN = cls.NNODE
         nD = cls.NDIM
@@ -262,15 +238,15 @@
             Locations of the evaluation points.
         N: int, Optional
             Number of unknowns per node.
 
         Returns
         -------
         numpy.ndarray
-            An array of shape (nP, nDOF, nDOF * nNE) where nP, nDOF and nNE
+            An array of shape (nP, nNE, N * nNE) where nP, nDOF and nNE
             are the number of evaluation points, degrees of freedom per node
             and nodes per cell.
         """
         nDOFN = getattr(cls, "NDOFN", N) if N is None else N
         pcoords = np.array(pcoords)
         if cls.shpmfnc is None:
             cls.generate_class_functions(update=True)
@@ -304,15 +280,15 @@
             an nP number of points and nP number cells and nD number of spatial dimensions.
             Default is None.
         dshp: numpy.ndarray, Optional
             Shape function derivatives wrt. the master element. Only relevant if 'jac' is
             provided. The purpose of this argument is to avoid repeated evaluation in situations
             where 'dshp' is required on its own and is already at hand when calling this function.
             Default is None, in which case it is calculated automatically.
-            
+
         Notes
         -----
         Only first derivatives are calculated.
 
         Returns
         -------
         numpy.ndarray
@@ -330,14 +306,70 @@
             return cls.dshpfnc(pcoords).astype(float)
         else:
             pcoords = np.array(pcoords) if pcoords is not None else cls.lcoords()
             if dshp is None:
                 dshp = cls.shape_function_derivatives(pcoords)
             return global_shape_function_derivatives(dshp, jac)
 
+    @classmethod
+    def interpolator(cls, x: Iterable = None) -> LagrangianCellInterpolator:
+        """
+        Returns a callable object that can be used to interpolate over
+        nodal values of one or more cells.
+        
+        Parameters
+        ----------
+        x: Iterable, Optional
+            The locations of known data. It can be fed into the returned interpolator
+            function directly, but since the operation involves the inversion of a matrix
+            related to these locations, it is a good idea to pre calculate it if you want
+            to reuse the interpolator with the same source coordinates.
+            
+        Returns
+        -------
+        :class:`~sigmaepsilon.mesh.cells.base.interpolator.LagrangianCellInterpolator`
+            A callable interpolator class. Refer to its documentation for more examples.
+        
+        Notes
+        -----
+        If the number of source coorindates does not match the number of nodes (and hence
+        the number of shape functions) of the master element of the class, the interpolation
+        is gonna be under or overdetermined and the operation involves the calculation of a 
+        generalized inverse.
+        
+        See also
+        --------
+        :class:`~sigmaepsilon.mesh.cells.LagrangianCellInterpolator`
+        
+        Examples
+        --------
+        Let assume that we know some data at some locations:
+        >>> source_data = [1, 2, 3, 4]
+        >>> source_location = [[-0.5, -0.5], [0.5, -0.5], [0.5, 0.5], [-0.5, 0.5]]
+    
+        We want to extrapolate from this information to the location
+        >>> target_location = [[-2, -2], [2, -2], [2, 2], [-2, 2]]
+        
+        We have provided four points and four data values. If we want an exact extrapolation,
+        we use 4-noded quadrilaterals:
+        
+        >>> from sigmaepsilon.mesh import Q4
+        >>> interpolator = Q4.interpolator()
+        >>> target_data = interpolator(source=source_location, values=source_data, target=target_location)
+        
+        Here we provided 3 inputs to the interpolator. If we want to reuse the interpolator
+        with the same source locations, it is best to provide them when creating the interpolator.
+        This saves some time for repeated evaluations.
+        
+        >>> from sigmaepsilon.mesh import Q4
+        >>> interpolator = Q4.interpolator(source_location)
+        >>> target_data = interpolator(values=source_data, target=target_location)
+        """
+        return LagrangianCellInterpolator(cls, x)
+        
     def jacobian_matrix(
         self, *, pcoords: Iterable[float] = None, dshp: ndarray = None, **__
     ) -> ndarray:
         """
         Returns the jacobian matrices of the cells in the block. The evaluation
         of the matrix is governed by the inputs in the following way:
         - if `dshp` is provided, it must be a matrix of shape function derivatives
@@ -462,15 +494,15 @@
         self,
         *,
         points: Union[float, Iterable] = None,
         cells: Union[int, Iterable] = None,
         target: Union[str, CartesianFrame] = "global",
     ) -> ndarray:
         """
-        Returns the points of the cells as a NumPy array.
+        Returns the points of selected cells as a NumPy array.
         """
         if cells is not None:
             cells = atleast1d(cells)
             conds = np.isin(cells, self.id)
             cells = atleast1d(cells[conds])
             assert len(cells) > 0, "Length of cells is zero!"
         else:
@@ -691,15 +723,15 @@
             return self.to_simplices()
         elif NDIM == 2:
             return self.to_triangles()
         elif NDIM == 3:
             return self.to_tetrahedra()
 
     def centers(self, target: FrameLike = None) -> ndarray:
-        """Returns the centers of the cells."""
+        """Returns the centers of the cells of the block."""
         coords = self.source_coords()
         t = self.topology().to_numpy()
         centers = cell_centers_bulk(coords, t)
         if target:
             pc = PointCloud(centers, frame=self.source_frame())
             centers = pc.show(target)
         return centers
@@ -711,547 +743,24 @@
         return np.unique(self.topology())
 
     def points_involved(self) -> PointCloud:
         """Returns the points involved in the cells of the block."""
         return self.source_points()[self.unique_indices()]
 
     def detach_points_cells(self) -> Tuple[ndarray]:
+        """
+        Returns the detached coordinate and topology array of the block.
+        """
         coords = self.container.source().coords()
         topo = self.topology().to_numpy()
         return detach_mesh_bulk(coords, topo)
 
     def _rotate_(self, *args, **kwargs):
         # this is triggered upon transformations performed on the hosting pointcloud
         if self.has_frames:
             source_frame = self.container.source().frame
             new_frames = (
                 CartesianFrame(self.frames, assume_cartesian=True)
                 .rotate(*args, **kwargs)
                 .show(source_frame)
             )
             self.frames = new_frames
-
-
-class PolyCell1d(PolyCell):
-    """Base class for 1d cells"""
-
-    NDIM = 1
-
-    def lenth(self) -> float:
-        """Returns the total length of the cells in the block."""
-        return np.sum(self.lengths())
-
-    def lengths(self) -> ndarray:
-        """
-        Returns the lengths as a NumPy array.
-        """
-        coords = self.container.source().coords()
-        topo = self.topology().to_numpy()
-        return lengths_of_lines(coords, topo)
-
-    def area(self) -> float:
-        # should return area of the surface of the volume
-        raise NotImplementedError
-
-    def areas(self) -> ndarray:
-        """
-        Returns the areas as a NumPy array.
-        """
-        areakey = self._dbkey_areas_
-        if areakey in self.fields:
-            return self[areakey].to_numpy()
-        else:
-            return np.ones((len(self)))
-
-    def volumes(self) -> ndarray:
-        """
-        Returns the volumes as a NumPy array.
-        """
-        return self.lengths() * self.areas()
-
-    def measures(self) -> ndarray:
-        return self.lengths()
-
-    def points_of_cells(
-        self,
-        *,
-        points: Union[float, Iterable] = None,
-        cells: Union[int, Iterable] = None,
-        flatten: bool = False,
-        target: Union[str, CartesianFrame] = "global",
-        rng: Iterable = None,
-        **kwargs,
-    ) -> ndarray:
-        if isinstance(target, str):
-            assert target.lower() in ["global", "g"]
-        else:
-            raise NotImplementedError
-        topo = kwargs.get("topo", self.topology().to_numpy())
-        coords = kwargs.get("coords", None)
-        if coords is None:
-            if self.pointdata is not None:
-                coords = self.pointdata.x
-            else:
-                coords = self.container.source().coords()
-        ecoords = points_of_cells(coords, topo, centralize=False)
-        if points is None and cells is None:
-            return ecoords
-
-        # points or cells is not None
-        if cells is not None:
-            cells = atleast1d(cells)
-            conds = np.isin(cells, self.id)
-            cells = atleast1d(cells[conds])
-            if len(cells) == 0:
-                return {}
-            ecoords = ecoords[cells]
-            topo = topo[cells]
-        else:
-            cells = np.s_[:]
-
-        if points is None:
-            points = np.array(self.lcoords()).flatten()
-            rng = [-1, 1]
-        else:
-            points = np.array(points)
-            rng = np.array([0, 1]) if rng is None else np.array(rng)
-
-        points, rng = to_range_1d(points, source=rng, target=[0, 1]).flatten(), [0, 1]
-        res = pcoords_to_coords_1d(points, ecoords)  # (nE * nP, nD)
-
-        if not flatten:
-            nE = ecoords.shape[0]
-            nP = points.shape[0]
-            res = res.reshape(nE, nP, res.shape[-1])  # (nE, nP, nD)
-
-        return res
-
-    @classmethod
-    def shape_function_values(
-        cls, pcoords: ndarray, *, rng: Iterable = None
-    ) -> ndarray:
-        """
-        Evaluates the shape functions at the specified locations.
-
-        Parameters
-        ----------
-        pcoords: float or Iterable[float]
-            Locations of the evaluation points.
-        rng: Iterable, Optional
-            The range in which the locations ought to be understood,
-            typically [0, 1] or [-1, 1]. Default is [0, 1].
-
-        Returns
-        -------
-        numpy.ndarray
-            An array of shape (nP, nNE) where nP and nNE are the number of
-            evaluation points and shape functions. If there is only one
-            evaluation point, the returned array is one dimensional.
-        """
-        rng = np.array([-1, 1]) if rng is None else np.array(rng)
-        pcoords = atleast1d(np.array(pcoords))
-        pcoords = to_range_1d(pcoords, source=rng, target=[-1, 1])
-        return super().shape_function_values(pcoords)
-
-    @classmethod
-    def shape_function_matrix(
-        cls, pcoords: ndarray, *, rng: Iterable = None, N: int = None
-    ) -> ndarray:
-        """
-        Evaluates the shape function matrix at the specified locations.
-
-        Parameters
-        ----------
-        pcoords: float or Iterable[float]
-            Locations of the evaluation points.
-        rng: Iterable, Optional
-            The range in which the locations ought to be understood,
-            typically [0, 1] or [-1, 1]. Default is [0, 1].
-        N: int, Optional
-            Number of unknowns per node.
-
-        Returns
-        -------
-        numpy.ndarray
-            An array of shape (nP, nDOF, nDOF * nNE) where nP, nDOF and nNE
-            are the number of evaluation points, degrees of freedom per node
-            and nodes per cell.
-        """
-        rng = np.array([-1, 1]) if rng is None else np.array(rng)
-        pcoords = atleast1d(np.array(pcoords))
-        pcoords = to_range_1d(pcoords, source=rng, target=[-1, 1])
-        return super().shape_function_matrix(pcoords, N=N)
-
-    @classmethod
-    def shape_function_derivatives(
-        cls,
-        pcoords: Union[float, Iterable[float]] = None,
-        *,
-        rng: Iterable = None,
-        jac: ndarray = None,
-        dshp: ndarray = None
-    ) -> ndarray:
-        """
-        Evaluates shape function derivatives wrt. the master element or the local
-        coordinate frames of some cells. To control the behaviour, either 'jac' or 'wrt'
-        can be provided.
-
-        Parameters
-        ----------
-        pcoords: float or Iterable[float], Optional
-            Locations of the evaluation points.
-        rng: Iterable, Optional
-            The range in which the locations ought to be understood,
-            typically [0, 1] or [-1, 1]. Default is [0, 1].
-        jac: Iterable, Optional
-            The jacobian matrix as a float array of shape (nE, nP, nD=1, nD=1), evaluated for
-            each point in each cell. Default is None.
-        dshp: numpy.ndarray, Optional
-            Shape function derivatives wrt. the master element. Only relevant if 'jac' is
-            provided. The purpose of this argument is to avoid repeated evaluation in situations
-            where 'dshp' is required on its own and is already at hand when calling this function.
-            Default is None, in which case it is calculated automatically.
-
-        Returns
-        -------
-        numpy.ndarray
-            An array of shape (nP, nNE, nD=1), where nP, nNE and nD are
-            the number of evaluation points, nodes and spatial dimensions.
-        """
-        rng = np.array([-1, 1], dtype=float) if rng is None else np.array(rng)
-        pcoords = atleast1d(np.array(pcoords, dtype=float))
-        pcoords = to_range_1d(pcoords, source=rng, target=[-1, 1])
-        return super().shape_function_derivatives(pcoords, jac=jac, dshp=dshp)
-
-
-class PolyCell2d(PolyCell):
-    """Base class for 2d cells"""
-
-    NDIM = 2
-
-    def area(self) -> float:
-        """
-        Returns the total area of the cells in the block.
-        """
-        return np.sum(self.areas())
-
-    @classmethod
-    def trimap(cls) -> Iterable:
-        """
-        Returns a mapper to transform topology and other data to
-        a collection of T3 triangles.
-        """
-        _, t, _ = triangulate(points=cls.lcoords())
-        return t
-
-    @classmethod
-    def lcenter(cls) -> ndarray:
-        """
-        Ought to return the local coordinates of the center of the
-        master element.
-
-        Returns
-        -------
-        numpy.ndarray
-        """
-        return cell_center_2d(cls.lcoords())
-
-    def to_triangles(self) -> ndarray:
-        """
-        Returns the topology as a collection of T3 triangles.
-        """
-        t = self.topology().to_numpy()
-        return transform_topology(t, self.trimap())
-
-    def areas(self) -> ndarray:
-        """
-        Returns the areas of the cells.
-        """
-        nE = len(self)
-        coords = self.source_coords()
-        topo = self.topology().to_numpy()
-        frames = self.frames
-        ec = points_of_cells(coords, topo, local_axes=frames)
-        trimap = self.__class__.trimap()
-        ec_tri = triangulate_cell_coords(ec, trimap)
-        areas_tri = area_tri_bulk(ec_tri)
-        res = np.sum(areas_tri.reshape(nE, int(len(areas_tri) / nE)), axis=1)
-        return res
-
-    def volumes(self) -> ndarray:
-        """
-        Returns the volumes of the cells.
-        """
-        areas = self.areas()
-        t = self.thickness()
-        return areas * t
-
-    def measures(self) -> ndarray:
-        """
-        Returns the areas of the cells.
-        """
-        return self.areas()
-
-    def local_coordinates(self, *_, target: CartesianFrame = None) -> ndarray:
-        """
-        Returns the local coordinates of the cells of the block.
-        """
-        ec = super(PolyCell2d, self).local_coordinates(target=target)
-        return ascont(ec[:, :, :2])
-
-    def thickness(self) -> ndarray:
-        """
-        Returns the thicknesses of the cells. If not set, a thickness
-        of 1.0 is returned for each cell.
-        """
-        dbkey = self._dbkey_thickness_
-        if dbkey in self.fields:
-            t = self.db[dbkey].to_numpy()
-        else:
-            t = np.ones(len(self), dtype=float)
-        return t
-
-    def pip(
-        self, x: Union[Iterable, ndarray], tol: float = 1e-12
-    ) -> Union[bool, ndarray]:
-        """
-        Returns an 1d boolean integer array that tells if the points specified by 'x'
-        are included in any of the cells in the block.
-
-        Parameters
-        ----------
-        x: Iterable or numpy.ndarray
-            The coordinates of the points that we want to investigate.
-
-        Returns
-        -------
-        bool or numpy.ndarray
-            A single or NumPy array of booleans for every input point.
-        """
-        x = atleast2d(x, front=True)
-        coords = self.source_coords()
-        topo = self.to_triangles()
-        ecoords = points_of_cells(coords, topo, centralize=False)
-        pips = _pip_tri_bulk_(x, ecoords, tol)
-        return np.squeeze(np.any(pips, axis=1))
-
-
-class PolyCell3d(PolyCell):
-    """Base class for 3d cells"""
-
-    NDIM = 3
-
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def measures(self, *args, **kwargs) -> ndarray:
-        """
-        Returns the measures of the block.
-        """
-        return self.volumes(*args, **kwargs)
-
-    @classmethod
-    def tetmap(cls) -> Iterable:
-        """
-        Returns a mapper to transform topology and other data to
-        a collection of T3 triangles.
-        """
-        raise NotImplementedError
-
-    def to_tetrahedra(self, flatten: bool = True) -> ndarray:
-        """
-        Returns the topology as a collection of TET4 tetrahedra.
-
-        Parameters
-        ----------
-        flatten: bool, Optional
-            If True, the topology is returned as a 2d array. If False, the
-            length of the first axis equals the number of cells in the block,
-            the length of the second axis equals the number of tetrahedra per
-            cell.
-        """
-        t = self.topology().to_numpy()
-        tetmap = self.tetmap()
-        tetra = transform_topology(t, tetmap)
-        if flatten:
-            return tetra
-        else:
-            nE = len(t)
-            nT = len(tetmap)
-            return tetra.reshape(nE, nT, 4)
-
-    def to_vtk(self, detach: bool = False):
-        """
-        Returns the block as a VTK object.
-        """
-        coords = self.container.source().coords()
-        topo = self.topology().to_numpy()
-        vtkid = self.__class__.vtkCellType
-        if detach:
-            ugrid = mesh_to_vtk(*detach_mesh_bulk(coords, topo), vtkid)
-        else:
-            ugrid = mesh_to_vtk(coords, topo, vtkid)
-        return ugrid
-
-    if __haspyvista__:
-
-        def to_pv(
-            self, detach: bool = False
-        ) -> Union[pv.UnstructuredGrid, pv.PolyData]:
-            """
-            Returns the block as a pyVista object.
-            """
-            return pv.wrap(self.to_vtk(detach=detach))
-
-    def extract_surface(self, detach: bool = False) -> Tuple[ndarray]:
-        """
-        Extracts the surface of the object.
-        """
-        coords = self.source_coords()
-        pvs = self.to_pv(detach=False).extract_surface()
-        s = pvs.triangulate().cast_to_unstructured_grid()
-        topo = s.cells_dict[5]
-        if detach:
-            return s.points, topo
-        else:
-            coords = self.source_coords()
-            imap = index_of_closest_point(coords, np.array(s.points, dtype=float))
-            topo = rewire(topo, imap)
-            return coords, topo
-
-    def boundary(self, detach: bool = False) -> Tuple[ndarray]:
-        """
-        Returns the boundary of the block as 2 NumPy arrays.
-        """
-        return self.extract_surface(detach=detach)
-
-    def volumes(self) -> ndarray:
-        """
-        Returns the volumes of the block as an 1d float array.
-        """
-        coords = self.source_coords()
-        topo = self.topology().to_numpy()
-        topo_tet = self.to_tetrahedra()
-        volumes = vol_tet_bulk(cells_coords(coords, topo_tet))
-        res = np.sum(
-            volumes.reshape(topo.shape[0], int(len(volumes) / topo.shape[0])), axis=1
-        )
-        return res
-
-    def locate(
-        self,
-        x: Union[Iterable, ndarray],
-        lazy: bool = True,
-        tol: float = 1e-12,
-        k: int = 4,
-    ) -> Tuple[ndarray]:
-        """
-        Locates a set of points inside the cells of the block.
-
-        Parameters
-        ----------
-        x: Iterable or numpy.ndarray
-            The coordinates of the points that we want to investigate.
-        tol: float, Optional
-            Floating point tolerance for detecting boundaries. Default is 1e-12.
-        lazy: bool, Optional
-            If False, the ckeck is performed for all cells in the block. If True,
-            it is used in combination with parameter 'k' and the check is only performed
-            for the k nearest neighbours of the input points. Default is True.
-        k: int, Optional
-            The number of neighbours for the case when 'lazy' is true. Default is 4.
-
-        Returns
-        -------
-        numpy.ndarray
-            The indices of 'x' that are inside one of the cells of the block.
-        numpy.ndarray
-            The block-local indices of the cells that include the points with
-            the returned indices.
-        numpy.ndarray
-            The master coordinates of the located points inside the including cells.
-        """
-        x = atleast2d(x, front=True)
-
-        coords = self.source_coords()
-        topo = self.topology()
-        topo_tet = self.to_tetrahedra(flatten=True)
-        ecoords_tet = points_of_cells(coords, topo_tet, centralize=False)
-        tetmap = self.tetmap()
-
-        # perform point-in-polygon test for tetrahedra
-        if lazy:
-            centers_tet = cell_centers_bulk(coords, topo_tet)
-            k_tet = min(k, len(centers_tet))
-            neighbours_tet = k_nearest_neighbours(centers_tet, x, k=k_tet)
-            nat_tet = _glob_to_nat_tet_bulk_knn_(
-                x, ecoords_tet, neighbours_tet
-            )  # (nP, kTET, 4)
-            pips_tet = __pip_tet_bulk__(nat_tet, tol)  # (nP, kTET)
-        else:
-            nat_tet = _glob_to_nat_tet_bulk_(x, ecoords_tet)  # (nP, nTET, 4)
-            pips_tet = __pip_tet_bulk__(nat_tet, tol)  # (nP, nTET)
-
-        # locate the points that are inside any of the cells
-        pip = np.squeeze(np.any(pips_tet, axis=1))  # (nP)
-        i_source = np.where(pip)[0]  # (nP_)
-        if lazy:
-            points_to_tets, points_to_neighbours = _find_first_hits_knn_(
-                pips_tet[i_source], neighbours_tet[i_source]
-            )
-        else:
-            points_to_tets, points_to_neighbours = _find_first_hits_(pips_tet[i_source])
-        tets_to_cells = np.floor(np.arange(len(topo_tet)) / len(tetmap)).astype(int)
-        i_target = tets_to_cells[points_to_tets]  # (nP_)
-
-        # locate the cells that contain the points
-        cell_tet_indices = np.tile(np.arange(tetmap.shape[0]), len(topo))[
-            points_to_tets
-        ]
-        nat_tet = nat_tet[i_source]  # (nP_, nTET, 4)
-        locations_target = _ntet_to_loc_bulk_(
-            self.lcoords(), nat_tet, tetmap, cell_tet_indices, points_to_neighbours
-        )
-
-        return i_source, i_target, locations_target
-
-    def pip(
-        self,
-        x: Union[Iterable, ndarray],
-        tol: float = 1e-12,
-        lazy: bool = True,
-        k: int = 4,
-    ) -> Union[bool, ndarray]:
-        """
-        Returns an 1d boolean integer array that tells if the points specified by 'x'
-        are included in any of the cells in the block.
-
-        Parameters
-        ----------
-        x: Iterable or numpy.ndarray
-            The coordinates of the points that we want to investigate.
-        tol: float, Optional
-            Floating point tolerance for detecting boundaries. Default is 1e-12.
-        lazy: bool, Optional
-            If False, the ckeck is performed for all cells in the block. If True,
-            it is used in combination with parameter 'k' and the check is only performed
-            for the k nearest neighbours of the input points. Default is True.
-        k: int, Optional
-            The number of neighbours for the case when 'lazy' is true. Default is 4.
-
-        Returns
-        -------
-        bool or numpy.ndarray
-            A single or NumPy array of booleans for every input point.
-        """
-        x = atleast2d(x, front=True)
-        coords = self.source_coords()
-        tetra = self.to_tetrahedra(flatten=True)
-        ecoords = points_of_cells(coords, tetra, centralize=False)
-        if lazy:
-            centers = cell_centers_bulk(coords, tetra)
-            k = min(k, len(centers))
-            knn = k_nearest_neighbours(centers, x, k=k)
-            pips = _pip_tet_bulk_knn_(x, ecoords, knn, tol)
-        else:
-            pips = _pip_tet_bulk_(x, ecoords, tol)
-        return np.squeeze(np.any(pips, axis=1))
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/celldata.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/celldata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/__init__.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from .tet4 import TET4
 from .tet4 import TET4 as Tetra
 from .tet10 import TET10
 from .w6 import W6
 from .w6 import W6 as Wedge
 from .w18 import W18
 
+from .base.interpolator import LagrangianCellInterpolator
 
 __all__ = [
     "L2",
     "Line",
     "L3",
     "QuadraticLine",
     "T3",
@@ -36,8 +37,9 @@
     "H27",
     "TET4",
     "Tetra",
     "TET10",
     "W6",
     "Wedge",
     "W18",
+    "LagrangianCellInterpolator"
 ]
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/h27.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/h27.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 import sympy as sy
 
 from sigmaepsilon.math.numint import gauss_points as gp
 
-from ..polyhedron import TriquadraticHexaHedron
+from .base.polyhedron import TriquadraticHexaHedron
 from ..utils.utils import cells_coords
 from ..utils.cells.h27 import (
     shp_H27_multi,
     dshp_H27_multi,
     volumes_H27,
     shape_function_matrix_H27_multi,
     monoms_H27,
 )
-from ..utils.cells.gauss import Gauss_Legendre_Hex_Grid
+from ..utils.cells.numint import Gauss_Legendre_Hex_Grid
 
 
 class H27(TriquadraticHexaHedron):
     """
     27-node isoparametric triquadratic hexahedron.
 
     ::
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/h8.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/h8.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from sympy import symbols
 import numpy as np
 from numpy import ndarray
 
 from sigmaepsilon.math.numint import gauss_points as gp
 
-from ..polyhedron import HexaHedron
+from .base.polyhedron import HexaHedron
 from ..utils.utils import cells_coords
 from ..utils.cells.h8 import (
     shp_H8_multi,
     dshp_H8_multi,
     volumes_H8,
     shape_function_matrix_H8_multi,
     monoms_H8,
 )
-from ..utils.cells.gauss import Gauss_Legendre_Hex_Grid
+from ..utils.cells.numint import Gauss_Legendre_Hex_Grid
 
 
 class H8(HexaHedron):
     """
     8-node isoparametric hexahedron.
 
     ::
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/l2.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/l2.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from typing import Tuple, List
 
 import numpy as np
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..line import Line
+from .base.line import Line
 from ..utils.cells.l2 import (
     shp_L2_multi,
     dshp_L2_multi,
     shape_function_matrix_L2_multi,
     monoms_L2,
 )
-from ..utils.cells.gauss import Gauss_Legendre_Line_Grid
+from ..utils.cells.numint import Gauss_Legendre_Line_Grid
 
 __all__ = ["L2"]
 
 
 class L2(Line):
     """
     2-Node line element.
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/l3.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/l3.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..line import QuadraticLine
-from ..utils.cells.gauss import Gauss_Legendre_Line_Grid
+from .base.line import QuadraticLine
+from ..utils.cells.numint import Gauss_Legendre_Line_Grid
 from ..utils.cells.l3 import monoms_L3
 
 
 __all__ = ["L3"]
 
 
 class L3(QuadraticLine):
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/q4.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/q4.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..polygon import Quadrilateral
+from .base.polygon import Quadrilateral
 from ..utils.cells.q4 import (
     shp_Q4_multi,
     dshp_Q4_multi,
     shape_function_matrix_Q4_multi,
     monoms_Q4,
 )
-from ..utils.cells.gauss import Gauss_Legendre_Quad_4
+from ..utils.cells.numint import Gauss_Legendre_Quad_4
 
 
 class Q4(Quadrilateral):
     """
     Polygon class for 4-noded bilinear quadrilaterals.
 
     See Also
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/q9.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/q9.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..polygon import BiQuadraticQuadrilateral
+from .base.polygon import BiQuadraticQuadrilateral
 from ..utils.cells.q9 import (
     shp_Q9_multi,
     dshp_Q9_multi,
     shape_function_matrix_Q9_multi,
     monoms_Q9,
 )
-from ..utils.cells.gauss import Gauss_Legendre_Quad_9
+from ..utils.cells.numint import Gauss_Legendre_Quad_9
 
 
 class Q9(BiQuadraticQuadrilateral):
     """
     Polygon class for 9-noded biquadratic quadrilaterals.
 
     See Also
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/t3.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/t3.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..polygon import Triangle
-from ..utils.cells.gauss import Gauss_Legendre_Tri_1
+from .base.polygon import Triangle
+from ..utils.cells.numint import Gauss_Legendre_Tri_1
 from ..utils.cells.t3 import (
     shp_T3_multi,
     dshp_T3_multi,
     shape_function_matrix_T3_multi,
     monoms_T3,
 )
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/t6.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/t6.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # -*- coding: utf-8 -*-
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
 from ..utils.utils import cells_coords
-from ..polygon import QuadraticTriangle as Triangle
+from .base.polygon import QuadraticTriangle as Triangle
 from ..utils.cells.t6 import (
     shp_T6_multi,
     dshp_T6_multi,
     areas_T6,
     shape_function_matrix_T6_multi,
     monoms_T6,
 )
-from ..utils.cells.gauss import Gauss_Legendre_Tri_3a
+from ..utils.cells.numint import Gauss_Legendre_Tri_3a
 
 
 class T6(Triangle):
     """
     A class to handle 6-noded triangles.
 
     See Also
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/tet10.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/tet10.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..polyhedron import QuadraticTetraHedron
+from .base.polyhedron import QuadraticTetraHedron
 from ..utils.cells.tet10 import (
     monoms_TET10,
 )
-from ..utils.cells.gauss import Gauss_Legendre_Tet_4
+from ..utils.cells.numint import Gauss_Legendre_Tet_4
 from ..utils.cells.utils import volumes
 from ..utils.utils import cells_coords
 
 
 class TET10(QuadraticTetraHedron):
     """
     10-node isoparametric hexahedron.
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/tet4.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/tet4.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..polyhedron import TetraHedron
+from .base.polyhedron import TetraHedron
 from ..utils.cells.tet4 import (
     shp_TET4_multi,
     dshp_TET4_multi,
     shape_function_matrix_TET4_multi,
     monoms_TET4,
 )
-from ..utils.cells.gauss import Gauss_Legendre_Tet_1
+from ..utils.cells.numint import Gauss_Legendre_Tet_1
 
 
 class TET4(TetraHedron):
     """
     4-node isoparametric hexahedron.
 
     See Also
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/w18.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/w18.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..polyhedron import BiquadraticWedge
-from ..utils.cells.gauss import Gauss_Legendre_Wedge_3x3
+from .base.polyhedron import BiquadraticWedge
+from ..utils.cells.numint import Gauss_Legendre_Wedge_3x3
 from ..utils.cells.utils import volumes
 from ..utils.utils import cells_coords
 from ..utils.cells.w18 import monoms_W18
 
 
 class W18(BiquadraticWedge):
     """
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/cells/w6.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/w6.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple, List
 import numpy as np
 from numpy import ndarray
 from sympy import symbols
 
-from ..polyhedron import Wedge
-from ..utils.cells.gauss import Gauss_Legendre_Wedge_3x2
+from .base.polyhedron import Wedge
+from ..utils.cells.numint import Gauss_Legendre_Wedge_3x2
 from ..utils.cells.utils import volumes
 from ..utils.utils import cells_coords
 from ..utils.cells.w6 import monoms_W6
 
 
 class W6(Wedge):
     """
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/config.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/config.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/downloads.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/downloads.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/extrude.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/extrude.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/grid.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/grid.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/inp2stl.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/io/inp2stl.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/io/io.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/io/io.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/linedata.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/linedata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/mesh1d.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/mesh1d.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/pointdata.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/pointdata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polydata.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/polydata.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     detach_mesh_bulk,
     cells_at_nodes,
 )
 from .topoarray import TopologyArray
 from .pointdata import PointData
 from .celldata import CellData
 from .base import PolyDataBase
-from .cell import PolyCell
+from .cells.base.cell import PolyCell
 from .helpers import meshio_to_celltype, vtk_to_celltype
 from .vtkutils import PolyData_to_mesh
 from .config import __hasvtk__, __haspyvista__, __hask3d__, __hasmatplotlib__
 
 if __hasvtk__:
     import vtk
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polygon.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/polygon.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 
-from .utils.utils import points_of_cells
-from .utils.tri import area_tri_bulk
-from .utils.topology import T6_to_T3, Q4_to_T3, Q9_to_Q4, T3_to_T6
-from .cell import PolyCell2d
+from ...utils.utils import points_of_cells
+from ...utils.tri import area_tri_bulk
+from ...utils.topology import T6_to_T3, Q4_to_T3, Q9_to_Q4, T3_to_T6
+from .cell2d import PolyCell2d
 
 
 class PolyGon(PolyCell2d):
     """
     Base class for polygons.
     """
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/polyhedron.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/cells/base/polyhedron.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 import numpy as np
 
 from .polygon import Triangle
-from .cell import PolyCell3d
-from .utils.topology import compose_trmap
+from .cell3d import PolyCell3d
+from ...utils.topology import compose_trmap
 
 
 class PolyHedron(PolyCell3d):
     """Base class to handle polyhedra."""
 
     _face_cls_ = Triangle
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/pop.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/pop.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/recipes.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/recipes.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/section.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/section.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/frame.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/space/frame.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/point.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/space/point.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/space/pointcloud.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/space/pointcloud.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tetmesh.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/tetmesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tetrahedralize.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/tetrahedralize.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/tile.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/tile.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/topoarray.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/topoarray.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/triang.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/triang.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/trimesh.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/trimesh.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/gauss.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/numint.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,90 +1,92 @@
+from typing import Tuple
 import numpy as np
+from numpy import ndarray
 
 from sigmaepsilon.math.numint import gauss_points as gp
 
 
 # LINES
 
 
-def Gauss_Legendre_Line_Grid(n: int):
+def Gauss_Legendre_Line_Grid(n: int) -> Tuple[ndarray]:
     return gp(n)
 
 
 #  TRIANGLES
 
 
-def Gauss_Legendre_Tri_1():
+def Gauss_Legendre_Tri_1() -> Tuple[ndarray]:
     return np.array([[1 / 3, 1 / 3]]), np.array([1 / 2])
 
 
-def Gauss_Legendre_Tri_3a():
+def Gauss_Legendre_Tri_3a() -> Tuple[ndarray]:
     p = np.array([[1 / 6, 1 / 6], [2 / 3, 1 / 6], [1 / 6, 2 / 3]])
     w = np.array([1 / 6, 1 / 6, 1 / 6])
     return p, w
 
 
-def Gauss_Legendre_Tri_3b():
+def Gauss_Legendre_Tri_3b() -> Tuple[ndarray]:
     p = np.array([[1 / 2, 1 / 2], [0, 1 / 2], [1 / 2, 0]])
     w = np.array([1 / 6, 1 / 6, 1 / 6])
     return p, w
 
 
 #  QUADRILATERALS
 
 
-def Gauss_Legendre_Quad_Grid(n: int, m: int = None):
-    m = n if m is None else m
-    return gp(n, m)
+def Gauss_Legendre_Quad_Grid(i: int, j: int = None) -> Tuple[ndarray]:
+    j = i if j is None else j
+    return gp(i, j)
 
 
-def Gauss_Legendre_Quad_1():
+def Gauss_Legendre_Quad_1() -> Tuple[ndarray]:
     return gp(1, 1)
 
 
-def Gauss_Legendre_Quad_4():
+def Gauss_Legendre_Quad_4() -> Tuple[ndarray]:
     return gp(2, 2)
 
 
-def Gauss_Legendre_Quad_9():
+def Gauss_Legendre_Quad_9() -> Tuple[ndarray]:
     return gp(3, 3)
 
 
 #  TETRAHEDRA
 
 
-def Gauss_Legendre_Tet_1():
+def Gauss_Legendre_Tet_1() -> Tuple[ndarray]:
     p = np.array([[1 / 4, 1 / 4, 1 / 4]])
     w = np.array([1 / 6])
     return p, w
 
 
-def Gauss_Legendre_Tet_4():
+def Gauss_Legendre_Tet_4() -> Tuple[ndarray]:
     a = (5 + 3 * np.sqrt(5)) / 20
     b = (5 - np.sqrt(5)) / 20
     p = np.array([[a, b, b], [b, a, b], [b, b, a], [b, b, b]])
     w = np.full(4, 1 / 24)
     return p, w
 
 
-def Gauss_Legendre_Tet_5():
+def Gauss_Legendre_Tet_5() -> Tuple[ndarray]:
     p = np.array(
         [
             [1 / 4, 1 / 4, 1 / 4],
             [1 / 2, 1 / 6, 1 / 6],
             [1 / 6, 1 / 2, 1 / 6],
             [1 / 6, 1 / 6, 1 / 2],
             [1 / 6, 1 / 6, 1 / 6],
         ]
     )
     w = np.array([-4 / 30, 9 / 120, 9 / 120, 9 / 120, 9 / 120])
     return p, w
 
 
-def Gauss_Legendre_Tet_11():
+def Gauss_Legendre_Tet_11() -> Tuple[ndarray]:
     a = (1 + 3 * np.sqrt(5 / 15)) / 4
     b = (1 - np.sqrt(5 / 14)) / 4
     p = np.array(
         [
             [1 / 4, 1 / 4, 1 / 4],
             [11 / 14, 1 / 14, 1 / 14],
             [1 / 14, 11 / 14, 1 / 14],
@@ -114,39 +116,38 @@
         ]
     )
     return p, w
 
 
 #  HEXAHEDRA
 
-
-def Gauss_Legendre_Hex_Grid(n: int, m: int = None, k: int = None):
-    m = n if m is None else m
-    k = m if k is None else k
-    return gp(n, m, k)
+def Gauss_Legendre_Hex_Grid(i: int, j: int = None, k: int = None) -> Tuple[ndarray]:
+    j = i if j is None else j
+    k = j if k is None else k
+    return gp(i, j, k)
 
 
 # WEDGES
 
 
-def Gauss_Legendre_Wedge_3x2():
+def Gauss_Legendre_Wedge_3x2() -> Tuple[ndarray]:
     p_tri, w_tri = Gauss_Legendre_Tri_3a()
     p_line, w_line = Gauss_Legendre_Line_Grid(2)
     p = np.zeros((6, 3), dtype=float)
     w = np.zeros((6,), dtype=float)
     p[:3, :2] = p_tri
     p[:3, 2] = p_line[0]
     w[:3] = w_tri * w_line[0]
     p[3:6, :2] = p_tri
     p[3:6, 2] = p_line[0]
     w[3:6] = w_tri * w_line[1]
     return p, w
 
 
-def Gauss_Legendre_Wedge_3x3():
+def Gauss_Legendre_Wedge_3x3() -> Tuple[ndarray]:
     p_tri, w_tri = Gauss_Legendre_Tri_3a()
     p_line, w_line = Gauss_Legendre_Line_Grid(3)
     n = len(w_line) * len(w_tri)
     p = np.zeros((n, 3), dtype=float)
     w = np.zeros((n,), dtype=float)
     for i in range(len(w_line)):
         p[i * 3 : (i + 1) * 3, :2] = p_tri
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/h27.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/h27.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/h8.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/h8.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/l2.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/l2.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/q4.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/q4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/q9.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/q9.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/t3.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/t3.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/t6.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/t6.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/tet10.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/tet10.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/tet4.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/tet4.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/utils.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/w18.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/w18.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/cells/w6.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/cells/w6.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/colors.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/colors.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/knn.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/knn.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/locate.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/locate.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/space.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/space.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/tet.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/tet.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topodata.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/topodata.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/topo.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/topology/topo.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/topology/tr.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/topology/tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/tri.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/tri.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/utils/utils.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/utils/utils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/voxelize.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/voxelize.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/vtkcelltypes.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/vtkcelltypes.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon/mesh/vtkutils.py` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon/mesh/vtkutils.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/PKG-INFO` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmaepsilon.mesh
-Version: 0.0.3
+Version: 1.0.0
 Summary: A Python package to build, manipulate and analyze polygonal meshes.
 Author-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 Maintainer-email: SigmaEpsilon <bencebalogh@sigmaepsilon.com>
 License: MIT License
         
         Copyright (c) 2021 SigmaEpsilon
         
@@ -51,44 +51,42 @@
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/sigma-epsilon/sigmaepsilon.mesh/tree/main)
 [![Documentation Status](https://readthedocs.org/projects/sigmaepsilonmesh/badge/?version=latest)](https://sigmaepsilonmesh.readthedocs.io/en/latest/?badge=latest)
 [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI](https://badge.fury.io/py/sigmaepsilon.mesh.svg)](https://pypi.org/project/sigmaepsilon.mesh)
 [![Python 3.7‒3.10](https://img.shields.io/badge/python-3.7%E2%80%923.10-blue)](https://www.python.org)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-> **Warning** sigmaepsilon.mesh is in the early stages of it's lifetime, and some concepts may change in the future. If you seek long-term stability, wait until version 1.0, which is planned to be released if the core concepts all seem to sit and the documentation covers all major concepts.
-
 The [sigmaepsilon.mesh](https://sigmaepsilon.mesh.readthedocs.io/en/latest/) library aims to provide the tools to build and analyse poligonal meshes with complex topologies. Meshes can be built like a dictionary, using arbitarily nested layouts and then be translated to other formats including [VTK](https://vtk.org/) and [PyVista](https://docs.pyvista.org/). For plotting, there is also support for [K3D](http://k3d-jupyter.org/), [Matplotlib](https://matplotlib.org/) and [Plotly](https://plotly.com/python/).
 
 The data model is built around [Awkward](https://awkward-array.org/doc/main/), which makes it possible to attach nested, variable-sized data to the points or the cells in a mesh, also providing interfaces to other popular libraries like [Pandas](https://vtk.org/) or [PyArrow](https://arrow.apache.org/docs/python/index.html). Implementations are fast as implementations rely on the vector math capabilities of [NumPy](https://numpy.org/doc/stable/index.html), while other computationally sensitive calculations are JIT-compiled using [Numba](https://numba.pydata.org/).
 
 Here and there we also use [NetworkX](https://networkx.org/documentation/stable/index.html#), [SciPy](https://scipy.org/), [SymPy](https://www.sympy.org/en/index.html) and [scikit-learn](https://scikit-learn.org/stable/).
 
 > **Note** Implementation of the performance critical parts of the library rely on the JIT-compilation capabilities of Numba. This means that the library performs well even for large scale problems, on the expense of a longer first call.
 
 ## Highlights
 
-- Classes to handle points, pointclouds, reference frames and jagged topologies.
-- Array-like mesh composition with a Numba-jittable database model. Join or split meshes, attach numerical data and save to and load from disk.
-- Simplified and preconfigured plotting facility using PyVista.
-- Grid generation in 1, 2 and 3 dimensions for arbitrarily structured Lagrangian cells.
-- A mechanism for all sorts of geometrical and topological transformations.
-- A customizable nodal distribution mechanism to effortlessly pass around data between points and cells.
-- Generation of *Pseudo Peripheral Nodes*, *Rooted Level Structures* and *Adjancency Matrices* for arbitrary polygonal meshes.
-- Symbolic shape function generation for arbitrarily structured Lagrangian cells in 1, 2 and 3 dimensions.
-- Connections to popular third party libraries.
+* Classes to handle points, pointclouds, reference frames and jagged topologies.
+* Array-like mesh composition with a Numba-jittable database model. Join or split meshes, attach numerical data and save to and load from disk.
+* Simplified and preconfigured plotting facility using PyVista.
+* Grid generation in 1, 2 and 3 dimensions for arbitrarily structured Lagrangian cells.
+* A mechanism for all sorts of geometrical and topological transformations.
+* A customizable nodal distribution mechanism to effortlessly pass around data between points and cells.
+* Generation of *Pseudo Peripheral Nodes*, *Rooted Level Structures* and *Adjancency Matrices* for arbitrary polygonal meshes.
+* Symbolic shape function generation for arbitrarily structured Lagrangian cells in 1, 2 and 3 dimensions with an extendible interpolation and extrapolation mechanism.
+* Connections to popular third party libraries like `networkx`, `pandas`, `vtk`, `PyVista` and others.
 
 ## Projects using sigmaepsilon.mesh
 
-- [SigmaEpsilon](https://github.com/dewloosh/SigmaEpsilon) - A Python library for computational solid mechanics.
-- [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
+* [SigmaEpsilon.Solid](https://github.com/sigma-epsilon/sigmaepsilon.solid) - A Python library for computational solid mechanics.
+* [PyAxisVM](https://github.com/AxisVM/pyaxisvm) - The official Python package of [AxisVM](https://axisvm.eu/), a popular structural analysis and design software.
 
 ## Documentation
 
-The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set examples, and the API Reference.
+The [documentation](https://sigmaepsilonmesh.readthedocs.io/en/latest/) is built with [Sphinx](https://www.sphinx-doc.org/en/master/) using the [PyData Sphinx Theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/index.html) and hosted on [ReadTheDocs](https://readthedocs.org/). Check it out for the user guide, an ever growing set of examples, and API Reference.
 
 ## Installation
 
 sigmaepsilon.mesh can be installed from PyPI using `pip` on Python >= 3.7:
 
 ```console
 >>> pip install sigmaepsilon.mesh
@@ -120,23 +118,23 @@
 >>> pip install "-e .[test, dev]"
 ```
 
 ## How to contribute?
 
 Contributions are currently expected in any the following ways:
 
-- finding bugs
+* finding bugs
   If you run into trouble when using the library and you think it is a bug, feel free to raise an issue.
-- feedback
+* feedback
   All kinds of ideas are welcome. For instance if you feel like something is still shady (after reading the user guide), we want to know. Be gentle though, the development of the library is financially not supported yet.
-- feature requests
+* feature requests
   Tell us what you think is missing (with realistic expectations).
-- examples
+* examples
   If you've done something with the library and you think that it would make for a good example, get in touch with the developers and we will happily inlude it in the documention.
-- sharing is caring
+* sharing is caring
   If you like the library, share it with your friends or colleagues so they can like it too.
 
 ## Acknowledgements
 
 Although `sigmaepsilon.mesh` works without `VTK` or `PyVista` being installed, it is highly influenced by these libraries and works best with them around. Also shout-out for the developers of `NumPy`, `Scipy`, `Numba`, `Awkward` and all the third-party libraries involved in the project. Whithout these libraries the concept of writing performant, yet elegant Python code would be much more difficult.
 
 **A lot of the packages mentioned on this document here and the introduction have a citable research paper. If you use them in your work through sigmaepsilon.mesh, take a moment to check out their documentations and cite their papers.**
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/SOURCES.txt` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 docs/source/_static/readme_1.png
 docs/source/_static/readme_2.png
 docs/source/_static/readme_3.png
 docs/source/_static/readme_4.png
 docs/source/_static/readme_5.png
 docs/source/api/api_cells.rst
 docs/source/api/api_db.rst
+docs/source/api/api_interpolator.rst
 docs/source/api/api_recipes.rst
 docs/source/api/api_space.rst
 docs/source/api/api_topo.rst
 docs/source/api/api_utils.rst
 docs/source/examples/compound1.ipynb
 docs/source/examples/compound2.ipynb
 docs/source/examples/compound3.ipynb
@@ -55,14 +56,15 @@
 docs/source/examples/import_pyvista.ipynb
 docs/source/examples/joint_cube.ipynb
 docs/source/examples/lighting.ipynb
 docs/source/examples/shape_functions_1d.ipynb
 docs/source/examples/trigridQ4.ipynb
 docs/source/notebooks/data.ipynb
 docs/source/notebooks/grids.ipynb
+docs/source/notebooks/interpolation.ipynb
 docs/source/notebooks/io.ipynb
 docs/source/notebooks/mesh_analysis.ipynb
 docs/source/notebooks/mesh_composition.ipynb
 docs/source/notebooks/mesh_structure.ipynb
 docs/source/notebooks/plotting.ipynb
 docs/source/notebooks/points_and_pointclouds.ipynb
 docs/source/notebooks/shape_function_generation.ipynb
@@ -73,28 +75,24 @@
 src/sigmaepsilon.mesh.egg-info/dependency_links.txt
 src/sigmaepsilon.mesh.egg-info/requires.txt
 src/sigmaepsilon.mesh.egg-info/top_level.txt
 src/sigmaepsilon/mesh/__init__.py
 src/sigmaepsilon/mesh/abcdata.py
 src/sigmaepsilon/mesh/akwrap.py
 src/sigmaepsilon/mesh/base.py
-src/sigmaepsilon/mesh/cell.py
 src/sigmaepsilon/mesh/celldata.py
 src/sigmaepsilon/mesh/config.py
 src/sigmaepsilon/mesh/downloads.py
 src/sigmaepsilon/mesh/extrude.py
 src/sigmaepsilon/mesh/grid.py
 src/sigmaepsilon/mesh/helpers.py
-src/sigmaepsilon/mesh/line.py
 src/sigmaepsilon/mesh/linedata.py
 src/sigmaepsilon/mesh/mesh1d.py
 src/sigmaepsilon/mesh/pointdata.py
 src/sigmaepsilon/mesh/polydata.py
-src/sigmaepsilon/mesh/polygon.py
-src/sigmaepsilon/mesh/polyhedron.py
 src/sigmaepsilon/mesh/pop.py
 src/sigmaepsilon/mesh/recipes.py
 src/sigmaepsilon/mesh/section.py
 src/sigmaepsilon/mesh/tetmesh.py
 src/sigmaepsilon/mesh/tetrahedralize.py
 src/sigmaepsilon/mesh/tile.py
 src/sigmaepsilon/mesh/topoarray.py
@@ -112,14 +110,24 @@
 src/sigmaepsilon/mesh/cells/q9.py
 src/sigmaepsilon/mesh/cells/t3.py
 src/sigmaepsilon/mesh/cells/t6.py
 src/sigmaepsilon/mesh/cells/tet10.py
 src/sigmaepsilon/mesh/cells/tet4.py
 src/sigmaepsilon/mesh/cells/w18.py
 src/sigmaepsilon/mesh/cells/w6.py
+src/sigmaepsilon/mesh/cells/base/__init__.py
+src/sigmaepsilon/mesh/cells/base/cell.py
+src/sigmaepsilon/mesh/cells/base/cell1d.py
+src/sigmaepsilon/mesh/cells/base/cell2d.py
+src/sigmaepsilon/mesh/cells/base/cell3d.py
+src/sigmaepsilon/mesh/cells/base/interpolator.py
+src/sigmaepsilon/mesh/cells/base/line.py
+src/sigmaepsilon/mesh/cells/base/polygon.py
+src/sigmaepsilon/mesh/cells/base/polyhedron.py
+src/sigmaepsilon/mesh/errors/__init__.py
 src/sigmaepsilon/mesh/io/__init__.py
 src/sigmaepsilon/mesh/io/inp2stl.py
 src/sigmaepsilon/mesh/io/io.py
 src/sigmaepsilon/mesh/space/__init__.py
 src/sigmaepsilon/mesh/space/frame.py
 src/sigmaepsilon/mesh/space/point.py
 src/sigmaepsilon/mesh/space/pointcloud.py
@@ -129,19 +137,20 @@
 src/sigmaepsilon/mesh/utils/locate.py
 src/sigmaepsilon/mesh/utils/space.py
 src/sigmaepsilon/mesh/utils/tet.py
 src/sigmaepsilon/mesh/utils/topodata.py
 src/sigmaepsilon/mesh/utils/tri.py
 src/sigmaepsilon/mesh/utils/utils.py
 src/sigmaepsilon/mesh/utils/cells/__init__.py
-src/sigmaepsilon/mesh/utils/cells/gauss.py
 src/sigmaepsilon/mesh/utils/cells/h27.py
 src/sigmaepsilon/mesh/utils/cells/h8.py
+src/sigmaepsilon/mesh/utils/cells/interpolator.py
 src/sigmaepsilon/mesh/utils/cells/l2.py
 src/sigmaepsilon/mesh/utils/cells/l3.py
+src/sigmaepsilon/mesh/utils/cells/numint.py
 src/sigmaepsilon/mesh/utils/cells/q4.py
 src/sigmaepsilon/mesh/utils/cells/q9.py
 src/sigmaepsilon/mesh/utils/cells/t3.py
 src/sigmaepsilon/mesh/utils/cells/t6.py
 src/sigmaepsilon/mesh/utils/cells/tet10.py
 src/sigmaepsilon/mesh/utils/cells/tet4.py
 src/sigmaepsilon/mesh/utils/cells/utils.py
@@ -162,9 +171,10 @@
 tests/test_recipes.py
 tests/test_topo.py
 tests/test_topo_tr.py
 tests/test_tri.py
 tests/cells/__init__.py
 tests/cells/test_cells.py
 tests/cells/test_hex.py
+tests/cells/test_interpolator.py
 tests/cells/test_lines.py
 tests/cells/test_tet.py
```

### Comparing `sigmaepsilon.mesh-0.0.3/src/sigmaepsilon.mesh.egg-info/requires.txt` & `sigmaepsilon.mesh-1.0.0/src/sigmaepsilon.mesh.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 packaging
 toml
-setuptools>=65.5.1
-wheel>=0.38.0
 linkeddeepdict>=1.1.0
-sigmaepsilon.core>=0.0.1
-sigmaepsilon.math>=0.0.1
+sigmaepsilon.core>=1.0.0
+sigmaepsilon.math>=1.0.0
 fsspec>=2023.1.0
 sectionproperties>=2.1.3
 meshio
 
 [dev]
 networkx>=3.0
 matplotlib
@@ -54,9 +52,7 @@
 pytest
 pytest-cov
 coverage
 pandas
 pyarrow
 networkx>=3.0
 k3d
-setuptools>=65.5.1
-wheel>=0.38.0
```

### Comparing `sigmaepsilon.mesh-0.0.3/tests/cells/test_cells.py` & `sigmaepsilon.mesh-1.0.0/tests/cells/test_cells.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import unittest
 
 from sigmaepsilon.mesh.cells import H8, TET10
 from sigmaepsilon.mesh import grid, PolyData, CartesianFrame
-from sigmaepsilon.mesh.cells import H8
 
 
 class TestGeneratedExpressions(unittest.TestCase):
     def test_generated_H8(self):
         pcoords = H8.lcoords()
         shpf = H8.shape_function_values
         shpmf = H8.shape_function_matrix
```

### Comparing `sigmaepsilon.mesh-0.0.3/tests/cells/test_hex.py` & `sigmaepsilon.mesh-1.0.0/tests/cells/test_hex.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/cells/test_lines.py` & `sigmaepsilon.mesh-1.0.0/tests/cells/test_lines.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/cells/test_tet.py` & `sigmaepsilon.mesh-1.0.0/tests/cells/test_tet.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_compound.py` & `sigmaepsilon.mesh-1.0.0/tests/test_compound.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_geom.py` & `sigmaepsilon.mesh-1.0.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_io.py` & `sigmaepsilon.mesh-1.0.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_linalg.py` & `sigmaepsilon.mesh-1.0.0/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_mesh_anal.py` & `sigmaepsilon.mesh-1.0.0/tests/test_mesh_anal.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_meshing.py` & `sigmaepsilon.mesh-1.0.0/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_pointcloud.py` & `sigmaepsilon.mesh-1.0.0/tests/test_pointcloud.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_recipes.py` & `sigmaepsilon.mesh-1.0.0/tests/test_recipes.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_topo_tr.py` & `sigmaepsilon.mesh-1.0.0/tests/test_topo_tr.py`

 * *Files identical despite different names*

### Comparing `sigmaepsilon.mesh-0.0.3/tests/test_tri.py` & `sigmaepsilon.mesh-1.0.0/tests/test_tri.py`

 * *Files identical despite different names*

