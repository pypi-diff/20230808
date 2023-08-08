# Comparing `tmp/gdsfactory-7.1.2.tar.gz` & `tmp/gdsfactory-7.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-7.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gdsfactory-7.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gdsfactory-7.1.2.tar` & `gdsfactory-7.1.3.tar`

### file list

```diff
@@ -1,477 +1,477 @@
--rw-r--r--   0        0        0     1072 2023-08-07 04:02:40.318502 gdsfactory-7.1.2/LICENSE
--rw-r--r--   0        0        0     7441 2023-08-07 04:02:40.318502 gdsfactory-7.1.2/README.md
--rw-r--r--   0        0        0     3417 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/__init__.py
--rw-r--r--   0        0        0     1870 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12537 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3682 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5016 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    16012 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14682 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2864 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2253 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1791 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1856 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/asserts.py
--rw-r--r--   0        0        0    14884 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/cell.py
--rw-r--r--   0        0        0     5620 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/cli.py
--rw-r--r--   0        0        0   102902 2023-08-07 04:02:40.326502 gdsfactory-7.1.2/gdsfactory/component.py
--rw-r--r--   0        0        0    24269 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    30803 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1179 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1105 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/L.py
--rw-r--r--   0        0        0    21495 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2599 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    13939 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3168 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2528 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4664 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4319 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1636 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     3048 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2614 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     8029 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2663 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3807 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5417 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5740 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2888 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1593 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1374 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1552 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5933 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8880 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5005 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6080 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2514 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9898 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0    11731 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/component_lattice_generic.py
--rw-r--r--   0        0        0     7130 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2128 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     4667 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler_bent.py
--rw-r--r--   0        0        0     3970 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     5829 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1816 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    13157 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-08-07 04:02:40.330502 gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5256 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6743 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3759 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2708 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4262 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2481 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3176 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3245 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4313 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1254 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3578 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2968 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2816 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     7984 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4121 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1188 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1756 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7046 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3225 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     2458 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4651 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7137 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7209 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4942 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4694 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1747 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9054 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1814 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4110 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4650 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3855 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1579 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8722 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3643 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1799 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1218 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1278 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     5005 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mmi.py
--rw-r--r--   0        0        0     3978 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2769 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3801 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3192 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4944 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3293 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7610 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2464 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5822 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12188 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4020 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1264 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6310 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3476 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6016 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6289 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3833 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1915 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3799 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1115 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1475 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2933 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1059 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/rectangular_ring.py
--rw-r--r--   0        0        0     1476 2023-08-07 04:02:40.334502 gdsfactory-7.1.2/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3276 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2629 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1260 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4118 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3247 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2348 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     2846 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_double_bend_coupler.py
--rw-r--r--   0        0        0     5102 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7747 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12046 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2909 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1923 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6868 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2743 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4231 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5307 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2281 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3745 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5832 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16624 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9155 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1733 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5289 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2640 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7863 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     8266 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8519 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     6044 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2805 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3955 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      656 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      821 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7973 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3539 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2801 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1235 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1787 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2887 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3886 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3186 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3897 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2430 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2413 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3034 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15895 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4516 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4918 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1065 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     7181 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0    10209 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/config.py
--rw-r--r--   0        0        0    38409 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/constants.py
--rw-r--r--   0        0        0    83618 2023-08-07 04:02:40.338502 gdsfactory-7.1.2/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2963 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/decorators.py
--rw-r--r--   0        0        0     8406 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/difftest.py
--rw-r--r--   0        0        0      668 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/difftest_git.py
--rw-r--r--   0        0        0     1029 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/events.py
--rw-r--r--   0        0        0      267 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3308 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     7531 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/export/to_gerber.py
--rw-r--r--   0        0        0     1908 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3095 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0    11831 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/fill.py
--rw-r--r--   0        0        0     7780 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/font.py
--rw-r--r--   0        0        0     8067 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/functions.py
--rw-r--r--   0        0        0     1025 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1957 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0     1008 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/containers.py
--rw-r--r--   0        0        0      169 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8117 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0      161 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0     6192 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0       27 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/.gitignore
--rw-r--r--   0        0        0      494 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/Makefile
--rw-r--r--   0        0        0     4062 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/README.md
--rw-r--r--   0        0        0     2419 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
--rw-r--r--   0        0        0     9696 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
--rw-r--r--   0        0        0    12379 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
--rw-r--r--   0        0        0     7235 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
--rw-r--r--   0        0        0     3446 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
--rw-r--r--   0        0        0      479 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
--rw-r--r--   0        0        0      582 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
--rw-r--r--   0        0        0      108 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
--rw-r--r--   0        0        0      186 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
--rw-r--r--   0        0        0      398 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
--rw-r--r--   0        0        0      574 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
--rw-r--r--   0        0        0     6034 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
--rw-r--r--   0        0        0    10697 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
--rw-r--r--   0        0        0      477 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
--rw-r--r--   0        0        0     4338 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
--rw-r--r--   0        0        0      926 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
--rw-r--r--   0        0        0    10945 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      709 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4312 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1800 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
--rw-r--r--   0        0        0     1519 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    41073 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0    40616 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/layers.lyp
--rw-r--r--   0        0        0     5977 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/tech.lyt
--rw-r--r--   0        0        0     4258 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1857 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0    10460 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10780 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0     3916 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-08-07 04:02:40.342502 gdsfactory-7.1.2/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4869 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3789 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1862 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      567 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2693 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2803 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3540 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1867 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     4954 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7017 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1655 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6614 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3686 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3055 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4184 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4759 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3248 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3810 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2465 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2952 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     3626 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/write_connectivity.py
--rw-r--r--   0        0        0    10476 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1152 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23637 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14481 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0     9689 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/grid.py
--rw-r--r--   0        0        0     5083 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/install.py
--rw-r--r--   0        0        0     1855 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3519 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3818 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3796 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4644 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4840 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     5247 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/name.py
--rw-r--r--   0        0        0    11574 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/pack.py
--rw-r--r--   0        0        0    52172 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/path.py
--rw-r--r--   0        0        0    29991 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6092 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5029 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/pixelate.py
--rw-r--r--   0        0        0      303 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/plugins/__init__.py
--rw-r--r--   0        0        0     4262 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/polygon.py
--rw-r--r--   0        0        0    33003 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/port.py
--rw-r--r--   0        0        0    37674 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1259 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1927 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2773 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0     4470 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/read/from_updk.py
--rw-r--r--   0        0        0    37973 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5997 2023-08-07 04:02:40.346502 gdsfactory-7.1.2/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5632 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3369 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     1614 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/route_info.py
--rw-r--r--   0        0        0     3767 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2907 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3075 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3031 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8726 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10573 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     9220 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38995 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3879 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      981 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4324 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2796 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    25075 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8642 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6904 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12925 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5258 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1912 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17052 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1486 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9226 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10829 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6090 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2962 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3246 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1773 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34260 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10037 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22673 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8643 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18074 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4341 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14296 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10141 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5040 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2433 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2767 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0      974 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      698 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      925 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1081 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1621 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2225 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0     1013 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1683 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1733 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0     1030 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      272 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-08-07 04:02:40.350502 gdsfactory-7.1.2/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      561 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      565 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      550 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      632 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      847 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0      924 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/23_reticle_passives_grid.py
--rw-r--r--   0        0        0     1177 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/23_reticle_passives_pack.py
--rw-r--r--   0        0        0      381 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      715 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      720 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1434 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1308 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     2393 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      614 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      638 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2296 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0      989 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4494 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      363 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0     1065 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     3668 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      233 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/fab_c_to_updk.py
--rw-r--r--   0        0        0      475 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1893 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1745 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     3102 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     2419 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1283 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     2252 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     2237 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     6899 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     6857 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     3434 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0     4531 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1569 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/show.py
--rw-r--r--   0        0        0      525 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     1689 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/snap.py
--rw-r--r--   0        0        0     4254 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/symbols.py
--rw-r--r--   0        0        0      308 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0      343 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/color_utils.py
--rw-r--r--   0        0        0     7550 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1041 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    19780 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    41893 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0     7428 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/processes.py
--rw-r--r--   0        0        0      674 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/xml_utils.py
--rw-r--r--   0        0        0     1413 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/technology/yaml_utils.py
--rw-r--r--   0        0        0    11084 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/typings.py
--rw-r--r--   0        0        0     5622 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/watch.py
--rw-r--r--   0        0        0     7419 2023-08-07 04:02:40.354502 gdsfactory-7.1.2/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     4300 2023-08-07 04:02:40.358502 gdsfactory-7.1.2/pyproject.toml
--rw-r--r--   0        0        0     9974 1970-01-01 00:00:00.000000 gdsfactory-7.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-08-08 05:06:21.769632 gdsfactory-7.1.3/LICENSE
+-rw-r--r--   0        0        0     7441 2023-08-08 05:06:21.769632 gdsfactory-7.1.3/README.md
+-rw-r--r--   0        0        0     3417 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     1870 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12537 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3682 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5016 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    16012 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14682 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2864 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2253 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1791 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1856 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    14884 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/cell.py
+-rw-r--r--   0        0        0     5620 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/cli.py
+-rw-r--r--   0        0        0   102902 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/component.py
+-rw-r--r--   0        0        0    24269 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    30803 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1179 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1105 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    21495 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2599 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    13939 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3168 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2528 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4664 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4319 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1636 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     3048 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2614 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     8029 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2663 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3807 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5417 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5740 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2888 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1593 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1374 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1552 2023-08-08 05:06:21.777632 gdsfactory-7.1.3/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5933 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8880 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5005 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6080 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2514 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9898 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0    11731 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/component_lattice_generic.py
+-rw-r--r--   0        0        0     7130 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2128 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     4667 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler_bent.py
+-rw-r--r--   0        0        0     3970 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     5829 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1816 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    13157 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5256 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6743 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3759 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2708 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4262 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2481 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3176 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3245 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4313 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1254 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3578 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2968 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2816 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     7984 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4121 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1188 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1756 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7046 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3225 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     2458 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4651 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7137 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7209 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4942 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4694 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1747 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9054 2023-08-08 05:06:21.781632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1814 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4110 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4650 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3855 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1579 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8722 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3643 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1799 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1218 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1278 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     5005 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mmi.py
+-rw-r--r--   0        0        0     3978 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2769 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3801 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3192 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4944 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3293 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7610 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2464 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5822 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12188 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4020 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1264 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6310 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3476 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6016 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6289 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3833 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1915 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3799 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1115 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1475 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2933 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1059 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/rectangular_ring.py
+-rw-r--r--   0        0        0     1476 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3276 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2629 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1260 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4118 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3247 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2348 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     2846 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_double_bend_coupler.py
+-rw-r--r--   0        0        0     5102 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7747 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12046 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2909 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1923 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6868 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2743 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4231 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5307 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2281 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3745 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5832 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16624 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9155 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1733 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5289 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2640 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7863 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-08-08 05:06:21.785632 gdsfactory-7.1.3/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     8266 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8519 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     6044 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2805 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3955 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      656 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      821 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7973 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3539 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2801 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1235 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1787 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2870 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3886 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3186 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3897 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2430 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2413 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3034 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15895 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4516 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4918 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1065 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     7181 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0    10209 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/config.py
+-rw-r--r--   0        0        0    38409 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/constants.py
+-rw-r--r--   0        0        0    83618 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2963 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     8529 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/difftest.py
+-rw-r--r--   0        0        0      668 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/difftest_git.py
+-rw-r--r--   0        0        0     1029 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/events.py
+-rw-r--r--   0        0        0      267 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3308 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     7531 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/export/to_gerber.py
+-rw-r--r--   0        0        0     1908 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3095 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0    11831 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7780 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/font.py
+-rw-r--r--   0        0        0     8067 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/functions.py
+-rw-r--r--   0        0        0     1025 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1957 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0     1008 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/containers.py
+-rw-r--r--   0        0        0      169 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8117 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0      161 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0     6192 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0       27 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/.gitignore
+-rw-r--r--   0        0        0      494 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/Makefile
+-rw-r--r--   0        0        0     4062 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-08-08 05:06:21.789632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12379 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7235 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3446 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    10697 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      477 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0     4338 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py
+-rw-r--r--   0        0        0      926 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      709 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4312 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1800 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25
+-rw-r--r--   0        0        0     1519 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    41073 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0    40616 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/layers.lyp
+-rw-r--r--   0        0        0     5977 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/tech.lyt
+-rw-r--r--   0        0        0     4258 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1857 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0    10460 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10780 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0     3916 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4869 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3789 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1862 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      567 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2693 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2803 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3540 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1867 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     4954 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7017 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1655 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6614 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3686 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3055 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4184 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4759 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3248 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3810 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2465 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2952 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     3626 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/write_connectivity.py
+-rw-r--r--   0        0        0    10476 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1152 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23637 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14481 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0     9689 2023-08-08 05:06:21.793632 gdsfactory-7.1.3/gdsfactory/grid.py
+-rw-r--r--   0        0        0     5083 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/install.py
+-rw-r--r--   0        0        0     1855 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3519 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3818 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3796 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4644 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4840 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     5247 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/name.py
+-rw-r--r--   0        0        0    11574 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/pack.py
+-rw-r--r--   0        0        0    52172 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/path.py
+-rw-r--r--   0        0        0    29991 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6092 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5029 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0      303 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/plugins/__init__.py
+-rw-r--r--   0        0        0     4262 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/polygon.py
+-rw-r--r--   0        0        0    33003 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/port.py
+-rw-r--r--   0        0        0    37674 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1259 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1927 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2773 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0     5320 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/from_updk.py
+-rw-r--r--   0        0        0    37973 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5997 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5632 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3369 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     1614 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/route_info.py
+-rw-r--r--   0        0        0     3767 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2907 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3075 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3031 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8726 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10573 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     9220 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38995 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3879 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      981 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4324 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2796 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    25075 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8642 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6904 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12925 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5258 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1912 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17052 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1486 2023-08-08 05:06:21.797632 gdsfactory-7.1.3/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9226 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10829 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6090 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2962 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3246 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1773 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34260 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10037 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22673 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8643 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18074 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4341 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14296 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10141 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5040 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2433 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2767 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0      974 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      698 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      925 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1081 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1621 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2225 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0     1013 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1683 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1733 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0     1030 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      272 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      561 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      565 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      550 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      632 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      847 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0      924 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/23_reticle_passives_grid.py
+-rw-r--r--   0        0        0     1177 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/23_reticle_passives_pack.py
+-rw-r--r--   0        0        0      381 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      715 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      720 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1434 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1308 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     2393 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      614 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      638 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2296 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0      989 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4494 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      363 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0     1065 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-08-08 05:06:21.801633 gdsfactory-7.1.3/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     3668 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      233 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/fab_c_to_updk.py
+-rw-r--r--   0        0        0      475 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1893 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1745 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     3102 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     2419 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1283 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     2252 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     2237 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     6899 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     6857 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     3434 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0     4531 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1569 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/show.py
+-rw-r--r--   0        0        0      525 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     1689 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4254 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      308 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0      343 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/color_utils.py
+-rw-r--r--   0        0        0     7550 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1041 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    19780 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    41893 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0     7428 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/processes.py
+-rw-r--r--   0        0        0      674 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/xml_utils.py
+-rw-r--r--   0        0        0     1413 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/technology/yaml_utils.py
+-rw-r--r--   0        0        0    11084 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/typings.py
+-rw-r--r--   0        0        0     5622 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/watch.py
+-rw-r--r--   0        0        0     7419 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     4300 2023-08-08 05:06:21.805632 gdsfactory-7.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9974 1970-01-01 00:00:00.000000 gdsfactory-7.1.3/PKG-INFO
```

### Comparing `gdsfactory-7.1.2/LICENSE` & `gdsfactory-7.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/README.md` & `gdsfactory-7.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gdsfactory 7.1.2
+# gdsfactory 7.1.3
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![Downloads](https://pepy.tech/badge/gdsfactory)](https://pepy.tech/project/gdsfactory)
```

### Comparing `gdsfactory-7.1.2/gdsfactory/__init__.py` & `gdsfactory-7.1.3/gdsfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,8 +144,8 @@
     "technology",
     "write_cells",
     "xsection",
     "PATH",
 )
 
 
-__version__ = "7.1.2"
+__version__ = "7.1.3"
```

### Comparing `gdsfactory-7.1.2/gdsfactory/add_keepout.py` & `gdsfactory-7.1.3/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/add_labels.py` & `gdsfactory-7.1.3/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/add_loopback.py` & `gdsfactory-7.1.3/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/add_padding.py` & `gdsfactory-7.1.3/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/add_pins.py` & `gdsfactory-7.1.3/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/add_ports.py` & `gdsfactory-7.1.3/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/add_tapers.py` & `gdsfactory-7.1.3/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-7.1.3/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/add_termination.py` & `gdsfactory-7.1.3/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/asserts.py` & `gdsfactory-7.1.3/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/cell.py` & `gdsfactory-7.1.3/gdsfactory/cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/cli.py` & `gdsfactory-7.1.3/gdsfactory/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "7.1.2"
+VERSION = "7.1.3"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `gdsfactory-7.1.2/gdsfactory/component.py` & `gdsfactory-7.1.3/gdsfactory/component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/component_layout.py` & `gdsfactory-7.1.3/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/component_reference.py` & `gdsfactory-7.1.3/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/C.py` & `gdsfactory-7.1.3/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/L.py` & `gdsfactory-7.1.3/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/__init__.py` & `gdsfactory-7.1.3/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/add_fiducials.py` & `gdsfactory-7.1.3/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-7.1.3/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/add_trenches.py` & `gdsfactory-7.1.3/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/align.py` & `gdsfactory-7.1.3/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/array_component.py` & `gdsfactory-7.1.3/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/array_with_fanout.py` & `gdsfactory-7.1.3/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/array_with_via.py` & `gdsfactory-7.1.3/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/awg.py` & `gdsfactory-7.1.3/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/bbox.py` & `gdsfactory-7.1.3/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/bend_circular.py` & `gdsfactory-7.1.3/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-7.1.3/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/bend_euler.py` & `gdsfactory-7.1.3/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/bend_port.py` & `gdsfactory-7.1.3/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/bend_s.py` & `gdsfactory-7.1.3/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/bezier.py` & `gdsfactory-7.1.3/gdsfactory/components/bezier.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cavity.py` & `gdsfactory-7.1.3/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cdc.py` & `gdsfactory-7.1.3/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cdsem_all.py` & `gdsfactory-7.1.3/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-7.1.3/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-7.1.3/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cdsem_straight.py` & `gdsfactory-7.1.3/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-7.1.3/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/circle.py` & `gdsfactory-7.1.3/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-7.1.3/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-7.1.3/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-7.1.3/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-7.1.3/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/compass.py` & `gdsfactory-7.1.3/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/component_lattice.py` & `gdsfactory-7.1.3/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/component_lattice_generic.py` & `gdsfactory-7.1.3/gdsfactory/components/component_lattice_generic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/component_sequence.py` & `gdsfactory-7.1.3/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/copy_layers.py` & `gdsfactory-7.1.3/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler90.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler90bend.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler_bent.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler_bent.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler_full.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler_ring.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler_straight.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-7.1.3/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cross.py` & `gdsfactory-7.1.3/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-7.1.3/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-7.1.3/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-7.1.3/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cutback_2x2.py` & `gdsfactory-7.1.3/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cutback_bend.py` & `gdsfactory-7.1.3/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cutback_component.py` & `gdsfactory-7.1.3/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/cutback_splitter.py` & `gdsfactory-7.1.3/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/dbr.py` & `gdsfactory-7.1.3/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/dbr_tapered.py` & `gdsfactory-7.1.3/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/delay_snake.py` & `gdsfactory-7.1.3/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/delay_snake2.py` & `gdsfactory-7.1.3/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/delay_snake3.py` & `gdsfactory-7.1.3/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-7.1.3/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/dicing_lane.py` & `gdsfactory-7.1.3/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/die.py` & `gdsfactory-7.1.3/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/die_bbox.py` & `gdsfactory-7.1.3/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-7.1.3/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/disk.py` & `gdsfactory-7.1.3/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-7.1.3/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ellipse.py` & `gdsfactory-7.1.3/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/extend_ports_list.py` & `gdsfactory-7.1.3/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/extension.py` & `gdsfactory-7.1.3/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/fiber.py` & `gdsfactory-7.1.3/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/fiber_array.py` & `gdsfactory-7.1.3/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/fiducial_squares.py` & `gdsfactory-7.1.3/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-7.1.3/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_elliptical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-7.1.3/gdsfactory/components/grating_coupler_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/greek_cross.py` & `gdsfactory-7.1.3/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/hline.py` & `gdsfactory-7.1.3/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-7.1.3/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/litho_calipers.py` & `gdsfactory-7.1.3/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/litho_ruler.py` & `gdsfactory-7.1.3/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/litho_steps.py` & `gdsfactory-7.1.3/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/logo.py` & `gdsfactory-7.1.3/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/loop_mirror.py` & `gdsfactory-7.1.3/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mmi.py` & `gdsfactory-7.1.3/gdsfactory/components/mmi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mmi1x2.py` & `gdsfactory-7.1.3/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-7.1.3/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mmi2x2.py` & `gdsfactory-7.1.3/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-7.1.3/gdsfactory/components/mmi2x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-7.1.3/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mode_converter.py` & `gdsfactory-7.1.3/gdsfactory/components/mode_converter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzi.py` & `gdsfactory-7.1.3/gdsfactory/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzi_arm.py` & `gdsfactory-7.1.3/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzi_arms.py` & `gdsfactory-7.1.3/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzi_lattice.py` & `gdsfactory-7.1.3/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-7.1.3/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-7.1.3/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzit.py` & `gdsfactory-7.1.3/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzit_lattice.py` & `gdsfactory-7.1.3/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/mzm.py` & `gdsfactory-7.1.3/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/nxn.py` & `gdsfactory-7.1.3/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/optimal_90deg.py` & `gdsfactory-7.1.3/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-7.1.3/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/optimal_step.py` & `gdsfactory-7.1.3/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/pack_doe.py` & `gdsfactory-7.1.3/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/pad.py` & `gdsfactory-7.1.3/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/pad_gsg.py` & `gdsfactory-7.1.3/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/pads_shorted.py` & `gdsfactory-7.1.3/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-7.1.3/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ramp.py` & `gdsfactory-7.1.3/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/rectangle.py` & `gdsfactory-7.1.3/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-7.1.3/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/rectangular_ring.py` & `gdsfactory-7.1.3/gdsfactory/components/rectangular_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/regular_polygon.py` & `gdsfactory-7.1.3/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/resistance_meander.py` & `gdsfactory-7.1.3/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/resistance_sheet.py` & `gdsfactory-7.1.3/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring.py` & `gdsfactory-7.1.3/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_crow.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_double.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_double_bend_coupler.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_double_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_double_heater.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_double_pn.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_section_based.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_single.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_single_array.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_single_dut.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_single_heater.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/ring_single_pn.py` & `gdsfactory-7.1.3/gdsfactory/components/ring_single_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/seal_ring.py` & `gdsfactory-7.1.3/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/snspd.py` & `gdsfactory-7.1.3/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/spiral_double.py` & `gdsfactory-7.1.3/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/spiral_external_io.py` & `gdsfactory-7.1.3/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/spiral_heater.py` & `gdsfactory-7.1.3/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-7.1.3/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/splitter_chain.py` & `gdsfactory-7.1.3/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/splitter_tree.py` & `gdsfactory-7.1.3/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight.py` & `gdsfactory-7.1.3/gdsfactory/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_array.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_pin.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/straight_rib.py` & `gdsfactory-7.1.3/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/switch_tree.py` & `gdsfactory-7.1.3/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/taper.py` & `gdsfactory-7.1.3/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-7.1.3/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/taper_cross_section.py` & `gdsfactory-7.1.3/gdsfactory/components/taper_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/taper_from_csv.py` & `gdsfactory-7.1.3/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/taper_parabolic.py` & `gdsfactory-7.1.3/gdsfactory/components/taper_parabolic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/terminator.py` & `gdsfactory-7.1.3/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/text.py` & `gdsfactory-7.1.3/gdsfactory/components/text.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,31 +41,30 @@
                 for poly in _glyph[ascii_val]:
                     xpts = np.array(poly)[:, 0] * scaling
                     ypts = np.array(poly)[:, 1] * scaling
                     label.add_polygon([xpts + xoffset, ypts + yoffset], layer=layer)
                 xoffset += (_width[ascii_val] + _indent[ascii_val]) * scaling
             else:
                 raise ValueError(f"No character with ascii value {ascii_val!r}")
-        ref = t.add_ref(label)
-        t.absorb(ref)
+        t.add_ref(label)
         yoffset -= 1500 * scaling
         xoffset = position[0]
     justify = justify.lower()
     for label in t.references:
         if justify == "left":
             pass
         elif justify == "right":
             label.xmax = position[0]
         elif justify == "center":
             label.move(origin=label.center, destination=position, axis="x")
         else:
             raise ValueError(
                 f"justify = {justify!r} not in ('center', 'right', 'left')"
             )
-    return t
+    return t.flatten()
 
 
 @gf.cell
 def text_lines(
     text: tuple[str, ...] = ("Chip", "01"),
     size: float = 0.4,
     layer: LayerSpec = "WG",
@@ -84,18 +83,19 @@
         tref = c.add_ref(t)
         tref.movey(-6 * size * (i + 1))
     return c
 
 
 if __name__ == "__main__":
     # c1 = gf.components.text("hello", size=10, layer=(1, 0))
-    c2 = gf.components.text("10.0")
-    # c = text(
-    #     text=".[,ABCDEFGHIKKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789:/",
-    #     size=4.0,
-    #     justify="right",
-    #     position=(120.5, 3),
-    # )
+    # c2 = gf.components.text("10.0")
+    c = text(
+        text=".[,ABCDEFGHIKKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789:/",
+        size=4.0,
+        justify="right",
+        position=(0, 0),
+    )
     # c = text_lines(text=["a", "b"], size=10)
     # c = text_lines()
-    c2.show(show_ports=True)
+    # c2.show(show_ports=True)
     # c.plot()
+    c.show()
```

### Comparing `gdsfactory-7.1.2/gdsfactory/components/text_freetype.py` & `gdsfactory-7.1.3/gdsfactory/components/text_freetype.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/text_rectangular.py` & `gdsfactory-7.1.3/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-7.1.3/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/triangles.py` & `gdsfactory-7.1.3/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/verniers.py` & `gdsfactory-7.1.3/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/version_stamp.py` & `gdsfactory-7.1.3/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/via.py` & `gdsfactory-7.1.3/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/via_corner.py` & `gdsfactory-7.1.3/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/via_cutback.py` & `gdsfactory-7.1.3/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/via_stack.py` & `gdsfactory-7.1.3/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/via_stack_slot.py` & `gdsfactory-7.1.3/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-7.1.3/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/wafer.py` & `gdsfactory-7.1.3/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/wire.py` & `gdsfactory-7.1.3/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/components/wire_sbend.py` & `gdsfactory-7.1.3/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/config.py` & `gdsfactory-7.1.3/gdsfactory/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from pydantic import BaseModel, BaseSettings, Field
 from rich.console import Console
 from rich.table import Table
 
 if TYPE_CHECKING:
     from loguru import Logger
 
-__version__ = "7.1.2"
+__version__ = "7.1.3"
 PathType = str | pathlib.Path
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
```

### Comparing `gdsfactory-7.1.2/gdsfactory/constants.py` & `gdsfactory-7.1.3/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/cross_section.py` & `gdsfactory-7.1.3/gdsfactory/cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/decorators.py` & `gdsfactory-7.1.3/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/difftest.py` & `gdsfactory-7.1.3/gdsfactory/difftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """GDS regression test. Inspired by lytest."""
 import filecmp
 import pathlib
 import shutil
 
 import gdsfactory as gf
-from gdsfactory.config import GDSDIR_TEMP, PATH, logger
+from gdsfactory.config import PATH, logger
 
 
 class GeometryDifference(Exception):
     pass
 
 
 PathType = pathlib.Path | str
@@ -133,39 +133,41 @@
 
 
 def difftest(
     component: gf.Component,
     test_name: gf.Component | None = None,
     dirpath: pathlib.Path = PATH.gds_ref,
     xor: bool = True,
+    dirpath_run: pathlib.Path = PATH.gds_run,
 ) -> None:
     """Avoids GDS regressions tests on the GeometryDifference.
 
     If files are the same it returns None. If files are different runs XOR
     between new component and the GDS reference stored in dirpath and
     raises GeometryDifference if there are differences and show differences in KLayout.
 
     If it runs for the fist time it just stores the GDS reference.
 
     Args:
         component: to test if it has changed.
         test_name: used to store the GDS file.
-        dirpath: default directory for storing reference files.
+        dirpath: directory where reference files are stored.
         xor: runs XOR.
+        dirpath_run: directory to store gds file generated by the test.
     """
     test_name = test_name or (
         f"{component.function_name}_{component.name}"
         if hasattr(component, "function_name")
         and component.name != component.function_name
         else f"{component.name}"
     )
     filename = f"{test_name}.gds"
     dirpath_ref = dirpath
     dirpath_ref.mkdir(exist_ok=True, parents=True)
-    dirpath_run = GDSDIR_TEMP
+    dirpath_run.mkdir(exist_ok=True, parents=True)
 
     ref_file = dirpath_ref / f"{test_name}.gds"
     run_file = dirpath_run / filename
 
     component = gf.get_component(component)
     run_file = component.write_gds(gdspath=run_file)
```

### Comparing `gdsfactory-7.1.2/gdsfactory/difftest_git.py` & `gdsfactory-7.1.3/gdsfactory/difftest_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/events.py` & `gdsfactory-7.1.3/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/export/to_3d.py` & `gdsfactory-7.1.3/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/export/to_gerber.py` & `gdsfactory-7.1.3/gdsfactory/export/to_gerber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/export/to_np.py` & `gdsfactory-7.1.3/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/export/to_stl.py` & `gdsfactory-7.1.3/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/fill.py` & `gdsfactory-7.1.3/gdsfactory/fill.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/font.py` & `gdsfactory-7.1.3/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/functions.py` & `gdsfactory-7.1.3/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/README.md` & `gdsfactory-7.1.3/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/__init__.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/containers.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 1% similar despite different names*

#### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>7.1.2</version>
+  <version>7.1.3</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/README.md` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/run_lvs.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/run_lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/layout/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 16% similar despite different names*

#### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;7.1.2&quot;
+__version__ = &quot;7.1.3&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/d25/generic.lyd25`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/layers.lyp` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/layers.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/tech.lyt` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-7.1.3/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/layer_stack.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-7.1.3/gdsfactory/generic_tech/layer_views.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/generic_tech/simulation_settings.py` & `gdsfactory-7.1.3/gdsfactory/generic_tech/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/__init__.py` & `gdsfactory-7.1.3/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/boolean.py` & `gdsfactory-7.1.3/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-7.1.3/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-7.1.3/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-7.1.3/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-7.1.3/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-7.1.3/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/check_space.py` & `gdsfactory-7.1.3/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/check_width.py` & `gdsfactory-7.1.3/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-7.1.3/gdsfactory/geometry/fill_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-7.1.3/gdsfactory/geometry/fill_tiled.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/fillet.py` & `gdsfactory-7.1.3/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/functions.py` & `gdsfactory-7.1.3/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/invert.py` & `gdsfactory-7.1.3/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/layer_priority.py` & `gdsfactory-7.1.3/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/manhattanize.py` & `gdsfactory-7.1.3/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/maskprep.py` & `gdsfactory-7.1.3/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-7.1.3/gdsfactory/geometry/maskprep_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/offset.py` & `gdsfactory-7.1.3/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/outline.py` & `gdsfactory-7.1.3/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/trim.py` & `gdsfactory-7.1.3/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/union.py` & `gdsfactory-7.1.3/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/write_connectivity.py` & `gdsfactory-7.1.3/gdsfactory/geometry/write_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/write_drc.py` & `gdsfactory-7.1.3/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/geometry/xor_diff.py` & `gdsfactory-7.1.3/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/get_factories.py` & `gdsfactory-7.1.3/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/get_netlist.py` & `gdsfactory-7.1.3/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/get_netlist_flat.py` & `gdsfactory-7.1.3/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/grid.py` & `gdsfactory-7.1.3/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/install.py` & `gdsfactory-7.1.3/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/klive.py` & `gdsfactory-7.1.3/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/labels/__init__.py` & `gdsfactory-7.1.3/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-7.1.3/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/labels/ehva.py` & `gdsfactory-7.1.3/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-7.1.3/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/labels/siepic.py` & `gdsfactory-7.1.3/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/labels/write_labels.py` & `gdsfactory-7.1.3/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/name.py` & `gdsfactory-7.1.3/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/pack.py` & `gdsfactory-7.1.3/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/path.py` & `gdsfactory-7.1.3/gdsfactory/path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/pdk.py` & `gdsfactory-7.1.3/gdsfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/picmodel.py` & `gdsfactory-7.1.3/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/pixelate.py` & `gdsfactory-7.1.3/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/polygon.py` & `gdsfactory-7.1.3/gdsfactory/polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/port.py` & `gdsfactory-7.1.3/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/quickplotter.py` & `gdsfactory-7.1.3/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/__init__.py` & `gdsfactory-7.1.3/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/from_dphox.py` & `gdsfactory-7.1.3/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/from_gdspaths.py` & `gdsfactory-7.1.3/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/from_np.py` & `gdsfactory-7.1.3/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/from_phidl.py` & `gdsfactory-7.1.3/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/from_updk.py` & `gdsfactory-7.1.3/gdsfactory/read/from_updk.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,35 +7,43 @@
 
 import io
 import pathlib
 from typing import IO
 
 from omegaconf import OmegaConf
 
-from gdsfactory.typings import PathType
+from gdsfactory.typings import LayerSpec, PathType
 
 
 def from_updk(
     filepath: PathType,
     filepath_out: PathType | None = None,
     layer_bbox: tuple[int, int] = (68, 0),
     layer_label: tuple[int, int] | None = None,
     optical_xsections: list[str] | None = None,
     electrical_xsections: list[str] | None = None,
+    layers_text: list[LayerSpec] | None = None,
+    text_size: float = 2.0,
+    activate_pdk: bool = False,
     prefix: str = "",
     suffix: str = "",
 ) -> str:
     """Read uPDK definition and returns a gdsfactory script.
 
     Args:
         filepath: uPDK filepath definition.
         filepath_out: optional filepath to save script. if None only returns script and does not save it.
         layer_bbox: layer to draw bounding boxes.
         optical_xsections: Optional list of names of xsections that will add optical ports.
         electrical_xsections: Optional list of names of xsections that will add electrical ports.
+        layers_text: Optional list of layers to add text labels.
+        text_size: text size for labels.
+        activate_pdk: if True, activate the pdk after writing the script.
+        prefix: optional prefix to add to the script.
+        suffix: optional suffix to add to the script.
     """
 
     optical_xsections = optical_xsections or []
     electrical_xsections = electrical_xsections or []
 
     if isinstance(filepath, str | pathlib.Path | IO):
         filepath = (
@@ -89,18 +97,22 @@
                     if hasattr(p, "min")
                 ]
             )
             if parameters
             else ""
         )
 
+        parameters = (
+            [f"{p_name}:{{{p_name}}}" for p_name in parameters] if parameters else []
+        )
+
         parameters_labels = (
             "\n".join(
                 [
-                    f"    c.add_label(text=f'{p_name}:{{{p_name}}}', position=(xc, yc-{i}/{len(parameters)}*ysize/2), layer=layer_label)"
+                    f"    c.add_label(text='{p_name}:{{{p_name}}}', position=(xc, yc-{i}/{len(parameters)}*ysize/2), layer=layer_label)"
                     for i, p_name in enumerate(parameters)
                 ]
             )
             if layer_label and parameters
             else ""
         )
 
@@ -114,34 +126,44 @@
 @gf.cell
 def {block_name}({parameters_string})->gf.Component:
     {doc}
     c = gf.Component()
     p = c.add_polygon({points}, layer=layer_bbox)
     xc, yc = p.center
     ysize = p.ysize
+    name = f"{block_name}_{'_'.join(parameters)}"
 """
         script += parameters_labels
 
         for port_name, port in block.pins.items():
             port_type = (
                 "electrical" if port.xsection in electrical_xsections else "optical"
             )
             cross_section = port.xsection if port.xsection != "None" else None
             script += f"""
     c.add_port(name={port_name!r}, width={port.width}, cross_section={cross_section!r}, center=({port.xya[0]}, {port.xya[1]}), orientation={port.xya[2]}, port_type={port_type!r})"""
 
+        if layers_text:
+            for layer_text in layers_text:
+                script += f"""
+    c << gf.c.text(text=name, size={text_size}, position=(xc, yc), layer={layer_text},justify='center')\n"""
+
         script += """
+    c.name = name
     return c
 """
 
-    script += f"""
+    if activate_pdk:
+        script += f"""
 cells = get_cells(sys.modules[__name__])
 pdk = gf.Pdk(name={conf.header.description!r}, cells=cells, cross_sections=cross_sections)
 pdk.activate()
+"""
 
+    script += f"""
 {suffix}
 
 if __name__ == "__main__":
     c = {block_name}()
     c.show(show_ports=True)
 """
     if filepath_out:
```

### Comparing `gdsfactory-7.1.2/gdsfactory/read/from_yaml.py` & `gdsfactory-7.1.3/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/from_yaml_template.py` & `gdsfactory-7.1.3/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/import_gds.py` & `gdsfactory-7.1.3/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/read/labels.py` & `gdsfactory-7.1.3/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/route_info.py` & `gdsfactory-7.1.3/gdsfactory/route_info.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/__init__.py` & `gdsfactory-7.1.3/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-7.1.3/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-7.1.3/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-7.1.3/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-7.1.3/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-7.1.3/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/add_pads.py` & `gdsfactory-7.1.3/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/all_angle.py` & `gdsfactory-7.1.3/gdsfactory/routing/all_angle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/auto_taper.py` & `gdsfactory-7.1.3/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/factories.py` & `gdsfactory-7.1.3/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/fanout.py` & `gdsfactory-7.1.3/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/fanout2x2.py` & `gdsfactory-7.1.3/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_bundle.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_input_labels.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_route.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_route.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_route_astar.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_route_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-7.1.3/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/manhattan.py` & `gdsfactory-7.1.3/gdsfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/path_length_matching.py` & `gdsfactory-7.1.3/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-7.1.3/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-7.1.3/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-7.1.3/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/route_quad.py` & `gdsfactory-7.1.3/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/route_sharp.py` & `gdsfactory-7.1.3/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/route_south.py` & `gdsfactory-7.1.3/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/sort_ports.py` & `gdsfactory-7.1.3/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/routing/utils.py` & `gdsfactory-7.1.3/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-7.1.3/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-7.1.3/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-7.1.3/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-7.1.3/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/03_move.py` & `gdsfactory-7.1.3/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/04_connect.py` & `gdsfactory-7.1.3/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-7.1.3/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-7.1.3/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-7.1.3/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/11_component_layout.py` & `gdsfactory-7.1.3/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/12_component_refs.py` & `gdsfactory-7.1.3/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-7.1.3/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/14_component_connectivity.py` & `gdsfactory-7.1.3/gdsfactory/samples/14_component_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-7.1.3/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-7.1.3/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/17_ports.py` & `gdsfactory-7.1.3/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/20_components.py` & `gdsfactory-7.1.3/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/21_add_fiber_array.py` & `gdsfactory-7.1.3/gdsfactory/samples/21_add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/22_add_fiber_single.py` & `gdsfactory-7.1.3/gdsfactory/samples/22_add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/22_add_pads.py` & `gdsfactory-7.1.3/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/23_reticle.py` & `gdsfactory-7.1.3/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/23_reticle_passives_grid.py` & `gdsfactory-7.1.3/gdsfactory/samples/23_reticle_passives_grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/23_reticle_passives_pack.py` & `gdsfactory-7.1.3/gdsfactory/samples/23_reticle_passives_pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/24_doe_2.py` & `gdsfactory-7.1.3/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/24_doe_3.py` & `gdsfactory-7.1.3/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/30_lidar.py` & `gdsfactory-7.1.3/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-7.1.3/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-7.1.3/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/big_device.py` & `gdsfactory-7.1.3/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-7.1.3/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-7.1.3/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-7.1.3/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-7.1.3/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/layers.py` & `gdsfactory-7.1.3/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/lvs.py` & `gdsfactory-7.1.3/gdsfactory/samples/demo/lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/demo/pcell.py` & `gdsfactory-7.1.3/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-7.1.3/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-7.1.3/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-7.1.3/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/serialization.py` & `gdsfactory-7.1.3/gdsfactory/serialization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/show.py` & `gdsfactory-7.1.3/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/simulation/__init__.py` & `gdsfactory-7.1.3/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/snap.py` & `gdsfactory-7.1.3/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/symbols.py` & `gdsfactory-7.1.3/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/technology/klayout_tech.py` & `gdsfactory-7.1.3/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/technology/layer_map.py` & `gdsfactory-7.1.3/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/technology/layer_stack.py` & `gdsfactory-7.1.3/gdsfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/technology/layer_views.py` & `gdsfactory-7.1.3/gdsfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/technology/processes.py` & `gdsfactory-7.1.3/gdsfactory/technology/processes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/technology/xml_utils.py` & `gdsfactory-7.1.3/gdsfactory/technology/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/technology/yaml_utils.py` & `gdsfactory-7.1.3/gdsfactory/technology/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/typings.py` & `gdsfactory-7.1.3/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/watch.py` & `gdsfactory-7.1.3/gdsfactory/watch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/gdsfactory/write_cells.py` & `gdsfactory-7.1.3/gdsfactory/write_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-7.1.2/pyproject.toml` & `gdsfactory-7.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 description = "python library to generate GDS layouts"
 keywords = ["eda", "photonics", "python"]
 license = {file = "LICENSE"}
 name = "gdsfactory"
 readme = "README.md"
 requires-python = ">=3.10"
-version = "7.1.2"
+version = "7.1.3"
 
 [project.optional-dependencies]
 cad = [
   "freetype-py",
   "ipycytoscape",
   "ipyevents",
   "ipykernel",
```

### Comparing `gdsfactory-7.1.2/PKG-INFO` & `gdsfactory-7.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 7.1.2
+Version: 7.1.3
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -66,15 +66,15 @@
 Requires-Dist: jupyter-book==0.15.1 ; extra == "docs"
 Requires-Dist: pydata_sphinx_theme==0.13.1 ; extra == "docs"
 Requires-Dist: plotly ; extra == "docs"
 Provides-Extra: cad
 Provides-Extra: dev
 Provides-Extra: docs
 
-# gdsfactory 7.1.2
+# gdsfactory 7.1.3
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![Downloads](https://pepy.tech/badge/gdsfactory)](https://pepy.tech/project/gdsfactory)
```

