# Comparing `tmp/gplugins-0.1.0.tar.gz` & `tmp/gplugins-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gplugins-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gplugins-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gplugins-0.1.0.tar` & `gplugins-0.1.1.tar`

### file list

```diff
@@ -1,208 +1,212 @@
--rw-r--r--   0        0        0     1077 2023-08-06 18:26:48.063156 gplugins-0.1.0/LICENSE
--rw-r--r--   0        0        0     2235 2023-08-06 18:26:48.063156 gplugins-0.1.0/README.md
--rw-r--r--   0        0        0      244 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/__init__.py
--rw-r--r--   0        0        0      603 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/config.py
--rw-r--r--   0        0        0       28 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/dagster/Makefile
--rw-r--r--   0        0        0        0 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/dagster/__init__.py
--rw-r--r--   0        0        0      933 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/database/README.md
--rw-r--r--   0        0        0        0 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/database/__init__.py
--rw-r--r--   0        0        0     6142 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/database/db_upload.py
--rw-r--r--   0        0        0    16141 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/database/models.py
--rw-r--r--   0        0        0      571 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/__init__.py
--rw-r--r--   0        0        0     2569 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/doping.py
--rw-r--r--   0        0        0    11898 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/get_simulation.py
--rw-r--r--   0        0        0    28255 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19679 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/get_solver.py
--rw-r--r--   0        0        0     1598 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/devsim/test_devsim.py
--rw-r--r--   0        0        0      198 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/eme/__init__.py
--rw-r--r--   0        0        0      207 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/fem/__init__.py
--rw-r--r--   0        0        0      107 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/femwell/__init__.py
--rw-r--r--   0        0        0     8522 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/femwell/mode_solver.py
--rw-r--r--   0        0        0     7772 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/femwell/solve_thermal.py
--rw-r--r--   0        0        0     1414 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/femwell/test_mode_solver.py
--rw-r--r--   0        0        0     1906 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/__init__.py
--rw-r--r--   0        0        0     1311 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/async_utils.py
--rw-r--r--   0        0        0     3151 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_material.py
--rw-r--r--   0        0        0     6037 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6028 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    10937 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15892 2023-08-06 18:26:48.067156 gplugins-0.1.0/gplugins/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    18153 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12263 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11862 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      820 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6189 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    13921 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21199 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8081 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9528 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1168 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/__init__.py
--rw-r--r--   0        0        0     6640 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11103 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/mesh.py
--rw-r--r--   0        0        0    11769 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7714 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3619 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/refine.py
--rw-r--r--   0        0        0    10756 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     1997 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14029 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7281 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0     9109 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0      220 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/gtidy3d/__init__.py
--rw-r--r--   0        0        0      536 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/__init__.py
--rw-r--r--   0        0        0    16025 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/interconnect.py
--rw-r--r--   0        0        0     4229 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/settings.py
--rw-r--r--   0        0        0     2353 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/tests/test_lumerical_read_sparameters.py
--rw-r--r--   0        0        0    19821 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1459 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0       67 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/meow/__init__.py
--rw-r--r--   0        0        0    16461 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/meow/meow_eme.py
--rw-r--r--   0        0        0     2301 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/meow/test_meow_simulation.py
--rw-r--r--   0        0        0      854 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/__init__.py
--rw-r--r--   0        0        0     1580 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/coupler.py
--rw-r--r--   0        0        0     4153 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2734 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8811 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_modes.py
--rwxr-xr-x   0        0        0     6968 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4445 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2715 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     7088 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4410 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5377 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     7965 2023-08-06 18:26:48.071156 gplugins-0.1.0/gplugins/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2443 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/overlap.py
--rw-r--r--   0        0        0      405 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0       83 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_dw_dh/test_dw_dh.obtained.csv
--rw-r--r--   0        0        0      548 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1124 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      636 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      341 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0      112 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.obtained.csv
--rw-r--r--   0        0        0    15422 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/types.py
--rw-r--r--   0        0        0     1140 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/modes/waveguide.py
--rw-r--r--   0        0        0      132 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/path_length_analysis/__init__.py
--rw-r--r--   0        0        0    19221 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/path_length_analysis/path_length_analysis.py
--rw-r--r--   0        0        0     5948 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/path_length_analysis/test_pathlength_extraction.py
--rw-r--r--   0        0        0     2013 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3009 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0        0 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/__init__.py
--rw-r--r--   0        0        0     4623 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/diffusion.py
--rw-r--r--   0        0        0     5318 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/implant_tables.py
--rw-r--r--   0        0        0     6879 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      165 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/__init__.py
--rw-r--r--   0        0        0    14710 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/build_model.py
--rw-r--r--   0        0        0        0 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/integrations/__init__.py
--rw-r--r--   0        0        0     7415 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/integrations/femwell_waveguide_model.py
--rw-r--r--   0        0        0     6720 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/integrations/meep_FDTD_model.py
--rw-r--r--   0        0        0     4492 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/integrations/meow_eme_model.py
--rw-r--r--   0        0        0     1546 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/interpolators.py
--rw-r--r--   0        0        0     5613 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/mlp.py
--rw-r--r--   0        0        0     7345 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/models.py
--rw-r--r--   0        0        0    13837 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/parameter.py
--rwxr-xr-x   0        0        0     2222 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/plot_model.py
--rw-r--r--   0        0        0     6672 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/read.py
--rw-r--r--   0        0        0     1349 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2255 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0       76 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.obtained.yml
--rw-r--r--   0        0        0       76 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.yml
--rw-r--r--   0        0        0     1393 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/sax/tests/test_parameters.py
--rw-r--r--   0        0        0      102 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/schematic_editor/__init__.py
--rw-r--r--   0        0        0    16197 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/schematic_editor/circuitviz.py
--rw-r--r--   0        0        0    17770 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/schematic_editor/schematic_editor.py
--rw-r--r--   0        0        0     1541 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/__init__.py
--rw-r--r--   0        0        0     4448 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/get_results.py
--rw-r--r--   0        0        0    19950 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/get_simulation.py
--rw-r--r--   0        0        0    21096 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     3263 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/materials.py
--rw-r--r--   0        0        0    37811 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/modes.py
--rw-r--r--   0        0        0     1943 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_materials.py
--rw-r--r--   0        0        0      730 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      260 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_modes/test_sweep_width.obtained.csv
--rw-r--r--   0        0        0      700 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_plot_simulation.py
--rw-r--r--   0        0        0      936 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py
--rw-r--r--   0        0        0      852 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/test_results.py
--rw-r--r--   0        0        0     9326 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml
--rw-r--r--   0        0        0     1562 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py
--rw-r--r--   0        0        0     1709 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py
--rw-r--r--   0        0        0     1891 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1192 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/utils.py
--rw-r--r--   0        0        0    11050 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/write_sparameters.py
--rw-r--r--   0        0        0     8567 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/tidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0        0 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/__init__.py
--rw-r--r--   0        0        0     4262 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/add_simulation_markers.py
--rw-r--r--   0        0        0     3276 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/convert_sparameters.py
--rw-r--r--   0        0        0      251 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/disable_print.py
--rw-r--r--   0        0        0     3407 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/get_effective_indices.py
--rw-r--r--   0        0        0     2893 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/get_sparameters_path.py
--rw-r--r--   0        0        0     5951 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/plot.py
--rw-r--r--   0        0        0     2439 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/plot_csv.py
--rw-r--r--   0        0        0      613 2023-08-06 18:26:48.075157 gplugins-0.1.0/gplugins/utils/port_symmetries.py
--rw-r--r--   0        0        0       32 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/Makefile
--rw-r--r--   0        0        0       23 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/__init__.py
--rw-r--r--   0        0        0      212 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/C.gds
--rw-r--r--   0        0        0      220 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/C_width20.gds
--rw-r--r--   0        0        0      218 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/C_width5.gds
--rw-r--r--   0        0        0    14536 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_rx_dual_pol.gds
--rw-r--r--   0        0        0    13550 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol.gds
--rw-r--r--   0        0        0    13564 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds
--rw-r--r--   0        0        0    13564 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds
--rw-r--r--   0        0        0    10292 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/coh_tx_dual_pol.gds
--rw-r--r--   0        0        0     1498 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/crossing_arm.gds
--rw-r--r--   0        0        0     7406 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/dbr_cavity.gds
--rw-r--r--   0        0        0      440 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/die_bbox_frame.gds
--rw-r--r--   0        0        0    27548 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/loss_deembedding_ch14_23.gds
--rw-r--r--   0        0        0      872 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/pad_array_add_fiducials.gds
--rw-r--r--   0        0        0    39252 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds
--rw-r--r--   0        0        0      182 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/gds_files/wg.gds
--rw-r--r--   0        0        0     8606 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/main.py
--rw-r--r--   0        0        0     1942 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/middleware.py
--rwxr-xr-x   0        0        0     7445 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/server.py
--rwxr-xr-x   0        0        0      636 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/server_jupyter.py
--rw-r--r--   0        0        0     1299 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/static/client.css
--rw-r--r--   0        0        0     9598 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/static/client.js
--rw-r--r--   0        0        0      840 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/client.html.j2
--rw-r--r--   0        0        0      481 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/file_browser.html.j2
--rw-r--r--   0        0        0     1999 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/filewatcher.html.j2
--rw-r--r--   0        0        0      236 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/footer.html.j2
--rw-r--r--   0        0        0      242 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/gds_history.html.j2
--rw-r--r--   0        0        0      578 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/header.html.j2
--rw-r--r--   0        0        0      376 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/index.html.j2
--rw-r--r--   0        0        0      995 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/navbar.html.j2
--rw-r--r--   0        0        0      272 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/pdk.html.j2
--rw-r--r--   0        0        0     1871 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/web/templates/viewer.html.j2
--rw-r--r--   0        0        0       87 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/widget/__init__.py
--rw-r--r--   0        0        0    14936 2023-08-06 18:26:48.079156 gplugins-0.1.0/gplugins/widget/interactive.py
--rw-r--r--   0        0        0     3174 2023-08-06 18:26:48.079156 gplugins-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4987 1970-01-01 00:00:00.000000 gplugins-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-08-08 21:52:47.854784 gplugins-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2234 2023-08-08 21:52:47.854784 gplugins-0.1.1/README.md
+-rw-r--r--   0        0        0      244 2023-08-08 21:52:47.858785 gplugins-0.1.1/gplugins/__init__.py
+-rw-r--r--   0        0        0      603 2023-08-08 21:52:47.858785 gplugins-0.1.1/gplugins/config.py
+-rw-r--r--   0        0        0       28 2023-08-08 21:52:47.858785 gplugins-0.1.1/gplugins/dagster/Makefile
+-rw-r--r--   0        0        0        0 2023-08-08 21:52:47.858785 gplugins-0.1.1/gplugins/dagster/__init__.py
+-rw-r--r--   0        0        0      933 2023-08-08 21:52:47.858785 gplugins-0.1.1/gplugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/database/README.md
+-rw-r--r--   0        0        0        0 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/database/__init__.py
+-rw-r--r--   0        0        0     6142 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/database/db_upload.py
+-rw-r--r--   0        0        0    16141 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/database/models.py
+-rw-r--r--   0        0        0      571 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/devsim/__init__.py
+-rw-r--r--   0        0        0     2569 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/devsim/doping.py
+-rw-r--r--   0        0        0    11898 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/devsim/get_simulation.py
+-rw-r--r--   0        0        0    28255 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19679 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/devsim/get_solver.py
+-rw-r--r--   0        0        0     1598 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/devsim/test_devsim.py
+-rw-r--r--   0        0        0      198 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/eme/__init__.py
+-rw-r--r--   0        0        0      207 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/fem/__init__.py
+-rw-r--r--   0        0        0      107 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/femwell/__init__.py
+-rw-r--r--   0        0        0     8522 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/femwell/mode_solver.py
+-rw-r--r--   0        0        0     7772 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/femwell/solve_thermal.py
+-rw-r--r--   0        0        0     1414 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/femwell/test_mode_solver.py
+-rw-r--r--   0        0        0     1906 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/__init__.py
+-rw-r--r--   0        0        0     1311 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/async_utils.py
+-rw-r--r--   0        0        0     3151 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/get_material.py
+-rw-r--r--   0        0        0     6037 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6028 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    10937 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15892 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    18153 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12263 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11862 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      820 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6189 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    13921 2023-08-08 21:52:47.862785 gplugins-0.1.1/gplugins/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21199 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8081 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9528 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1168 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/__init__.py
+-rw-r--r--   0        0        0     6640 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11103 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/mesh.py
+-rw-r--r--   0        0        0    11769 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7714 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3619 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/refine.py
+-rw-r--r--   0        0        0    10756 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     1997 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14029 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7281 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0     9109 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0      220 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/gtidy3d/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/klayout/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/klayout/dataprep/__init__.py
+-rw-r--r--   0        0        0     5906 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/klayout/dataprep/regions.py
+-rw-r--r--   0        0        0     2386 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/klayout/tests/test_dataprep_regions.py
+-rw-r--r--   0        0        0      536 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/lumerical/__init__.py
+-rw-r--r--   0        0        0    16025 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4229 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/lumerical/settings.py
+-rw-r--r--   0        0        0     2353 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/lumerical/tests/test_lumerical_read_sparameters.py
+-rw-r--r--   0        0        0    19821 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1459 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0       67 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/meow/__init__.py
+-rw-r--r--   0        0        0    16461 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/meow/meow_eme.py
+-rw-r--r--   0        0        0     2301 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/meow/test_meow_simulation.py
+-rw-r--r--   0        0        0      854 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/__init__.py
+-rw-r--r--   0        0        0     1580 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/coupler.py
+-rw-r--r--   0        0        0     4153 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2734 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8811 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/find_modes.py
+-rwxr-xr-x   0        0        0     6968 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4445 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2715 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     7088 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4410 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5377 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     7965 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2443 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/overlap.py
+-rw-r--r--   0        0        0      405 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0       83 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_dw_dh/test_dw_dh.obtained.csv
+-rw-r--r--   0        0        0      548 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1124 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      636 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      341 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0      112 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/tests/test_neff_vs_width/test_neff_vs_width.obtained.csv
+-rw-r--r--   0        0        0    15422 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/types.py
+-rw-r--r--   0        0        0     1140 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/modes/waveguide.py
+-rw-r--r--   0        0        0      132 2023-08-08 21:52:47.866785 gplugins-0.1.1/gplugins/path_length_analysis/__init__.py
+-rw-r--r--   0        0        0    19221 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/path_length_analysis/path_length_analysis.py
+-rw-r--r--   0        0        0     5948 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/path_length_analysis/test_pathlength_extraction.py
+-rw-r--r--   0        0        0     2013 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3009 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/__init__.py
+-rw-r--r--   0        0        0     4623 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/diffusion.py
+-rw-r--r--   0        0        0     5318 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/implant_tables.py
+-rw-r--r--   0        0        0     6879 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      165 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/__init__.py
+-rw-r--r--   0        0        0    14710 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/build_model.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/integrations/__init__.py
+-rw-r--r--   0        0        0     7415 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/integrations/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     6720 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/integrations/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4492 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/integrations/meow_eme_model.py
+-rw-r--r--   0        0        0     1546 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/interpolators.py
+-rw-r--r--   0        0        0     5613 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/mlp.py
+-rw-r--r--   0        0        0     7345 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/models.py
+-rw-r--r--   0        0        0    13837 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/parameter.py
+-rwxr-xr-x   0        0        0     2222 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/plot_model.py
+-rw-r--r--   0        0        0     6672 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/read.py
+-rw-r--r--   0        0        0     1349 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2255 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0       76 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.obtained.yml
+-rw-r--r--   0        0        0       76 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/tests/test_mzi_lattice/test_mzi_lattice.yml
+-rw-r--r--   0        0        0     1393 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0      102 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/schematic_editor/__init__.py
+-rw-r--r--   0        0        0    16197 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/schematic_editor/circuitviz.py
+-rw-r--r--   0        0        0    17770 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/schematic_editor/schematic_editor.py
+-rw-r--r--   0        0        0     1541 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/__init__.py
+-rw-r--r--   0        0        0     4448 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/get_results.py
+-rw-r--r--   0        0        0    19916 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21096 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     3263 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/materials.py
+-rw-r--r--   0        0        0    38727 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/modes.py
+-rw-r--r--   0        0        0     1924 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/test_materials.py
+-rw-r--r--   0        0        0      730 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      260 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/test_modes/test_sweep_width.obtained.csv
+-rw-r--r--   0        0        0      700 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/test_plot_simulation.py
+-rw-r--r--   0        0        0      936 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py
+-rw-r--r--   0        0        0      852 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     9326 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml
+-rw-r--r--   0        0        0     1562 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py
+-rw-r--r--   0        0        0     1629 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters.py
+-rw-r--r--   0        0        0     1891 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1192 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/utils.py
+-rw-r--r--   0        0        0    11050 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     8567 2023-08-08 21:52:47.870785 gplugins-0.1.1/gplugins/tidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0        0 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/__init__.py
+-rw-r--r--   0        0        0     4262 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/add_simulation_markers.py
+-rw-r--r--   0        0        0     3276 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/convert_sparameters.py
+-rw-r--r--   0        0        0      251 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/disable_print.py
+-rw-r--r--   0        0        0     3407 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/get_effective_indices.py
+-rw-r--r--   0        0        0     2893 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/get_sparameters_path.py
+-rw-r--r--   0        0        0     5951 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/plot.py
+-rw-r--r--   0        0        0     2439 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/plot_csv.py
+-rw-r--r--   0        0        0      613 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/utils/port_symmetries.py
+-rw-r--r--   0        0        0       32 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/Makefile
+-rw-r--r--   0        0        0       23 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/__init__.py
+-rw-r--r--   0        0        0      212 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/C.gds
+-rw-r--r--   0        0        0      220 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/C_width20.gds
+-rw-r--r--   0        0        0      218 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/C_width5.gds
+-rw-r--r--   0        0        0    14536 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/coh_rx_dual_pol.gds
+-rw-r--r--   0        0        0    13550 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/coh_rx_single_pol.gds
+-rw-r--r--   0        0        0    13564 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds
+-rw-r--r--   0        0        0    13564 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds
+-rw-r--r--   0        0        0    10292 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/coh_tx_dual_pol.gds
+-rw-r--r--   0        0        0     1498 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/crossing_arm.gds
+-rw-r--r--   0        0        0     7406 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/dbr_cavity.gds
+-rw-r--r--   0        0        0      440 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/die_bbox_frame.gds
+-rw-r--r--   0        0        0    27548 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/loss_deembedding_ch14_23.gds
+-rw-r--r--   0        0        0      872 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/pad_array_add_fiducials.gds
+-rw-r--r--   0        0        0    39252 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds
+-rw-r--r--   0        0        0      182 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/gds_files/wg.gds
+-rw-r--r--   0        0        0     8606 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/main.py
+-rw-r--r--   0        0        0     1942 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/middleware.py
+-rwxr-xr-x   0        0        0     7445 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/server.py
+-rwxr-xr-x   0        0        0      636 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/server_jupyter.py
+-rw-r--r--   0        0        0     1299 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/static/client.css
+-rw-r--r--   0        0        0     9598 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/static/client.js
+-rw-r--r--   0        0        0      840 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/client.html.j2
+-rw-r--r--   0        0        0      481 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/file_browser.html.j2
+-rw-r--r--   0        0        0     1999 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/filewatcher.html.j2
+-rw-r--r--   0        0        0      236 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/footer.html.j2
+-rw-r--r--   0        0        0      242 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/gds_history.html.j2
+-rw-r--r--   0        0        0      578 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/header.html.j2
+-rw-r--r--   0        0        0      376 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/index.html.j2
+-rw-r--r--   0        0        0      995 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/navbar.html.j2
+-rw-r--r--   0        0        0      272 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/pdk.html.j2
+-rw-r--r--   0        0        0     1871 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/web/templates/viewer.html.j2
+-rw-r--r--   0        0        0       87 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/widget/__init__.py
+-rw-r--r--   0        0        0    14936 2023-08-08 21:52:47.874786 gplugins-0.1.1/gplugins/widget/interactive.py
+-rw-r--r--   0        0        0     3217 2023-08-08 21:52:47.874786 gplugins-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5071 1970-01-01 00:00:00.000000 gplugins-0.1.1/PKG-INFO
```

### Comparing `gplugins-0.1.0/LICENSE` & `gplugins-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/README.md` & `gplugins-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gplugins 0.1.0
+# gplugins 0.1.1
 
 [![docs](https://github.com/gdsfactory/gplugins/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gplugins/)
 [![PyPI](https://img.shields.io/pypi/v/gplugins)](https://pypi.org/project/gplugins/)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gplugins.svg)](https://pypi.python.org/pypi/gplugins)
 [![MIT](https://img.shields.io/github/license/gdsfactory/gplugins)](https://choosealicense.com/licenses/mit/)
 [![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gplugins)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gplugins)
 
@@ -11,15 +11,15 @@
 - `database` for simulation and measurement database and dagster for data pipelines.
 - `devsim` TCAD device simulator.
 - `meow` Eigen Mode Expansion (EME).
 - `femwell` Finite Element Method Solver (heaters, modes, TCAD, RF waveguides).
 - `gmsh` mesh structures.
 - `tidy3d` Finite Difference Time Domain (FDTD) simulations on the cloud using GPU.
 - `lumerical` For Ansys FDTD and Circuit interconnect.
-- `kfactory` for fill, dataprep and testing.
+- `klayout` for fill, dataprep and testing.
 - `ray` for distributed computing and optimization.
 - `sax` S-parameter circuit solver.
 - `schematic`: for bokeh schematic editor and `path_length_analysis`
 - `meep` for FDTD.
 - `mpb` for MPB mode solver.
 - `web`: for gdsfactory webapp
```

### Comparing `gplugins-0.1.0/gplugins/config.py` & `gplugins-0.1.1/gplugins/config.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/dagster/workflow.py` & `gplugins-0.1.1/gplugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/database/README.md` & `gplugins-0.1.1/gplugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/database/db_upload.py` & `gplugins-0.1.1/gplugins/database/db_upload.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/database/models.py` & `gplugins-0.1.1/gplugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/devsim/__init__.py` & `gplugins-0.1.1/gplugins/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/devsim/doping.py` & `gplugins-0.1.1/gplugins/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/devsim/get_simulation.py` & `gplugins-0.1.1/gplugins/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/devsim/get_simulation_xsection.py` & `gplugins-0.1.1/gplugins/devsim/get_simulation_xsection.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/devsim/get_solver.py` & `gplugins-0.1.1/gplugins/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/devsim/test_devsim.py` & `gplugins-0.1.1/gplugins/devsim/test_devsim.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/femwell/mode_solver.py` & `gplugins-0.1.1/gplugins/femwell/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/femwell/solve_thermal.py` & `gplugins-0.1.1/gplugins/femwell/solve_thermal.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/femwell/test_mode_solver.py` & `gplugins-0.1.1/gplugins/femwell/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/__init__.py` & `gplugins-0.1.1/gplugins/gmeep/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/async_utils.py` & `gplugins-0.1.1/gplugins/gmeep/async_utils.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/get_material.py` & `gplugins-0.1.1/gplugins/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/get_meep_geometry.py` & `gplugins-0.1.1/gplugins/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/get_port_eigenmode.py` & `gplugins-0.1.1/gplugins/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/get_simulation.py` & `gplugins-0.1.1/gplugins/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/get_simulation_grating_farfield.py` & `gplugins-0.1.1/gplugins/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/get_simulation_grating_fiber.py` & `gplugins-0.1.1/gplugins/gmeep/get_simulation_grating_fiber.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/meep_adjoint_optimization.py` & `gplugins-0.1.1/gplugins/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_eigenmode.py` & `gplugins-0.1.1/gplugins/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_materials.py` & `gplugins-0.1.1/gplugins/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gplugins-0.1.1/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gplugins-0.1.1/gplugins/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep.py` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gplugins-0.1.1/gplugins/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/write_sparameters_grating.py` & `gplugins-0.1.1/gplugins/gmeep/write_sparameters_grating.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep.py` & `gplugins-0.1.1/gplugins/gmeep/write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep_batch.py` & `gplugins-0.1.1/gplugins/gmeep/write_sparameters_meep_batch.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmeep/write_sparameters_meep_mpi.py` & `gplugins-0.1.1/gplugins/gmeep/write_sparameters_meep_mpi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/__init__.py` & `gplugins-0.1.1/gplugins/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/break_geometry.py` & `gplugins-0.1.1/gplugins/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/mesh.py` & `gplugins-0.1.1/gplugins/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/meshtracker.py` & `gplugins-0.1.1/gplugins/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/parse_component.py` & `gplugins-0.1.1/gplugins/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/parse_gds.py` & `gplugins-0.1.1/gplugins/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/parse_layerstack.py` & `gplugins-0.1.1/gplugins/gmsh/parse_layerstack.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/refine.py` & `gplugins-0.1.1/gplugins/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/scratch/mesh3D.py` & `gplugins-0.1.1/gplugins/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/tests/test_meshing.py` & `gplugins-0.1.1/gplugins/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/uz_xsection_mesh.py` & `gplugins-0.1.1/gplugins/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/xy_xsection_mesh.py` & `gplugins-0.1.1/gplugins/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/gmsh/xyz_mesh.py` & `gplugins-0.1.1/gplugins/gmsh/xyz_mesh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/lumerical/__init__.py` & `gplugins-0.1.1/gplugins/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/lumerical/interconnect.py` & `gplugins-0.1.1/gplugins/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/lumerical/read.py` & `gplugins-0.1.1/gplugins/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/lumerical/settings.py` & `gplugins-0.1.1/gplugins/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/lumerical/tests/test_lumerical_read_sparameters.py` & `gplugins-0.1.1/gplugins/lumerical/tests/test_lumerical_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/lumerical/write_sparameters_lumerical.py` & `gplugins-0.1.1/gplugins/lumerical/write_sparameters_lumerical.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/lumerical/write_sparameters_lumerical_components.py` & `gplugins-0.1.1/gplugins/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/meow/meow_eme.py` & `gplugins-0.1.1/gplugins/meow/meow_eme.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/meow/test_meow_simulation.py` & `gplugins-0.1.1/gplugins/meow/test_meow_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/__init__.py` & `gplugins-0.1.1/gplugins/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/coupler.py` & `gplugins-0.1.1/gplugins/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/find_coupling_vs_gap.py` & `gplugins-0.1.1/gplugins/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/find_mode_dispersion.py` & `gplugins-0.1.1/gplugins/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/find_modes.py` & `gplugins-0.1.1/gplugins/modes/find_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/find_modes_cross_section.py` & `gplugins-0.1.1/gplugins/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/find_neff_ng_dw_dh.py` & `gplugins-0.1.1/gplugins/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/find_neff_vs_width.py` & `gplugins-0.1.1/gplugins/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/get_mode_solver_coupler.py` & `gplugins-0.1.1/gplugins/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/get_mode_solver_cross_section.py` & `gplugins-0.1.1/gplugins/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/get_mode_solver_rib.py` & `gplugins-0.1.1/gplugins/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_nitride.csv` & `gplugins-0.1.1/gplugins/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_rib.csv` & `gplugins-0.1.1/gplugins/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/modes/neff_vs_width_strip.csv` & `gplugins-0.1.1/gplugins/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/neff_convergence_test.py` & `gplugins-0.1.1/gplugins/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/overlap.py` & `gplugins-0.1.1/gplugins/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gplugins-0.1.1/gplugins/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/tests/test_find_modes.py` & `gplugins-0.1.1/gplugins/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/tests/test_find_modes_dispersion.py` & `gplugins-0.1.1/gplugins/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/types.py` & `gplugins-0.1.1/gplugins/modes/types.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/modes/waveguide.py` & `gplugins-0.1.1/gplugins/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/path_length_analysis/path_length_analysis.py` & `gplugins-0.1.1/gplugins/path_length_analysis/path_length_analysis.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/path_length_analysis/test_pathlength_extraction.py` & `gplugins-0.1.1/gplugins/path_length_analysis/test_pathlength_extraction.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/photonic_circuit_models/__init__.py` & `gplugins-0.1.1/gplugins/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/photonic_circuit_models/coupler.py` & `gplugins-0.1.1/gplugins/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/photonic_circuit_models/mzi.py` & `gplugins-0.1.1/gplugins/photonic_circuit_models/mzi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/photonic_circuit_models/ring.py` & `gplugins-0.1.1/gplugins/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/process/diffusion.py` & `gplugins-0.1.1/gplugins/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/process/implant_tables.py` & `gplugins-0.1.1/gplugins/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/process/pysrim.py` & `gplugins-0.1.1/gplugins/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/process/silicon.py` & `gplugins-0.1.1/gplugins/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/process/skew/antimony_si_skew.csv` & `gplugins-0.1.1/gplugins/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/process/skew/arsenic_si_skew.csv` & `gplugins-0.1.1/gplugins/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/process/skew/boron_si_skew.csv` & `gplugins-0.1.1/gplugins/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/process/skew/phosphorus_si_skew.csv` & `gplugins-0.1.1/gplugins/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/build_model.py` & `gplugins-0.1.1/gplugins/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/integrations/femwell_waveguide_model.py` & `gplugins-0.1.1/gplugins/sax/integrations/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/integrations/meep_FDTD_model.py` & `gplugins-0.1.1/gplugins/sax/integrations/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/integrations/meow_eme_model.py` & `gplugins-0.1.1/gplugins/sax/integrations/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/interpolators.py` & `gplugins-0.1.1/gplugins/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/mlp.py` & `gplugins-0.1.1/gplugins/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/models.py` & `gplugins-0.1.1/gplugins/sax/models.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/parameter.py` & `gplugins-0.1.1/gplugins/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/plot_model.py` & `gplugins-0.1.1/gplugins/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/read.py` & `gplugins-0.1.1/gplugins/sax/read.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/tests/test_mzi.py` & `gplugins-0.1.1/gplugins/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/tests/test_mzi_lattice.py` & `gplugins-0.1.1/gplugins/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/sax/tests/test_parameters.py` & `gplugins-0.1.1/gplugins/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/schematic_editor/circuitviz.py` & `gplugins-0.1.1/gplugins/schematic_editor/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/schematic_editor/schematic_editor.py` & `gplugins-0.1.1/gplugins/schematic_editor/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/__init__.py` & `gplugins-0.1.1/gplugins/tidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/get_results.py` & `gplugins-0.1.1/gplugins/tidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/get_simulation.py` & `gplugins-0.1.1/gplugins/tidy3d/get_simulation.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     num_modes: int = 2,
     run_time_ps: float = 10.0,
     material_name_to_tidy3d: None | dict[str, str] = None,
     is_3d: bool = True,
     with_all_monitors: bool = False,
     boundary_spec: td.BoundarySpec | None = None,
     grid_spec: td.GridSpec | None = None,
-    sidewall_angle_deg: float = 0,
+    sidewall_angle_deg: float | None = None,
     dilation: float = 0.0,
     **kwargs,
 ) -> td.Simulation:
     r"""Returns tidy3d Simulation object from a gdsfactory Component.
 
     based on GDS example
     https://simulation.cloud/docs/html/examples/ParameterScan.html
@@ -139,17 +139,17 @@
         boundary_spec: Specification of boundary conditions along each dimension.
             Defaults to td.BoundarySpec.all_sides(boundary=td.PML())
 
         dilation: float = 0.0
             Dilation of the polygon in the base by shifting each edge along its
             normal outwards direction by a distance;
             a negative value corresponds to erosion.
-        sidewall_angle_deg : float = 0
+        sidewall_angle_deg : float | None = None
             Angle of the sidewall.
-            ``sidewall_angle=0`` (default) specifies vertical wall,
+            ``sidewall_angle=None`` (default) pulls the sidewall angle from the PDK,
             while ``0<sidewall_angle_deg<90`` for the base to be larger than the top.
 
     keyword Args:
         symmetry: Define Symmetries.
             Tuple of integers defining reflection symmetry across a plane
             bisecting the simulation domain normal to the x-, y-, and z-axis
             at the simulation center of each axis, respectively.
@@ -189,25 +189,25 @@
     layer_stack = layer_stack or get_layer_stack()
     if is_3d:
         boundary_spec = boundary_spec or td.BoundarySpec.all_sides(boundary=td.PML())
 
     else:
         boundary_spec = boundary_spec or td.BoundarySpec(
             x=td.Boundary.pml(),
-            y=td.Boundary.periodic(),
-            z=td.Boundary.pml(),
+            y=td.Boundary.pml(),
+            z=td.Boundary.periodic(),
         )
 
     wavelength = (wavelength_start + wavelength_stop) / 2
     grid_spec = grid_spec or td.GridSpec.auto(wavelength=wavelength)
 
     layer_to_thickness = layer_stack.get_layer_to_thickness()
     layer_to_material = layer_stack.get_layer_to_material()
     layer_to_zmin = layer_stack.get_layer_to_zmin()
-    # layer_to_sidewall_angle = layer_stack.get_layer_to_sidewall_angle()
+    layer_to_sidewall_angle = layer_stack.get_layer_to_sidewall_angle()
 
     if port_source_name not in component.ports:
         warnings.warn(
             f"port_source_name={port_source_name!r} not in {list(component.ports.keys())}"
         )
         port_source = component.get_ports_list(port_type="optical")[0]
         port_source_name = port_source.name
@@ -292,21 +292,27 @@
                 material_index = (
                     material_name(wavelength)
                     if callable(material_name)
                     else material_name
                 )
                 medium = get_medium(material_index)
 
+            sidewall_angle_deg = (
+                layer_to_sidewall_angle[layer]
+                if sidewall_angle_deg is None
+                else sidewall_angle_deg
+            )
+
             polygons = td.PolySlab.from_gds(
                 gds_cell=component_extended._cell,
                 gds_layer=layer[0],
                 gds_dtype=layer[1],
                 axis=2,
                 slab_bounds=(zmin, zmax),
-                sidewall_angle=np.deg2rad(sidewall_angle_deg),
+                sidewall_angle=np.deg2rad(sidewall_angle_deg) if is_3d else 0,
                 dilation=dilation,
             )
 
             for polygon in polygons:
                 geometry = td.Structure(geometry=polygon, medium=medium)
                 structures.append(geometry)
 
@@ -405,26 +411,19 @@
                     "Ey", "abs", f=freq0, mode_index=mode_ind, ax=axs[mode_ind, 0]
                 )
                 ms.plot_field(
                     "Ez", "abs", f=freq0, mode_index=mode_ind, ax=axs[mode_ind, 1]
                 )
         else:
             fig, axs = plt.subplots(num_modes, 3, figsize=(12, 12))
+            axs = np.atleast_2d(axs)
             for mode_ind in range(num_modes):
-                ax1 = axs[mode_ind, 0]
-                ax2 = axs[mode_ind, 1]
-                ax3 = axs[mode_ind, 2]
-
-                abs(modes.fields.Ex.sel(mode_index=mode_ind).abs).plot(ax=ax1)
-                abs(modes.fields.Ey.sel(mode_index=mode_ind).abs).plot(ax=ax2)
-                abs(modes.fields.Ez.sel(mode_index=mode_ind).abs).plot(ax=ax3)
-
-                ax1.set_title(f"|Ex|: mode_index={mode_ind}")
-                ax2.set_title(f"|Ey|: mode_index={mode_ind}")
-                ax3.set_title(f"|Ez|: mode_index={mode_ind}")
+                axs[mode_ind, 0].plot(modes.Ex.sel(mode_index=mode_ind).y.abs)
+                axs[mode_ind, 1].plot(modes.Ey.sel(mode_index=mode_ind).y.abs)
+                axs[mode_ind, 2].plot(modes.Ez.sel(mode_index=mode_ind).y.abs)
 
         plt.show()
     return sim
 
 
 def plot_simulation_yz(
     sim: td.Simulation,
```

### Comparing `gplugins-0.1.0/gplugins/tidy3d/get_simulation_grating_coupler.py` & `gplugins-0.1.1/gplugins/tidy3d/get_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/materials.py` & `gplugins-0.1.1/gplugins/tidy3d/materials.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/modes.py` & `gplugins-0.1.1/gplugins/tidy3d/modes.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,25 +19,42 @@
 
 import numpy as np
 import pydantic
 import tidy3d as td
 import xarray
 from gdsfactory.config import logger
 from gdsfactory.pdk import get_modes_path
-from gdsfactory.serialization import clean_value_name
 from gdsfactory.typings import PathType
+from pydantic import BaseModel
 from tidy3d.plugins import waveguide
 from tqdm.auto import tqdm
 
 from gplugins.tidy3d.materials import MaterialSpecTidy3d, get_medium
 
 Precision = Literal["single", "double"]
 nm = 1e-3
 
 
+def custom_serializer(data: str | float | BaseModel) -> str:
+    # If data is a string, just return it.
+    if isinstance(data, str | None | np.ndarray):
+        return data
+
+    # If data is a float, convert it to a string.
+    if isinstance(data, float | int):
+        return str(data)
+
+    # If data is an instance of Pydantic's BaseModel, serialize it to JSON.
+    if isinstance(data, BaseModel):
+        return data.json()
+
+    # For all other data types, raise an exception.
+    raise ValueError(f"Unsupported data type: {type(data)}")
+
+
 class Waveguide(pydantic.BaseModel):
     """Waveguide Model.
 
     All dimensions must be specified in μm (1e-6 m).
 
     Parameters:
         wavelength: wavelength in free space.
@@ -151,18 +168,17 @@
         """Cache file path"""
         if not self.cache:
             return None
         cache_path = pathlib.Path(self.cache_path)
         cache_path.mkdir(exist_ok=True, parents=True)
 
         settings = [
-            f"{setting}={clean_value_name(getattr(self, setting))}"
+            f"{setting}={custom_serializer(getattr(self, setting))}"
             for setting in sorted(self.__fields__.keys())
         ]
-
         named_args_string = "_".join(settings)
         h = hashlib.md5(named_args_string.encode()).hexdigest()[:16]
         return cache_path / f"{self.__class__.__name__}_{h}.npz"
 
     @property
     def waveguide(self):
         """Tidy3D waveguide used by this instance."""
@@ -243,19 +259,18 @@
         return self._waveguide
 
     @property
     def _data(self):
         """Mode data for this waveguide (cached if cache is enabled)."""
         if not hasattr(self, "_cached_data"):
             filepath = self.filepath
-            if filepath and filepath.exists():
-                if not self.overwrite:
-                    logger.info(f"load data from {filepath}.")
-                    self._cached_data = np.load(filepath)
-                    return self._cached_data
+            if filepath and filepath.exists() and not self.overwrite:
+                logger.info(f"load data from {filepath}.")
+                self._cached_data = np.load(filepath)
+                return self._cached_data
 
             wg = self.waveguide
 
             fields = wg.mode_solver.data._centered_fields
             self._cached_data = {
                 f + c: fields[f + c].squeeze(drop=True).values
                 for f in "EH"
@@ -369,29 +384,34 @@
         artist.axes.set_aspect("equal")
 
     def plot_field(
         self,
         field_name: str,
         value: str = "real",
         mode_index: int = 0,
-        wavelength: float = None,
+        wavelength: float | None = None,
         **kwargs,
     ) -> None:
         """Plot the selected field distribution from a waveguide mode.
 
         Parameters:
             field_name: one of 'Ex', 'Ey', 'Ez', 'Hx', 'Hy', 'Hz'.
             value: component of the field to plot. One of 'real',
                 'imag', 'abs', 'phase', 'dB'.
             mode_index: mode selection.
             wavelength: wavelength selection.
             kwargs: keyword arguments passed to xarray.DataArray.plot.
         """
         data = self._data[field_name]
 
+        if mode_index >= self.num_modes:
+            raise ValueError(
+                f"mode_index = {mode_index} must be less than num_modes {self.num_modes}"
+            )
+
         if self.num_modes > 1:
             data = data[..., mode_index]
         if self.wavelength.size > 1:
             i = (
                 np.argmin(np.abs(wavelength - self.wavelength))
                 if wavelength
                 else self.wavelength.size // 2
@@ -412,27 +432,34 @@
         else:
             raise ValueError(
                 "value must be one of 'real', 'imag', 'abs', 'phase', 'dB'"
             )
         data_array = xarray.DataArray(
             data.T, coords={"y": self._data["y"], "x": self._data["x"]}
         )
+
+        if value == "dB":
+            kwargs.update(vmin=-20)
+
         data_array.name = field_name
         artist = data_array.plot(**kwargs)
         artist.axes.set_aspect("equal")
 
     def _ipython_display_(self) -> None:
         """Show index in matplotlib for Jupyter Notebooks."""
         self.plot_index()
 
     def __repr__(self) -> str:
         """Show waveguide representation."""
         return (
             f"{self.__class__.__name__}("
-            + ", ".join(f"{k}={getattr(self, k)!r}" for k in self.__fields__.keys())
+            + ", ".join(
+                f"{k}={custom_serializer(getattr(self, k))!r}"
+                for k in self.__fields__.keys()
+            )
             + ")"
         )
 
     def __str__(self) -> str:
         """Show waveguide representation."""
         return self.__repr__()
 
@@ -985,15 +1012,18 @@
         slab_thickness=0.0,
         # core_material="si",
         core_material=td.material_library["cSi"]["Li1993_293K"],
         clad_material="sio2",
         core_thickness=220 * nm,
         num_modes=4,
     )
-    strip.plot_index()
+    # strip._data
+    # strip.filepath
+    # strip.plot_index()
+    strip.plot_field("Ex", mode_index=0, wavelength=1.55, value="dB")
     plt.show()
     # w = np.linspace(400 * nm, 1000 * nm, 7)
     # n_eff = sweep_n_eff(strip, core_width=w)
     # fraction_te = sweep_fraction_te(strip, core_width=w)
 
     # t = np.linspace(0.2, 0.25, 6)
     # w = np.linspace(0.4, 0.6, 5)
```

### Comparing `gplugins-0.1.0/gplugins/tidy3d/tests/test_materials.py` & `gplugins-0.1.1/gplugins/tidy3d/tests/test_materials.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,70 +19,71 @@
 
 def test_material_medium() -> None:
     strip = gt.modes.Waveguide(
         core_material=td.Medium(permittivity=(2.1) ** 2),
         clad_material=td.Medium(permittivity=(1.448) ** 2),
         **settings,
     )
-    strip.plot_index()
+    strip._data
 
 
 def test_material_float() -> None:
     strip = gt.modes.Waveguide(
         core_material=3.4,
         clad_material=1.4,
         **settings,
     )
-    strip.plot_index()
+    strip._data
 
 
 def test_material_string() -> None:
     strip = gt.modes.Waveguide(
         core_material="si",
         clad_material="sio2",
         **settings,
     )
-    strip.plot_index()
+    strip._data
 
 
 def test_material_validation_error() -> None:
     with pytest.raises(ValidationError):
         strip = gt.modes.Waveguide(
             core_material=td.material_library["cSi"],
             clad_material="sio2",
             **settings,
         )
-        strip.plot_index()
+        strip._data
 
 
 def test_material_library_many_variants() -> None:
     with pytest.raises(ValueError):
         strip = gt.modes.Waveguide(
             core_material="cSi",
             clad_material="sio2",
             **settings,
         )
-        strip.plot_index()
+        strip._data
 
 
 def test_material_library_single_variant() -> None:
     strip = gt.modes.Waveguide(
         core_material="SiO2",
         clad_material="sio2",
         **settings,
     )
-    strip.plot_index()
+    strip._data
 
 
 def test_material_library() -> None:
     strip = gt.modes.Waveguide(
         core_material=td.material_library["cSi"]["Li1993_293K"],
         clad_material="sio2",
         **settings,
     )
-    strip.plot_index()
+    strip._data
 
 
 if __name__ == "__main__":
+    pytest.main([__file__])
     # test_material_medium()
     # test_material_float()
-    test_material_library()
+    # test_material_library()
```

### Comparing `gplugins-0.1.0/gplugins/tidy3d/tests/test_modes.py` & `gplugins-0.1.1/gplugins/tidy3d/tests/test_modes.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/tests/test_plot_simulation.py` & `gplugins-0.1.1/gplugins/tidy3d/tests/test_plot_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py` & `gplugins-0.1.1/gplugins/tidy3d/tests/test_plot_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/tests/test_results.py` & `gplugins-0.1.1/gplugins/tidy3d/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml` & `gplugins-0.1.1/gplugins/tidy3d/tests/tests_sparameters/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py` & `gplugins-0.1.1/gplugins/tidy3d/tests/tests_sparameters/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py` & `gplugins-0.1.1/gplugins/tidy3d/tests/tests_sparameters/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/utils.py` & `gplugins-0.1.1/gplugins/tidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/write_sparameters.py` & `gplugins-0.1.1/gplugins/tidy3d/write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/tidy3d/write_sparameters_grating_coupler.py` & `gplugins-0.1.1/gplugins/tidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/utils/add_simulation_markers.py` & `gplugins-0.1.1/gplugins/utils/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/utils/convert_sparameters.py` & `gplugins-0.1.1/gplugins/utils/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/utils/get_effective_indices.py` & `gplugins-0.1.1/gplugins/utils/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/utils/get_sparameters_path.py` & `gplugins-0.1.1/gplugins/utils/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/utils/plot.py` & `gplugins-0.1.1/gplugins/utils/plot.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/utils/plot_csv.py` & `gplugins-0.1.1/gplugins/utils/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/utils/port_symmetries.py` & `gplugins-0.1.1/gplugins/utils/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/coh_rx_dual_pol.gds` & `gplugins-0.1.1/gplugins/web/gds_files/coh_rx_dual_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol.gds` & `gplugins-0.1.1/gplugins/web/gds_files/coh_rx_single_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds` & `gplugins-0.1.1/gplugins/web/gds_files/coh_rx_single_pol_pad_d_19b6c499.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds` & `gplugins-0.1.1/gplugins/web/gds_files/coh_rx_single_pol_pad_d_d4526895.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/coh_tx_dual_pol.gds` & `gplugins-0.1.1/gplugins/web/gds_files/coh_tx_dual_pol.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/crossing_arm.gds` & `gplugins-0.1.1/gplugins/web/gds_files/crossing_arm.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/dbr_cavity.gds` & `gplugins-0.1.1/gplugins/web/gds_files/dbr_cavity.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/loss_deembedding_ch14_23.gds` & `gplugins-0.1.1/gplugins/web/gds_files/loss_deembedding_ch14_23.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/pad_array_add_fiducials.gds` & `gplugins-0.1.1/gplugins/web/gds_files/pad_array_add_fiducials.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds` & `gplugins-0.1.1/gplugins/web/gds_files/spiral_inner_io_add_gra_f2760628.gds`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/main.py` & `gplugins-0.1.1/gplugins/web/main.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/middleware.py` & `gplugins-0.1.1/gplugins/web/middleware.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/server.py` & `gplugins-0.1.1/gplugins/web/server.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/server_jupyter.py` & `gplugins-0.1.1/gplugins/web/server_jupyter.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/static/client.css` & `gplugins-0.1.1/gplugins/web/static/client.css`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/static/client.js` & `gplugins-0.1.1/gplugins/web/static/client.js`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/templates/client.html.j2` & `gplugins-0.1.1/gplugins/web/templates/client.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/templates/filewatcher.html.j2` & `gplugins-0.1.1/gplugins/web/templates/filewatcher.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/templates/header.html.j2` & `gplugins-0.1.1/gplugins/web/templates/header.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/templates/navbar.html.j2` & `gplugins-0.1.1/gplugins/web/templates/navbar.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/web/templates/viewer.html.j2` & `gplugins-0.1.1/gplugins/web/templates/viewer.html.j2`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/gplugins/widget/interactive.py` & `gplugins-0.1.1/gplugins/widget/interactive.py`

 * *Files identical despite different names*

### Comparing `gplugins-0.1.0/pyproject.toml` & `gplugins-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ]
 description = "gdsfactory plugins"
 keywords = ["python"]
 license = {file = "LICENSE"}
 name = "gplugins"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "0.1.0"
+version = "0.1.1"
 
 [project.optional-dependencies]
 database = [
   "sqlalchemy",
   "sqlalchemy-utils",
   "dagster",
   "dagit",
@@ -65,15 +65,18 @@
   "h5py",
   "mapbox_earcut",
   "meshio",
   "pygmsh",
   "pyvista",
   "trimesh",
   "shapely",
-  "meshwell>=0.0.9,<0.1.0"
+  "meshwell>=0.0.9,<0.1.1"
+]
+klayout = [
+  "kfactory[git,ipy]==0.7.5"
 ]
 meow = [
   "meow-sim>=0.7.1,<0.8.0",
   "tidy3d>=2.3.3,<2.4.0"
 ]
 sax = [
   "sax>=0.8.8,<0.9.0",
```

### Comparing `gplugins-0.1.0/PKG-INFO` & `gplugins-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gplugins
-Version: 0.1.0
+Version: 0.1.1
 Summary: gdsfactory plugins
 Keywords: python
 Author-email: gdsfactory <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -39,15 +39,16 @@
 Requires-Dist: h5py ; extra == "gmsh"
 Requires-Dist: mapbox_earcut ; extra == "gmsh"
 Requires-Dist: meshio ; extra == "gmsh"
 Requires-Dist: pygmsh ; extra == "gmsh"
 Requires-Dist: pyvista ; extra == "gmsh"
 Requires-Dist: trimesh ; extra == "gmsh"
 Requires-Dist: shapely ; extra == "gmsh"
-Requires-Dist: meshwell>=0.0.9,<0.1.0 ; extra == "gmsh"
+Requires-Dist: meshwell>=0.0.9,<0.1.1 ; extra == "gmsh"
+Requires-Dist: kfactory[git,ipy]==0.7.5 ; extra == "klayout"
 Requires-Dist: meow-sim>=0.7.1,<0.8.0 ; extra == "meow"
 Requires-Dist: tidy3d>=2.3.3,<2.4.0 ; extra == "meow"
 Requires-Dist: sax>=0.8.8,<0.9.0 ; extra == "sax"
 Requires-Dist: jaxlib ; extra == "sax"
 Requires-Dist: jax ; extra == "sax"
 Requires-Dist: scikit-learn ; extra == "sax"
 Requires-Dist: bokeh ; extra == "schematic"
@@ -59,21 +60,22 @@
 Requires-Dist: uvicorn[standard] ; extra == "web"
 Provides-Extra: database
 Provides-Extra: dev
 Provides-Extra: devsim
 Provides-Extra: docs
 Provides-Extra: femwell
 Provides-Extra: gmsh
+Provides-Extra: klayout
 Provides-Extra: meow
 Provides-Extra: sax
 Provides-Extra: schematic
 Provides-Extra: tidy3d
 Provides-Extra: web
 
-# gplugins 0.1.0
+# gplugins 0.1.1
 
 [![docs](https://github.com/gdsfactory/gplugins/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gplugins/)
 [![PyPI](https://img.shields.io/pypi/v/gplugins)](https://pypi.org/project/gplugins/)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gplugins.svg)](https://pypi.python.org/pypi/gplugins)
 [![MIT](https://img.shields.io/github/license/gdsfactory/gplugins)](https://choosealicense.com/licenses/mit/)
 [![codecov](https://img.shields.io/codecov/c/github/gdsfactory/gplugins)](https://codecov.io/gh/gdsfactory/gdsfactory/tree/main/gplugins)
 
@@ -82,15 +84,15 @@
 - `database` for simulation and measurement database and dagster for data pipelines.
 - `devsim` TCAD device simulator.
 - `meow` Eigen Mode Expansion (EME).
 - `femwell` Finite Element Method Solver (heaters, modes, TCAD, RF waveguides).
 - `gmsh` mesh structures.
 - `tidy3d` Finite Difference Time Domain (FDTD) simulations on the cloud using GPU.
 - `lumerical` For Ansys FDTD and Circuit interconnect.
-- `kfactory` for fill, dataprep and testing.
+- `klayout` for fill, dataprep and testing.
 - `ray` for distributed computing and optimization.
 - `sax` S-parameter circuit solver.
 - `schematic`: for bokeh schematic editor and `path_length_analysis`
 - `meep` for FDTD.
 - `mpb` for MPB mode solver.
 - `web`: for gdsfactory webapp
```

