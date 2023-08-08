# Comparing `tmp/dftpy-2.0.2.tar.gz` & `tmp/dftpy-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dftpy-2.0.2.tar", last modified: Thu Jun 29 00:36:51 2023, max compression
+gzip compressed data, was "dftpy-2.0.3.tar", last modified: Tue Aug  8 15:22:35 2023, max compression
```

## Comparing `dftpy-2.0.2.tar` & `dftpy-2.0.3.tar`

### file list

```diff
@@ -1,280 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.303022 dftpy-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 00:36:39.000000 dftpy-2.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.243022 dftpy-2.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.255022 dftpy-2.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-29 00:36:39.000000 dftpy-2.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-29 00:36:39.000000 dftpy-2.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-29 00:36:39.000000 dftpy-2.0.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-29 00:36:39.000000 dftpy-2.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-29 00:36:39.000000 dftpy-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-29 00:36:51.303022 dftpy-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-29 00:36:39.000000 dftpy-2.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.255022 dftpy-2.0.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     4189 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/gen_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.259022 dftpy-2.0.2/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/contact.rst
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/ofdft.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/releases.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.259022 dftpy-2.0.2/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)   270398 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/static/dftpy.ico
--rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/static/dftpy.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/static/dftpy.png
--rw-r--r--   0 runner    (1001) docker     (123)   254932 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/static/dftpy_new_bkg.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.259022 dftpy-2.0.2/doc/source/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.259022 dftpy-2.0.2/doc/source/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.263022 dftpy-2.0.2/doc/source/tutorials/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)    23595 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/jupyter/density.png
--rw-r--r--   0 runner    (1001) docker     (123)   220165 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/jupyter/density_optimization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/jupyter/ions.png
--rw-r--r--   0 runner    (1001) docker     (123)   747735 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/jupyter/movie.gif
--rw-r--r--   0 runner    (1001) docker     (123)   393516 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/jupyter/td-ofdft-tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.267022 dftpy-2.0.2/doc/source/tutorials/ofdft/
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/ofdft/ase_traj.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/ofdft/md.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/ofdft/nvt.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/ofdft/optimize.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/ofdft/relax.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/ofdft/relax.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.267022 dftpy-2.0.2/doc/source/tutorials/tddft/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/tddft/optimize.ini
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/tddft/propagate.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/tddft/propagate.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-29 00:36:39.000000 dftpy-2.0.2/doc/source/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.247022 dftpy-2.0.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.283022 dftpy-2.0.2/examples/DATA/
--rw-r--r--   0 runner    (1001) docker     (123)  1605583 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/Al_fde_rho.pp
--rw-r--r--   0 runner    (1001) docker     (123)   196436 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/Al_lda.oe01.recpot
--rw-r--r--   0 runner    (1001) docker     (123)   196502 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/As_lda.oe04.recpot
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/GaAs.cif
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/GaAs.vasp
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/GaAs.xyz
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/GaAs_random.vasp
--rw-r--r--   0 runner    (1001) docker     (123)   208643 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/GaAs_random.xsf
--rw-r--r--   0 runner    (1001) docker     (123)   196489 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/Ga_lda.oe04.recpot
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/Mg8.vasp
--rw-r--r--   0 runner    (1001) docker     (123)    98081 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/Mg_OEPP_PZ.UPF
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/Mg_cluster.vasp
--rw-r--r--   0 runner    (1001) docker     (123)   196232 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/Mg_lda.oe01.recpot
--rw-r--r--   0 runner    (1001) docker     (123)   233666 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/al.gga.recpot
--rw-r--r--   0 runner    (1001) docker     (123)    69674 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/al.lda.lps
--rw-r--r--   0 runner    (1001) docker     (123)    69674 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/al.lda.psp
--rw-r--r--   0 runner    (1001) docker     (123)   492756 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/al.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)   224896 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/al.lda.upf
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/al_random.in
--rw-r--r--   0 runner    (1001) docker     (123)  3705904 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/al_random.xsf
--rw-r--r--   0 runner    (1001) docker     (123)   101843 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/as.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/ase_opt.traj
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/cd.vasp
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/fcc.vasp
--rw-r--r--   0 runner    (1001) docker     (123)    67650 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/ga.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/hd.vasp
--rw-r--r--   0 runner    (1001) docker     (123)   507599 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/in.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/initial_atoms_md.traj
--rw-r--r--   0 runner    (1001) docker     (123)   233593 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/li.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/md.traj
--rw-r--r--   0 runner    (1001) docker     (123)   492424 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/mg.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)   337875 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/p.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)   338504 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/sb.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)   233695 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/si.gga.recpot
--rw-r--r--   0 runner    (1001) docker     (123)    95514 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/si.lda.recpot
--rw-r--r--   0 runner    (1001) docker     (123)  1280986 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/ti.xsf
--rw-r--r--   0 runner    (1001) docker     (123)   577420 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/DATA/ti_pbe_v1.4.uspp.F.UPF
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.283022 dftpy-2.0.2/examples/md/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2463 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/md/test_ase_npt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/md/test_ase_nvt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2346 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/md/test_ase_nvt_nh.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/md/traj2xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.283022 dftpy-2.0.2/examples/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)   220165 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/notebooks/density_optimization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   393516 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/notebooks/td-ofdft-tutorial.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.287021 dftpy-2.0.2/examples/ofdft/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/ofdft/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/ofdft/isolate.ini
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/ofdft/optim.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/ofdft/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/ofdft/optim_pbe.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/ofdft/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.287021 dftpy-2.0.2/examples/relax/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1916 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/relax/test_ase_opt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.287021 dftpy-2.0.2/examples/td-ofdft/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/td-ofdft/casida.ini
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/td-ofdft/optimize.ini
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/td-ofdft/propagate-restart.ini
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/td-ofdft/propagate.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.287021 dftpy-2.0.2/examples/test/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_ase_md.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_ase_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_ase_pmg_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_density_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_ewald.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_functional_LibXC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_linear_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_mpi_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_pme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_propagator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_read_pp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_rvv10.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_snpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-29 00:36:39.000000 dftpy-2.0.2/examples/test/test_xc.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 00:36:39.000000 dftpy-2.0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.291022 dftpy-2.0.2/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/convertPP.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1499 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/convert_den.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/convert_td.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      217 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/dftpy
--rwxr-xr-x   0 runner    (1001) docker     (123)     1161 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/invert
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/opt_layer_pseudo.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8906 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/quadrupole.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2121 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/rtc_runner
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-06-29 00:36:39.000000 dftpy-2.0.2/scripts/test_layer_pseudo.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-29 00:36:51.303022 dftpy-2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-06-29 00:36:39.000000 dftpy-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.247022 dftpy-2.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.291022 dftpy-2.0.2/src/dftpy/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.291022 dftpy-2.0.2/src/dftpy/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/api/api4ase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/api/dftd4.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.291022 dftpy-2.0.2/src/dftpy/config/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/config/config_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/config/configentries.json
--rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.291022 dftpy-2.0.2/src/dftpy/cui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/cui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/cui/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.291022 dftpy-2.0.2/src/dftpy/density/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/density/density.py
--rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/ewald.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/fft.py
--rw-r--r--   0 runner    (1001) docker     (123)    29611 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.295022 dftpy-2.0.2/src/dftpy/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/ase_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/chg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/cube.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/den.py
--rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/npy.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/pmg_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/qepp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/snpy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/vasp.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/xsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/formats/xyz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.295022 dftpy-2.0.2/src/dftpy/functional/
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/abstract_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/external_potential.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/functional_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/hartree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.295022 dftpy-2.0.2/src/dftpy/functional/kedf/
--rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/fp.py
--rw-r--r--   0 runner    (1001) docker     (123)    48091 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/gga.py
--rw-r--r--   0 runner    (1001) docker     (123)    16248 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/hc.py
--rw-r--r--   0 runner    (1001) docker     (123)    16487 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/lkt.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/lwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/mgp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/sm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/tf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/vw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/kedf/wt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.295022 dftpy-2.0.2/src/dftpy/functional/nonadiabatic/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/nonadiabatic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/nonadiabatic/jp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/nonadiabatic/wcdhc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/functional/pseudo/
--rw-r--r--   0 runner    (1001) docker     (123)    28890 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/pseudo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/pseudo/abstract_pseudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/pseudo/layer_pseudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/pseudo/psp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/pseudo/recpot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/pseudo/upf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/pseudo/usp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/pseudo/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/semilocal_xc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/total_functional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/functional/xc/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/xc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/xc/rvv10.py
--rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/xc/semilocal_xc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/functional/xc/xc.json
--rw-r--r--   0 runner    (1001) docker     (123)    27063 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/invert/
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/invert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/invert/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/inverter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/ions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/linear_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mixer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mixer/mixer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mixer/pulay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/mpi/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mpi/mp_mpi4py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mpi/mp_serial.py
--rw-r--r--   0 runner    (1001) docker     (123)    10314 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mpi/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/mpi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/optimization/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/optimization/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/properties/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/properties/potential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/td/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/casida.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/hamiltonian.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/predictor_corrector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/td/propagator/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/propagator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/propagator/abstract_propagator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/propagator/crank_nicholson.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/propagator/taylor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13333 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/real_time_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/td/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/time_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.299022 dftpy-2.0.2/src/dftpy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.303022 dftpy-2.0.2/src/dftpy/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/visualize/ase_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/visualize/ipv_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/visualize/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/visualize/mpl_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-29 00:36:39.000000 dftpy-2.0.2/src/dftpy/visualize/vesta_viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 00:36:51.291022 dftpy-2.0.2/src/dftpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-29 00:36:51.000000 dftpy-2.0.2/src/dftpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-06-29 00:36:51.000000 dftpy-2.0.2/src/dftpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 00:36:51.000000 dftpy-2.0.2/src/dftpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-29 00:36:51.000000 dftpy-2.0.2/src/dftpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-29 00:36:51.000000 dftpy-2.0.2/src/dftpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.063122 dftpy-2.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-08-08 15:22:24.000000 dftpy-2.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:34.991121 dftpy-2.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.003121 dftpy-2.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-08-08 15:22:24.000000 dftpy-2.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-08-08 15:22:24.000000 dftpy-2.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-08-08 15:22:24.000000 dftpy-2.0.3/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-08-08 15:22:24.000000 dftpy-2.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-08-08 15:22:24.000000 dftpy-2.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-08 15:22:35.063122 dftpy-2.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-08 15:22:24.000000 dftpy-2.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.003121 dftpy-2.0.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4189 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/gen_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.007122 dftpy-2.0.3/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/contact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/ofdft.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/releases.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.007122 dftpy-2.0.3/doc/source/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)   270398 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/static/dftpy.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    27665 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/static/dftpy.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     7269 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/static/dftpy.png
+-rw-r--r--   0 runner    (1001) docker     (123)   254932 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/static/dftpy_new_bkg.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.007122 dftpy-2.0.3/doc/source/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.007122 dftpy-2.0.3/doc/source/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.011122 dftpy-2.0.3/doc/source/tutorials/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)    23595 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/jupyter/density.png
+-rw-r--r--   0 runner    (1001) docker     (123)   220165 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/jupyter/density_optimization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    19646 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/jupyter/ions.png
+-rw-r--r--   0 runner    (1001) docker     (123)   747735 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/jupyter/movie.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   393516 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/jupyter/td-ofdft-tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.015122 dftpy-2.0.3/doc/source/tutorials/ofdft/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/ofdft/ase_traj.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/ofdft/md.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/ofdft/nvt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/ofdft/optimize.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1301 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/ofdft/relax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/ofdft/relax.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.015122 dftpy-2.0.3/doc/source/tutorials/tddft/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/tddft/optimize.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/tddft/propagate.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/tddft/propagate.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-08 15:22:24.000000 dftpy-2.0.3/doc/source/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:34.995121 dftpy-2.0.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.035122 dftpy-2.0.3/examples/DATA/
+-rw-r--r--   0 runner    (1001) docker     (123)  1605583 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/Al_fde_rho.pp
+-rw-r--r--   0 runner    (1001) docker     (123)   196436 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/Al_lda.oe01.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)   196502 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/As_lda.oe04.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/GaAs.cif
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/GaAs.vasp
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/GaAs.xyz
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/GaAs_random.vasp
+-rw-r--r--   0 runner    (1001) docker     (123)   208643 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/GaAs_random.xsf
+-rw-r--r--   0 runner    (1001) docker     (123)   196489 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/Ga_lda.oe04.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/Mg8.vasp
+-rw-r--r--   0 runner    (1001) docker     (123)    98081 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/Mg_OEPP_PZ.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/Mg_cluster.vasp
+-rw-r--r--   0 runner    (1001) docker     (123)   196232 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/Mg_lda.oe01.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)   233666 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/al.gga.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)    69674 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/al.lda.lps
+-rw-r--r--   0 runner    (1001) docker     (123)    69674 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/al.lda.psp
+-rw-r--r--   0 runner    (1001) docker     (123)   492756 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/al.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)   224896 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/al.lda.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/al_random.in
+-rw-r--r--   0 runner    (1001) docker     (123)  3705904 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/al_random.xsf
+-rw-r--r--   0 runner    (1001) docker     (123)   101843 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/as.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/ase_opt.traj
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/cd.vasp
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/fcc.vasp
+-rw-r--r--   0 runner    (1001) docker     (123)    67650 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/ga.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/hd.vasp
+-rw-r--r--   0 runner    (1001) docker     (123)   507599 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/in.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)     6437 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/initial_atoms_md.traj
+-rw-r--r--   0 runner    (1001) docker     (123)   233593 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/li.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)    25874 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/md.traj
+-rw-r--r--   0 runner    (1001) docker     (123)   492424 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/mg.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)   337875 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/p.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)   338504 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/sb.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)   233695 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/si.gga.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)    95514 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/si.lda.recpot
+-rw-r--r--   0 runner    (1001) docker     (123)  1280986 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/ti.xsf
+-rw-r--r--   0 runner    (1001) docker     (123)   577420 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/DATA/ti_pbe_v1.4.uspp.F.UPF
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.039122 dftpy-2.0.3/examples/md/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2463 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/md/test_ase_npt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2156 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/md/test_ase_nvt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2346 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/md/test_ase_nvt_nh.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      197 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/md/traj2xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.039122 dftpy-2.0.3/examples/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)   220165 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/notebooks/density_optimization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   393516 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/notebooks/td-ofdft-tutorial.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.039122 dftpy-2.0.3/examples/ofdft/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/ofdft/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/ofdft/isolate.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/ofdft/optim.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/ofdft/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/ofdft/optim_pbe.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/ofdft/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.039122 dftpy-2.0.3/examples/relax/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1916 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/relax/test_ase_opt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.043122 dftpy-2.0.3/examples/td-ofdft/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/td-ofdft/casida.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/td-ofdft/optimize.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/td-ofdft/propagate-restart.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/td-ofdft/propagate.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.043122 dftpy-2.0.3/examples/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_ase_md.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_ase_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_ase_pmg_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_density_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_ewald.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_functional_LibXC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_linear_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-08 15:22:24.000000 dftpy-2.0.3/examples/test/test_mpi_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-08 15:22:25.000000 dftpy-2.0.3/examples/test/test_pme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-08-08 15:22:25.000000 dftpy-2.0.3/examples/test/test_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-08 15:22:25.000000 dftpy-2.0.3/examples/test/test_read_pp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-08 15:22:25.000000 dftpy-2.0.3/examples/test/test_rvv10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-08-08 15:22:25.000000 dftpy-2.0.3/examples/test/test_snpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-08 15:22:25.000000 dftpy-2.0.3/examples/test/test_xc.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-08 15:22:25.000000 dftpy-2.0.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.047122 dftpy-2.0.3/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/convertPP.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1499 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/convert_den.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/convert_td.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      217 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/dftpy
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1161 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/invert
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/opt_layer_pseudo.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8906 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/quadrupole.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2121 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/rtc_runner
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-08-08 15:22:25.000000 dftpy-2.0.3/scripts/test_layer_pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-08 15:22:35.063122 dftpy-2.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-08-08 15:22:25.000000 dftpy-2.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:34.995121 dftpy-2.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.047122 dftpy-2.0.3/src/dftpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.047122 dftpy-2.0.3/src/dftpy/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/api/api4ase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3658 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/api/dftd4.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.047122 dftpy-2.0.3/src/dftpy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/config/config_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23587 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/config/configentries.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.051122 dftpy-2.0.3/src/dftpy/cui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/cui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/cui/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.051122 dftpy-2.0.3/src/dftpy/density/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/density/density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36420 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/ewald.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/fft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29834 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.051122 dftpy-2.0.3/src/dftpy/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/ase_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/chg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/cube.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/den.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8417 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/npy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/pmg_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/qepp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/snpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/xsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/formats/xyz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.051122 dftpy-2.0.3/src/dftpy/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/abstract_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/external_potential.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/functional_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/hartree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.055122 dftpy-2.0.3/src/dftpy/functional/kedf/
+-rw-r--r--   0 runner    (1001) docker     (123)    17358 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/fp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48091 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/gga.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16248 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/hc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16487 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/lkt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/lwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/mgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/sm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/tf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/vw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/kedf/wt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.055122 dftpy-2.0.3/src/dftpy/functional/nonadiabatic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/nonadiabatic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/nonadiabatic/jp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/nonadiabatic/wcdhc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.055122 dftpy-2.0.3/src/dftpy/functional/pseudo/
+-rw-r--r--   0 runner    (1001) docker     (123)    28890 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/pseudo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/pseudo/abstract_pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/pseudo/layer_pseudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5089 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/pseudo/psp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/pseudo/recpot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/pseudo/upf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/pseudo/usp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/pseudo/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/semilocal_xc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/total_functional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.055122 dftpy-2.0.3/src/dftpy/functional/xc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/xc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9520 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/xc/rvv10.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20079 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/xc/semilocal_xc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/functional/xc/xc.json
+-rw-r--r--   0 runner    (1001) docker     (123)    27080 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13715 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.059122 dftpy-2.0.3/src/dftpy/invert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/invert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/invert/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/inverter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/ions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/linear_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15721 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.059122 dftpy-2.0.3/src/dftpy/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mixer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mixer/mixer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mixer/pulay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.059122 dftpy-2.0.3/src/dftpy/mpi/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mpi/mp_mpi4py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mpi/mp_serial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10489 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mpi/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/mpi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.059122 dftpy-2.0.3/src/dftpy/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21103 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/optimization/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/optimization/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.059122 dftpy-2.0.3/src/dftpy/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/properties/potential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.059122 dftpy-2.0.3/src/dftpy/td/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/casida.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/hamiltonian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/predictor_corrector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.063122 dftpy-2.0.3/src/dftpy/td/propagator/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/propagator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/propagator/abstract_propagator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6806 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/propagator/crank_nicholson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/propagator/taylor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/real_time_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/td/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/time_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.063122 dftpy-2.0.3/src/dftpy/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.063122 dftpy-2.0.3/src/dftpy/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/visualize/ase_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/visualize/ipv_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/visualize/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/visualize/mpl_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-08-08 15:22:25.000000 dftpy-2.0.3/src/dftpy/visualize/vesta_viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 15:22:35.047122 dftpy-2.0.3/src/dftpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-08 15:22:34.000000 dftpy-2.0.3/src/dftpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-08-08 15:22:34.000000 dftpy-2.0.3/src/dftpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 15:22:34.000000 dftpy-2.0.3/src/dftpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-08 15:22:34.000000 dftpy-2.0.3/src/dftpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 15:22:34.000000 dftpy-2.0.3/src/dftpy.egg-info/top_level.txt
```

### Comparing `dftpy-2.0.2/.github/workflows/publish.yml` & `dftpy-2.0.3/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/.gitlab-ci.yml` & `dftpy-2.0.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/LICENSE.txt` & `dftpy-2.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/PKG-INFO` & `dftpy-2.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dftpy
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python3 packages for Density Functional Theory
 Home-page: http://dftpy.rutgers.edu
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dftpy-2.0.2/doc/Makefile` & `dftpy-2.0.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/gen_doc.py` & `dftpy-2.0.3/doc/gen_doc.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/make.bat` & `dftpy-2.0.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/conf.py` & `dftpy-2.0.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/contact.rst` & `dftpy-2.0.3/doc/source/contact.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/faq.rst` & `dftpy-2.0.3/doc/source/faq.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/index.rst` & `dftpy-2.0.3/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/install.rst` & `dftpy-2.0.3/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/ofdft.rst` & `dftpy-2.0.3/doc/source/ofdft.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/releases.rst` & `dftpy-2.0.3/doc/source/releases.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/static/dftpy.ico` & `dftpy-2.0.3/doc/source/static/dftpy.ico`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/static/dftpy.jpg` & `dftpy-2.0.3/doc/source/static/dftpy.jpg`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/static/dftpy.png` & `dftpy-2.0.3/doc/source/static/dftpy.png`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/static/dftpy_new_bkg.png` & `dftpy-2.0.3/doc/source/static/dftpy_new_bkg.png`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/templates/breadcrumbs.html` & `dftpy-2.0.3/doc/source/templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/templates/footer.html` & `dftpy-2.0.3/doc/source/templates/footer.html`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/jupyter/density.png` & `dftpy-2.0.3/doc/source/tutorials/jupyter/density.png`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/jupyter/density_optimization.ipynb` & `dftpy-2.0.3/doc/source/tutorials/jupyter/density_optimization.ipynb`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/jupyter/ions.png` & `dftpy-2.0.3/doc/source/tutorials/jupyter/ions.png`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/jupyter/movie.gif` & `dftpy-2.0.3/doc/source/tutorials/jupyter/movie.gif`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/jupyter/td-ofdft-tutorial.ipynb` & `dftpy-2.0.3/doc/source/tutorials/jupyter/td-ofdft-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/ofdft/nvt.py` & `dftpy-2.0.3/doc/source/tutorials/ofdft/nvt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/ofdft/relax.py` & `dftpy-2.0.3/doc/source/tutorials/ofdft/relax.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/ofdft/relax.rst` & `dftpy-2.0.3/doc/source/tutorials/ofdft/relax.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/tddft/propagate.ini` & `dftpy-2.0.3/doc/source/tutorials/tddft/propagate.ini`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/doc/source/tutorials/tddft/propagate.rst` & `dftpy-2.0.3/doc/source/tutorials/tddft/propagate.rst`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/Al_fde_rho.pp` & `dftpy-2.0.3/examples/DATA/Al_fde_rho.pp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/Al_lda.oe01.recpot` & `dftpy-2.0.3/examples/DATA/Al_lda.oe01.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/As_lda.oe04.recpot` & `dftpy-2.0.3/examples/DATA/As_lda.oe04.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/GaAs.cif` & `dftpy-2.0.3/examples/DATA/GaAs.cif`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/GaAs.vasp` & `dftpy-2.0.3/examples/DATA/GaAs.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/GaAs_random.vasp` & `dftpy-2.0.3/examples/DATA/GaAs_random.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/GaAs_random.xsf` & `dftpy-2.0.3/examples/DATA/GaAs_random.xsf`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/Ga_lda.oe04.recpot` & `dftpy-2.0.3/examples/DATA/Ga_lda.oe04.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/Mg8.vasp` & `dftpy-2.0.3/examples/DATA/Mg8.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/Mg_OEPP_PZ.UPF` & `dftpy-2.0.3/examples/DATA/Mg_OEPP_PZ.UPF`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/Mg_cluster.vasp` & `dftpy-2.0.3/examples/DATA/Mg_cluster.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/Mg_lda.oe01.recpot` & `dftpy-2.0.3/examples/DATA/Mg_lda.oe01.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/al.gga.recpot` & `dftpy-2.0.3/examples/DATA/al.gga.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/al.lda.lps` & `dftpy-2.0.3/examples/DATA/al.lda.lps`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/al.lda.psp` & `dftpy-2.0.3/examples/DATA/al.lda.psp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/al.lda.recpot` & `dftpy-2.0.3/examples/DATA/al.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/al.lda.upf` & `dftpy-2.0.3/examples/DATA/al.lda.upf`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/al_random.in` & `dftpy-2.0.3/examples/DATA/al_random.in`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/al_random.xsf` & `dftpy-2.0.3/examples/DATA/al_random.xsf`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/as.lda.recpot` & `dftpy-2.0.3/examples/DATA/as.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/ase_opt.traj` & `dftpy-2.0.3/examples/DATA/ase_opt.traj`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/cd.vasp` & `dftpy-2.0.3/examples/DATA/cd.vasp`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/ga.lda.recpot` & `dftpy-2.0.3/examples/DATA/ga.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/in.lda.recpot` & `dftpy-2.0.3/examples/DATA/in.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/initial_atoms_md.traj` & `dftpy-2.0.3/examples/DATA/initial_atoms_md.traj`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/li.lda.recpot` & `dftpy-2.0.3/examples/DATA/li.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/md.traj` & `dftpy-2.0.3/examples/DATA/md.traj`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/mg.lda.recpot` & `dftpy-2.0.3/examples/DATA/mg.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/p.lda.recpot` & `dftpy-2.0.3/examples/DATA/p.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/sb.lda.recpot` & `dftpy-2.0.3/examples/DATA/sb.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/si.gga.recpot` & `dftpy-2.0.3/examples/DATA/si.gga.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/si.lda.recpot` & `dftpy-2.0.3/examples/DATA/si.lda.recpot`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/ti.xsf` & `dftpy-2.0.3/examples/DATA/ti.xsf`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/DATA/ti_pbe_v1.4.uspp.F.UPF` & `dftpy-2.0.3/examples/DATA/ti_pbe_v1.4.uspp.F.UPF`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/md/test_ase_npt.py` & `dftpy-2.0.3/examples/md/test_ase_npt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/md/test_ase_nvt.py` & `dftpy-2.0.3/examples/md/test_ase_nvt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/md/test_ase_nvt_nh.py` & `dftpy-2.0.3/examples/md/test_ase_nvt_nh.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/notebooks/density_optimization.ipynb` & `dftpy-2.0.3/examples/notebooks/density_optimization.ipynb`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/notebooks/td-ofdft-tutorial.ipynb` & `dftpy-2.0.3/examples/notebooks/td-ofdft-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/ofdft/config.ini` & `dftpy-2.0.3/examples/ofdft/config.ini`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/ofdft/isolate.ini` & `dftpy-2.0.3/examples/ofdft/isolate.ini`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/ofdft/optim.py` & `dftpy-2.0.3/examples/ofdft/optim.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/ofdft/simple.py` & `dftpy-2.0.3/examples/ofdft/simple.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/relax/test_ase_opt.py` & `dftpy-2.0.3/examples/relax/test_ase_opt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/common.py` & `dftpy-2.0.3/examples/test/common.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_ase_md.py` & `dftpy-2.0.3/examples/test/test_ase_md.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 #!/usr/bin/env python3
 import os
 import unittest
 import numpy as np
 
 from dftpy.config import DefaultOption, OptionFormat
 from dftpy.api.api4ase import DFTpyCalculator
-import pytest
 
 
 class Test(unittest.TestCase):
     def test_md(self):
-        pytest.importorskip("ase")
         from ase.md.langevin import Langevin
         from ase.md.verlet import VelocityVerlet
         from ase.md.velocitydistribution import MaxwellBoltzmannDistribution
         from ase.io.trajectory import Trajectory
         from ase import units
         from ase.io import write, read
         dftpy_data_path = os.environ.get('DFTPY_DATA_PATH')
```

### Comparing `dftpy-2.0.2/examples/test/test_ase_opt.py` & `dftpy-2.0.3/examples/test/test_ase_opt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 #!/usr/bin/env python3
 import os
 import unittest
 import numpy as np
-import pytest
 
 from dftpy.config import DefaultOption, OptionFormat
 from dftpy.api.api4ase import DFTpyCalculator
 
 class Test(unittest.TestCase):
     def test_opt(self):
-        pytest.importorskip("ase")
         from ase.optimize import BFGS, LBFGS, FIRE
         from ase.optimize.sciopt import SciPyFminBFGS, SciPyFminCG
         from ase.constraints import StrainFilter, UnitCellFilter
         from ase.io.trajectory import Trajectory
         from ase import units
         from ase.io import read, write
         dftpy_data_path = os.environ.get('DFTPY_DATA_PATH')
```

### Comparing `dftpy-2.0.2/examples/test/test_ase_pmg_io.py` & `dftpy-2.0.3/examples/test/test_ase_pmg_io.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import numpy as np
 import dftpy.formats.io as dftpy_io
 import pytest
 
 
 class Test(unittest.TestCase):
     def test_io_ase(self):
-        pytest.importorskip("ase")
         dftpy_data_path = os.environ.get('DFTPY_DATA_PATH')
         a1 = dftpy_io.read(dftpy_data_path + '/fcc.vasp', driver='ase')
         a2 = dftpy_io.read(dftpy_data_path + '/fcc.vasp')
 
         self.assertTrue(np.allclose(a1.cell, a2.cell))
         self.assertTrue(np.allclose(a1.positions, a2.positions))
```

### Comparing `dftpy-2.0.2/examples/test/test_density_opt.py` & `dftpy-2.0.3/examples/test/test_density_opt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_ewald.py` & `dftpy-2.0.3/examples/test/test_ewald.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_field.py` & `dftpy-2.0.3/examples/test/test_field.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_functional.py` & `dftpy-2.0.3/examples/test/test_functional.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_functional_LibXC.py` & `dftpy-2.0.3/examples/test/test_functional_LibXC.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_grid.py` & `dftpy-2.0.3/examples/test/test_grid.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_linear_solver.py` & `dftpy-2.0.3/examples/test/test_linear_solver.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_mpi_grid.py` & `dftpy-2.0.3/examples/test/test_mpi_grid.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_pme.py` & `dftpy-2.0.3/examples/test/test_pme.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_propagator.py` & `dftpy-2.0.3/examples/test/test_propagator.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_read_pp.py` & `dftpy-2.0.3/examples/test/test_read_pp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_rvv10.py` & `dftpy-2.0.3/examples/test/test_rvv10.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_snpy.py` & `dftpy-2.0.3/examples/test/test_snpy.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/examples/test/test_xc.py` & `dftpy-2.0.3/examples/test/test_xc.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/scripts/convertPP.py` & `dftpy-2.0.3/scripts/convertPP.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/scripts/convert_den.py` & `dftpy-2.0.3/scripts/convert_den.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/scripts/convert_td.py` & `dftpy-2.0.3/scripts/convert_td.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/scripts/invert` & `dftpy-2.0.3/scripts/invert`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/scripts/opt_layer_pseudo.py` & `dftpy-2.0.3/scripts/opt_layer_pseudo.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/scripts/quadrupole.py` & `dftpy-2.0.3/scripts/quadrupole.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/scripts/rtc_runner` & `dftpy-2.0.3/scripts/rtc_runner`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/scripts/test_layer_pseudo.py` & `dftpy-2.0.3/scripts/test_layer_pseudo.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/setup.py` & `dftpy-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/api/dftd4.py` & `dftpy-2.0.3/src/dftpy/api/dftd4.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/config/config.py` & `dftpy-2.0.3/src/dftpy/config/config.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/config/config_entry.py` & `dftpy-2.0.3/src/dftpy/config/config_entry.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/config/configentries.json` & `dftpy-2.0.3/src/dftpy/config/configentries.json`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/constants.py` & `dftpy-2.0.3/src/dftpy/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -82,18 +82,15 @@
 C_TF = 2.87123400018819181594
 TKF0 = 6.18733545256027186194
 CBRT_TWO = 1.25992104989487316477
 ZERO = 1E-30
 
 environ = {} # You can change it anytime you want
 environ['STDOUT'] = sys.stdout # file descriptor of sprint
-try:
-    environ['LOGLEVEL'] = int(os.environ.get('DFTPY_LOGLEVEL', 2)) # The level of sprint
-except Exception :
-    environ['LOGLEVEL'] = 2 # The level of sprint
+environ['LOGLEVEL'] = int(os.environ.get('DFTPY_LOGLEVEL', 2)) # The level of sprint
 """
     0 : all
     1 : debug
     2 : info
     3 : warning
     4 : error
 """
```

### Comparing `dftpy-2.0.2/src/dftpy/cui/main.py` & `dftpy-2.0.3/src/dftpy/cui/main.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/density/density.py` & `dftpy-2.0.3/src/dftpy/density/density.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/ewald.py` & `dftpy-2.0.3/src/dftpy/ewald.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/fft.py` & `dftpy-2.0.3/src/dftpy/fft.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/field.py` & `dftpy-2.0.3/src/dftpy/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,20 @@
                 input_values = np.zeros(nr, dtype ='complex128', order = order)
             else :
                 input_values = np.zeros(nr, order = order)
         else :
             input_values = np.asarray(data)
             input_values = np.reshape(input_values, nr, order=order)
 
-        obj = np.asarray(input_values).view(cls)
+        obj = np.asarray(input_values)
+        if order == 'C' and not obj.flags['C_CONTIGUOUS']:
+            obj = np.ascontiguousarray(obj)
+        elif order == 'F' and not obj.flags['F_CONTIGUOUS']:
+            obj = np.asfortranarray(obj)
+        obj = obj.view(cls)
         # add the new attribute to the created instance
         obj.grid = grid
         obj.span = (grid.nr > 1).sum()
         obj.memo = str(memo)
         obj.mp = obj.grid.mp
         # Finally, we must return the newly created object:
         return obj
```

### Comparing `dftpy-2.0.2/src/dftpy/formats/ase_io.py` & `dftpy-2.0.3/src/dftpy/formats/ase_io.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/chg.py` & `dftpy-2.0.3/src/dftpy/formats/chg.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/cube.py` & `dftpy-2.0.3/src/dftpy/formats/cube.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/den.py` & `dftpy-2.0.3/src/dftpy/formats/den.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/io.py` & `dftpy-2.0.3/src/dftpy/formats/io.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/npy.py` & `dftpy-2.0.3/src/dftpy/formats/npy.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/pmg_io.py` & `dftpy-2.0.3/src/dftpy/formats/pmg_io.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/qepp.py` & `dftpy-2.0.3/src/dftpy/formats/qepp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/snpy.py` & `dftpy-2.0.3/src/dftpy/formats/snpy.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/vasp.py` & `dftpy-2.0.3/src/dftpy/formats/vasp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/xsf.py` & `dftpy-2.0.3/src/dftpy/formats/xsf.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/formats/xyz.py` & `dftpy-2.0.3/src/dftpy/formats/xyz.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/__init__.py` & `dftpy-2.0.3/src/dftpy/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/abstract_functional.py` & `dftpy-2.0.3/src/dftpy/functional/abstract_functional.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/external_potential.py` & `dftpy-2.0.3/src/dftpy/functional/external_potential.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/functional_output.py` & `dftpy-2.0.3/src/dftpy/functional/functional_output.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/hartree.py` & `dftpy-2.0.3/src/dftpy/functional/hartree.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/__init__.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/fp.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/fp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/gga.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/gga.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/hc.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/hc.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/kernel.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/kernel.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/lkt.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/lkt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/lwt.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/lwt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/mgp.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/mgp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/sm.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/sm.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/tf.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/tf.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/vw.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/vw.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/kedf/wt.py` & `dftpy-2.0.3/src/dftpy/functional/kedf/wt.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/nonadiabatic/__init__.py` & `dftpy-2.0.3/src/dftpy/functional/nonadiabatic/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/nonadiabatic/jp.py` & `dftpy-2.0.3/src/dftpy/functional/nonadiabatic/jp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/nonadiabatic/wcdhc.py` & `dftpy-2.0.3/src/dftpy/functional/nonadiabatic/wcdhc.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/pseudo/__init__.py` & `dftpy-2.0.3/src/dftpy/functional/pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/pseudo/abstract_pseudo.py` & `dftpy-2.0.3/src/dftpy/functional/pseudo/abstract_pseudo.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/pseudo/layer_pseudo.py` & `dftpy-2.0.3/src/dftpy/functional/pseudo/layer_pseudo.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/pseudo/psp.py` & `dftpy-2.0.3/src/dftpy/functional/pseudo/psp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/pseudo/recpot.py` & `dftpy-2.0.3/src/dftpy/functional/pseudo/recpot.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/pseudo/upf.py` & `dftpy-2.0.3/src/dftpy/functional/pseudo/upf.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/pseudo/usp.py` & `dftpy-2.0.3/src/dftpy/functional/pseudo/usp.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/pseudo/xml.py` & `dftpy-2.0.3/src/dftpy/functional/pseudo/xml.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/total_functional.py` & `dftpy-2.0.3/src/dftpy/functional/total_functional.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/xc/__init__.py` & `dftpy-2.0.3/src/dftpy/functional/xc/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/xc/rvv10.py` & `dftpy-2.0.3/src/dftpy/functional/xc/rvv10.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/xc/semilocal_xc.py` & `dftpy-2.0.3/src/dftpy/functional/xc/semilocal_xc.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/functional/xc/xc.json` & `dftpy-2.0.3/src/dftpy/functional/xc/xc.json`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/grid.py` & `dftpy-2.0.3/src/dftpy/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
     Node:
     Virtual class, DirectGrid and ReciprocalGrid should be used in actual applications
 
     """
 
     def __init__(self, lattice, nr = None, origin=np.array([0.0, 0.0, 0.0]), full=True, direct=True,
-                 cplx=False, mp=None, ecut = None, **kwargs):
+                 cplx=False, mp=None, ecut = None, comm = None, **kwargs):
         if mp is None :
-            mp = MP()
+            mp = MP(comm)
         self._origin = np.asarray(origin)
         if not isinstance(lattice, Cell):
             cell=Cell(lattice)
         else:
             cell=lattice
         #
         self.cplx = cplx
```

### Comparing `dftpy-2.0.2/src/dftpy/interface.py` & `dftpy-2.0.3/src/dftpy/interface.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/invert/__init__.py` & `dftpy-2.0.3/src/dftpy/invert/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/inverter.py` & `dftpy-2.0.3/src/dftpy/inverter.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/ions.py` & `dftpy-2.0.3/src/dftpy/ions.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/linear_solver.py` & `dftpy-2.0.3/src/dftpy/linear_solver.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/math_utils.py` & `dftpy-2.0.3/src/dftpy/math_utils.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/mixer/__init__.py` & `dftpy-2.0.3/src/dftpy/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/mixer/linear.py` & `dftpy-2.0.3/src/dftpy/mixer/linear.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/mixer/mixer.py` & `dftpy-2.0.3/src/dftpy/mixer/mixer.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/mixer/pulay.py` & `dftpy-2.0.3/src/dftpy/mixer/pulay.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/mpi/mp_mpi4py.py` & `dftpy-2.0.3/src/dftpy/mpi/mp_mpi4py.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         backend = environ["FFTLIB"]
     if backend not in fft_support :
         backend = 'numpy'
 
     cplx = cplx or full
     if cplx :
         backend = 'numpy' # If cplx, use numpy for safe
-        dtype = np.complex
+        dtype = np.complex128
     else :
         dtype = np.float64
 
     global fft_saved
     saved = 0
     item = fft_saved.get(id(comm), None)
     if item is not None and item.global_shape() == tuple(nr):
```

### Comparing `dftpy-2.0.2/src/dftpy/mpi/mp_serial.py` & `dftpy-2.0.3/src/dftpy/mpi/mp_serial.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/mpi/mpi.py` & `dftpy-2.0.3/src/dftpy/mpi/mpi.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,14 +286,19 @@
         return a
 
     def _sum_mul(self, *args):
         a = self._mul(*args)
         s = self._sum_1(a)
         return s
 
+    def sprint(self, *args, comm = None, **kwargs):
+        from .utils import sprint
+        if comm is None : comm = self.comm
+        sprint(*args, comm = comm, **kwargs)
+
 class PMI :
     """
     Detect mpi
     ref :
         https://www.open-mpi.org/faq/?category=running#mpi-environmental-variables
         https://docs.microsoft.com/en-us/powershell/high-performance-computing/environment-variables-for-the-mpiexec-command
     """
```

### Comparing `dftpy-2.0.2/src/dftpy/mpi/utils.py` & `dftpy-2.0.3/src/dftpy/mpi/utils.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/optimization/optimization.py` & `dftpy-2.0.3/src/dftpy/optimization/optimization.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/optimization/scf.py` & `dftpy-2.0.3/src/dftpy/optimization/scf.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/optimize.py` & `dftpy-2.0.3/src/dftpy/optimize.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/casida.py` & `dftpy-2.0.3/src/dftpy/td/casida.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/hamiltonian.py` & `dftpy-2.0.3/src/dftpy/td/hamiltonian.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/interface.py` & `dftpy-2.0.3/src/dftpy/td/interface.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/operator.py` & `dftpy-2.0.3/src/dftpy/td/operator.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/predictor_corrector.py` & `dftpy-2.0.3/src/dftpy/td/predictor_corrector.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/propagator/__init__.py` & `dftpy-2.0.3/src/dftpy/td/propagator/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/propagator/abstract_propagator.py` & `dftpy-2.0.3/src/dftpy/td/propagator/abstract_propagator.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/propagator/crank_nicholson.py` & `dftpy-2.0.3/src/dftpy/td/propagator/crank_nicholson.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/propagator/taylor.py` & `dftpy-2.0.3/src/dftpy/td/propagator/taylor.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/td/real_time_runner.py` & `dftpy-2.0.3/src/dftpy/td/real_time_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         converged = self.predictor_corrector.run()
         if not converged:
             self.predictor_corrector.print_not_converged_info()
 
         if self.correction:
             correct_potential = self.correct_functionals(self.rho, calcType=['V'], current=self.j).potential
             self.correct_propagator.hamiltonian.v = correct_potential
-            self.predictor_corrector.psi_pred = self.correct_propagator(self.predictor_corrector.psi_pred)
+            self.predictor_corrector.psi_pred, info = self.correct_propagator(self.predictor_corrector.psi_pred)
             self.predictor_corrector.rho_pred = calc_rho(self.predictor_corrector.psi_pred)
             self.predictor_corrector.j_pred = calc_j(self.predictor_corrector.psi_pred)
 
         self.psi = self.predictor_corrector.psi_pred
         self.rho = self.predictor_corrector.rho_pred
         self.j = self.predictor_corrector.j_pred
```

### Comparing `dftpy-2.0.2/src/dftpy/td/utils.py` & `dftpy-2.0.3/src/dftpy/td/utils.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/time_data.py` & `dftpy-2.0.3/src/dftpy/time_data.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/utils/__init__.py` & `dftpy-2.0.3/src/dftpy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/utils/utils.py` & `dftpy-2.0.3/src/dftpy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/visualize/__init__.py` & `dftpy-2.0.3/src/dftpy/visualize/__init__.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/visualize/ipv_viewer.py` & `dftpy-2.0.3/src/dftpy/visualize/ipv_viewer.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/visualize/jupyter.py` & `dftpy-2.0.3/src/dftpy/visualize/jupyter.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/visualize/mpl_viewer.py` & `dftpy-2.0.3/src/dftpy/visualize/mpl_viewer.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy/visualize/vesta_viewer.py` & `dftpy-2.0.3/src/dftpy/visualize/vesta_viewer.py`

 * *Files identical despite different names*

### Comparing `dftpy-2.0.2/src/dftpy.egg-info/PKG-INFO` & `dftpy-2.0.3/src/dftpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dftpy
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python3 packages for Density Functional Theory
 Home-page: http://dftpy.rutgers.edu
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `dftpy-2.0.2/src/dftpy.egg-info/SOURCES.txt` & `dftpy-2.0.3/src/dftpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

