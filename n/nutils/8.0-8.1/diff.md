# Comparing `tmp/nutils-8.0.tar.gz` & `tmp/nutils-8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutils-8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "nutils-8.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nutils-8.0.tar` & `nutils-8.1.tar`

### file list

```diff
@@ -1,132 +1,132 @@
--rw-r--r--   0        0        0       13 2023-07-28 10:56:30.854624 nutils-8.0/.codecov.yml
--rw-r--r--   0        0        0       58 2023-07-28 10:56:30.854624 nutils-8.0/.coveragerc
--rw-r--r--   0        0        0      539 2023-07-28 10:56:30.854624 nutils-8.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     9543 2023-07-28 10:56:30.854624 nutils-8.0/.github/workflows/test.yaml
--rw-r--r--   0        0        0       65 2023-07-28 10:56:30.854624 nutils-8.0/.gitignore
--rw-r--r--   0        0        0     8296 2023-07-28 10:56:30.854624 nutils-8.0/CHANGELOG
--rw-r--r--   0        0        0     1062 2023-07-28 10:56:30.854624 nutils-8.0/LICENSE
--rw-r--r--   0        0        0     6035 2023-07-28 10:56:30.854624 nutils-8.0/README.md
--rw-r--r--   0        0        0     1437 2023-07-28 10:56:30.854624 nutils-8.0/devtools/__init__.py
--rw-r--r--   0        0        0     1303 2023-07-28 10:56:30.854624 nutils-8.0/devtools/_git.py
--rw-r--r--   0        0        0      732 2023-07-28 10:56:30.854624 nutils-8.0/devtools/_log_default.py
--rw-r--r--   0        0        0      701 2023-07-28 10:56:30.854624 nutils-8.0/devtools/_log_gha.py
--rw-r--r--   0        0        0     3985 2023-07-28 10:56:30.854624 nutils-8.0/devtools/container/__init__.py
--rw-r--r--   0        0        0     5961 2023-07-28 10:56:30.854624 nutils-8.0/devtools/container/build.py
--rw-r--r--   0        0        0     1698 2023-07-28 10:56:30.854624 nutils-8.0/devtools/container/build_base.py
--rw-r--r--   0        0        0        0 2023-07-28 10:56:30.854624 nutils-8.0/devtools/gha/__init__.py
--rw-r--r--   0        0        0     1242 2023-07-28 10:56:30.854624 nutils-8.0/devtools/gha/configure_mkl.py
--rw-r--r--   0        0        0     1697 2023-07-28 10:56:30.854624 nutils-8.0/devtools/gha/coverage_report_xml.py
--rw-r--r--   0        0        0      776 2023-07-28 10:56:30.854624 nutils-8.0/devtools/gha/get_base_and_image_tags.py
--rw-r--r--   0        0        0      105 2023-07-28 10:56:30.854624 nutils-8.0/docs/_static/mods.css
--rw-r--r--   0        0        0      585 2023-07-28 10:56:30.854624 nutils-8.0/docs/_templates/breadcrumbs.html
--rw-r--r--   0        0        0    11343 2023-07-28 10:56:30.854624 nutils-8.0/docs/conf.py
--rw-r--r--   0        0        0   360414 2023-07-28 10:56:30.854624 nutils-8.0/docs/favicon.ico
--rw-r--r--   0        0        0      510 2023-07-28 10:56:30.854624 nutils-8.0/docs/index.rst
--rw-r--r--   0        0        0     5591 2023-07-28 10:56:30.854624 nutils-8.0/docs/sphinx_mods.py
--rw-r--r--   0        0        0      456 2023-07-28 10:56:30.854624 nutils-8.0/examples/__init__.py
--rw-r--r--   0        0        0     7534 2023-07-28 10:56:30.854624 nutils-8.0/examples/adaptivity.py
--rw-r--r--   0        0        0     3561 2023-07-28 10:56:30.854624 nutils-8.0/examples/burgers.py
--rw-r--r--   0        0        0    12672 2023-07-28 10:56:30.854624 nutils-8.0/examples/cahnhilliard.py
--rw-r--r--   0        0        0    11156 2023-07-28 10:56:30.854624 nutils-8.0/examples/coil.py
--rw-r--r--   0        0        0    12287 2023-07-28 10:56:30.854624 nutils-8.0/examples/cylinderflow.py
--rw-r--r--   0        0        0    14036 2023-07-28 10:56:30.854624 nutils-8.0/examples/drivencavity.py
--rw-r--r--   0        0        0     6133 2023-07-28 10:56:30.854624 nutils-8.0/examples/elasticity.py
--rw-r--r--   0        0        0     4916 2023-07-28 10:56:30.854624 nutils-8.0/examples/finitestrain.py
--rw-r--r--   0        0        0     6972 2023-07-28 10:56:30.854624 nutils-8.0/examples/laplace.py
--rw-r--r--   0        0        0     9749 2023-07-28 10:56:30.858625 nutils-8.0/examples/platewithhole.py
--rw-r--r--   0        0        0     1564 2023-07-28 10:56:30.858625 nutils-8.0/examples/poisson.py
--rw-r--r--   0        0        0     5665 2023-07-28 10:56:30.858625 nutils-8.0/examples/torsion.py
--rw-r--r--   0        0        0    20989 2023-07-28 10:56:30.858625 nutils-8.0/nutils/SI.py
--rw-r--r--   0        0        0      860 2023-07-28 10:56:30.858625 nutils-8.0/nutils/__init__.py
--rw-r--r--   0        0        0     1537 2023-07-28 10:56:30.858625 nutils-8.0/nutils/_backports.py
--rw-r--r--   0        0        0    11089 2023-07-28 10:56:30.858625 nutils-8.0/nutils/_graph.py
--rw-r--r--   0        0        0    26523 2023-07-28 10:56:30.858625 nutils-8.0/nutils/_util.py
--rw-r--r--   0        0        0    15246 2023-07-28 10:56:30.858625 nutils-8.0/nutils/cache.py
--rw-r--r--   0        0        0     1539 2023-07-28 10:56:30.858625 nutils-8.0/nutils/cli.py
--rw-r--r--   0        0        0      468 2023-07-28 10:56:30.858625 nutils-8.0/nutils/debug_flags.py
--rw-r--r--   0        0        0    48181 2023-07-28 10:56:30.858625 nutils-8.0/nutils/element.py
--rw-r--r--   0        0        0    20568 2023-07-28 10:56:30.858625 nutils-8.0/nutils/elementseq.py
--rw-r--r--   0        0        0   200146 2023-07-28 10:56:30.858625 nutils-8.0/nutils/evaluable.py
--rw-r--r--   0        0        0    11441 2023-07-28 10:56:30.858625 nutils-8.0/nutils/export.py
--rw-r--r--   0        0        0    84259 2023-07-28 10:56:30.858625 nutils-8.0/nutils/expression_v1.py
--rw-r--r--   0        0        0    41347 2023-07-28 10:56:30.858625 nutils-8.0/nutils/expression_v2.py
--rw-r--r--   0        0        0   168665 2023-07-28 10:56:30.862625 nutils-8.0/nutils/function.py
--rw-r--r--   0        0        0     2233 2023-07-28 10:56:30.862625 nutils-8.0/nutils/matrix/__init__.py
--rw-r--r--   0        0        0      219 2023-07-28 10:56:30.862625 nutils-8.0/nutils/matrix/_auto.py
--rw-r--r--   0        0        0    13463 2023-07-28 10:56:30.862625 nutils-8.0/nutils/matrix/_base.py
--rw-r--r--   0        0        0    14350 2023-07-28 10:56:30.862625 nutils-8.0/nutils/matrix/_mkl.py
--rw-r--r--   0        0        0     2292 2023-07-28 10:56:30.862625 nutils-8.0/nutils/matrix/_numpy.py
--rw-r--r--   0        0        0     4267 2023-07-28 10:56:30.862625 nutils-8.0/nutils/matrix/_scipy.py
--rw-r--r--   0        0        0    35487 2023-07-28 10:56:30.862625 nutils-8.0/nutils/mesh.py
--rw-r--r--   0        0        0    23614 2023-07-28 10:56:30.862625 nutils-8.0/nutils/numeric.py
--rw-r--r--   0        0        0     5682 2023-07-28 10:56:30.862625 nutils-8.0/nutils/parallel.py
--rw-r--r--   0        0        0    19627 2023-07-28 10:56:30.862625 nutils-8.0/nutils/points.py
--rw-r--r--   0        0        0    22300 2023-07-28 10:56:30.862625 nutils-8.0/nutils/pointsseq.py
--rw-r--r--   0        0        0    45140 2023-07-28 10:56:30.862625 nutils-8.0/nutils/sample.py
--rw-r--r--   0        0        0    48637 2023-07-28 10:56:30.862625 nutils-8.0/nutils/solver.py
--rw-r--r--   0        0        0    13225 2023-07-28 10:56:30.862625 nutils-8.0/nutils/sparse.py
--rw-r--r--   0        0        0    11497 2023-07-28 10:56:30.862625 nutils-8.0/nutils/testing.py
--rw-r--r--   0        0        0   155030 2023-07-28 10:56:30.862625 nutils-8.0/nutils/topology.py
--rw-r--r--   0        0        0    16670 2023-07-28 10:56:30.862625 nutils-8.0/nutils/transform.py
--rw-r--r--   0        0        0    34922 2023-07-28 10:56:30.862625 nutils-8.0/nutils/transformseq.py
--rw-r--r--   0        0        0    23704 2023-07-28 10:56:30.862625 nutils-8.0/nutils/types.py
--rw-r--r--   0        0        0     6934 2023-07-28 10:56:30.862625 nutils-8.0/nutils/unit.py
--rw-r--r--   0        0        0      872 2023-07-28 10:56:30.862625 nutils-8.0/nutils/warnings.py
--rw-r--r--   0        0        0      772 2023-07-28 10:56:30.862625 nutils-8.0/pyproject.toml
--rw-r--r--   0        0        0      118 2023-07-28 10:56:30.862625 nutils-8.0/readthedocs.yml
--rw-r--r--   0        0        0        0 2023-07-28 10:56:30.862625 nutils-8.0/tests/__init__.py
--rw-r--r--   0        0        0     9897 2023-07-28 10:56:30.862625 nutils-8.0/tests/test_SI.py
--rw-r--r--   0        0        0      793 2023-07-28 10:56:30.862625 nutils-8.0/tests/test_backports.py
--rw-r--r--   0        0        0    16428 2023-07-28 10:56:30.862625 nutils-8.0/tests/test_basis.py
--rw-r--r--   0        0        0    14044 2023-07-28 10:56:30.862625 nutils-8.0/tests/test_cache.py
--rw-r--r--   0        0        0     2116 2023-07-28 10:56:30.862625 nutils-8.0/tests/test_cli.py
--rw-r--r--   0        0        0     2977 2023-07-28 10:56:30.862625 nutils-8.0/tests/test_docs.py
--rw-r--r--   0        0        0     6271 2023-07-28 10:56:30.862625 nutils-8.0/tests/test_element.py
--rw-r--r--   0        0        0     9541 2023-07-28 10:56:30.862625 nutils-8.0/tests/test_elementseq.py
--rw-r--r--   0        0        0    78239 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_evaluable.py
--rw-r--r--   0        0        0    10908 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_export.py
--rw-r--r--   0        0        0    52161 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_expression_v1.py
--rw-r--r--   0        0        0    24679 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_expression_v2.py
--rw-r--r--   0        0        0    18942 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_finitecell.py
--rw-r--r--   0        0        0    74822 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_function.py
--rw-r--r--   0        0        0    13788 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_graph.py
--rw-r--r--   0        0        0     3253 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_ischeme.py
--rw-r--r--   0        0        0    11189 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_matrix.py
--rw-r--r--   0        0        0     9685 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh.py
--rw-r--r--   0        0        0     1388 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d.geo
--rw-r--r--   0        0        0     6702 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d_p1_v2.msh
--rw-r--r--   0        0        0     5618 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d_p1_v4.msh
--rw-r--r--   0        0        0    17648 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d_p2_v2.msh
--rw-r--r--   0        0        0    16228 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d_p2_v4.msh
--rw-r--r--   0        0        0    35340 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d_p3_v2.msh
--rw-r--r--   0        0        0    33181 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d_p3_v4.msh
--rw-r--r--   0        0        0    59708 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d_p4_v2.msh
--rw-r--r--   0        0        0    56807 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh2d_p4_v4.msh
--rw-r--r--   0        0        0     3221 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh3d.geo
--rw-r--r--   0        0        0    78920 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh3d_p1_v2.msh
--rw-r--r--   0        0        0    59146 2023-07-28 10:56:30.866624 nutils-8.0/tests/test_mesh/mesh3d_p1_v4.msh
--rw-r--r--   0        0        0   254705 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_mesh/mesh3d_p2_v2.msh
--rw-r--r--   0        0        0   225898 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_mesh/mesh3d_p2_v4.msh
--rw-r--r--   0        0        0      742 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_mesh/mesh3dmani.geo
--rw-r--r--   0        0        0     5893 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_mesh/mesh3dmani_p1_v2.msh
--rw-r--r--   0        0        0     5587 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_mesh/mesh3dmani_p1_v4.msh
--rw-r--r--   0        0        0    17016 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_mesh/mesh3dmani_p2_v2.msh
--rw-r--r--   0        0        0    16281 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_mesh/mesh3dmani_p2_v4.msh
--rw-r--r--   0        0        0     2708 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_normals.py
--rw-r--r--   0        0        0    16473 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_numeric.py
--rw-r--r--   0        0        0     2206 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_parallel.py
--rw-r--r--   0        0        0     5654 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_points.py
--rw-r--r--   0        0        0    11346 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_pointsseq.py
--rw-r--r--   0        0        0     2297 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_quadrature.py
--rw-r--r--   0        0        0    27471 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_sample.py
--rw-r--r--   0        0        0    15933 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_solver.py
--rw-r--r--   0        0        0    13697 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_sparse.py
--rw-r--r--   0        0        0     1712 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_testing.py
--rw-r--r--   0        0        0    64170 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_topology.py
--rw-r--r--   0        0        0     4607 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_transform.py
--rw-r--r--   0        0        0    20363 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_transformseq.py
--rw-r--r--   0        0        0    23999 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_types.py
--rw-r--r--   0        0        0     2317 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_unit.py
--rw-r--r--   0        0        0    12562 2023-07-28 10:56:30.870624 nutils-8.0/tests/test_util.py
--rw-r--r--   0        0        0      379 2023-07-28 10:56:30.874624 nutils-8.0/tests/test_warnings.py
--rw-r--r--   0        0        0     7032 1970-01-01 00:00:00.000000 nutils-8.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-08-08 14:13:39.688683 nutils-8.1/.codecov.yml
+-rw-r--r--   0        0        0       58 2023-08-08 14:13:39.688683 nutils-8.1/.coveragerc
+-rw-r--r--   0        0        0      539 2023-08-08 14:13:39.688683 nutils-8.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     9543 2023-08-08 14:13:39.688683 nutils-8.1/.github/workflows/test.yaml
+-rw-r--r--   0        0        0       65 2023-08-08 14:13:39.688683 nutils-8.1/.gitignore
+-rw-r--r--   0        0        0     8296 2023-08-08 14:13:39.688683 nutils-8.1/CHANGELOG
+-rw-r--r--   0        0        0     1062 2023-08-08 14:13:39.688683 nutils-8.1/LICENSE
+-rw-r--r--   0        0        0     6035 2023-08-08 14:13:39.688683 nutils-8.1/README.md
+-rw-r--r--   0        0        0     1437 2023-08-08 14:13:39.688683 nutils-8.1/devtools/__init__.py
+-rw-r--r--   0        0        0     1303 2023-08-08 14:13:39.688683 nutils-8.1/devtools/_git.py
+-rw-r--r--   0        0        0      732 2023-08-08 14:13:39.688683 nutils-8.1/devtools/_log_default.py
+-rw-r--r--   0        0        0      701 2023-08-08 14:13:39.688683 nutils-8.1/devtools/_log_gha.py
+-rw-r--r--   0        0        0     3985 2023-08-08 14:13:39.688683 nutils-8.1/devtools/container/__init__.py
+-rw-r--r--   0        0        0     5961 2023-08-08 14:13:39.688683 nutils-8.1/devtools/container/build.py
+-rw-r--r--   0        0        0     1698 2023-08-08 14:13:39.688683 nutils-8.1/devtools/container/build_base.py
+-rw-r--r--   0        0        0        0 2023-08-08 14:13:39.688683 nutils-8.1/devtools/gha/__init__.py
+-rw-r--r--   0        0        0     1242 2023-08-08 14:13:39.688683 nutils-8.1/devtools/gha/configure_mkl.py
+-rw-r--r--   0        0        0     1697 2023-08-08 14:13:39.688683 nutils-8.1/devtools/gha/coverage_report_xml.py
+-rw-r--r--   0        0        0      776 2023-08-08 14:13:39.688683 nutils-8.1/devtools/gha/get_base_and_image_tags.py
+-rw-r--r--   0        0        0      105 2023-08-08 14:13:39.688683 nutils-8.1/docs/_static/mods.css
+-rw-r--r--   0        0        0      585 2023-08-08 14:13:39.688683 nutils-8.1/docs/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0    11343 2023-08-08 14:13:39.688683 nutils-8.1/docs/conf.py
+-rw-r--r--   0        0        0   360414 2023-08-08 14:13:39.692683 nutils-8.1/docs/favicon.ico
+-rw-r--r--   0        0        0      510 2023-08-08 14:13:39.692683 nutils-8.1/docs/index.rst
+-rw-r--r--   0        0        0     5591 2023-08-08 14:13:39.692683 nutils-8.1/docs/sphinx_mods.py
+-rw-r--r--   0        0        0      456 2023-08-08 14:13:39.692683 nutils-8.1/examples/__init__.py
+-rw-r--r--   0        0        0     7534 2023-08-08 14:13:39.692683 nutils-8.1/examples/adaptivity.py
+-rw-r--r--   0        0        0     3561 2023-08-08 14:13:39.692683 nutils-8.1/examples/burgers.py
+-rw-r--r--   0        0        0    12672 2023-08-08 14:13:39.692683 nutils-8.1/examples/cahnhilliard.py
+-rw-r--r--   0        0        0    11156 2023-08-08 14:13:39.692683 nutils-8.1/examples/coil.py
+-rw-r--r--   0        0        0    12287 2023-08-08 14:13:39.692683 nutils-8.1/examples/cylinderflow.py
+-rw-r--r--   0        0        0    14036 2023-08-08 14:13:39.692683 nutils-8.1/examples/drivencavity.py
+-rw-r--r--   0        0        0     6133 2023-08-08 14:13:39.692683 nutils-8.1/examples/elasticity.py
+-rw-r--r--   0        0        0     4916 2023-08-08 14:13:39.692683 nutils-8.1/examples/finitestrain.py
+-rw-r--r--   0        0        0     6972 2023-08-08 14:13:39.692683 nutils-8.1/examples/laplace.py
+-rw-r--r--   0        0        0     9749 2023-08-08 14:13:39.692683 nutils-8.1/examples/platewithhole.py
+-rw-r--r--   0        0        0     1564 2023-08-08 14:13:39.692683 nutils-8.1/examples/poisson.py
+-rw-r--r--   0        0        0     5665 2023-08-08 14:13:39.692683 nutils-8.1/examples/torsion.py
+-rw-r--r--   0        0        0    20989 2023-08-08 14:13:39.692683 nutils-8.1/nutils/SI.py
+-rw-r--r--   0        0        0      860 2023-08-08 14:13:39.692683 nutils-8.1/nutils/__init__.py
+-rw-r--r--   0        0        0     1537 2023-08-08 14:13:39.692683 nutils-8.1/nutils/_backports.py
+-rw-r--r--   0        0        0    11089 2023-08-08 14:13:39.692683 nutils-8.1/nutils/_graph.py
+-rw-r--r--   0        0        0    26774 2023-08-08 14:13:39.692683 nutils-8.1/nutils/_util.py
+-rw-r--r--   0        0        0    15246 2023-08-08 14:13:39.692683 nutils-8.1/nutils/cache.py
+-rw-r--r--   0        0        0     1565 2023-08-08 14:13:39.692683 nutils-8.1/nutils/cli.py
+-rw-r--r--   0        0        0      468 2023-08-08 14:13:39.692683 nutils-8.1/nutils/debug_flags.py
+-rw-r--r--   0        0        0    48181 2023-08-08 14:13:39.692683 nutils-8.1/nutils/element.py
+-rw-r--r--   0        0        0    20568 2023-08-08 14:13:39.692683 nutils-8.1/nutils/elementseq.py
+-rw-r--r--   0        0        0   200146 2023-08-08 14:13:39.696683 nutils-8.1/nutils/evaluable.py
+-rw-r--r--   0        0        0    11441 2023-08-08 14:13:39.696683 nutils-8.1/nutils/export.py
+-rw-r--r--   0        0        0    84259 2023-08-08 14:13:39.696683 nutils-8.1/nutils/expression_v1.py
+-rw-r--r--   0        0        0    41347 2023-08-08 14:13:39.696683 nutils-8.1/nutils/expression_v2.py
+-rw-r--r--   0        0        0   168665 2023-08-08 14:13:39.696683 nutils-8.1/nutils/function.py
+-rw-r--r--   0        0        0     2233 2023-08-08 14:13:39.696683 nutils-8.1/nutils/matrix/__init__.py
+-rw-r--r--   0        0        0      219 2023-08-08 14:13:39.696683 nutils-8.1/nutils/matrix/_auto.py
+-rw-r--r--   0        0        0    13463 2023-08-08 14:13:39.696683 nutils-8.1/nutils/matrix/_base.py
+-rw-r--r--   0        0        0    14350 2023-08-08 14:13:39.696683 nutils-8.1/nutils/matrix/_mkl.py
+-rw-r--r--   0        0        0     2292 2023-08-08 14:13:39.696683 nutils-8.1/nutils/matrix/_numpy.py
+-rw-r--r--   0        0        0     4267 2023-08-08 14:13:39.696683 nutils-8.1/nutils/matrix/_scipy.py
+-rw-r--r--   0        0        0    35487 2023-08-08 14:13:39.696683 nutils-8.1/nutils/mesh.py
+-rw-r--r--   0        0        0    23614 2023-08-08 14:13:39.696683 nutils-8.1/nutils/numeric.py
+-rw-r--r--   0        0        0     5682 2023-08-08 14:13:39.696683 nutils-8.1/nutils/parallel.py
+-rw-r--r--   0        0        0    19627 2023-08-08 14:13:39.696683 nutils-8.1/nutils/points.py
+-rw-r--r--   0        0        0    22300 2023-08-08 14:13:39.696683 nutils-8.1/nutils/pointsseq.py
+-rw-r--r--   0        0        0    45140 2023-08-08 14:13:39.696683 nutils-8.1/nutils/sample.py
+-rw-r--r--   0        0        0    48637 2023-08-08 14:13:39.700683 nutils-8.1/nutils/solver.py
+-rw-r--r--   0        0        0    13225 2023-08-08 14:13:39.700683 nutils-8.1/nutils/sparse.py
+-rw-r--r--   0        0        0    11497 2023-08-08 14:13:39.700683 nutils-8.1/nutils/testing.py
+-rw-r--r--   0        0        0   155030 2023-08-08 14:13:39.700683 nutils-8.1/nutils/topology.py
+-rw-r--r--   0        0        0    16670 2023-08-08 14:13:39.700683 nutils-8.1/nutils/transform.py
+-rw-r--r--   0        0        0    34922 2023-08-08 14:13:39.700683 nutils-8.1/nutils/transformseq.py
+-rw-r--r--   0        0        0    23704 2023-08-08 14:13:39.700683 nutils-8.1/nutils/types.py
+-rw-r--r--   0        0        0     6934 2023-08-08 14:13:39.700683 nutils-8.1/nutils/unit.py
+-rw-r--r--   0        0        0      872 2023-08-08 14:13:39.700683 nutils-8.1/nutils/warnings.py
+-rw-r--r--   0        0        0      772 2023-08-08 14:13:39.700683 nutils-8.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-08-08 14:13:39.700683 nutils-8.1/readthedocs.yml
+-rw-r--r--   0        0        0        0 2023-08-08 14:13:39.700683 nutils-8.1/tests/__init__.py
+-rw-r--r--   0        0        0     9897 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_SI.py
+-rw-r--r--   0        0        0      793 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_backports.py
+-rw-r--r--   0        0        0    16428 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_basis.py
+-rw-r--r--   0        0        0    14044 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_cache.py
+-rw-r--r--   0        0        0     2116 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_cli.py
+-rw-r--r--   0        0        0     2977 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_docs.py
+-rw-r--r--   0        0        0     6271 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_element.py
+-rw-r--r--   0        0        0     9541 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_elementseq.py
+-rw-r--r--   0        0        0    78239 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_evaluable.py
+-rw-r--r--   0        0        0    10908 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_export.py
+-rw-r--r--   0        0        0    52161 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_expression_v1.py
+-rw-r--r--   0        0        0    24679 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_expression_v2.py
+-rw-r--r--   0        0        0    18942 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_finitecell.py
+-rw-r--r--   0        0        0    74822 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_function.py
+-rw-r--r--   0        0        0    13788 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_graph.py
+-rw-r--r--   0        0        0     3253 2023-08-08 14:13:39.700683 nutils-8.1/tests/test_ischeme.py
+-rw-r--r--   0        0        0    11189 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_matrix.py
+-rw-r--r--   0        0        0     9685 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh.py
+-rw-r--r--   0        0        0     1388 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d.geo
+-rw-r--r--   0        0        0     6702 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d_p1_v2.msh
+-rw-r--r--   0        0        0     5618 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d_p1_v4.msh
+-rw-r--r--   0        0        0    17648 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d_p2_v2.msh
+-rw-r--r--   0        0        0    16228 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d_p2_v4.msh
+-rw-r--r--   0        0        0    35340 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d_p3_v2.msh
+-rw-r--r--   0        0        0    33181 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d_p3_v4.msh
+-rw-r--r--   0        0        0    59708 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d_p4_v2.msh
+-rw-r--r--   0        0        0    56807 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh2d_p4_v4.msh
+-rw-r--r--   0        0        0     3221 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh3d.geo
+-rw-r--r--   0        0        0    78920 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh3d_p1_v2.msh
+-rw-r--r--   0        0        0    59146 2023-08-08 14:13:39.704684 nutils-8.1/tests/test_mesh/mesh3d_p1_v4.msh
+-rw-r--r--   0        0        0   254705 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_mesh/mesh3d_p2_v2.msh
+-rw-r--r--   0        0        0   225898 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_mesh/mesh3d_p2_v4.msh
+-rw-r--r--   0        0        0      742 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_mesh/mesh3dmani.geo
+-rw-r--r--   0        0        0     5893 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_mesh/mesh3dmani_p1_v2.msh
+-rw-r--r--   0        0        0     5587 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_mesh/mesh3dmani_p1_v4.msh
+-rw-r--r--   0        0        0    17016 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_mesh/mesh3dmani_p2_v2.msh
+-rw-r--r--   0        0        0    16281 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_mesh/mesh3dmani_p2_v4.msh
+-rw-r--r--   0        0        0     2708 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_normals.py
+-rw-r--r--   0        0        0    16473 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_numeric.py
+-rw-r--r--   0        0        0     2206 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_parallel.py
+-rw-r--r--   0        0        0     5654 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_points.py
+-rw-r--r--   0        0        0    11346 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_pointsseq.py
+-rw-r--r--   0        0        0     2297 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_quadrature.py
+-rw-r--r--   0        0        0    27471 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_sample.py
+-rw-r--r--   0        0        0    15933 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_solver.py
+-rw-r--r--   0        0        0    13697 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_sparse.py
+-rw-r--r--   0        0        0     1712 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_testing.py
+-rw-r--r--   0        0        0    64170 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_topology.py
+-rw-r--r--   0        0        0     4607 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_transform.py
+-rw-r--r--   0        0        0    20363 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_transformseq.py
+-rw-r--r--   0        0        0    23999 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_types.py
+-rw-r--r--   0        0        0     2317 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_unit.py
+-rw-r--r--   0        0        0    12562 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_util.py
+-rw-r--r--   0        0        0      379 2023-08-08 14:13:39.708684 nutils-8.1/tests/test_warnings.py
+-rw-r--r--   0        0        0     7032 1970-01-01 00:00:00.000000 nutils-8.1/PKG-INFO
```

### Comparing `nutils-8.0/.github/workflows/release.yml` & `nutils-8.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `nutils-8.0/.github/workflows/test.yaml` & `nutils-8.1/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `nutils-8.0/CHANGELOG` & `nutils-8.1/CHANGELOG`

 * *Files identical despite different names*

### Comparing `nutils-8.0/LICENSE` & `nutils-8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nutils-8.0/README.md` & `nutils-8.1/README.md`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/__init__.py` & `nutils-8.1/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/_git.py` & `nutils-8.1/devtools/_git.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/_log_default.py` & `nutils-8.1/devtools/_log_default.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/_log_gha.py` & `nutils-8.1/devtools/_log_gha.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/container/__init__.py` & `nutils-8.1/devtools/container/__init__.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/container/build.py` & `nutils-8.1/devtools/container/build.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/container/build_base.py` & `nutils-8.1/devtools/container/build_base.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/gha/configure_mkl.py` & `nutils-8.1/devtools/gha/configure_mkl.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/gha/coverage_report_xml.py` & `nutils-8.1/devtools/gha/coverage_report_xml.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/devtools/gha/get_base_and_image_tags.py` & `nutils-8.1/devtools/gha/get_base_and_image_tags.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/docs/_templates/breadcrumbs.html` & `nutils-8.1/docs/_templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `nutils-8.0/docs/conf.py` & `nutils-8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/docs/favicon.ico` & `nutils-8.1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `nutils-8.0/docs/sphinx_mods.py` & `nutils-8.1/docs/sphinx_mods.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/adaptivity.py` & `nutils-8.1/examples/adaptivity.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/burgers.py` & `nutils-8.1/examples/burgers.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/cahnhilliard.py` & `nutils-8.1/examples/cahnhilliard.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/coil.py` & `nutils-8.1/examples/coil.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/cylinderflow.py` & `nutils-8.1/examples/cylinderflow.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/drivencavity.py` & `nutils-8.1/examples/drivencavity.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/elasticity.py` & `nutils-8.1/examples/elasticity.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/finitestrain.py` & `nutils-8.1/examples/finitestrain.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/laplace.py` & `nutils-8.1/examples/laplace.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/platewithhole.py` & `nutils-8.1/examples/platewithhole.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/poisson.py` & `nutils-8.1/examples/poisson.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/examples/torsion.py` & `nutils-8.1/examples/torsion.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/SI.py` & `nutils-8.1/nutils/SI.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/__init__.py` & `nutils-8.1/nutils/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import sys
 import numpy
 from distutils.version import LooseVersion
 
 assert sys.version_info >= (3, 5)
 assert LooseVersion(numpy.version.version) >= LooseVersion('1.16'), 'nutils requires numpy 1.16 or higher, got {}'.format(numpy.version.version)
 
-__version__ = version = '8.0'
+__version__ = version = '8.1'
 version_name = 'idiyappam'
 long_version = ('{} "{}"' if version_name else '{}').format(version, version_name)
 
 __all__ = [
     'cache',
     'cli',
     'element',
```

### Comparing `nutils-8.0/nutils/_backports.py` & `nutils-8.1/nutils/_backports.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/_graph.py` & `nutils-8.1/nutils/_graph.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/_util.py` & `nutils-8.1/nutils/_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -487,14 +487,26 @@
         sig = inspect.signature(f)
         in_context.__signature__ = sig.replace(parameters=(*sig.parameters.values(), *params))
         return in_context
 
     return in_context_wrapper
 
 
+def log_version(f):
+
+    from . import version, version_name
+
+    @functools.wraps(f)
+    def log_version(*args, **kwargs):
+        treelog.info(f'NUTILS {version} "{version_name.title()}"')
+        return f(*args, **kwargs)
+
+    return log_version
+
+
 def log_arguments(f):
     '''Decorator to log a function's arguments.
 
     The arguments are logged in the 'arguments' context. ``Stringly.loads``
     will be used whenever an argument supports it, transparently falling back
     on ``str`` otherwise.'''
```

### Comparing `nutils-8.0/nutils/cache.py` & `nutils-8.1/nutils/cache.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/cli.py` & `nutils-8.1/nutils/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,14 +19,15 @@
         util.in_context(parallel.maxprocs),
         util.in_context(matrix.backend),
         util.in_context(util.set_stdoutlog),
         util.in_context(util.add_htmllog),
         util.in_context(util.log_traceback),
         util.in_context(util.post_mortem),
         warnings.via(treelog.warning),
+        util.log_version,
         util.log_arguments,
         util.timeit(),
     )
 
     for decorator in reversed(decorators):
         f = decorator(f)
```

### Comparing `nutils-8.0/nutils/element.py` & `nutils-8.1/nutils/element.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/elementseq.py` & `nutils-8.1/nutils/elementseq.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/evaluable.py` & `nutils-8.1/nutils/evaluable.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/export.py` & `nutils-8.1/nutils/export.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/expression_v1.py` & `nutils-8.1/nutils/expression_v1.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/expression_v2.py` & `nutils-8.1/nutils/expression_v2.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/function.py` & `nutils-8.1/nutils/function.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/matrix/__init__.py` & `nutils-8.1/nutils/matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/matrix/_base.py` & `nutils-8.1/nutils/matrix/_base.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/matrix/_mkl.py` & `nutils-8.1/nutils/matrix/_mkl.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/matrix/_numpy.py` & `nutils-8.1/nutils/matrix/_numpy.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/matrix/_scipy.py` & `nutils-8.1/nutils/matrix/_scipy.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/mesh.py` & `nutils-8.1/nutils/mesh.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/numeric.py` & `nutils-8.1/nutils/numeric.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/parallel.py` & `nutils-8.1/nutils/parallel.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/points.py` & `nutils-8.1/nutils/points.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/pointsseq.py` & `nutils-8.1/nutils/pointsseq.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/sample.py` & `nutils-8.1/nutils/sample.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/solver.py` & `nutils-8.1/nutils/solver.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/sparse.py` & `nutils-8.1/nutils/sparse.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/testing.py` & `nutils-8.1/nutils/testing.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/topology.py` & `nutils-8.1/nutils/topology.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/transform.py` & `nutils-8.1/nutils/transform.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/transformseq.py` & `nutils-8.1/nutils/transformseq.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/types.py` & `nutils-8.1/nutils/types.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/unit.py` & `nutils-8.1/nutils/unit.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/nutils/warnings.py` & `nutils-8.1/nutils/warnings.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/pyproject.toml` & `nutils-8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_SI.py` & `nutils-8.1/tests/test_SI.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_backports.py` & `nutils-8.1/tests/test_backports.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_basis.py` & `nutils-8.1/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_cache.py` & `nutils-8.1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_cli.py` & `nutils-8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_docs.py` & `nutils-8.1/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_element.py` & `nutils-8.1/tests/test_element.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_elementseq.py` & `nutils-8.1/tests/test_elementseq.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_evaluable.py` & `nutils-8.1/tests/test_evaluable.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_export.py` & `nutils-8.1/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_expression_v1.py` & `nutils-8.1/tests/test_expression_v1.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_expression_v2.py` & `nutils-8.1/tests/test_expression_v2.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_finitecell.py` & `nutils-8.1/tests/test_finitecell.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_function.py` & `nutils-8.1/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_graph.py` & `nutils-8.1/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_ischeme.py` & `nutils-8.1/tests/test_ischeme.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_matrix.py` & `nutils-8.1/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh.py` & `nutils-8.1/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d.geo` & `nutils-8.1/tests/test_mesh/mesh2d.geo`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d_p1_v2.msh` & `nutils-8.1/tests/test_mesh/mesh2d_p1_v2.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d_p1_v4.msh` & `nutils-8.1/tests/test_mesh/mesh2d_p1_v4.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d_p2_v2.msh` & `nutils-8.1/tests/test_mesh/mesh2d_p2_v2.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d_p2_v4.msh` & `nutils-8.1/tests/test_mesh/mesh2d_p2_v4.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d_p3_v2.msh` & `nutils-8.1/tests/test_mesh/mesh2d_p3_v2.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d_p3_v4.msh` & `nutils-8.1/tests/test_mesh/mesh2d_p3_v4.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d_p4_v2.msh` & `nutils-8.1/tests/test_mesh/mesh2d_p4_v2.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh2d_p4_v4.msh` & `nutils-8.1/tests/test_mesh/mesh2d_p4_v4.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3d.geo` & `nutils-8.1/tests/test_mesh/mesh3d.geo`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3d_p1_v2.msh` & `nutils-8.1/tests/test_mesh/mesh3d_p1_v2.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3d_p1_v4.msh` & `nutils-8.1/tests/test_mesh/mesh3d_p1_v4.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3d_p2_v2.msh` & `nutils-8.1/tests/test_mesh/mesh3d_p2_v2.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3d_p2_v4.msh` & `nutils-8.1/tests/test_mesh/mesh3d_p2_v4.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3dmani.geo` & `nutils-8.1/tests/test_mesh/mesh3dmani.geo`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3dmani_p1_v2.msh` & `nutils-8.1/tests/test_mesh/mesh3dmani_p1_v2.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3dmani_p1_v4.msh` & `nutils-8.1/tests/test_mesh/mesh3dmani_p1_v4.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3dmani_p2_v2.msh` & `nutils-8.1/tests/test_mesh/mesh3dmani_p2_v2.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_mesh/mesh3dmani_p2_v4.msh` & `nutils-8.1/tests/test_mesh/mesh3dmani_p2_v4.msh`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_normals.py` & `nutils-8.1/tests/test_normals.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_numeric.py` & `nutils-8.1/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_parallel.py` & `nutils-8.1/tests/test_parallel.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_points.py` & `nutils-8.1/tests/test_points.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_pointsseq.py` & `nutils-8.1/tests/test_pointsseq.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_quadrature.py` & `nutils-8.1/tests/test_quadrature.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_sample.py` & `nutils-8.1/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_solver.py` & `nutils-8.1/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_sparse.py` & `nutils-8.1/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_testing.py` & `nutils-8.1/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_topology.py` & `nutils-8.1/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_transform.py` & `nutils-8.1/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_transformseq.py` & `nutils-8.1/tests/test_transformseq.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_types.py` & `nutils-8.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_unit.py` & `nutils-8.1/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/tests/test_util.py` & `nutils-8.1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `nutils-8.0/PKG-INFO` & `nutils-8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutils
-Version: 8.0
+Version: 8.1
 Summary: Numerical Utilities for Finite Element Analysis
 Author-email: Evalf <info@evalf.com>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
```

