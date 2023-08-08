# Comparing `tmp/pyxy3d-0.1.8.tar.gz` & `tmp/pyxy3d-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.1.8.tar", max compression
+gzip compressed data, was "pyxy3d-0.1.9.tar", max compression
```

## Comparing `pyxy3d-0.1.8.tar` & `pyxy3d-0.1.9.tar`

### file list

```diff
@@ -1,264 +1,69 @@
--rw-r--r--   0        0        0    35190 2023-07-29 18:07:40.894411 pyxy3d-0.1.8/LICENSE.md
--rw-r--r--   0        0        0      992 2023-07-30 20:47:07.883242 pyxy3d-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     2644 2023-06-21 22:25:18.660194 pyxy3d-0.1.8/pyxy3d/__init__.py
--rw-r--r--   0        0        0      695 2023-07-30 16:25:04.903298 pyxy3d-0.1.8/pyxy3d/__main__.py
--rw-r--r--   0        0        0     7205 2023-07-27 15:08:47.133986 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
--rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
--rw-r--r--   0        0        0     1003 2023-07-10 14:32:44.845579 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     7195 2023-07-12 17:52:16.571084 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.1.8/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     6970 2023-07-25 16:53:47.249548 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
--rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
--rw-r--r--   0        0        0     3517 2023-07-25 13:35:55.293247 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
--rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
--rw-r--r--   0        0        0     7296 2023-07-27 15:08:56.537729 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
--rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
--rw-r--r--   0        0        0    10127 2023-07-25 16:27:24.407269 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
--rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     2928 2023-07-10 14:32:47.796517 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
--rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
--rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4705 2023-07-09 21:29:42.079500 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     4010 2023-07-25 12:13:14.867974 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10870 2023-07-27 00:41:13.149630 pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9514 2023-07-27 00:41:13.151631 pyxy3d-0.1.8/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1063 2023-07-09 21:29:42.080499 pyxy3d-0.1.8/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     9829 2023-07-12 17:51:09.000113 pyxy3d-0.1.8/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.1.8/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0     7224 2023-07-30 16:33:14.613807 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
--rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
--rw-r--r--   0        0        0     7133 2023-07-30 16:33:14.623808 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
--rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
--rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
--rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
--rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
--rw-r--r--   0        0        0     8085 2023-07-30 16:33:14.607808 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
--rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
--rw-r--r--   0        0        0     9312 2023-07-26 23:56:12.921506 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
--rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.1.8/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
--rw-r--r--   0        0        0    10779 2023-07-30 16:25:04.905291 pyxy3d-0.1.8/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     8011 2023-07-30 16:25:04.906290 pyxy3d-0.1.8/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.1.8/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0    11937 2023-07-30 16:29:59.573256 pyxy3d-0.1.8/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    12288 2023-07-26 23:56:05.774680 pyxy3d-0.1.8/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0    14423 2023-07-25 23:58:50.235435 pyxy3d-0.1.8/pyxy3d/configurator.py
--rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.1.8/pyxy3d/export.py
--rw-r--r--   0        0        0     3490 2023-07-27 15:08:58.244729 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5691 2023-06-22 12:39:42.763393 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
--rw-r--r--   0        0        0     7124 2023-07-27 15:08:58.214730 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9398 2023-07-27 15:08:58.249730 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2411 2023-07-27 15:08:58.208730 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0    11669 2023-07-29 17:27:31.448171 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2664 2023-07-27 15:08:58.218730 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
--rw-r--r--   0        0        0     2468 2023-07-11 17:24:44.068539 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
--rw-r--r--   0        0        0    11339 2023-07-30 19:29:33.442855 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
--rw-r--r--   0        0        0     1180 2023-07-27 15:09:03.632307 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
--rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
--rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
--rw-r--r--   0        0        0    12316 2023-07-30 18:41:33.655908 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
--rw-r--r--   0        0        0     4462 2023-07-26 21:07:51.938115 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/recording_widget_minimal.cpython-310.pyc
--rw-r--r--   0        0        0    10374 2023-07-30 18:07:18.613707 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/single_main_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
--rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
--rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.1.8/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
--rw-r--r--   0        0        0     4052 2023-07-27 00:41:13.153630 pyxy3d-0.1.8/pyxy3d/gui/calibrate_capture_volume_widget.py
--rw-r--r--   0        0        0    13155 2023-07-27 15:08:58.230730 pyxy3d-0.1.8/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
--rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.1.8/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
--rw-r--r--   0        0        0     3662 2023-07-27 15:08:58.239730 pyxy3d-0.1.8/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.1.8/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
--rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.1.8/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
--rw-r--r--   0        0        0     3463 2023-07-27 15:08:58.234731 pyxy3d-0.1.8/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
--rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.1.8/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
--rw-r--r--   0        0        0     3627 2023-07-27 15:08:58.224730 pyxy3d-0.1.8/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0    17913 2023-07-27 00:41:13.154630 pyxy3d-0.1.8/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     5800 2023-07-27 00:41:13.155630 pyxy3d-0.1.8/pyxy3d/gui/camera_config/camera_summary_widget.py
--rw-r--r--   0        0        0     4178 2023-07-27 00:41:13.157632 pyxy3d-0.1.8/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0     3776 2023-07-27 00:41:13.158647 pyxy3d-0.1.8/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
--rw-r--r--   0        0        0    11157 2023-07-27 00:41:13.159631 pyxy3d-0.1.8/pyxy3d/gui/charuco_widget.py
--rw-r--r--   0        0        0    11741 2023-07-27 00:41:13.160631 pyxy3d-0.1.8/pyxy3d/gui/extrinsic_calibration_widget.py
--rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0     9841 2023-07-11 17:24:42.356540 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
--rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    13910 2023-07-11 13:59:26.584884 pyxy3d-0.1.8/pyxy3d/gui/frame_builders/paired_frame_builder.py
--rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.1.8/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.1.8/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.1.8/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     2608 2023-07-27 00:41:13.161631 pyxy3d-0.1.8/pyxy3d/gui/log_widget.py
--rw-r--r--   0        0        0    16030 2023-07-27 00:41:13.162631 pyxy3d-0.1.8/pyxy3d/gui/main_widget.py
--rw-r--r--   0        0        0     3292 2023-07-27 00:41:13.163646 pyxy3d-0.1.8/pyxy3d/gui/navigation_bars.py
--rw-r--r--   0        0        0    14373 2023-07-30 19:29:24.120823 pyxy3d-0.1.8/pyxy3d/gui/post_processing_widget.py
--rw-r--r--   0        0        0      954 2023-07-27 00:41:13.165630 pyxy3d-0.1.8/pyxy3d/gui/progress_dialog.py
--rw-r--r--   0        0        0    15159 2023-07-30 18:39:48.500788 pyxy3d-0.1.8/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0    13556 2023-07-30 20:24:02.212523 pyxy3d-0.1.8/pyxy3d/gui/single_main_widget.py
--rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.1.8/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
--rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.1.8/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
--rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.1.8/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
--rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.1.8/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.1.8/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     4920 2023-07-27 15:09:03.628305 pyxy3d-0.1.8/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.1.8/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2999 2023-07-25 22:50:10.592707 pyxy3d-0.1.8/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
--rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.1.8/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5773 2023-07-30 16:33:16.503013 pyxy3d-0.1.8/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.1.8/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     3404 2023-07-25 22:49:59.747262 pyxy3d-0.1.8/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6851 2023-07-30 16:25:04.908290 pyxy3d-0.1.8/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.1.8/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     5054 2023-07-27 00:41:13.170632 pyxy3d-0.1.8/pyxy3d/gui/vizualize/playback_triangulation_widget.py
--rw-r--r--   0        0        0     5452 2023-07-27 00:41:13.172632 pyxy3d-0.1.8/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
--rw-r--r--   0        0        0     1135 2023-07-09 18:24:33.273377 pyxy3d-0.1.8/pyxy3d/helper.py
--rw-r--r--   0        0        0     7815 2023-07-24 21:54:31.011407 pyxy3d-0.1.8/pyxy3d/interface.py
--rw-r--r--   0        0        0     3071 2023-07-30 16:38:05.760567 pyxy3d-0.1.8/pyxy3d/logger.py
--rw-r--r--   0        0        0     2320 2023-07-24 21:05:53.230943 pyxy3d-0.1.8/pyxy3d/post_processing/__pycache__/blender_tools.cpython-310.pyc
--rw-r--r--   0        0        0     2676 2023-07-29 19:19:21.465044 pyxy3d-0.1.8/pyxy3d/post_processing/__pycache__/gap_filling.cpython-310.pyc
--rw-r--r--   0        0        0     4995 2023-07-30 20:42:51.454576 pyxy3d-0.1.8/pyxy3d/post_processing/__pycache__/post_processor.cpython-310.pyc
--rw-r--r--   0        0        0     2208 2023-07-30 16:33:19.004634 pyxy3d-0.1.8/pyxy3d/post_processing/__pycache__/smoothing.cpython-310.pyc
--rw-r--r--   0        0        0     3060 2023-07-24 20:44:55.531665 pyxy3d-0.1.8/pyxy3d/post_processing/blender_tools.py
--rw-r--r--   0        0        0     4790 2023-07-29 18:07:40.899412 pyxy3d-0.1.8/pyxy3d/post_processing/gap_filling.py
--rw-r--r--   0        0        0     5964 2023-07-30 20:41:32.098493 pyxy3d-0.1.8/pyxy3d/post_processing/post_processor.py
--rw-r--r--   0        0        0     2662 2023-07-30 16:25:04.909290 pyxy3d-0.1.8/pyxy3d/post_processing/smoothing.py
--rw-r--r--   0        0        0     8568 2023-07-29 19:45:34.678076 pyxy3d-0.1.8/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
--rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.1.8/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
--rw-r--r--   0        0        0     6208 2023-07-27 15:08:58.197730 pyxy3d-0.1.8/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
--rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.1.8/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
--rw-r--r--   0        0        0    11823 2023-07-29 19:39:24.838999 pyxy3d-0.1.8/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     9313 2023-07-27 00:41:13.175630 pyxy3d-0.1.8/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.1.8/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
--rw-r--r--   0        0        0    17056 2023-07-30 18:02:33.836341 pyxy3d-0.1.8/pyxy3d/session/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0    22463 2023-07-30 18:02:15.994692 pyxy3d-0.1.8/pyxy3d/session/session.py
--rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.1.8/pyxy3d/trackers/__init__.py
--rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3979 2023-07-10 14:32:44.840901 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     8170 2023-07-30 16:33:18.974618 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     6262 2023-07-25 14:53:27.615678 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.1.8/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
--rw-r--r--   0        0        0     4945 2023-07-09 21:29:42.088499 pyxy3d-0.1.8/pyxy3d/trackers/charuco_tracker.py
--rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.1.8/pyxy3d/trackers/hand_tracker.py
--rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.1.8/pyxy3d/trackers/helper.py
--rw-r--r--   0        0        0    13049 2023-07-30 16:25:04.910290 pyxy3d-0.1.8/pyxy3d/trackers/holistic_opensim_tracker.py
--rw-r--r--   0        0        0     9435 2023-07-24 21:54:31.013407 pyxy3d-0.1.8/pyxy3d/trackers/holistic_tracker.py
--rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.1.8/pyxy3d/trackers/pose_tracker.py
--rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.1.8/pyxy3d/trackers/tracker_enum.py
--rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
--rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
--rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
--rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
--rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
--rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
--rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
--rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
--rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
--rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
--rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
--rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
--rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
--rw-r--r--   0        0        0     4259 2023-07-30 20:24:13.538918 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
--rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
--rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
--rw-r--r--   0        0        0   275452 2023-06-27 19:48:44.535266 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.4.nbc
--rw-r--r--   0        0        0     4841 2023-06-27 19:48:44.532265 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
--rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
--rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
--rw-r--r--   0        0        0   274956 2023-07-27 00:11:19.816821 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-174.py310.1.nbc
--rw-r--r--   0        0        0   278013 2023-07-27 00:16:40.548310 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-174.py310.2.nbc
--rw-r--r--   0        0        0   278337 2023-07-27 00:16:47.376567 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-174.py310.3.nbc
--rw-r--r--   0        0        0     3855 2023-07-27 00:16:47.373566 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-174.py310.nbi
--rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
--rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
--rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
--rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
--rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
--rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
--rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
--rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
--rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
--rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
--rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
--rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
--rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
--rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
--rw-r--r--   0        0        0   278015 2023-07-30 14:29:42.828653 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-200.py310.1.nbc
--rw-r--r--   0        0        0   278359 2023-07-30 14:29:50.208434 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-200.py310.2.nbc
--rw-r--r--   0        0        0   275256 2023-07-30 14:30:15.589048 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-200.py310.3.nbc
--rw-r--r--   0        0        0     3826 2023-07-30 14:30:15.587048 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-200.py310.nbi
--rw-r--r--   0        0        0    80894 2023-07-30 14:29:35.120628 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-07-30 14:30:11.488048 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-07-30 14:30:11.486066 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
--rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
--rw-r--r--   0        0        0     2811 2023-07-30 20:41:38.685057 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.cpython-310.pyc
--rw-r--r--   0        0        0   274196 2023-07-30 15:00:17.450860 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.triangulate_sync_index-59.py310.1.nbc
--rw-r--r--   0        0        0   280009 2023-07-30 14:46:37.890889 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.triangulate_sync_index-59.py310.2.nbc
--rw-r--r--   0        0        0     1807 2023-07-30 15:00:17.447857 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.triangulate_sync_index-59.py310.nbi
--rw-r--r--   0        0        0   274236 2023-07-30 20:41:56.594241 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.triangulate_sync_index-62.py310.1.nbc
--rw-r--r--   0        0        0   277241 2023-07-30 20:43:18.194255 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.triangulate_sync_index-62.py310.2.nbc
--rw-r--r--   0        0        0   277585 2023-07-30 20:43:24.917584 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.triangulate_sync_index-62.py310.3.nbc
--rw-r--r--   0        0        0     3819 2023-07-30 20:43:24.914579 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.triangulate_sync_index-62.py310.nbi
--rw-r--r--   0        0        0    77263 2023-07-30 15:00:12.124139 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.unique_with_counts-11.py310.1.nbc
--rw-r--r--   0        0        0     1268 2023-07-30 15:00:12.121138 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.unique_with_counts-11.py310.nbi
--rw-r--r--   0        0        0    77263 2023-07-30 20:41:46.901942 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.unique_with_counts-14.py310.1.nbc
--rw-r--r--   0        0        0    80568 2023-07-30 20:43:10.897248 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.unique_with_counts-14.py310.2.nbc
--rw-r--r--   0        0        0     2268 2023-07-30 20:43:10.894246 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulation.unique_with_counts-14.py310.nbi
--rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.1.8/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.1.8/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.1.8/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     5964 2023-07-30 16:25:04.911290 pyxy3d-0.1.8/pyxy3d/triangulate/sync_packet_triangulator.py
--rw-r--r--   0        0        0     6022 2023-07-30 20:41:12.907370 pyxy3d-0.1.8/pyxy3d/triangulate/triangulation.py
--rw-r--r--   0        0        0     5941 2023-07-29 18:07:40.895425 pyxy3d-0.1.8/README.md
--rw-r--r--   0        0        0     6755 1970-01-01 00:00:00.000000 pyxy3d-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35192 2023-08-02 16:44:19.711417 pyxy3d-0.1.9/LICENSE.md
+-rw-r--r--   0        0        0     1061 2023-08-08 16:52:04.525441 pyxy3d-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     2644 2023-06-21 16:47:49.102536 pyxy3d-0.1.9/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      695 2023-07-27 11:47:40.426640 pyxy3d-0.1.9/pyxy3d/__main__.py
+-rw-r--r--   0        0        0    10127 2023-07-27 11:47:40.426640 pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0     3898 2023-05-06 23:17:45.300248 pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4705 2023-07-11 21:01:41.445361 pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     4010 2023-06-28 15:19:10.033043 pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-24 15:08:32.472149 pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-05-06 23:17:45.315853 pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10870 2023-07-27 11:47:40.426640 pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9514 2023-07-27 11:47:40.434642 pyxy3d-0.1.9/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1063 2023-07-11 21:01:41.445361 pyxy3d-0.1.9/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9829 2023-07-11 21:01:41.445361 pyxy3d-0.1.9/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-07 20:46:34.092944 pyxy3d-0.1.9/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0    10779 2023-07-31 21:25:55.724871 pyxy3d-0.1.9/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     8011 2023-07-31 21:25:55.724871 pyxy3d-0.1.9/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-06 23:17:45.315853 pyxy3d-0.1.9/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    12227 2023-08-08 16:49:18.596289 pyxy3d-0.1.9/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    12288 2023-07-25 12:17:04.560609 pyxy3d-0.1.9/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    14423 2023-07-27 11:47:40.434642 pyxy3d-0.1.9/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     6800 2023-07-31 21:25:55.732870 pyxy3d-0.1.9/pyxy3d/export.py
+-rw-r--r--   0        0        0     4052 2023-07-27 11:47:40.434642 pyxy3d-0.1.9/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0    17913 2023-07-27 11:47:40.434642 pyxy3d-0.1.9/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5800 2023-07-27 11:47:40.434642 pyxy3d-0.1.9/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     4178 2023-07-27 11:47:40.434642 pyxy3d-0.1.9/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3776 2023-07-27 11:47:40.442642 pyxy3d-0.1.9/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-07-27 11:47:40.442642 pyxy3d-0.1.9/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    11741 2023-07-27 11:47:40.442642 pyxy3d-0.1.9/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    13910 2023-07-11 21:01:41.461361 pyxy3d-0.1.9/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-05-06 23:17:45.322358 pyxy3d-0.1.9/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-05-06 23:17:45.322358 pyxy3d-0.1.9/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-05-06 23:17:45.322358 pyxy3d-0.1.9/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2608 2023-07-27 11:47:40.442642 pyxy3d-0.1.9/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    16030 2023-07-27 11:47:40.450639 pyxy3d-0.1.9/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-07-27 11:47:40.450639 pyxy3d-0.1.9/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0    14373 2023-07-31 21:25:55.732870 pyxy3d-0.1.9/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      954 2023-07-27 11:47:40.450639 pyxy3d-0.1.9/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    15255 2023-08-02 16:44:19.713467 pyxy3d-0.1.9/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0    13556 2023-07-31 21:25:55.732870 pyxy3d-0.1.9/pyxy3d/gui/single_main_widget.py
+-rw-r--r--   0        0        0     3404 2023-06-07 20:46:34.102378 pyxy3d-0.1.9/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6851 2023-07-31 21:25:55.732870 pyxy3d-0.1.9/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-17 15:15:57.175775 pyxy3d-0.1.9/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-07-27 11:47:40.458638 pyxy3d-0.1.9/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5452 2023-07-27 11:47:40.458638 pyxy3d-0.1.9/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-17 16:18:01.121529 pyxy3d-0.1.9/pyxy3d/helper.py
+-rw-r--r--   0        0        0     7815 2023-07-25 12:17:04.560609 pyxy3d-0.1.9/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3071 2023-07-27 11:47:40.458638 pyxy3d-0.1.9/pyxy3d/logger.py
+-rw-r--r--   0        0        0     3060 2023-07-25 12:17:04.560609 pyxy3d-0.1.9/pyxy3d/post_processing/blender_tools.py
+-rw-r--r--   0        0        0     4790 2023-07-31 21:25:55.732870 pyxy3d-0.1.9/pyxy3d/post_processing/gap_filling.py
+-rw-r--r--   0        0        0     6424 2023-07-31 21:25:55.732870 pyxy3d-0.1.9/pyxy3d/post_processing/post_processor.py
+-rw-r--r--   0        0        0     2662 2023-07-31 21:25:55.732870 pyxy3d-0.1.9/pyxy3d/post_processing/smoothing.py
+-rw-r--r--   0        0        0    12075 2023-08-07 18:43:54.041728 pyxy3d-0.1.9/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     9681 2023-08-08 16:49:18.597289 pyxy3d-0.1.9/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0    22463 2023-07-27 11:47:40.458638 pyxy3d-0.1.9/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-05-06 23:17:45.337987 pyxy3d-0.1.9/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0     4945 2023-07-11 21:01:41.469362 pyxy3d-0.1.9/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-17 15:15:57.196405 pyxy3d-0.1.9/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-17 15:15:57.196405 pyxy3d-0.1.9/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    13049 2023-07-31 21:25:55.741535 pyxy3d-0.1.9/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9435 2023-07-25 12:17:04.560609 pyxy3d-0.1.9/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-17 15:15:57.196405 pyxy3d-0.1.9/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-06-28 16:24:50.078474 pyxy3d-0.1.9/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     8778 2023-05-06 23:17:45.337987 pyxy3d-0.1.9/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-05-06 23:17:45.337987 pyxy3d-0.1.9/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     5964 2023-07-31 21:25:55.741535 pyxy3d-0.1.9/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     6022 2023-07-31 21:25:55.741535 pyxy3d-0.1.9/pyxy3d/triangulate/triangulation.py
+-rw-r--r--   0        0        0     6002 2023-08-02 16:44:19.712417 pyxy3d-0.1.9/README.md
+-rw-r--r--   0        0        0     6953 1970-01-01 00:00:00.000000 pyxy3d-0.1.9/PKG-INFO
```

### Comparing `pyxy3d-0.1.8/LICENSE.md` & `pyxy3d-0.1.9/LICENSE.md`

 * *Files 0% similar despite different names*

```diff
@@ -658,7 +658,8 @@
 solutions will be better for different programs; see section 13 for the
 specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
 <https://www.gnu.org/licenses/>.
+
```

### Comparing `pyxy3d-0.1.8/pyproject.toml` & `pyxy3d-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 [tool.poetry]
 name = "pyxy3d"
-version = "0.1.8"
+version = "0.1.9"
 description = "A package for calibrating standard webcams to enable 3d motion tracking"
 authors = ["Mac Prible <prible@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.10.11"  #frequent segfaults in python 3.10.11
-opencv-contrib-python = "^4.7"
 pandas = "^1.5.0"
 scipy = "^1.10.1"
 pyqtgraph = "^0.13.2"
 PyOpenGL = "^3.1.6"
 toml = "^0.10.2"
 numba = "^0.56.4"
 mediapipe = "0.10.1"
 pyside6 = "^6.5.2"
 pyqtdarktheme = "^2.1.0"
+polars = "^0.18.11"
+plotnine = "^0.12.2"
+pyarrow = "^12.0.1"
+opencv-contrib-python = "^4.8.0.74"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
 pytest = "^7.3.0"
 ipykernel = "^6.22.0"
 pymdown-extensions = ">=9.11,<11.0"
 mkdocs-material = "^9.1.6"
```

### Comparing `pyxy3d-0.1.8/pyxy3d/__init__.py` & `pyxy3d-0.1.9/pyxy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/__main__.py` & `pyxy3d-0.1.9/pyxy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.1.9/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/charuco.py` & `pyxy3d-0.1.9/pyxy3d/calibration/charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.1.9/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.1.9/pyxy3d/calibration/monocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.1.9/pyxy3d/calibration/stereocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/cameras/camera.py` & `pyxy3d-0.1.9/pyxy3d/cameras/camera.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.1.9/pyxy3d/cameras/camera_array.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.1.9/pyxy3d/cameras/camera_array_initializer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.1.9/pyxy3d/cameras/live_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,14 +53,20 @@
         self.thread = Thread(target=self.process_frames, args=(), daemon=True)
         self.thread.start()
 
         # initialize time trackers for actual FPS determination
         self.frame_time = perf_counter()
         self.avg_delta_time = 1  # initialize to something to avoid errors elsewhere
 
+    @property
+    def size(self):
+        # because the camera resolution will potentially change after stream initialization, this should be 
+        # read directly from the camera whenever a caller (e.g. videorecorder) wants the current resolution
+        return self.camera.size
+
     def set_tracking_on(self, track: bool):
         if track:
             logger.info(f"Turning tracking on on stream {self.port}")
             self.track_points.set()
         else:
             logger.info(f"Turning tracking off on stream {self.port}")
             self.track_points.clear()
```

### Comparing `pyxy3d-0.1.8/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.1.9/pyxy3d/cameras/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/configurator.py` & `pyxy3d-0.1.9/pyxy3d/configurator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/export.py` & `pyxy3d-0.1.9/pyxy3d/export.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,124 +2,119 @@
 logger = pyxy3d.logger.get(__name__)
 from pathlib import Path
 import pandas as pd
 import csv
 
 from pyxy3d.interface import Tracker
 
-def xyz_to_wide_csv(xyz_path:Path, tracker:Tracker):
+def xyz_to_wide_labelled(xyz:pd.DataFrame, tracker:Tracker)->pd.DataFrame:
     """
     Will save a csv file in the same directory as the long xyz point data
     Column headings will be based on the point_id names in the Tracker
     """
-    df_xyz = pd.read_csv(xyz_path)
-    target_path = Path(xyz_path.parent, f"{xyz_path.stem}_labelled.csv")
+
     # save out named data in a tabular format
-    df_xyz = df_xyz.rename(
+    xyz = xyz.rename(
         {
             "x_coord": "x",
             "y_coord": "y",
             "z_coord": "z",
         },
         axis=1,
     )
-    df_xyz = df_xyz[["sync_index", "point_id", "x", "y", "z"]]
+    xyz = xyz[["sync_index", "point_id", "x", "y", "z"]]
 
-    df_xyz["point_name"] = df_xyz["point_id"].map(tracker.get_point_name)
+    xyz["point_name"] = xyz["point_id"].map(tracker.get_point_name)
     # pivot the DataFrame wider
-    df_wide = df_xyz.pivot_table(
+    df_wide = xyz.pivot_table(
         index=["sync_index"], columns="point_name", values=["x", "y", "z"]
     )
     # flatten the column names
     df_wide.columns = ["{}_{}".format(y, x) for x, y in df_wide.columns]
     # reset the index
     df_wide = df_wide.reset_index()
     # merge the rows with the same sync_index
     df_merged = df_wide.groupby("sync_index").agg("first")
     # sort the dataframe
     df_merged = df_merged.sort_index(axis=1, ascending=True)
-    df_merged.to_csv(target_path)
+    return df_merged
 
-def xyz_to_trc(xyz_path:Path, tracker:Tracker):
+def xyz_to_trc(xyz:pd.DataFrame, tracker:Tracker, time_history_path:Path, target_path:Path):
     """
     Will save a .trc file in the same folder as the long xyz data
     relies on xyz_to_wide_csv for input data
     """  
     # create xyz_labelled file to provide input for trc creation
-    xyz_to_wide_csv(xyz_path, tracker)
-
-    # load in the csv file that just got created
-    xyz_labelled_path = Path(xyz_path.parent, f"{xyz_path.stem}_labelled.csv")
-    df_xyz_labelled = pd.read_csv(xyz_labelled_path)
-    # assert(not df_xyz_labelled.empty)
+    xyz_labelled = xyz_to_wide_labelled(xyz, tracker)
 
     # from here I need to get a .trc file format. For part of that I also need to know the framerate.
-    time_history_path = Path(xyz_path.parent, "frame_time_history.csv")
+    # time_history_path = Path(target_path.parent, "frame_time_history.csv")
     time_history = pd.read_csv(time_history_path)
 
     # get the mean time by sync index
     # Group by 'sync_index' and calculate mean 'frame_time'
     sync_time = time_history.groupby("sync_index")["frame_time"].mean()
 
     # Shift times so that it starts at zero
     min_time = sync_time.min()
     sync_time = round(sync_time - min_time,3)
-    df_xyz_labelled.insert(1, "mean_frame_time", sync_time)
+    xyz_labelled.insert(1, "mean_frame_time", sync_time)
     # %%
 
     # Calculate time differences between consecutive frames
-    df_xyz_labelled.sort_values(by="mean_frame_time", inplace=True)
-    df_xyz_labelled["time_diff"] = df_xyz_labelled["mean_frame_time"].diff()
+    xyz_labelled.sort_values(by="mean_frame_time", inplace=True)
+    xyz_labelled["time_diff"] = xyz_labelled["mean_frame_time"].diff()
 
         
 
     # Calculate frame rate for each pair of frames (avoid division by zero)
-    df_xyz_labelled["frame_rate"] = df_xyz_labelled["time_diff"].apply(
+    xyz_labelled["frame_rate"] = xyz_labelled["time_diff"].apply(
         lambda x: 1 / x if x != 0 else 0
     )
 
     # Calculate mean frame rate (drop the first value which is NaN due to the diff operation)
-    mean_frame_rate = df_xyz_labelled["frame_rate"].dropna().mean()
-
+    mean_frame_rate = xyz_labelled["frame_rate"].dropna().mean()
+    
     # Rename 'sync_index' to 'Frame' and 'mean_frame_time' to 'Time'
-    df_xyz_labelled.rename(columns={'sync_index': 'Frame', 'mean_frame_time': 'Time'}, inplace=True)
-    df_xyz_labelled.drop(columns=["time_diff", "frame_rate"], inplace=True) # no longer needed
+    xyz_labelled = xyz_labelled.reset_index() # need sync_index to be just a regular column
+    xyz_labelled.rename(columns={'sync_index': 'Frame', 'mean_frame_time': 'Time'}, inplace=True)
+    xyz_labelled.drop(columns=["time_diff", "frame_rate"], inplace=True) # no longer needed
 
     # Make sure all following fields are in alphabetical order
     # First, get the columns to be sorted, i.e., all columns excluding 'Frame' and 'Time'
-    cols_to_sort = df_xyz_labelled.columns.tolist()[2:]
+    cols_to_sort = xyz_labelled.columns.tolist()[2:]
     cols_to_sort = [col for col in cols_to_sort if not col.startswith("face")]
 
     # Now, sort these columns
     cols_to_sort.sort()
     # Now, create the final column order and rearrange the DataFrame
     final_col_order = ['Frame', 'Time'] + cols_to_sort
-    df_xyz_labelled = df_xyz_labelled[final_col_order]
+    xyz_labelled = xyz_labelled[final_col_order]
 
     # trying a fix...
-    df_xyz_labelled["Frame"] = df_xyz_labelled["Frame"].astype(int)
+    xyz_labelled["Frame"] = xyz_labelled["Frame"].astype(int)
     
     # Get column names from dataframe
-    columns = df_xyz_labelled.columns
+    columns = xyz_labelled.columns
 
     # Remove '_x', '_y', and '_z' suffixes and get unique names
     tracked_points = list(
         set([col.rsplit("_", 1)[0] for col in columns if col.endswith(("_x", "_y", "_z"))])
     )
     tracked_points.sort()
 
 
     num_markers = len(tracked_points)
     data_rate = int(mean_frame_rate)
     units = "m"
     original_data_rate = int(mean_frame_rate)
     orig_data_start_frame = 0
-    num_frames = len(df_xyz_labelled)-1
+    num_frames = len(xyz_labelled)-1
 
-    trc_path = Path(xyz_path.parent,f"{xyz_path.stem}.trc")
+    trc_path = Path(target_path.parent,f"{target_path.stem}.trc")
     trc_filename = str(trc_path)
 
     # this will create the formatted .trc file
     with open(trc_path, 'wt', newline='', encoding='utf-8') as out_file:
         tsv_writer = csv.writer(out_file, delimiter='\t')
         tsv_writer.writerow(["PathFileType",
                             "4", 
@@ -166,15 +161,15 @@
 
         # this is here primarily for testing purposes right now..
         # filLs None with zeros.
         # df_xyz_labelled.fillna(0,inplace=True)
 
 
         # and finally actually write the trajectories
-        for row in range(0, len(df_xyz_labelled)):
-            row_data = df_xyz_labelled.iloc[row].tolist()
+        for row in range(0, len(xyz_labelled)):
+            row_data = xyz_labelled.iloc[row].tolist()
     
             # Convert the 'Frame' column value to int to satisfy trc format requirements
-            frame_index = df_xyz_labelled.columns.get_loc('Frame')
+            frame_index = xyz_labelled.columns.get_loc('Frame')
             row_data[frame_index] = int(row_data[frame_index])
 
             tsv_writer.writerow(row_data)
```

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/calibrate_capture_volume_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/calibrate_capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.1.9/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/camera_config/camera_summary_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/camera_config/camera_summary_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.1.9/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/charuco_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/charuco_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/extrinsic_calibration_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/frame_builders/paired_frame_builder.py` & `pyxy3d-0.1.9/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.1.9/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.1.9/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.1.9/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/log_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/main_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/main_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/navigation_bars.py` & `pyxy3d-0.1.9/pyxy3d/gui/navigation_bars.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/post_processing_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/post_processing_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/progress_dialog.py` & `pyxy3d-0.1.9/pyxy3d/gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/recording_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,18 @@
         # all video output routed to qlabels stored in a dictionariy 
         # make it as square as you can get it
         self.recording_displays = {str(port):QLabel() for port in self.ports}
         # self.recording_frame_display = QLabel()
         
         self.place_widgets()
         self.connect_widgets()        
-        self.update_btn_eligibility()
+        
+        # commenting this out for now...just let people record whenever.
+        # self.update_btn_eligibility()
+        
         logger.info("Recording widget init complete")
     
     def update_btn_eligibility(self):
         if self.session.is_recording_eligible():
             self.start_stop.setEnabled(True)
             logger.info("Record button eligibility updated: Eligible")
         else:
```

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/single_main_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/single_main_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.1.9/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.1.9/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/vizualize/playback_triangulation_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/gui/vizualize/realtime_triangulation_widget.py` & `pyxy3d-0.1.9/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/helper.py` & `pyxy3d-0.1.9/pyxy3d/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/interface.py` & `pyxy3d-0.1.9/pyxy3d/interface.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/logger.py` & `pyxy3d-0.1.9/pyxy3d/logger.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/post_processing/blender_tools.py` & `pyxy3d-0.1.9/pyxy3d/post_processing/blender_tools.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/post_processing/gap_filling.py` & `pyxy3d-0.1.9/pyxy3d/post_processing/gap_filling.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/post_processing/post_processor.py` & `pyxy3d-0.1.9/pyxy3d/post_processing/post_processor.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pyxy3d.triangulate.triangulation import triangulate_xy
 
 from pyxy3d.interface import FramePacket, Tracker
 from pyxy3d.trackers.tracker_enum import TrackerEnum
 
 # specify a source directory (with recordings)
 from pyxy3d.helper import copy_contents
-from pyxy3d.export import xyz_to_trc
+from pyxy3d.export import xyz_to_trc, xyz_to_wide_labelled
 from pyxy3d.post_processing.gap_filling import gap_fill_xy, gap_fill_xyz
 from pyxy3d.post_processing.smoothing import smooth_xyz
 
 class PostProcessor:
     """
     The post processer operates independently of the session. It does not need to worry about camera management.
     Provide it with a path to the directory that contains the following:
@@ -130,16 +130,21 @@
             logger.info("Filling small gaps in (x,y,z) data")
             xyz = gap_fill_xyz(xyz)
             logger.info(f"Smoothing (x,y,z) using butterworth filter with cutoff frequency of 6hz")
             xyz = smooth_xyz(xyz, order=2, fps=self.fps, cutoff=cutoff_freq)
             logger.info("Saving (x,y,z) to csv file")       
             xyz_csv_path = Path(tracker_output_path, f"xyz_{output_suffix}.csv")
             xyz.to_csv(xyz_csv_path)
+            xyz_wide_csv_path = Path(tracker_output_path, f"xyz_{output_suffix}_labelled.csv")
+            xyz_labelled  = xyz_to_wide_labelled(xyz,self.tracker_enum.value())
+            xyz_labelled.to_csv(xyz_wide_csv_path)
 
         else: 
             logger.warn("No points triangulated. Terminating post-processing early.")
             return
 
         # only include trc if wanted and only if there is actually good data to export
         if include_trc and xyz.shape[0] > 0:
-           xyz_to_trc(xyz_csv_path, tracker = self.tracker_enum.value()) 
+           trc_path = Path(tracker_output_path, f"xyz_{output_suffix}.trc")
+           time_history_path = Path(tracker_output_path, f"frame_time_history.csv")
+           xyz_to_trc(xyz,tracker=self.tracker_enum.value(), time_history_path=time_history_path,target_path= trc_path)
```

### Comparing `pyxy3d-0.1.8/pyxy3d/post_processing/smoothing.py` & `pyxy3d-0.1.9/pyxy3d/post_processing/smoothing.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.1.9/pyxy3d/recording/recorded_stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,27 @@
     """
     Analogous to the live stream, this will place frames on a queue
     These can then be harvested and synchronized by a Synchronizer
     Within the stream, point detection occurs.
     """
 
     def __init__(
-        self, camera: CameraData, directory: Path, fps_target:int=6, tracker: Tracker = None
+        self,
+        directory: Path,
+        port: int,
+        size, 
+        rotation_count: int,
+        fps_target: int = 6,
+        tracker: Tracker = None,
     ):
         # self.port = port
         self.directory = directory
-        self.camera = camera
-        self.port = camera.port
+        self.port = port
+        self.size = size
+        self.rotation_count = rotation_count
 
         if tracker is not None:
             self.tracker = tracker
             self.track_points = True
         else:
             self.track_points = False
 
@@ -60,16 +67,18 @@
             Path(self.directory, f"frame_time_history.csv")
         )
         synched_frames_history = pd.read_csv(synched_frames_history_path)
 
         self.port_history = synched_frames_history[
             synched_frames_history["port"] == self.port
         ]
-       
-        self.port_history['frame_index'] = self.port_history['frame_time'].rank(method='min').astype(int) - 1
+
+        self.port_history["frame_index"] = (
+            self.port_history["frame_time"].rank(method="min").astype(int) - 1
+        )
         self.start_frame_index = self.port_history["frame_index"].min()
         self.last_frame_index = self.port_history["frame_index"].max()
 
         # initializing to something to avoid errors elsewhere
         self.frame_index = 0
         self.frame_time = 0
         self.set_fps_target(fps_target)
@@ -164,30 +173,30 @@
 
             success, self.frame = self.capture.read()
 
             if not success:
                 break
 
             if self.track_points:
-                self.point_data = self.tracker.get_points(self.frame, self.port, self.camera.rotation_count)
+                self.point_data = self.tracker.get_points(
+                    self.frame, self.port, self.rotation_count
+                )
                 draw_instructions = self.tracker.draw_instructions
             else:
                 self.point_data = None
                 draw_instructions = None
 
-
             frame_packet = FramePacket(
                 port=self.port,
                 frame_time=self.frame_time,
                 frame=self.frame,
                 # frame_index=self.frame_index,
                 points=self.point_data,
-                draw_instructions=draw_instructions
+                draw_instructions=draw_instructions,
             )
-            
 
             logger.debug(
                 f"Placing frame on reel {self.port} for frame time: {self.frame_time} and frame index: {self.frame_index}"
             )
 
             for q in self.subscribers:
                 q.put(frame_packet)
@@ -214,16 +223,18 @@
         tracker: Tracker = None,
     ):
         self.streams = {}
         self.camera_array = config.get_camera_array()
 
         for port, camera in self.camera_array.cameras.items():
             # tracker: Tracker = tracker.value()
+            rotation_count = camera.rotation_count
+            size = camera.size
             self.streams[port] = RecordedStream(
-                camera, directory, fps_target=fps_target, tracker=tracker
+                directory, port,size, rotation_count, fps_target=fps_target, tracker=tracker
             )
 
     def play_videos(self):
         for port, stream in self.streams.items():
             stream.play_video()
```

### Comparing `pyxy3d-0.1.8/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.1.9/pyxy3d/recording/video_recorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         """
         # create a dictionary of videowriters
         self.video_writers = {}
         for port, stream in self.synchronizer.streams.items():
             path = str(Path(self.destination_folder, f"port_{port}{self.suffix}.mp4"))
             logger.info(f"Building video writer for port {port}; recording to {path}")
             fourcc = cv2.VideoWriter_fourcc(*"MP4V")
-            frame_size = stream.camera.size
-
+            frame_size = stream.size
+            logger.info(f"Creating video writer with fps of {stream.fps} and frame size of {frame_size}")
             writer = cv2.VideoWriter(path, fourcc, stream.fps, frame_size)
             self.video_writers[port] = writer
 
     def save_data_worker(self, include_video: bool, show_points: bool, store_point_history:bool):
         # connect video recorder to synchronizer via an "in" queue
         if include_video:
             self.build_video_writers()
@@ -113,15 +113,18 @@
                         frame = frame_packet.frame
 
                     # frame_index = frame_packet.frame_index
                     frame_time = frame_packet.frame_time
 
                     if include_video:
                         # store the frame
-                        logger.debug("Writing frame")
+                        if self.sync_index %50==0:
+                            logger.info(f"Writing frame for port {port} and sync index {self.sync_index}")
+                            logger.info(f"frame size  {frame.shape}")
+                    
                         self.video_writers[port].write(frame)
 
                         # store to assocated data in the dictionary
                         self.frame_history["sync_index"].append(self.sync_index)
                         self.frame_history["port"].append(port)
                         # self.frame_history["frame_index"].append(frame_index)
                         self.frame_history["frame_time"].append(frame_time)
@@ -139,14 +142,15 @@
                 # self.sync_packet_in_q = Queue(-1)
                 # self.recording_stop_signal.emit()
 
         # a proper release is strictly necessary to ensure file is readable
         if include_video:
             logger.info("releasing video writers...")
             for port in self.synchronizer.ports:
+                logger.info(f"releasing video writer for port {port}")
                 self.video_writers[port].release()
 
             # del self.video_writers
 
             logger.info("Initiate storing of frame history")
             self.store_frame_history()
```

### Comparing `pyxy3d-0.1.8/pyxy3d/session/session.py` & `pyxy3d-0.1.9/pyxy3d/session/session.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/trackers/charuco_tracker.py` & `pyxy3d-0.1.9/pyxy3d/trackers/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/trackers/hand_tracker.py` & `pyxy3d-0.1.9/pyxy3d/trackers/hand_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/trackers/helper.py` & `pyxy3d-0.1.9/pyxy3d/trackers/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/trackers/holistic_opensim_tracker.py` & `pyxy3d-0.1.9/pyxy3d/trackers/holistic_opensim_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/trackers/holistic_tracker.py` & `pyxy3d-0.1.9/pyxy3d/trackers/holistic_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/trackers/pose_tracker.py` & `pyxy3d-0.1.9/pyxy3d/trackers/pose_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/trackers/tracker_enum.py` & `pyxy3d-0.1.9/pyxy3d/trackers/tracker_enum.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.1.9/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.1.9/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/triangulate/sync_packet_triangulator.py` & `pyxy3d-0.1.9/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/pyxy3d/triangulate/triangulation.py` & `pyxy3d-0.1.9/pyxy3d/triangulate/triangulation.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.1.8/README.md` & `pyxy3d-0.1.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 
 Pyxy3D (*pixie-3d*) is an open-source motion capture tool that allows for markerless motion tracking with a typical computer (Windows or MacOS currently) and 2 or more webcams. In other words, it is a **Py**thon package for converting 2D **(x,y)** point data to **3D** estimates. It's core functionality includes: 
 
 - the estimation of intrinsic (focal length/optical center/distortion) and extrinsic (rotation and translation) camera parameters via a GUI
 - API for slotting various tracking solutions into the data pipeline
 - triangulation of tracked points
 
-The package comes included with a sample tracker using Google's Mediapipe which illustrates how to use the tracker API and provides markerless motion tracking capacity. The camera management backend allows for recording of synchronized frames from connected webcams. The frame rate, resolution and number of cameras combine to create a pixel processing rate that will ultimately hit a limit for any given hardware configuration. A long term goal of this project is developing integrated open-source hardware that will allow for arbitrary system scalability, but in the meantime, you will need to decide on a balance of resolution, fps and camera count for your given needs.
-
+The package comes included with a sample tracker using Google's Mediapipe which illustrates how to use the tracker API and provides markerless motion tracking capacity. The camera management backend allows for recording of synchronized frames from connected webcams. The frame rate, resolution and number of cameras combine to create a pixel processing rate that will ultimately hit a limit for any given hardware configuration. A long term goal of this project is developing integrated open-source hardware that will allow for arbitrary system scalability, but in the meantime, you will need to decide on a balance of resolution, fps and camera count for your given needs
 
 The gif below gives a quick demo of the following steps:
 1. Single Camera Calibration
 2. Multicamera Calibration
 3. Synchronized Recording
 4. Post-processing with Mediapipe Holistic
 5. Visualization of triangulated results
@@ -83,15 +82,15 @@
 - Triangulation of tracked landmarks
 - Visualization of triangulated points for quick confirmation of output quality
 - Currently exporting to `.csv` and `.trc` file formats
 
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
-- It does not support anything other than standard webcams at the moment 
+- It does not support anything other than standard webcams at the moment (a pipeline for processing pre-recorded videos is in the works).
 - The frame capture backend presents a primary bottleneck that will limit the number of cameras/resolution/frame rates that can be used, which ultimately limits the size and precision of the capture volume.
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
 
 
 ## Reporting Issues and Requesting Features
```

### Comparing `pyxy3d-0.1.8/PKG-INFO` & `pyxy3d-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: pyxy3d
-Version: 0.1.8
+Version: 0.1.9
 Summary: A package for calibrating standard webcams to enable 3d motion tracking
 License: AGPL-3.0-only
 Author: Mac Prible
 Author-email: prible@gmail.com
 Requires-Python: >=3.10,<3.10.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyOpenGL (>=3.1.6,<4.0.0)
 Requires-Dist: mediapipe (==0.10.1)
 Requires-Dist: numba (>=0.56.4,<0.57.0)
-Requires-Dist: opencv-contrib-python (>=4.7,<5.0)
+Requires-Dist: opencv-contrib-python (>=4.8.0.74,<5.0.0.0)
 Requires-Dist: pandas (>=1.5.0,<2.0.0)
+Requires-Dist: plotnine (>=0.12.2,<0.13.0)
+Requires-Dist: polars (>=0.18.11,<0.19.0)
+Requires-Dist: pyarrow (>=12.0.1,<13.0.0)
 Requires-Dist: pyqtdarktheme (>=2.1.0,<3.0.0)
 Requires-Dist: pyqtgraph (>=0.13.2,<0.14.0)
 Requires-Dist: pyside6 (>=6.5.2,<7.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Project-URL: repository, https://github.com/mprib/pyxy3d
 Description-Content-Type: text/markdown
@@ -37,16 +40,15 @@
 
 Pyxy3D (*pixie-3d*) is an open-source motion capture tool that allows for markerless motion tracking with a typical computer (Windows or MacOS currently) and 2 or more webcams. In other words, it is a **Py**thon package for converting 2D **(x,y)** point data to **3D** estimates. It's core functionality includes: 
 
 - the estimation of intrinsic (focal length/optical center/distortion) and extrinsic (rotation and translation) camera parameters via a GUI
 - API for slotting various tracking solutions into the data pipeline
 - triangulation of tracked points
 
-The package comes included with a sample tracker using Google's Mediapipe which illustrates how to use the tracker API and provides markerless motion tracking capacity. The camera management backend allows for recording of synchronized frames from connected webcams. The frame rate, resolution and number of cameras combine to create a pixel processing rate that will ultimately hit a limit for any given hardware configuration. A long term goal of this project is developing integrated open-source hardware that will allow for arbitrary system scalability, but in the meantime, you will need to decide on a balance of resolution, fps and camera count for your given needs.
-
+The package comes included with a sample tracker using Google's Mediapipe which illustrates how to use the tracker API and provides markerless motion tracking capacity. The camera management backend allows for recording of synchronized frames from connected webcams. The frame rate, resolution and number of cameras combine to create a pixel processing rate that will ultimately hit a limit for any given hardware configuration. A long term goal of this project is developing integrated open-source hardware that will allow for arbitrary system scalability, but in the meantime, you will need to decide on a balance of resolution, fps and camera count for your given needs
 
 The gif below gives a quick demo of the following steps:
 1. Single Camera Calibration
 2. Multicamera Calibration
 3. Synchronized Recording
 4. Post-processing with Mediapipe Holistic
 5. Visualization of triangulated results
@@ -107,15 +109,15 @@
 - Triangulation of tracked landmarks
 - Visualization of triangulated points for quick confirmation of output quality
 - Currently exporting to `.csv` and `.trc` file formats
 
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
-- It does not support anything other than standard webcams at the moment 
+- It does not support anything other than standard webcams at the moment (a pipeline for processing pre-recorded videos is in the works).
 - The frame capture backend presents a primary bottleneck that will limit the number of cameras/resolution/frame rates that can be used, which ultimately limits the size and precision of the capture volume.
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
 
 
 ## Reporting Issues and Requesting Features
```

