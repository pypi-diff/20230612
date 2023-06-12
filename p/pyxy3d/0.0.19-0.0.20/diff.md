# Comparing `tmp/pyxy3d-0.0.19.tar.gz` & `tmp/pyxy3d-0.0.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.0.19.tar", max compression
+gzip compressed data, was "pyxy3d-0.0.20.tar", max compression
```

## Comparing `pyxy3d-0.0.19.tar` & `pyxy3d-0.0.20.tar`

### file list

```diff
@@ -1,233 +1,233 @@
--rw-r--r--   0        0        0    35184 2023-03-13 23:46:36.918754 pyxy3d-0.0.19/LICENSE.md
--rw-r--r--   0        0        0      925 2023-06-12 17:18:54.002781 pyxy3d-0.0.19/pyproject.toml
--rw-r--r--   0        0        0     2007 2023-05-20 12:18:55.240529 pyxy3d-0.0.19/pyxy3d/__init__.py
--rw-r--r--   0        0        0      934 2023-06-12 16:51:54.169618 pyxy3d-0.0.19/pyxy3d/__main__.py
--rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
--rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
--rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     7208 2023-06-12 15:03:14.886290 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
--rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
--rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
--rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
--rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
--rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
--rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
--rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
--rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
--rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
--rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
--rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.0.19/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.0.19/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.0.19/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.0.19/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
--rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
--rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
--rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
--rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
--rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
--rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
--rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
--rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
--rw-r--r--   0        0        0    11255 2023-06-10 20:05:09.592548 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
--rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
--rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.0.19/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.0.19/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.0.19/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.0.19/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    15573 2023-06-10 20:04:49.722607 pyxy3d-0.0.19/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.0.19/pyxy3d/configurator.py
--rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.0.19/pyxy3d/export.py
--rw-r--r--   0        0        0     3538 2023-06-12 15:03:16.496290 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5645 2023-06-10 20:05:11.196557 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
--rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8098 2023-06-12 15:03:15.902289 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main.cpython-310.pyc
--rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0    10204 2023-06-12 15:03:16.485299 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
--rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
--rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
--rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
--rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
--rw-r--r--   0        0        0    11941 2023-06-12 16:32:28.139452 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
--rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
--rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
--rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
--rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
--rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
--rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
--rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.0.19/pyxy3d/gui/calibrate_capture_volume_widget.py
--rw-r--r--   0        0        0     7438 2023-06-12 17:07:44.747202 pyxy3d-0.0.19/pyxy3d/gui/calibration_widget.py
--rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
--rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
--rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
--rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
--rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
--rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
--rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.0.19/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.0.19/pyxy3d/gui/camera_config/camera_summary_widget.py
--rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.0.19/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.0.19/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
--rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.0.19/pyxy3d/gui/charuco_widget.py
--rw-r--r--   0        0        0    10279 2023-06-12 16:49:05.520130 pyxy3d-0.0.19/pyxy3d/gui/extrinsic_calibration_widget.py
--rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
--rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0     9807 2023-06-02 14:30:41.606273 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
--rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
--rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    14193 2023-06-02 00:29:03.392704 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/paired_frame_builder.py
--rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.0.19/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.0.19/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.0.19/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.0.19/pyxy3d/gui/log_widget.py
--rw-r--r--   0        0        0    14273 2023-06-12 16:49:05.521130 pyxy3d-0.0.19/pyxy3d/gui/main_widget.py
--rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.0.19/pyxy3d/gui/navigation_bars.py
--rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.0.19/pyxy3d/gui/playback_widget.py
--rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.0.19/pyxy3d/gui/post_processing_widget.py
--rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.0.19/pyxy3d/gui/progress_dialog.py
--rw-r--r--   0        0        0    14618 2023-06-12 16:49:05.522130 pyxy3d-0.0.19/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
--rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
--rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
--rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
--rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
--rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
--rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.0.19/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.0.19/pyxy3d/gui/vizualize/playback_triangulation_widget.py
--rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.0.19/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
--rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.0.19/pyxy3d/helper.py
--rw-r--r--   0        0        0     6646 2023-06-01 14:21:56.755811 pyxy3d-0.0.19/pyxy3d/interface.py
--rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.0.19/pyxy3d/logger.py
--rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.0.19/pyxy3d/post_processor.py
--rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.0.19/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
--rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.0.19/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
--rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.0.19/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
--rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.0.19/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
--rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.0.19/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.0.19/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.0.19/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
--rw-r--r--   0        0        0    15991 2023-06-12 15:10:34.851320 pyxy3d-0.0.19/pyxy3d/session/__pycache__/session.cpython-310.pyc
--rw-r--r--   0        0        0    20797 2023-06-12 16:49:05.524130 pyxy3d-0.0.19/pyxy3d/session/session.py
--rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.0.19/pyxy3d/trackers/__init__.py
--rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
--rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
--rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.0.19/pyxy3d/trackers/charuco_tracker.py
--rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.0.19/pyxy3d/trackers/hand_tracker.py
--rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.0.19/pyxy3d/trackers/helper.py
--rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.0.19/pyxy3d/trackers/holistic_opensim_tracker.py
--rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.0.19/pyxy3d/trackers/holistic_tracker.py
--rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.0.19/pyxy3d/trackers/pose_tracker.py
--rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.0.19/pyxy3d/trackers/tracker_enum.py
--rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
--rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
--rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
--rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
--rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
--rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
--rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
--rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
--rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
--rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
--rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
--rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
--rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
--rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
--rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
--rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
--rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
--rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
--rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
--rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
--rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
--rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
--rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
--rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
--rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
--rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
--rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
--rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
--rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
--rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
--rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
--rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
--rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
--rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
--rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
--rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
--rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
--rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
--rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
--rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
--rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
--rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
--rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
--rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
--rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
--rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
--rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.0.19/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.0.19/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.0.19/pyxy3d/triangulate/sync_packet_triangulator.py
--rw-r--r--   0        0        0     8240 2023-06-12 17:10:55.916740 pyxy3d-0.0.19/README.md
--rw-r--r--   0        0        0     9057 1970-01-01 00:00:00.000000 pyxy3d-0.0.19/PKG-INFO
+-rw-r--r--   0        0        0    35184 2023-03-13 23:46:36.918754 pyxy3d-0.0.20/LICENSE.md
+-rw-r--r--   0        0        0      925 2023-06-12 19:45:40.581459 pyxy3d-0.0.20/pyproject.toml
+-rw-r--r--   0        0        0     2007 2023-05-20 12:18:55.240529 pyxy3d-0.0.20/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      934 2023-06-12 16:51:54.169618 pyxy3d-0.0.20/pyxy3d/__main__.py
+-rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     7208 2023-06-12 18:45:04.367154 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
+-rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
+-rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
+-rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
+-rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
+-rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.0.20/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.0.20/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.0.20/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.0.20/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
+-rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
+-rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
+-rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
+-rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
+-rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
+-rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
+-rw-r--r--   0        0        0    11255 2023-06-10 20:05:09.592548 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
+-rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.0.20/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.0.20/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.0.20/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.0.20/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    15573 2023-06-10 20:04:49.722607 pyxy3d-0.0.20/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.0.20/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.0.20/pyxy3d/export.py
+-rw-r--r--   0        0        0     3538 2023-06-12 18:45:08.762112 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5684 2023-06-12 18:45:02.565389 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
+-rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8098 2023-06-12 18:45:07.819053 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0    10204 2023-06-12 18:45:08.757113 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
+-rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
+-rw-r--r--   0        0        0    11941 2023-06-12 18:45:08.751113 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
+-rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.0.20/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0     7438 2023-06-12 17:07:44.747202 pyxy3d-0.0.20/pyxy3d/gui/calibration_widget.py
+-rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
+-rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
+-rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
+-rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
+-rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
+-rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.0.20/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.0.20/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.0.20/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.0.20/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.0.20/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    10279 2023-06-12 16:49:05.520130 pyxy3d-0.0.20/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     9807 2023-06-02 14:30:41.606273 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    14193 2023-06-02 00:29:03.392704 pyxy3d-0.0.20/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.0.20/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.0.20/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.0.20/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.0.20/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    14273 2023-06-12 16:49:05.521130 pyxy3d-0.0.20/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.0.20/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.0.20/pyxy3d/gui/playback_widget.py
+-rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.0.20/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.0.20/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    14618 2023-06-12 16:49:05.522130 pyxy3d-0.0.20/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
+-rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
+-rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
+-rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
+-rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.0.20/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.0.20/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.0.20/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.0.20/pyxy3d/helper.py
+-rw-r--r--   0        0        0     6646 2023-06-01 14:21:56.755811 pyxy3d-0.0.20/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.0.20/pyxy3d/logger.py
+-rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.0.20/pyxy3d/post_processor.py
+-rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.0.20/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.0.20/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.0.20/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
+-rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.0.20/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
+-rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.0.20/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.0.20/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.0.20/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
+-rw-r--r--   0        0        0    15991 2023-06-12 18:45:02.579375 pyxy3d-0.0.20/pyxy3d/session/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0    20797 2023-06-12 16:49:05.524130 pyxy3d-0.0.20/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.0.20/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
+-rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.0.20/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.0.20/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.0.20/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.0.20/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.0.20/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.0.20/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.0.20/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
+-rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
+-rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
+-rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
+-rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
+-rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
+-rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
+-rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
+-rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
+-rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
+-rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
+-rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
+-rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
+-rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
+-rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
+-rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
+-rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
+-rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
+-rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
+-rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
+-rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
+-rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
+-rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
+-rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
+-rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
+-rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
+-rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
+-rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
+-rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
+-rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
+-rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
+-rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
+-rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
+-rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.0.20/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.0.20/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.0.20/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     9401 2023-06-12 19:45:15.810322 pyxy3d-0.0.20/README.md
+-rw-r--r--   0        0        0    10203 1970-01-01 00:00:00.000000 pyxy3d-0.0.20/PKG-INFO
```

### Comparing `pyxy3d-0.0.19/LICENSE.md` & `pyxy3d-0.0.20/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyproject.toml` & `pyxy3d-0.0.20/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyxy3d"
-version = "0.0.19"
+version = "0.0.20"
 description = "A package for calibrating standard webcams to enable 3d motion tracking"
 authors = ["Mac Prible <prible@gmail.com>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10, <3.12"
```

### Comparing `pyxy3d-0.0.19/pyxy3d/__init__.py` & `pyxy3d-0.0.20/pyxy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/__main__.py` & `pyxy3d-0.0.20/pyxy3d/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 14:52:15 2023 UTC, .py size: 9886 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1f31 8764 9e26 0000  o........1.d.&..
+00000000: 6f0d 0d0a 0000 0000 814c 8764 9e26 0000  o........L.d.&..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 1002 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6400 6401 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
 00000070: 6401 6c0c 5a0d 6400 6401 6c0e 6d0f 0200  d.l.Z.d.d.l.m...
```

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.0.20/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/charuco.py` & `pyxy3d-0.0.20/pyxy3d/calibration/charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.0.20/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.0.20/pyxy3d/calibration/monocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.0.20/pyxy3d/calibration/stereocalibrator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/camera.py` & `pyxy3d-0.0.20/pyxy3d/cameras/camera.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.0.20/pyxy3d/cameras/camera_array.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.0.20/pyxy3d/cameras/camera_array_initializer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.0.20/pyxy3d/cameras/live_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.0.20/pyxy3d/cameras/synchronizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/configurator.py` & `pyxy3d-0.0.20/pyxy3d/configurator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/export.py` & `pyxy3d-0.0.20/pyxy3d/export.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 14:34:40 2023 UTC, .py size: 4052 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 002d 8764 d40f 0000  o........-.d....
+00000000: 6f0d 0d0a 0000 0000 814c 8764 d40f 0000  o........L.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1001 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6401 6c07 5a07 6400 6401 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 5a08 6400 6402 6c09 6d0a 5a0a 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6403 6c0b 6d0c 5a0c 0100 6400 6404 6c0d  d.l.m.Z...d.d.l.
```

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Sat Jun 10 20:04:49 2023 UTC, .py size: 7374 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 61d7 8464 ce1c 0000  o.......a..d....
+00000000: 6f0d 0d0a 0000 0000 e050 8764 0e1d 0000  o........P.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 1e01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6401 6c07 5a07 6400 6401 6c08  Z.d.d.l.Z.d.d.l.
 00000060: 5a08 6400 6402 6c09 6d0a 5a0a 0100 6400  Z.d.d.l.m.Z...d.
 00000070: 6403 6c0b 6d0c 5a0c 0100 6400 6404 6c0d  d.l.m.Z...d.d.l.
@@ -73,16 +73,16 @@
 00000480: 7469 6e67 2063 6861 7275 636f 2077 697a  ting charuco wiz
 00000490: 6172 6420 7365 7373 696f 6e7a 1541 6464  ard sessionz.Add
 000004a0: 696e 6720 6368 6172 7563 6f20 7769 7a61  ing charuco wiza
 000004b0: 7264 7a25 5365 7474 696e 6720 696e 6465  rdz%Setting inde
 000004c0: 7820 746f 2032 2074 6f20 6163 7469 7661  x to 2 to activa
 000004d0: 7465 2077 6964 6765 7429 1cda 0573 7570  te widget)...sup
 000004e0: 6572 da08 5f5f 696e 6974 5f5f 5a0f 4341  er..__init__Z.CA
-000004f0: 4d53 5f49 4e5f 5052 4f43 4553 53da 0e73  MS_IN_PROCESS..s
-00000500: 6574 5769 6e64 6f77 5469 746c 65da 0d73  etWindowTitle..s
+000004f0: 4d53 5f49 4e5f 5052 4f43 4553 535a 0e73  MS_IN_PROCESSZ.s
+00000500: 6574 5769 6e64 6f77 5469 746c 655a 0d73  etWindowTitleZ.s
 00000510: 6574 5769 6e64 6f77 4963 6f6e 7206 0000  etWindowIconr...
 00000520: 00da 0373 7472 7202 0000 0072 1300 0000  ...strr....r....
 00000530: da04 7061 7468 da0c 7365 7373 696f 6e5f  ..path..session_
 00000540: 7061 7468 721b 0000 00da 0663 6f6e 6669  pathr......confi
 00000550: 67da 066c 6f67 6765 72da 0469 6e66 6f72  g..logger..infor
 00000560: 1100 0000 da0e 7769 7a61 7264 5f63 6861  ......wizard_cha
 00000570: 7275 636f da0e 6e61 7669 6761 7469 6f6e  ruco..navigation
@@ -103,17 +103,17 @@
 00000660: 7769 6467 6574 2e70 7972 1d00 0000 2800  widget.pyr....(.
 00000670: 0000 7324 0000 000a 0106 010a 0218 0108  ..s$............
 00000680: 0106 0108 010a 030c 010c 0204 0104 ff0a  ................
 00000690: 030e 010c 010a 020c 010c 027a 1a43 616c  ...........z.Cal
 000006a0: 6962 7261 7469 6f6e 5769 6467 6574 2e5f  ibrationWidget._
 000006b0: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
 000006c0: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
-000006d0: 7304 0000 0064 0053 00a9 014e 7233 0000  s....d.S...Nr3..
-000006e0: 00a9 0172 3000 0000 7233 0000 0072 3300  ...r0...r3...r3.
-000006f0: 0000 7234 0000 0072 2f00 0000 4200 0000  ..r4...r/...B...
+000006d0: 7304 0000 0064 0053 00a9 014e 7231 0000  s....d.S...Nr1..
+000006e0: 00a9 0172 2e00 0000 7231 0000 0072 3100  ...r....r1...r1.
+000006f0: 0000 7232 0000 0072 2d00 0000 4200 0000  ..r2...r-...B...
 00000700: 7302 0000 0004 037a 2143 616c 6962 7261  s......z!Calibra
 00000710: 7469 6f6e 5769 6467 6574 2e63 6f6e 6e65  tionWidget.conne
 00000720: 6374 5f77 6964 6765 7473 6301 0000 0000  ct_widgetsc.....
 00000730: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
 00000740: 0000 0073 6e00 0000 7c00 6a00 a001 7402  ...sn...|.j...t.
 00000750: 6a03 a101 0100 7404 7c00 6401 8302 7325  j.....t.|.d...s%
 00000760: 7405 a006 6402 a101 0100 7407 7c00 6a00  t...d.....t.|.j.
@@ -126,34 +126,34 @@
 000007d0: 5f77 6964 6765 747a 2d4e 6f20 6361 6d65  _widgetz-No came
 000007e0: 7261 2063 6f6e 6669 6775 7261 7469 6f6e  ra configuration
 000007f0: 2079 6574 2e2e 2e63 7265 6174 696e 6720   yet...creating 
 00000800: 7769 7a61 7264 7a3a 4361 6d65 7261 2063  wizardz:Camera c
 00000810: 6f6e 6669 6720 616c 7265 6164 7920 6578  onfig already ex
 00000820: 6973 7473 3b20 6368 616e 6769 6e67 2073  ists; changing s
 00000830: 7461 636b 2063 7572 7265 6e74 2069 6e64  tack current ind
-00000840: 6578 290c 721b 0000 0072 2b00 0000 7210  ex).r....r+...r.
-00000850: 0000 00da 1449 6e74 7269 6e73 6963 4361  .....IntrinsicCa
+00000840: 6578 290c 721b 0000 0072 2900 0000 7210  ex).r....r)...r.
+00000850: 0000 005a 1449 6e74 7269 6e73 6963 4361  ...Z.IntrinsicCa
 00000860: 6c69 6272 6174 696f 6eda 0768 6173 6174  libration..hasat
-00000870: 7472 7224 0000 0072 2500 0000 7212 0000  trr$...r%...r...
-00000880: 0072 3700 0000 722d 0000 0072 2e00 0000  .r7...r-...r....
-00000890: da17 6163 7469 7661 7465 5f6d 6f6e 6f63  ..activate_monoc
-000008a0: 616c 6962 7261 746f 7272 3600 0000 7233  alibratorr6...r3
-000008b0: 0000 0072 3300 0000 7234 0000 0072 2a00  ...r3...r4...r*.
+00000870: 7472 7222 0000 0072 2300 0000 7212 0000  trr"...r#...r...
+00000880: 0072 3500 0000 722b 0000 0072 2c00 0000  .r5...r+...r,...
+00000890: 5a17 6163 7469 7661 7465 5f6d 6f6e 6f63  Z.activate_monoc
+000008a0: 616c 6962 7261 746f 7272 3400 0000 7231  alibratorr4...r1
+000008b0: 0000 0072 3100 0000 7232 0000 0072 2800  ...r1...r2...r(.
 000008c0: 0000 4900 0000 7312 0000 000e 010a 010a  ..I...s.........
 000008d0: 010c 010c 0110 010a 080c 030e 017a 2843  .............z(C
 000008e0: 616c 6962 7261 7469 6f6e 5769 6467 6574  alibrationWidget
 000008f0: 2e61 6374 6976 6174 655f 6361 6d65 7261  .activate_camera
 00000900: 5f63 6f6e 6669 6763 0100 0000 0000 0000  _configc........
 00000910: 0000 0000 0100 0000 0300 0000 4300 0000  ............C...
 00000920: 731e 0000 007c 006a 00a0 0174 026a 03a1  s....|.j...t.j..
 00000930: 0101 007c 00a0 047c 006a 05a1 0101 0064  ...|...|.j.....d
-00000940: 0053 0072 3500 0000 2906 721b 0000 0072  .S.r5...).r....r
-00000950: 2b00 0000 7210 0000 0072 2c00 0000 722e  +...r....r,...r.
-00000960: 0000 0072 2600 0000 7236 0000 0072 3300  ...r&...r6...r3.
-00000970: 0000 7233 0000 0072 3400 0000 da17 6163  ..r3...r4.....ac
+00000940: 0053 0072 3300 0000 2906 721b 0000 0072  .S.r3...).r....r
+00000950: 2900 0000 7210 0000 0072 2a00 0000 722c  )...r....r*...r,
+00000960: 0000 0072 2400 0000 7234 0000 0072 3100  ...r$...r4...r1.
+00000970: 0000 7231 0000 0072 3200 0000 da17 6163  ..r1...r2.....ac
 00000980: 7469 7661 7465 5f63 6861 7275 636f 5f77  tivate_charuco_w
 00000990: 697a 6172 645e 0000 0073 0400 0000 0e01  izard^...s......
 000009a0: 1001 7a29 4361 6c69 6272 6174 696f 6e57  ..z)CalibrationW
 000009b0: 6964 6765 742e 6163 7469 7661 7465 5f63  idget.activate_c
 000009c0: 6861 7275 636f 5f77 697a 6172 6463 0100  haruco_wizardc..
 000009d0: 0000 0000 0000 0000 0000 0100 0000 0300  ................
 000009e0: 0000 4300 0000 7384 0000 007c 006a 00a0  ..C...s....|.j..
@@ -163,28 +163,28 @@
 00000a20: 00a0 087c 006a 06a1 0101 007c 00a0 057c  ...|.j.....|...|
 00000a30: 006a 06a1 0101 007c 006a 066a 096a 0a6a  .j.....|.j.j.j.j
 00000a40: 0ba0 0c7c 006a 0da1 0101 007c 006a 066a  ...|.j.....|.j.j
 00000a50: 0ea0 0c7c 006a 0fa1 0101 007c 006a 066a  ...|.j.....|.j.j
 00000a60: 10a0 0c7c 006a 11a1 0101 0064 0053 0029  ...|.j.....d.S.)
 00000a70: 024e da1c 6578 7472 696e 7369 635f 6361  .N..extrinsic_ca
 00000a80: 6c69 6272 6174 696f 6e5f 7769 6467 6574  libration_widget
-00000a90: 2912 721b 0000 0072 2b00 0000 7210 0000  ).r....r+...r...
+00000a90: 2912 721b 0000 0072 2900 0000 7210 0000  ).r....r)...r...
 00000aa0: 00da 1445 7874 7269 6e73 6963 4361 6c69  ...ExtrinsicCali
-00000ab0: 6272 6174 696f 6e72 3900 0000 722e 0000  brationr9...r...
-00000ac0: 0072 3c00 0000 7216 0000 0072 2d00 0000  .r<...r....r-...
-00000ad0: 7227 0000 00da 0862 6163 6b5f 6274 6e72  r'.....back_btnr
-00000ae0: 2800 0000 7229 0000 00da 1c62 6163 6b5f  (...r).....back_
+00000ab0: 6272 6174 696f 6e72 3600 0000 722c 0000  brationr6...r,..
+00000ac0: 0072 3800 0000 7216 0000 0072 2b00 0000  .r8...r....r+...
+00000ad0: 7225 0000 00da 0862 6163 6b5f 6274 6e72  r%.....back_btnr
+00000ae0: 2600 0000 7227 0000 00da 1c62 6163 6b5f  &...r'.....back_
 00000af0: 746f 5f63 616d 6572 615f 636f 6e66 6967  to_camera_config
 00000b00: 5f77 697a 6172 645a 1463 616c 6962 7261  _wizardZ.calibra
 00000b10: 7469 6f6e 5f63 6f6d 706c 6574 65da 166e  tion_complete..n
 00000b20: 6578 745f 746f 5f63 6170 7475 7265 5f76  ext_to_capture_v
-00000b30: 6f6c 756d 65da 0974 6572 6d69 6e61 7465  olume..terminate
+00000b30: 6f6c 756d 655a 0974 6572 6d69 6e61 7465  olumeZ.terminate
 00000b40: da13 7265 6672 6573 685f 7374 6572 656f  ..refresh_stereo
-00000b50: 6672 616d 6572 3600 0000 7233 0000 0072  framer6...r3...r
-00000b60: 3300 0000 7234 0000 00da 136e 6578 745f  3...r4.....next_
+00000b50: 6672 616d 6572 3400 0000 7231 0000 0072  framer4...r1...r
+00000b60: 3100 0000 7232 0000 00da 136e 6578 745f  1...r2.....next_
 00000b70: 746f 5f73 7465 7265 6f66 7261 6d65 6200  to_stereoframeb.
 00000b80: 0000 7316 0000 000e 010a 0210 010c 040c  ..s.............
 00000b90: 010c 010c 0204 0104 ff10 0414 027a 2543  .............z%C
 00000ba0: 616c 6962 7261 7469 6f6e 5769 6467 6574  alibrationWidget
 00000bb0: 2e6e 6578 745f 746f 5f73 7465 7265 6f66  .next_to_stereof
 00000bc0: 7261 6d65 6301 0000 0000 0000 0000 0000  ramec...........
 00000bd0: 0001 0000 0003 0000 0043 0000 0073 5200  .........C...sR.
@@ -195,47 +195,47 @@
 00000c20: a001 6403 a101 0100 7c00 a008 a100 0100  ..d.....|.......
 00000c30: 6400 5300 2904 4efa 2853 6574 2063 7572  d.S.).N.(Set cur
 00000c40: 7265 6e74 2077 6964 6765 7420 746f 2063  rent widget to c
 00000c50: 6f6e 6669 6720 7465 6d70 6f72 6172 696c  onfig temporaril
 00000c60: 79fa 1252 656d 6f76 6520 7374 6572 656f  y..Remove stereo
 00000c70: 6672 616d 65fa 1643 7265 6174 6520 6e65  frame..Create ne
 00000c80: 7720 7374 6572 656f 6672 616d 6529 0972  w stereoframe).r
-00000c90: 2400 0000 7225 0000 0072 2e00 0000 7237  $...r%...r....r7
+00000c90: 2200 0000 7223 0000 0072 2c00 0000 7235  "...r#...r,...r5
 00000ca0: 0000 00da 0c72 656d 6f76 6557 6964 6765  .....removeWidge
-00000cb0: 7472 3c00 0000 da0d 6672 616d 655f 6275  tr<.....frame_bu
+00000cb0: 7472 3800 0000 da0d 6672 616d 655f 6275  tr8.....frame_bu
 00000cc0: 696c 6465 72da 1d75 6e73 7562 7363 7269  ilder..unsubscri
 00000cd0: 6265 5f66 726f 6d5f 7379 6e63 6872 6f6e  be_from_synchron
 00000ce0: 697a 6572 da16 6c61 756e 6368 5f6e 6577  izer..launch_new
-00000cf0: 5f73 7465 7265 6f66 7261 6d65 7236 0000  _stereoframer6..
-00000d00: 0072 3300 0000 7233 0000 0072 3400 0000  .r3...r3...r4...
-00000d10: 7242 0000 0077 0000 0073 1000 0000 0a01  rB...w...s......
+00000cf0: 5f73 7465 7265 6f66 7261 6d65 7234 0000  _stereoframer4..
+00000d00: 0072 3100 0000 7231 0000 0072 3200 0000  .r1...r1...r2...
+00000d10: 723d 0000 0077 0000 0073 1000 0000 0a01  r=...w...s......
 00000d20: 0c01 0a02 0c01 0c01 0401 0a02 0c01 7a25  ..............z%
 00000d30: 4361 6c69 6272 6174 696f 6e57 6964 6765  CalibrationWidge
 00000d40: 742e 7265 6672 6573 685f 7374 6572 656f  t.refresh_stereo
 00000d50: 6672 616d 6563 0100 0000 0000 0000 0000  framec..........
 00000d60: 0000 0200 0000 0300 0000 4300 0000 735a  ..........C...sZ
 00000d70: 0000 0074 00a0 0164 01a1 0101 007c 00a0  ...t...d.....|..
 00000d80: 027c 006a 03a1 0101 007c 006a 04a0 05a1  .|.j.....|.j....
 00000d90: 0001 007c 006a 066a 07a0 08a1 0001 007c  ...|.j.j.......|
 00000da0: 00a0 097c 006a 06a1 0101 007c 0060 067c  ...|.j.....|.`.|
 00000db0: 006a 036a 0aa0 0ba1 007d 017c 006a 036a  .j.j.....}.|.j.j
 00000dc0: 0aa0 0c7c 01a1 0101 0064 0053 0029 024e  ...|.....d.S.).N
 00000dd0: 7a2d 4d6f 7669 6e67 2062 6163 6b20 746f  z-Moving back to
 00000de0: 2063 616d 6572 6120 636f 6e66 6967 2066   camera config f
 00000df0: 726f 6d20 7374 6572 656f 6672 616d 6529  rom stereoframe)
-00000e00: 0d72 2400 0000 7225 0000 0072 2e00 0000  .r$...r%...r....
-00000e10: 7237 0000 0072 1b00 0000 da12 7061 7573  r7...r......paus
-00000e20: 655f 7379 6e63 6872 6f6e 697a 6572 723c  e_synchronizerr<
-00000e30: 0000 0072 4800 0000 7249 0000 0072 4700  ...rH...rI...rG.
-00000e40: 0000 5a0b 6361 6d65 7261 5f74 6162 73da  ..Z.camera_tabs.
+00000e00: 0d72 2200 0000 7223 0000 0072 2c00 0000  .r"...r#...r,...
+00000e10: 7235 0000 0072 1b00 0000 5a12 7061 7573  r5...r....Z.paus
+00000e20: 655f 7379 6e63 6872 6f6e 697a 6572 7238  e_synchronizerr8
+00000e30: 0000 0072 4300 0000 7244 0000 0072 4200  ...rC...rD...rB.
+00000e40: 0000 5a0b 6361 6d65 7261 5f74 6162 735a  ..Z.camera_tabsZ
 00000e50: 0c63 7572 7265 6e74 496e 6465 785a 1461  .currentIndexZ.a
 00000e60: 6374 6976 6174 655f 6375 7272 656e 745f  ctivate_current_
-00000e70: 7461 6229 0272 3000 0000 da0b 6163 7469  tab).r0.....acti
-00000e80: 7665 5f70 6f72 7472 3300 0000 7233 0000  ve_portr3...r3..
-00000e90: 0072 3400 0000 723f 0000 0084 0000 0073  .r4...r?.......s
+00000e70: 7461 6229 0272 2e00 0000 5a0b 6163 7469  tab).r....Z.acti
+00000e80: 7665 5f70 6f72 7472 3100 0000 7231 0000  ve_portr1...r1..
+00000e90: 0072 3200 0000 723b 0000 0084 0000 0073  .r2...r;.......s
 00000ea0: 1000 0000 0a01 0c01 0a01 0c02 0c01 0401  ................
 00000eb0: 0c02 1201 7a2e 4361 6c69 6272 6174 696f  ....z.Calibratio
 00000ec0: 6e57 6964 6765 742e 6261 636b 5f74 6f5f  nWidget.back_to_
 00000ed0: 6361 6d65 7261 5f63 6f6e 6669 675f 7769  camera_config_wi
 00000ee0: 7a61 7264 6301 0000 0000 0000 0000 0000  zardc...........
 00000ef0: 0001 0000 0003 0000 0043 0000 0073 5e00  .........C...s^.
 00000f00: 0000 7400 a001 6401 a101 0100 7402 7c00  ..t...d.....t.|.
@@ -247,107 +247,110 @@
 00000f60: 2904 4e7a 1e43 7265 6174 696e 6720 4361  ).Nz.Creating Ca
 00000f70: 7074 7572 6520 566f 6c75 6d65 2077 6964  pture Volume wid
 00000f80: 6765 747a 2b41 6464 696e 6720 6361 7074  getz+Adding capt
 00000f90: 7572 6520 766f 6c75 6d65 2077 6964 6765  ure volume widge
 00000fa0: 7420 746f 206d 6169 6e20 5769 7a61 7264  t to main Wizard
 00000fb0: 7a2a 5365 7420 6375 7272 656e 7420 696e  z*Set current in
 00000fc0: 6465 7820 746f 2063 6170 7475 7265 2076  dex to capture v
-00000fd0: 6f6c 756d 6520 7769 6467 6574 290d 7224  olume widget).r$
-00000fe0: 0000 0072 2500 0000 7218 0000 0072 1b00  ...r%...r....r..
+00000fd0: 6f6c 756d 6520 7769 6467 6574 290d 7222  olume widget).r"
+00000fe0: 0000 0072 2300 0000 7218 0000 0072 1b00  ...r#...r....r..
 00000ff0: 0000 da0e 6361 7074 7572 655f 766f 6c75  ....capture_volu
-00001000: 6d65 722d 0000 0072 2e00 0000 7227 0000  mer-...r....r'..
-00001010: 0072 3e00 0000 7228 0000 0072 2900 0000  .r>...r(...r)...
+00001000: 6d65 722b 0000 0072 2c00 0000 7225 0000  mer+...r,...r%..
+00001010: 0072 3a00 0000 7226 0000 0072 2700 0000  .r:...r&...r'...
 00001020: da14 6261 636b 5f74 6f5f 7374 6572 656f  ..back_to_stereo
 00001030: 5f66 7261 6d65 5a09 7174 5f6c 6f67 6765  _frameZ.qt_logge
-00001040: 7272 3600 0000 7233 0000 0072 3300 0000  rr6...r3...r3...
-00001050: 7234 0000 0072 4000 0000 9000 0000 7314  r4...r@.......s.
+00001040: 7272 3400 0000 7231 0000 0072 3100 0000  rr4...r1...r1...
+00001050: 7232 0000 0072 3c00 0000 9000 0000 7314  r2...r<.......s.
 00001060: 0000 000a 010c 010a 010c 010a 010c 010c  ................
 00001070: 0104 0104 ff08 047a 2843 616c 6962 7261  .......z(Calibra
 00001080: 7469 6f6e 5769 6467 6574 2e6e 6578 745f  tionWidget.next_
 00001090: 746f 5f63 6170 7475 7265 5f76 6f6c 756d  to_capture_volum
 000010a0: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
 000010b0: 0000 0300 0000 4300 0000 7376 0000 0074  ......C...sv...t
 000010c0: 00a0 0164 01a1 0101 007c 00a0 027c 006a  ...d.....|...|.j
 000010d0: 03a1 0101 0074 00a0 0164 02a1 0101 007c  .....t...d.....|
 000010e0: 00a0 047c 006a 05a1 0101 0074 00a0 0164  ...|.j.....t...d
 000010f0: 03a1 0101 007c 00a0 047c 006a 06a1 0101  .....|...|.j....
 00001100: 007c 0060 067c 006a 056a 07a0 08a1 0001  .|.`.|.j.j......
 00001110: 007c 0060 0574 00a0 0164 04a1 0101 007c  .|.`.t...d.....|
 00001120: 00a0 09a1 0001 007c 006a 0aa0 0ba1 0001  .......|.j......
-00001130: 0064 0053 0029 054e 7244 0000 0072 4500  .d.S.).NrD...rE.
+00001130: 0064 0053 0029 054e 723f 0000 0072 4000  .d.S.).Nr?...r@.
 00001140: 0000 7a15 5265 6d6f 7665 2063 6170 7475  ..z.Remove captu
-00001150: 7265 2076 6f6c 756d 6572 4600 0000 290c  re volumerF...).
-00001160: 7224 0000 0072 2500 0000 722e 0000 0072  r$...r%...r....r
-00001170: 3700 0000 7247 0000 0072 3c00 0000 724e  7...rG...r<...rN
-00001180: 0000 0072 4800 0000 7249 0000 0072 4a00  ...rH...rI...rJ.
-00001190: 0000 721b 0000 00da 1475 6e70 6175 7365  ..r......unpause
-000011a0: 5f73 796e 6368 726f 6e69 7a65 7272 3600  _synchronizerr6.
-000011b0: 0000 7233 0000 0072 3300 0000 7234 0000  ..r3...r3...r4..
-000011c0: 0072 4f00 0000 9e00 0000 7318 0000 000a  .rO.......s.....
+00001150: 7265 2076 6f6c 756d 6572 4100 0000 290c  re volumerA...).
+00001160: 7222 0000 0072 2300 0000 722c 0000 0072  r"...r#...r,...r
+00001170: 3500 0000 7242 0000 0072 3800 0000 7246  5...rB...r8...rF
+00001180: 0000 0072 4300 0000 7244 0000 0072 4500  ...rC...rD...rE.
+00001190: 0000 721b 0000 005a 1475 6e70 6175 7365  ..r....Z.unpause
+000011a0: 5f73 796e 6368 726f 6e69 7a65 7272 3400  _synchronizerr4.
+000011b0: 0000 7231 0000 0072 3100 0000 7232 0000  ..r1...r1...r2..
+000011c0: 0072 4700 0000 9e00 0000 7318 0000 000a  .rG.......s.....
 000011d0: 010c 010a 020c 010a 010c 0104 010c 0104  ................
 000011e0: 010a 0208 010e 017a 2643 616c 6962 7261  .......z&Calibra
 000011f0: 7469 6f6e 5769 6467 6574 2e62 6163 6b5f  tionWidget.back_
 00001200: 746f 5f73 7465 7265 6f5f 6672 616d 6529  to_stereo_frame)
 00001210: 10da 085f 5f6e 616d 655f 5fda 0a5f 5f6d  ...__name__..__m
 00001220: 6f64 756c 655f 5fda 0c5f 5f71 7561 6c6e  odule__..__qualn
 00001230: 616d 655f 5f72 0500 0000 5a11 6361 6d65  ame__r....Z.came
 00001240: 7261 735f 636f 6e6e 6563 7465 6472 0f00  ras_connectedr..
-00001250: 0000 721d 0000 0072 2f00 0000 722a 0000  ..r....r/...r*..
-00001260: 0072 3b00 0000 7243 0000 0072 4200 0000  .r;...rC...rB...
-00001270: 723f 0000 0072 4000 0000 724f 0000 00da  r?...r@...rO....
-00001280: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7233  .__classcell__r3
-00001290: 0000 0072 3300 0000 7231 0000 0072 3400  ...r3...r1...r4.
+00001250: 0000 721d 0000 0072 2d00 0000 7228 0000  ..r....r-...r(..
+00001260: 0072 3700 0000 723e 0000 0072 3d00 0000  .r7...r>...r=...
+00001270: 723b 0000 0072 3c00 0000 7247 0000 00da  r;...r<...rG....
+00001280: 0d5f 5f63 6c61 7373 6365 6c6c 5f5f 7231  .__classcell__r1
+00001290: 0000 0072 3100 0000 722f 0000 0072 3200  ...r1...r/...r2.
 000012a0: 0000 721a 0000 0025 0000 0073 1600 0000  ..r....%...s....
 000012b0: 0800 0601 1202 081a 0807 0815 0804 0815  ................
-000012c0: 080d 080c 100e 721a 0000 0072 2200 0000  ......r....r"...
+000012c0: 080d 080c 100e 721a 0000 0072 2000 0000  ......r....r ...
 000012d0: 6301 0000 0000 0000 0000 0000 0005 0000  c...............
-000012e0: 0002 0000 0043 0000 0073 3600 0000 7400  .....C...s6...t.
-000012f0: 7c00 8301 7d01 7401 7c01 8301 7d02 7402  |...}.t.|...}.t.
-00001300: 7403 6a04 8301 7d03 7405 7c02 8301 7d04  t.j...}.t.|...}.
-00001310: 7c04 a006 a100 0100 7c03 a007 a100 0100  |.......|.......
-00001320: 6400 5300 7235 0000 0029 0872 1900 0000  d.S.r5...).r....
-00001330: 720f 0000 0072 0900 0000 da03 7379 73da  r....r......sys.
-00001340: 0461 7267 7672 1a00 0000 da04 7368 6f77  .argvr......show
-00001350: da04 6578 6563 2905 7222 0000 0072 2300  ..exec).r"...r#.
-00001360: 0000 721b 0000 00da 0361 7070 da06 7769  ..r......app..wi
-00001370: 6e64 6f77 7233 0000 0072 3300 0000 7234  ndowr3...r3...r4
-00001380: 0000 00da 196c 6175 6e63 685f 6361 6c69  .....launch_cali
-00001390: 6272 6174 696f 6e5f 7769 6467 6574 af00  bration_widget..
-000013a0: 0000 730c 0000 0008 0108 010a 0208 0208  ..s.............
-000013b0: 010c 0172 5b00 0000 292f da0d 7079 7879  ...r[...)/..pyxy
-000013c0: 3364 2e6c 6f67 6765 72da 0670 7978 7933  3d.logger..pyxy3
-000013d0: 6472 2400 0000 da03 6765 7472 5100 0000  dr$.....getrQ...
-000013e0: da02 6f73 7255 0000 00da 0673 6875 7469  ..osrU.....shuti
-000013f0: 6cda 0474 696d 65da 0770 6174 686c 6962  l..time..pathlib
-00001400: 7202 0000 00da 0974 6872 6561 6469 6e67  r......threading
-00001410: 7203 0000 00da 0c50 7951 7436 2e51 7443  r......PyQt6.QtC
-00001420: 6f72 6572 0400 0000 7205 0000 00da 0b50  orer....r......P
-00001430: 7951 7436 2e51 7447 7569 7206 0000 0072  yQt6.QtGuir....r
-00001440: 0700 0000 da0f 5079 5174 362e 5174 5769  ......PyQt6.QtWi
-00001450: 6467 6574 7372 0800 0000 7209 0000 0072  dgetsr....r....r
-00001460: 0a00 0000 720b 0000 0072 0c00 0000 720d  ....r....r....r.
-00001470: 0000 0072 0e00 0000 da16 7079 7879 3364  ...r......pyxy3d
-00001480: 2e73 6573 7369 6f6e 2e73 6573 7369 6f6e  .session.session
-00001490: 720f 0000 0072 1000 0000 da19 7079 7879  r....r......pyxy
-000014a0: 3364 2e67 7569 2e63 6861 7275 636f 5f77  3d.gui.charuco_w
-000014b0: 6964 6765 7472 1100 0000 da35 7079 7879  idgetr.....5pyxy
-000014c0: 3364 2e67 7569 2e63 616d 6572 615f 636f  3d.gui.camera_co
-000014d0: 6e66 6967 2e69 6e74 7269 6e73 6963 5f63  nfig.intrinsic_c
-000014e0: 616c 6962 7261 7469 6f6e 5f77 6964 6765  alibration_widge
-000014f0: 7472 1200 0000 7213 0000 0072 1400 0000  tr....r....r....
-00001500: da1f 7079 7879 3364 2e74 7261 636b 6572  ..pyxy3d.tracker
-00001510: 732e 6368 6172 7563 6f5f 7472 6163 6b65  s.charuco_tracke
-00001520: 7272 1500 0000 5a27 7079 7879 3364 2e67  rr....Z'pyxy3d.g
-00001530: 7569 2e65 7874 7269 6e73 6963 5f63 616c  ui.extrinsic_cal
-00001540: 6962 7261 7469 6f6e 5f77 6964 6765 7472  ibration_widgetr
-00001550: 1600 0000 7217 0000 00da 3670 7978 7933  ....r.....6pyxy3
-00001560: 642e 6775 692e 7669 7a75 616c 697a 652e  d.gui.vizualize.
-00001570: 6361 6c69 6272 6174 696f 6e2e 6361 7074  calibration.capt
-00001580: 7572 655f 766f 6c75 6d65 5f77 6964 6765  ure_volume_widge
-00001590: 7472 1800 0000 da13 7079 7879 3364 2e63  tr......pyxy3d.c
-000015a0: 6f6e 6669 6775 7261 746f 7272 1900 0000  onfiguratorr....
-000015b0: 721a 0000 0072 5b00 0000 7233 0000 0072  r....r[...r3...r
-000015c0: 3300 0000 7233 0000 0072 3400 0000 da08  3...r3...r4.....
-000015d0: 3c6d 6f64 756c 653e 0100 0000 732c 0000  <module>....s,..
-000015e0: 0008 000c 0208 0208 0108 0108 010c 010c  ................
-000015f0: 0110 0110 0124 0110 0a0c 010c 0110 010c  .....$..........
-00001600: 0110 020c 040c 0110 0300 7f12 0b         .............
+000012e0: 0003 0000 0043 0000 0073 4200 0000 7400  .....C...sB...t.
+000012f0: 7c00 8301 7d01 7401 7c01 8301 7d02 7c02  |...}.t.|...}.|.
+00001300: a002 7403 6a04 a101 0100 7405 7406 6a07  ..t.j.....t.t.j.
+00001310: 8301 7d03 7408 7c02 8301 7d04 7c04 a009  ..}.t.|...}.|...
+00001320: a100 0100 7c03 a00a a100 0100 6400 5300  ....|.......d.S.
+00001330: 7233 0000 0029 0b72 1900 0000 720f 0000  r3...).r....r...
+00001340: 0072 2900 0000 7210 0000 0072 3900 0000  .r)...r....r9...
+00001350: 7209 0000 00da 0373 7973 da04 6172 6776  r......sys..argv
+00001360: 721a 0000 005a 0473 686f 77da 0465 7865  r....Z.show..exe
+00001370: 6329 0572 2000 0000 7221 0000 0072 1b00  c).r ...r!...r..
+00001380: 0000 5a03 6170 705a 0677 696e 646f 7772  ..Z.appZ.windowr
+00001390: 3100 0000 7231 0000 0072 3200 0000 da23  1...r1...r2....#
+000013a0: 6c61 756e 6368 5f65 7874 7269 6e73 6963  launch_extrinsic
+000013b0: 5f63 616c 6962 7261 7469 6f6e 5f77 6964  _calibration_wid
+000013c0: 6765 74af 0000 0073 0e00 0000 0801 0801  get....s........
+000013d0: 0c01 0a02 0801 0801 0c01 724f 0000 0029  ..........rO...)
+000013e0: 2fda 0d70 7978 7933 642e 6c6f 6767 6572  /..pyxy3d.logger
+000013f0: da06 7079 7879 3364 7222 0000 00da 0367  ..pyxy3dr".....g
+00001400: 6574 7248 0000 00da 026f 7372 4c00 0000  etrH.....osrL...
+00001410: 5a06 7368 7574 696c da04 7469 6d65 da07  Z.shutil..time..
+00001420: 7061 7468 6c69 6272 0200 0000 da09 7468  pathlibr......th
+00001430: 7265 6164 696e 6772 0300 0000 5a0c 5079  readingr....Z.Py
+00001440: 5174 362e 5174 436f 7265 7204 0000 0072  Qt6.QtCorer....r
+00001450: 0500 0000 5a0b 5079 5174 362e 5174 4775  ....Z.PyQt6.QtGu
+00001460: 6972 0600 0000 7207 0000 00da 0f50 7951  ir....r......PyQ
+00001470: 7436 2e51 7457 6964 6765 7473 7208 0000  t6.QtWidgetsr...
+00001480: 0072 0900 0000 720a 0000 0072 0b00 0000  .r....r....r....
+00001490: 720c 0000 0072 0d00 0000 720e 0000 005a  r....r....r....Z
+000014a0: 1670 7978 7933 642e 7365 7373 696f 6e2e  .pyxy3d.session.
+000014b0: 7365 7373 696f 6e72 0f00 0000 7210 0000  sessionr....r...
+000014c0: 005a 1970 7978 7933 642e 6775 692e 6368  .Z.pyxy3d.gui.ch
+000014d0: 6172 7563 6f5f 7769 6467 6574 7211 0000  aruco_widgetr...
+000014e0: 005a 3570 7978 7933 642e 6775 692e 6361  .Z5pyxy3d.gui.ca
+000014f0: 6d65 7261 5f63 6f6e 6669 672e 696e 7472  mera_config.intr
+00001500: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
+00001510: 6e5f 7769 6467 6574 7212 0000 0072 1300  n_widgetr....r..
+00001520: 0000 7214 0000 005a 1f70 7978 7933 642e  ..r....Z.pyxy3d.
+00001530: 7472 6163 6b65 7273 2e63 6861 7275 636f  trackers.charuco
+00001540: 5f74 7261 636b 6572 7215 0000 005a 2770  _trackerr....Z'p
+00001550: 7978 7933 642e 6775 692e 6578 7472 696e  yxy3d.gui.extrin
+00001560: 7369 635f 6361 6c69 6272 6174 696f 6e5f  sic_calibration_
+00001570: 7769 6467 6574 7216 0000 0072 1700 0000  widgetr....r....
+00001580: 5a36 7079 7879 3364 2e67 7569 2e76 697a  Z6pyxy3d.gui.viz
+00001590: 7561 6c69 7a65 2e63 616c 6962 7261 7469  ualize.calibrati
+000015a0: 6f6e 2e63 6170 7475 7265 5f76 6f6c 756d  on.capture_volum
+000015b0: 655f 7769 6467 6574 7218 0000 005a 1370  e_widgetr....Z.p
+000015c0: 7978 7933 642e 636f 6e66 6967 7572 6174  yxy3d.configurat
+000015d0: 6f72 7219 0000 0072 1a00 0000 724f 0000  orr....r....rO..
+000015e0: 0072 3100 0000 7231 0000 0072 3100 0000  .r1...r1...r1...
+000015f0: 7232 0000 00da 083c 6d6f 6475 6c65 3e01  r2.....<module>.
+00001600: 0000 0073 2c00 0000 0800 0c02 0802 0801  ...s,...........
+00001610: 0801 0801 0c01 0c01 1001 1001 2401 100a  ............$...
+00001620: 0c01 0c01 1001 0c01 1002 0c04 0c01 1003  ................
+00001630: 007f 120b                                ....
```

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 14:33:05 2023 UTC, .py size: 10279 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a12c 8764 2728 0000  o........,.d'(..
+00000000: 6f0d 0d0a 0000 0000 814c 8764 2728 0000  o........L.d'(..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 bc01 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6402 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 6d07 5a07 0100 6400 6403 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 6d0a 5a0a 0100 6400 6401 6c0b 5a0b 6400  m.Z...d.d.l.Z.d.
 00000070: 6404 6c0c 6d0d 5a0d 0100 6400 6401 6c0e  d.l.m.Z...d.d.l.
```

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 15:02:45 2023 UTC, .py size: 14273 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 9533 8764 c137 0000  o........3.d.7..
+00000000: 6f0d 0d0a 0000 0000 814c 8764 c137 0000  o........L.d.7..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 8201 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c00 5a01 6501  d.l.Z.d.d.l.Z.e.
 00000040: 6a02 a003 6504 a101 5a02 6400 6402 6c05  j...e...Z.d.d.l.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 0100 6501  m.Z.m.Z.m.Z...e.
 00000060: 6a02 a003 6504 a101 5a02 6400 6403 6c09  j...e...Z.d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6404 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
```

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 16:30:37 2023 UTC, .py size: 14618 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 2d48 8764 1a39 0000  o.......-H.d.9..
+00000000: 6f0d 0d0a 0000 0000 814c 8764 1a39 0000  o........L.d.9..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7a01 0000 6400  .....@...sz...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6401 6c05 5a05 6400 6401 6c06  Z.d.d.l.Z.d.d.l.
 00000050: 5a06 6400 6402 6c07 6d08 5a08 0100 6400  Z.d.d.l.m.Z...d.
 00000060: 6403 6c09 6d0a 5a0a 6d0b 5a0b 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6401 6c0c 5a0d 6400 6404 6c0e 6d0f 5a0f  d.l.Z.d.d.l.m.Z.
@@ -99,15 +99,15 @@
 00000620: 6169 7265 6446 7261 6d65 4275 696c 6465  airedFrameBuilde
 00000630: 72da 0d66 7261 6d65 5f62 7569 6c64 6572  r..frame_builder
 00000640: da14 556e 7061 6972 6564 4672 616d 6545  ..UnpairedFrameE
 00000650: 6d69 7474 6572 da0d 6672 616d 655f 656d  mitter..frame_em
 00000660: 6974 7465 72da 0573 7461 7274 7221 0000  itter..startr!..
 00000670: 00da 0e76 6964 656f 5f72 6563 6f72 6465  ...video_recorde
 00000680: 7272 1000 0000 da0f 6672 616d 655f 7261  rr......frame_ra
-00000690: 7465 5f73 7069 6e5a 0873 6574 5661 6c75  te_spinZ.setValu
+00000690: 7465 5f73 7069 6eda 0873 6574 5661 6c75  te_spin..setValu
 000006a0: 65da 0d66 7073 5f72 6563 6f72 6469 6e67  e..fps_recording
 000006b0: 7223 0000 0072 2700 0000 da0b 6e65 7874  r#...r'.....next
 000006c0: 5f61 6374 696f 6e72 1b00 0000 da05 7661  _actionr......va
 000006d0: 6c75 65da 0a73 7461 7274 5f73 746f 7072  lue..start_stopr
 000006e0: 1a00 0000 da11 6465 7374 696e 6174 696f  ......destinatio
 000006f0: 6e5f 6c61 6265 6c72 1500 0000 da1c 6765  n_labelr......ge
 00000700: 745f 6e65 7874 5f72 6563 6f72 6469 6e67  t_next_recording
@@ -128,18 +128,18 @@
 000007f0: 6469 6e67 5769 6467 6574 2e5f 5f69 6e69  dingWidget.__ini
 00000800: 745f 5f63 0100 0000 0000 0000 0000 0000  t__c............
 00000810: 0100 0000 0300 0000 4300 0000 732a 0000  ........C...s*..
 00000820: 007c 006a 00a0 01a1 0072 0d7c 006a 02a0  .|.j.....r.|.j..
 00000830: 0364 01a1 0101 0064 0053 007c 006a 02a0  .d.....d.S.|.j..
 00000840: 0364 02a1 0101 0064 0053 0029 034e 5446  .d.....d.S.).NTF
 00000850: 2904 722d 0000 00da 1569 735f 7265 636f  ).r-.....is_reco
-00000860: 7264 696e 675f 656c 6967 6962 6c65 723b  rding_eligibler;
+00000860: 7264 696e 675f 656c 6967 6962 6c65 723c  rding_eligibler<
 00000870: 0000 00da 0a73 6574 456e 6162 6c65 64a9  .....setEnabled.
-00000880: 0172 4400 0000 722a 0000 0072 2a00 0000  .rD...r*...r*...
-00000890: 722b 0000 0072 4300 0000 5300 0000 7306  r+...rC...S...s.
+00000880: 0172 4500 0000 722a 0000 0072 2a00 0000  .rE...r*...r*...
+00000890: 722b 0000 0072 4400 0000 5300 0000 7306  r+...rD...S...s.
 000008a0: 0000 000a 0110 0110 027a 2652 6563 6f72  .........z&Recor
 000008b0: 6469 6e67 5769 6467 6574 2e75 7064 6174  dingWidget.updat
 000008c0: 655f 6274 6e5f 656c 6967 6962 696c 6974  e_btn_eligibilit
 000008d0: 7963 0100 0000 0000 0000 0000 0000 0500  yc..............
 000008e0: 0000 0400 0000 4300 0000 736c 0000 0064  ......C...sl...d
 000008f0: 0164 0284 007c 006a 006a 01a0 02a1 0044  .d...|.j.j.....D
 00000900: 0083 017d 0164 0364 0284 007c 0144 0083  ...}.d.d...|.D..
@@ -161,42 +161,42 @@
 00000a00: 675f 6469 7265 6374 6f72 792e 3c6c 6f63  g_directory.<loc
 00000a10: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
 00000a20: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 00000a30: 0500 0000 5300 0000 731a 0000 0067 007c  ....S...s....g.|
 00000a40: 005d 097d 017c 01a0 0064 00a1 0172 027c  .].}.|...d...r.|
 00000a50: 0191 0271 0253 0029 01da 0a72 6563 6f72  ...q.S.)...recor
 00000a60: 6469 6e67 5f29 01da 0a73 7461 7274 7377  ding_)...startsw
-00000a70: 6974 68a9 0272 4c00 0000 da06 666f 6c64  ith..rL.....fold
+00000a70: 6974 68a9 0272 4d00 0000 da06 666f 6c64  ith..rM.....fold
 00000a80: 6572 722a 0000 0072 2a00 0000 722b 0000  err*...r*...r+..
-00000a90: 0072 4e00 0000 5d00 0000 724f 0000 0063  .rN...]...rO...c
+00000a90: 0072 4f00 0000 5d00 0000 7250 0000 0063  .rO...]...rP...c
 00000aa0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
 00000ab0: 0500 0000 5300 0000 731a 0000 0067 007c  ....S...s....g.|
 00000ac0: 005d 097d 017c 01a0 0064 00a1 0164 0119  .].}.|...d...d..
 00000ad0: 0091 0271 0253 0029 02da 015f e901 0000  ...q.S.)..._....
-00000ae0: 0029 01da 0573 706c 6974 7252 0000 0072  .)...splitrR...r
-00000af0: 2a00 0000 722a 0000 0072 2b00 0000 724e  *...r*...r+...rN
-00000b00: 0000 005e 0000 0072 4f00 0000 6301 0000  ...^...rO...c...
+00000ae0: 0029 01da 0573 706c 6974 7253 0000 0072  .)...splitrS...r
+00000af0: 2a00 0000 722a 0000 0072 2b00 0000 724f  *...r*...r+...rO
+00000b00: 0000 005e 0000 0072 5000 0000 6301 0000  ...^...rP...c...
 00000b10: 0000 0000 0000 0000 0002 0000 0004 0000  ................
 00000b20: 0053 0000 0073 1c00 0000 6700 7c00 5d0a  .S...s....g.|.].
 00000b30: 7d01 7c01 a000 a100 7202 7401 7c01 8301  }.|.....r.t.|...
 00000b40: 9102 7102 5300 722a 0000 0029 02da 0969  ..q.S.r*...)...i
 00000b50: 736e 756d 6572 6963 da03 696e 7429 0272  snumeric..int).r
-00000b60: 4c00 0000 5a09 7265 635f 636f 756e 7472  L...Z.rec_countr
-00000b70: 2a00 0000 722a 0000 0072 2b00 0000 724e  *...r*...r+...rN
+00000b60: 4d00 0000 5a09 7265 635f 636f 756e 7472  M...Z.rec_countr
+00000b70: 2a00 0000 722a 0000 0072 2b00 0000 724f  *...r*...r+...rO
 00000b80: 0000 005f 0000 00f3 0200 0000 1c00 7201  ..._..........r.
-00000b90: 0000 00da 0b72 6563 6f72 6469 6e67 5f31  .....recording_1
-00000ba0: 7250 0000 0072 5500 0000 2906 722d 0000  rP...rU...).r-..
+00000b90: 0000 005a 0b72 6563 6f72 6469 6e67 5f31  ...Z.recording_1
+00000ba0: 7251 0000 0072 5600 0000 2906 722d 0000  rQ...rV...).r-..
 00000bb0: 00da 0470 6174 68da 0769 7465 7264 6972  ...path..iterdir
 00000bc0: da03 6c65 6eda 0373 7472 da03 6d61 7829  ..len..str..max)
-00000bd0: 0572 4400 0000 da07 666f 6c64 6572 735a  .rD.....foldersZ
+00000bd0: 0572 4500 0000 da07 666f 6c64 6572 735a  .rE.....foldersZ
 00000be0: 1172 6563 6f72 6469 6e67 5f66 6f6c 6465  .recording_folde
 00000bf0: 7273 5a10 7265 636f 7264 696e 675f 636f  rsZ.recording_co
 00000c00: 756e 7473 5a0e 6e65 7874 5f64 6972 6563  untsZ.next_direc
 00000c10: 746f 7279 722a 0000 0072 2a00 0000 722b  toryr*...r*...r+
-00000c20: 0000 0072 3d00 0000 5a00 0000 7312 0000  ...r=...Z...s...
+00000c20: 0000 0072 3e00 0000 5a00 0000 7312 0000  ...r>...Z...s...
 00000c30: 0016 020e 010e 010e 010c 0204 0104 0514  ................
 00000c40: fe04 027a 2c52 6563 6f72 6469 6e67 5769  ...z,RecordingWi
 00000c50: 6467 6574 2e67 6574 5f6e 6578 745f 7265  dget.get_next_re
 00000c60: 636f 7264 696e 675f 6469 7265 6374 6f72  cording_director
 00000c70: 7963 0100 0000 0000 0000 0000 0000 0100  yc..............
 00000c80: 0000 0400 0000 4300 0000 73da 0000 007c  ......C...s....|
 00000c90: 00a0 0074 0183 00a1 0101 0074 0264 0183  ...t.......t.d..
@@ -208,25 +208,25 @@
 00000cf0: 097c 006a 09a0 0074 0483 00a1 0101 007c  .|.j...t.......|
 00000d00: 006a 09a0 05a1 00a0 067c 006a 0aa1 0101  .j.......|.j....
 00000d10: 007c 006a 09a0 05a1 00a0 067c 006a 0ba1  .|.j.......|.j..
 00000d20: 0101 007c 006a 09a0 05a1 00a0 067c 006a  ...|.j.......|.j
 00000d30: 0ca1 0101 007c 00a0 05a1 00a0 067c 006a  .....|.......|.j
 00000d40: 09a1 0101 007c 00a0 05a1 00a0 067c 006a  .....|.......|.j
 00000d50: 0da1 0101 007c 00a0 05a1 00a0 067c 006a  .....|.......|.j
-00000d60: 0ea1 0101 0064 0053 0029 034e 5a08 5365  .....d.S.).NZ.Se
+00000d60: 0ea1 0101 0064 0053 0029 034e da08 5365  .....d.S.).N..Se
 00000d70: 7474 696e 6773 7a0b 4672 616d 6520 5261  ttingsz.Frame Ra
 00000d80: 7465 3a29 0fda 0973 6574 4c61 796f 7574  te:)...setLayout
-00000d90: 721d 0000 0072 1700 0000 5a0e 7365 7474  r....r....Z.sett
+00000d90: 721d 0000 0072 1700 0000 da0e 7365 7474  r....r......sett
 00000da0: 696e 6773 5f67 726f 7570 7219 0000 00da  ings_groupr.....
-00000db0: 066c 6179 6f75 745a 0961 6464 5769 6467  .layoutZ.addWidg
+00000db0: 066c 6179 6f75 74da 0961 6464 5769 6467  .layout..addWidg
 00000dc0: 6574 721a 0000 0072 3700 0000 5a0f 7265  etr....r7...Z.re
-00000dd0: 636f 7264 5f63 6f6e 7472 6f6c 7372 3b00  cord_controlsr;.
-00000de0: 0000 723c 0000 0072 3e00 0000 723f 0000  ..r<...r>...r?..
-00000df0: 0072 4000 0000 7249 0000 0072 2a00 0000  .r@...rI...r*...
-00000e00: 722a 0000 0072 2b00 0000 7241 0000 006b  r*...r+...rA...k
+00000dd0: 636f 7264 5f63 6f6e 7472 6f6c 7372 3c00  cord_controlsr<.
+00000de0: 0000 723d 0000 0072 3f00 0000 7240 0000  ..r=...r?...r@..
+00000df0: 0072 4100 0000 724a 0000 0072 2a00 0000  .rA...rJ...r*...
+00000e00: 722a 0000 0072 2b00 0000 7242 0000 006b  r*...r+...rB...k
 00000e10: 0000 0073 1c00 0000 0c01 0a01 0e01 1401  ...s............
 00000e20: 1201 1001 0802 0e01 1201 1201 1201 1002  ................
 00000e30: 1001 1402 7a1d 5265 636f 7264 696e 6757  ....z.RecordingW
 00000e40: 6964 6765 742e 706c 6163 655f 7769 6467  idget.place_widg
 00000e50: 6574 7363 0100 0000 0000 0000 0000 0000  etsc............
 00000e60: 0100 0000 0300 0000 4300 0000 7356 0000  ........C...sV..
 00000e70: 007c 006a 006a 01a0 027c 006a 03a1 0101  .|.j.j...|.j....
@@ -234,26 +234,26 @@
 00000e90: 0101 007c 006a 006a 08a0 027c 006a 09a1  ...|.j.j...|.j..
 00000ea0: 0101 007c 006a 0a6a 0ba0 027c 006a 0ca1  ...|.j.j...|.j..
 00000eb0: 0101 007c 006a 066a 0da0 027c 006a 0ea1  ...|.j.j...|.j..
 00000ec0: 0101 0064 0053 00a9 014e 290f 7234 0000  ...d.S...N).r4..
 00000ed0: 00da 0e49 6d61 6765 4272 6f61 6463 6173  ...ImageBroadcas
 00000ee0: 74da 0763 6f6e 6e65 6374 da0f 496d 6167  t..connect..Imag
 00000ef0: 6555 7064 6174 6553 6c6f 7472 3700 0000  eUpdateSlotr7...
-00000f00: 5a0c 7661 6c75 6543 6861 6e67 6564 722d  Z.valueChangedr-
+00000f00: da0c 7661 6c75 6543 6861 6e67 6564 722d  ..valueChangedr-
 00000f10: 0000 00da 1373 6574 5f61 6374 6976 655f  .....set_active_
 00000f20: 6d6f 6465 5f66 7073 da0b 6472 6f70 7065  mode_fps..droppe
 00000f30: 645f 6670 73da 1275 7064 6174 655f 6472  d_fps..update_dr
-00000f40: 6f70 7065 645f 6670 7372 3b00 0000 da07  opped_fpsr;.....
+00000f40: 6f70 7065 645f 6670 7372 3c00 0000 da07  opped_fpsr<.....
 00000f50: 636c 6963 6b65 64da 1174 6f67 676c 655f  clicked..toggle_
 00000f60: 7374 6172 745f 7374 6f70 da19 7265 636f  start_stop..reco
 00000f70: 7264 696e 675f 636f 6d70 6c65 7465 5f73  rding_complete_s
 00000f80: 6967 6e61 6cda 156f 6e5f 7265 636f 7264  ignal..on_record
-00000f90: 696e 675f 636f 6d70 6c65 7465 7249 0000  ing_completerI..
+00000f90: 696e 675f 636f 6d70 6c65 7465 724a 0000  ing_completerJ..
 00000fa0: 0072 2a00 0000 722a 0000 0072 2b00 0000  .r*...r*...r+...
-00000fb0: 7242 0000 007f 0000 0073 0a00 0000 1002  rB.......s......
+00000fb0: 7243 0000 007f 0000 0073 0a00 0000 1002  rC.......s......
 00000fc0: 1201 1001 1001 1401 7a1f 5265 636f 7264  ........z.Record
 00000fd0: 696e 6757 6964 6765 742e 636f 6e6e 6563  ingWidget.connec
 00000fe0: 745f 7769 6467 6574 7363 0100 0000 0000  t_widgetsc......
 00000ff0: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
 00001000: 0000 73c6 0000 007c 006a 0074 016a 026b  ..s....|.j.t.j.k
 00001010: 0272 2f74 016a 037c 005f 007c 006a 04a0  .r/t.j.|._.|.j..
 00001020: 057c 006a 006a 06a1 0101 007c 006a 07a0  .|.j.j.....|.j..
@@ -267,25 +267,25 @@
 000010a0: 006a 07a0 0864 03a1 0101 0074 09a0 0a64  .j...d.....t...d
 000010b0: 04a1 0101 007c 006a 07a0 057c 00a0 12a1  .....|.j...|....
 000010c0: 00a1 0101 0064 0053 0064 0053 0029 054e  .....d.S.d.S.).N
 000010d0: 467a 1249 6e69 7469 6174 6520 7265 636f  Fz.Initiate reco
 000010e0: 7264 696e 6754 7a2e 5374 6f70 2072 6563  rdingTz.Stop rec
 000010f0: 6f72 6469 6e67 2061 6e64 2069 6e69 7469  ording and initi
 00001100: 6174 6520 6669 6e61 6c20 7361 7665 206f  ate final save o
-00001110: 6620 6669 6c65 2913 7239 0000 0072 2300  f file).r9...r#.
-00001120: 0000 7227 0000 0072 2800 0000 723b 0000  ..r'...r(...r;..
-00001130: 00da 0773 6574 5465 7874 723a 0000 0072  ...setTextr:...r
-00001140: 3e00 0000 7248 0000 00da 066c 6f67 6765  >...rH.....logge
+00001110: 6620 6669 6c65 2913 723a 0000 0072 2300  f file).r:...r#.
+00001120: 0000 7227 0000 0072 2800 0000 723c 0000  ..r'...r(...r<..
+00001130: 00da 0773 6574 5465 7874 723b 0000 0072  ...setTextr;...r
+00001140: 3f00 0000 7249 0000 00da 066c 6f67 6765  ?...rI.....logge
 00001150: 72da 0469 6e66 6f72 0200 0000 722d 0000  r..infor....r-..
 00001160: 0072 5b00 0000 da04 7465 7874 da0f 7374  .r[.....text..st
 00001170: 6172 745f 7265 636f 7264 696e 6772 2900  art_recordingr).
 00001180: 0000 da0e 7374 6f70 5f72 6563 6f72 6469  ....stop_recordi
-00001190: 6e67 723d 0000 0029 0272 4400 0000 da0e  ngr=...).rD.....
+00001190: 6e67 723e 0000 0029 0272 4500 0000 5a0e  ngr>...).rE...Z.
 000011a0: 7265 636f 7264 696e 675f 7061 7468 722a  recording_pathr*
-000011b0: 0000 0072 2a00 0000 722b 0000 0072 6b00  ...r*...r+...rk.
+000011b0: 0000 0072 2a00 0000 722b 0000 0072 6f00  ...r*...r+...ro.
 000011c0: 0000 8700 0000 7320 0000 000c 0108 0110  ......s ........
 000011d0: 010c 010a 0214 0110 010c 020c 0108 0210  ................
 000011e0: 020a 010c 020a 0114 0104 f67a 2152 6563  ...........z!Rec
 000011f0: 6f72 6469 6e67 5769 6467 6574 2e74 6f67  ordingWidget.tog
 00001200: 676c 655f 7374 6172 745f 7374 6f70 6301  gle_start_stopc.
 00001210: 0000 0000 0000 0000 0000 0001 0000 0003  ................
 00001220: 0000 0043 0000 0073 3c00 0000 7400 a001  ...C...s<...t...
@@ -295,64 +295,64 @@
 00001260: a101 0100 6400 5300 2904 4e7a 4452 6563  ....d.S.).NzDRec
 00001270: 6f72 6469 6e67 2063 6f6d 706c 6574 6520  ording complete 
 00001280: 7369 676e 616c 2072 6563 6569 7665 642e  signal received.
 00001290: 2e2e 7570 6461 7469 6e67 206e 6578 7420  ..updating next 
 000012a0: 6163 7469 6f6e 2061 6e64 2062 7574 746f  action and butto
 000012b0: 6e54 7a24 456e 6162 6c69 6e67 2073 7461  nTz$Enabling sta
 000012c0: 7274 2f73 746f 7020 7265 636f 7264 696e  rt/stop recordin
-000012d0: 6720 6275 7474 6f6e 2909 726f 0000 0072  g button).ro...r
-000012e0: 7000 0000 7223 0000 0072 2700 0000 7239  p...r#...r'...r9
-000012f0: 0000 0072 3b00 0000 726e 0000 0072 3a00  ...r;...rn...r:.
-00001300: 0000 7248 0000 0072 4900 0000 722a 0000  ..rH...rI...r*..
-00001310: 0072 2a00 0000 722b 0000 0072 6d00 0000  .r*...r+...rm...
+000012d0: 6720 6275 7474 6f6e 2909 7273 0000 0072  g button).rs...r
+000012e0: 7400 0000 7223 0000 0072 2700 0000 723a  t...r#...r'...r:
+000012f0: 0000 0072 3c00 0000 7272 0000 0072 3b00  ...r<...rr...r;.
+00001300: 0000 7249 0000 0072 4a00 0000 722a 0000  ..rI...rJ...r*..
+00001310: 0072 2a00 0000 722b 0000 0072 7100 0000  .r*...r+...rq...
 00001320: 9d00 0000 730a 0000 000a 0108 0110 010c  ....s...........
 00001330: 010e 017a 2552 6563 6f72 6469 6e67 5769  ...z%RecordingWi
 00001340: 6467 6574 2e6f 6e5f 7265 636f 7264 696e  dget.on_recordin
-00001350: 675f 636f 6d70 6c65 7465 7268 0000 0063  g_completerh...c
+00001350: 675f 636f 6d70 6c65 7465 726c 0000 0063  g_completerl...c
 00001360: 0200 0000 0000 0000 0000 0000 0500 0000  ................
 00001370: 0600 0000 4300 0000 733c 0000 0064 017d  ....C...s<...d.}
 00001380: 027c 01a0 00a1 0044 005d 0f5c 027d 037d  .|.....D.].\.}.}
 00001390: 047c 027c 039b 0064 027c 0464 039b 0464  .|.|...d.|.d...d
 000013a0: 049d 0437 007d 0271 067c 006a 01a0 027c  ...7.}.q.|.j...|
 000013b0: 02a1 0101 0064 0553 0029 067a 3855 6e72  .....d.S.).z8Unr
 000013c0: 6176 656c 2064 726f 7070 6564 2066 7073  avel dropped fps
 000013d0: 2064 6963 7469 6f6e 6172 7920 746f 2061   dictionary to a
 000013e0: 206d 6f72 6520 7265 6164 6162 6c65 2073   more readable s
 000013f0: 7472 696e 677a 2352 6174 6520 6f66 2046  tringz#Rate of F
 00001400: 7261 6d65 2044 726f 7070 696e 6720 6279  rame Dropping by
 00001410: 2050 6f72 743a 2020 2020 7a02 3a20 7a03   Port:    z.: z.
 00001420: 2e30 257a 0820 2020 2020 2020 204e 2903  .0%z.        N).
-00001430: da05 6974 656d 7372 3f00 0000 726e 0000  ..itemsr?...rn..
-00001440: 0029 0572 4400 0000 7268 0000 0072 7100  .).rD...rh...rq.
+00001430: da05 6974 656d 7372 4000 0000 7272 0000  ..itemsr@...rr..
+00001440: 0029 0572 4500 0000 726c 0000 0072 7500  .).rE...rl...ru.
 00001450: 0000 da04 706f 7274 5a09 6472 6f70 5f72  ....portZ.drop_r
 00001460: 6174 6572 2a00 0000 722a 0000 0072 2b00  ater*...r*...r+.
-00001470: 0000 7269 0000 00a4 0000 0073 0800 0000  ..ri.......s....
+00001470: 0000 726d 0000 00a4 0000 0073 0800 0000  ..rm.......s....
 00001480: 0402 1001 1801 1002 7a22 5265 636f 7264  ........z"Record
 00001490: 696e 6757 6964 6765 742e 7570 6461 7465  ingWidget.update
 000014a0: 5f64 726f 7070 6564 5f66 7073 6302 0000  _dropped_fpsc...
 000014b0: 0000 0000 0000 0000 0003 0000 0004 0000  ................
 000014c0: 0043 0000 0073 2c00 0000 7c00 6a00 a001  .C...s,...|.j...
 000014d0: 7c00 6a00 a002 a100 a101 0100 7403 a004  |.j.........t...
 000014e0: 7c01 a101 7d02 7c00 6a00 a005 7c02 a101  |...}.|.j...|...
-000014f0: 0100 6400 5300 7263 0000 0029 0672 4000  ..d.S.rc...).r@.
+000014f0: 0100 6400 5300 7266 0000 0029 0672 4100  ..d.S.rf...).rA.
 00001500: 0000 da06 7265 7369 7a65 da08 7369 7a65  ....resize..size
 00001510: 4869 6e74 720b 0000 00da 0966 726f 6d49  Hintr......fromI
 00001520: 6d61 6765 da09 7365 7450 6978 6d61 7029  mage..setPixmap)
-00001530: 0372 4400 0000 da07 715f 696d 6167 65da  .rD.....q_image.
+00001530: 0372 4500 0000 da07 715f 696d 6167 65da  .rE.....q_image.
 00001540: 0771 7069 786d 6170 722a 0000 0072 2a00  .qpixmapr*...r*.
-00001550: 0000 722b 0000 0072 6600 0000 ad00 0000  ..r+...rf.......
+00001550: 0000 722b 0000 0072 6900 0000 ad00 0000  ..r+...ri.......
 00001560: 7306 0000 0012 010a 0110 017a 1f52 6563  s..........z.Rec
 00001570: 6f72 6469 6e67 5769 6467 6574 2e49 6d61  ordingWidget.Ima
 00001580: 6765 5570 6461 7465 536c 6f74 290f 7224  geUpdateSlot).r$
 00001590: 0000 0072 2500 0000 7226 0000 0072 1e00  ...r%...r&...r..
-000015a0: 0000 722f 0000 0072 4300 0000 723d 0000  ..r/...rC...r=..
-000015b0: 0072 4100 0000 7242 0000 0072 6b00 0000  .rA...rB...rk...
-000015c0: 726d 0000 00da 0464 6963 7472 6900 0000  rm.....dictri...
-000015d0: 7266 0000 00da 0d5f 5f63 6c61 7373 6365  rf.....__classce
-000015e0: 6c6c 5f5f 722a 0000 0072 2a00 0000 7245  ll__r*...r*...rE
+000015a0: 0000 722f 0000 0072 4400 0000 723e 0000  ..r/...rD...r>..
+000015b0: 0072 4200 0000 7243 0000 0072 6f00 0000  .rB...rC...ro...
+000015c0: 7271 0000 00da 0464 6963 7472 6d00 0000  rq.....dictrm...
+000015d0: 7269 0000 00da 0d5f 5f63 6c61 7373 6365  ri.....__classce
+000015e0: 6c6c 5f5f 722a 0000 0072 2a00 0000 7246  ll__r*...r*...rF
 000015f0: 0000 0072 2b00 0000 722c 0000 0031 0000  ...r+...r,...1..
 00001600: 0073 1400 0000 0800 1202 0820 0807 0811  .s......... ....
 00001610: 0814 0808 0816 0e07 1009 722c 0000 0063  ..........r,...c
 00001620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001630: 0400 0000 4000 0000 7344 0000 0065 005a  ....@...sD...e.Z
 00001640: 0164 005a 0264 1064 0265 0366 0264 0364  .d.Z.d.d.e.f.d.d
 00001650: 0484 055a 0464 0564 0684 005a 0564 0764  ...Z.d.d...Z.d.d
@@ -369,40 +369,40 @@
 00001700: 6401 1300 a101 8301 7c00 5f0b 7408 7409  d.......|._.t.t.
 00001710: a00a 7c05 7c00 6a0b 1b00 a101 8301 7c00  ..|.|.j.......|.
 00001720: 5f0c 740d 8300 7c00 5f0e 7c00 6a00 a00f  _.t...|._.|.j...
 00001730: 7c00 6a0e a101 0100 6400 5300 2902 4e67  |.j.....d.S.).Ng
 00001740: 0000 0000 0000 e03f 2910 7230 0000 00da  .......?).r0....
 00001750: 1373 696e 676c 655f 6672 616d 655f 6865  .single_frame_he
 00001760: 6967 6874 da05 706f 7274 73da 0773 7472  ight..ports..str
-00001770: 6561 6d73 7275 0000 00da 0661 7070 656e  eamsru.....appen
-00001780: 64da 0473 6f72 7472 5d00 0000 7258 0000  d..sortr]...rX..
+00001770: 6561 6d73 7278 0000 00da 0661 7070 656e  eamsrx.....appen
+00001780: 64da 0473 6f72 7472 5d00 0000 7259 0000  d..sortr]...rY..
 00001790: 00da 046d 6174 68da 0463 6569 6cda 0d66  ...math..ceil..f
 000017a0: 7261 6d65 5f63 6f6c 756d 6e73 da0a 6672  rame_columns..fr
 000017b0: 616d 655f 726f 7773 7205 0000 00da 166e  ame_rowsr......n
 000017c0: 6577 5f73 796e 635f 7061 636b 6574 5f6e  ew_sync_packet_n
 000017d0: 6f74 6963 65da 1373 7562 7363 7269 6265  otice..subscribe
-000017e0: 5f74 6f5f 6e6f 7469 6365 2906 7244 0000  _to_notice).rD..
-000017f0: 0072 3000 0000 7280 0000 0072 7600 0000  .r0...r....rv...
+000017e0: 5f74 6f5f 6e6f 7469 6365 2906 7245 0000  _to_notice).rE..
+000017f0: 0072 3000 0000 7283 0000 0072 7900 0000  .r0...r....ry...
 00001800: da06 7374 7265 616d 5a0c 6361 6d65 7261  ..streamZ.camera
 00001810: 5f63 6f75 6e74 722a 0000 0072 2a00 0000  _countr*...r*...
 00001820: 722b 0000 0072 2f00 0000 b300 0000 7316  r+...r/.......s.
 00001830: 0000 0006 0106 0106 0314 010e 030a 010a  ................
 00001840: 0414 0116 0108 0212 017a 1d55 6e70 6169  .........z.Unpai
 00001850: 7265 6446 7261 6d65 4275 696c 6465 722e  redFrameBuilder.
 00001860: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
 00001870: 0000 0000 0001 0000 0003 0000 0043 0000  .............C..
 00001880: 0073 1c00 0000 7400 a001 6401 a101 0100  .s....t...d.....
 00001890: 7c00 6a02 a003 7c00 6a04 a101 0100 6400  |.j...|.j.....d.
 000018a0: 5300 2902 4e7a 2c55 6e73 7562 7363 7269  S.).Nz,Unsubscri
 000018b0: 6265 2066 7261 6d65 2062 7569 6c64 6572  be frame builder
 000018c0: 2066 726f 6d20 7379 6e63 6872 6f6e 697a   from synchroniz
-000018d0: 6572 2e29 0572 6f00 0000 7270 0000 0072  er.).ro...rp...r
+000018d0: 6572 2e29 0572 7300 0000 7274 0000 0072  er.).rs...rt...r
 000018e0: 3000 0000 da15 756e 7375 6273 6372 6962  0.....unsubscrib
-000018f0: 655f 746f 5f6e 6f74 6963 6572 8900 0000  e_to_noticer....
-00001900: 7249 0000 0072 2a00 0000 722a 0000 0072  rI...r*...r*...r
+000018f0: 655f 746f 5f6e 6f74 6963 6572 8c00 0000  e_to_noticer....
+00001900: 724a 0000 0072 2a00 0000 722a 0000 0072  rJ...r*...r*...r
 00001910: 2b00 0000 da1d 756e 7375 6273 6372 6962  +.....unsubscrib
 00001920: 655f 6672 6f6d 5f73 796e 6368 726f 6e69  e_from_synchroni
 00001930: 7a65 72c8 0000 0073 0400 0000 0a01 1201  zer....s........
 00001940: 7a32 556e 7061 6972 6564 4672 616d 6542  z2UnpairedFrameB
 00001950: 7569 6c64 6572 2e75 6e73 7562 7363 7269  uilder.unsubscri
 00001960: 6265 5f66 726f 6d5f 7379 6e63 6872 6f6e  be_from_synchron
 00001970: 697a 6572 6302 0000 0000 0000 0000 0000  izerc...........
@@ -417,19 +417,19 @@
 00001a00: 2062 6569 6e67 204e 6f6e 6520 616d 6f6e   being None amon
 00001a10: 670a 2020 2020 2020 2020 7468 6520 7379  g.        the sy
 00001a20: 6e63 6865 6420 6672 616d 6573 2c20 736f  nched frames, so
 00001a30: 2070 6c75 6720 7468 6174 2077 6974 6820   plug that with 
 00001a40: 6120 626c 616e 6b20 6672 616d 654e 7a19  a blank frameNz.
 00001a50: 706c 7567 6769 6e67 2062 6c61 6e6b 2066  plugging blank f
 00001a60: 7261 6d65 2064 6174 61e9 0300 0000 2901  rame data.....).
-00001a70: da05 6474 7970 6529 0772 8000 0000 726f  ..dtype).r....ro
+00001a70: da05 6474 7970 6529 0772 8300 0000 7273  ..dtype).r....rs
 00001a80: 0000 00da 0564 6562 7567 da02 6e70 da05  .....debug..np..
 00001a90: 7a65 726f 73da 0575 696e 7438 da05 6672  zeros..uint8..fr
-00001aa0: 616d 6529 0472 4400 0000 da0c 6672 616d  ame).rD.....fram
-00001ab0: 655f 7061 636b 6574 da04 6564 6765 7294  e_packet..edger.
+00001aa0: 616d 6529 0472 4500 0000 da0c 6672 616d  ame).rE.....fram
+00001ab0: 655f 7061 636b 6574 da04 6564 6765 7297  e_packet..edger.
 00001ac0: 0000 0072 2a00 0000 722a 0000 0072 2b00  ...r*...r*...r+.
 00001ad0: 0000 da12 6765 745f 6672 616d 655f 6f72  ....get_frame_or
 00001ae0: 5f62 6c61 6e6b cd00 0000 730e 0000 0006  _blank....s.....
 00001af0: 0408 020a 0116 0104 0406 fe04 027a 2755  .............z'U
 00001b00: 6e70 6169 7265 6446 7261 6d65 4275 696c  npairedFrameBuil
 00001b10: 6465 722e 6765 745f 6672 616d 655f 6f72  der.get_frame_or
 00001b20: 5f62 6c61 6e6b 6302 0000 0000 0000 0000  _blankc.........
@@ -446,28 +446,28 @@
 00001bd0: 206d 616b 6520 7375 7265 2074 6861 7420   make sure that 
 00001be0: 6672 616d 6573 2061 6c69 676e 2077 656c  frames align wel
 00001bf0: 6c2c 2073 6361 6c65 2074 6865 6d20 616c  l, scale them al
 00001c00: 6c20 746f 2074 6875 6d62 6e61 696c 730a  l to thumbnails.
 00001c10: 2020 2020 2020 2020 7371 7561 7265 7320          squares 
 00001c20: 7769 7468 2062 6c61 636b 2062 6f72 6465  with black borde
 00001c30: 7273 2e7a 0f72 6573 697a 696e 6720 7371  rs.z.resizing sq
-00001c40: 7561 7265 7201 0000 0072 5500 0000 e902  uarer....rU.....
+00001c40: 7561 7265 7201 0000 0072 5600 0000 e902  uarer....rV.....
 00001c50: 0000 0029 0372 0100 0000 7201 0000 0072  ...).r....r....r
 00001c60: 0100 0000 7a13 6162 6f75 7420 746f 2070  ....z.about to p
-00001c70: 6164 2062 6f72 6465 7229 0172 3a00 0000  ad border).r:...
+00001c70: 6164 2062 6f72 6465 7229 0172 3b00 0000  ad border).r;...
 00001c80: 2901 da0a 6e65 775f 6865 6967 6874 290a  )...new_height).
-00001c90: 726f 0000 0072 9000 0000 da05 7368 6170  ro...r......shap
-00001ca0: 6572 5f00 0000 7258 0000 00da 0363 7632  er_...rX.....cv2
+00001c90: 7273 0000 0072 9300 0000 da05 7368 6170  rs...r......shap
+00001ca0: 6572 5f00 0000 7259 0000 00da 0363 7632  er_...rY.....cv2
 00001cb0: da0e 636f 7079 4d61 6b65 426f 7264 6572  ..copyMakeBorder
 00001cc0: da0f 424f 5244 4552 5f43 4f4e 5354 414e  ..BORDER_CONSTAN
-00001cd0: 5472 7700 0000 7280 0000 0029 0872 4400  Trw...r....).rD.
-00001ce0: 0000 7294 0000 00da 0668 6569 6768 74da  ..r......height.
-00001cf0: 0577 6964 7468 5a0b 7061 6464 6564 5f73  .widthZ.padded_s
-00001d00: 697a 655a 0a68 6569 6768 745f 7061 645a  izeZ.height_padZ
-00001d10: 0977 6964 7468 5f70 6164 5a09 7061 645f  .width_padZ.pad_
+00001cd0: 5472 7a00 0000 7283 0000 0029 0872 4500  Trz...r....).rE.
+00001ce0: 0000 7297 0000 00da 0668 6569 6768 74da  ..r......height.
+00001cf0: 0577 6964 7468 da0b 7061 6464 6564 5f73  .width..padded_s
+00001d00: 697a 65da 0a68 6569 6768 745f 7061 64da  ize..height_pad.
+00001d10: 0977 6964 7468 5f70 6164 da09 7061 645f  .width_pad..pad_
 00001d20: 636f 6c6f 7272 2a00 0000 722a 0000 0072  colorr*...r*...r
 00001d30: 2b00 0000 da10 7265 7369 7a65 5f74 6f5f  +.....resize_to_
 00001d40: 7371 7561 7265 dc00 0000 7326 0000 000a  square....s&....
 00001d50: 030a 040a 010a 0210 0210 0108 010a 0204  ................
 00001d60: 0102 0102 0102 0102 0102 0104 0102 0106  ................
 00001d70: f90e 0a04 017a 2555 6e70 6169 7265 6446  .....z%UnpairedF
 00001d80: 7261 6d65 4275 696c 6465 722e 7265 7369  rameBuilder.resi
@@ -477,25 +477,25 @@
 00001dc0: 7c02 1900 6a02 6a03 7d03 7c03 6401 6b02  |...j.j.}.|.d.k.
 00001dd0: 720f 0900 7c01 5300 7c03 6402 7600 721c  r...|.S.|.d.v.r.
 00001de0: 7404 a005 7c01 7404 6a06 a102 7d01 7c01  t...|.t.j...}.|.
 00001df0: 5300 7c03 6403 7600 7229 7404 a005 7c01  S.|.d.v.r)t...|.
 00001e00: 7404 6a07 a102 7d01 7c01 5300 7c03 6404  t.j...}.|.S.|.d.
 00001e10: 7600 7234 7404 a005 7c01 7404 6a08 a102  v.r4t...|.t.j...
 00001e20: 7d01 7c01 5300 2905 4e72 0100 0000 2902  }.|.S.).Nr....).
-00001e30: 7255 0000 00e9 fdff ffff 2902 7298 0000  rU........).r...
-00001e40: 00e9 feff ffff 2902 e9ff ffff ff72 8e00  ......)......r..
-00001e50: 0000 2909 7230 0000 0072 8200 0000 da06  ..).r0...r......
+00001e30: 7256 0000 00e9 fdff ffff 2902 729b 0000  rV........).r...
+00001e40: 00e9 feff ffff 2902 e9ff ffff ff72 9100  ......)......r..
+00001e50: 0000 2909 7230 0000 0072 8500 0000 da06  ..).r0...r......
 00001e60: 6361 6d65 7261 da0e 726f 7461 7469 6f6e  camera..rotation
-00001e70: 5f63 6f75 6e74 729b 0000 00da 0672 6f74  _countr......rot
+00001e70: 5f63 6f75 6e74 729e 0000 00da 0672 6f74  _countr......rot
 00001e80: 6174 65da 1352 4f54 4154 455f 3930 5f43  ate..ROTATE_90_C
 00001e90: 4c4f 434b 5749 5345 da0a 524f 5441 5445  LOCKWISE..ROTATE
 00001ea0: 5f31 3830 da1a 524f 5441 5445 5f39 305f  _180..ROTATE_90_
 00001eb0: 434f 554e 5445 5243 4c4f 434b 5749 5345  COUNTERCLOCKWISE
-00001ec0: 2904 7244 0000 0072 9400 0000 7276 0000  ).rD...r....rv..
-00001ed0: 0072 a500 0000 722a 0000 0072 2a00 0000  .r....r*...r*...
+00001ec0: 2904 7245 0000 0072 9700 0000 7279 0000  ).rE...r....ry..
+00001ed0: 0072 ac00 0000 722a 0000 0072 2a00 0000  .r....r*...r*...
 00001ee0: 722b 0000 00da 0e61 7070 6c79 5f72 6f74  r+.....apply_rot
 00001ef0: 6174 696f 6efb 0000 0073 1a00 0000 1002  ation....s......
 00001f00: 0801 0201 0408 08f9 0e01 0406 08fb 0e01  ................
 00001f10: 0404 08fd 0e01 0402 7a23 556e 7061 6972  ........z#Unpair
 00001f20: 6564 4672 616d 6542 7569 6c64 6572 2e61  edFrameBuilder.a
 00001f30: 7070 6c79 5f72 6f74 6174 696f 6e63 0100  pply_rotationc..
 00001f40: 0000 0000 0000 0000 0000 1100 0000 0a00  ................
@@ -535,57 +535,57 @@
 00002160: 7274 6963 616c 6c79 2c20 6275 7420 7468  rtically, but th
 00002170: 6973 2073 686f 756c 6420 6265 2065 7870  is should be exp
 00002180: 616e 6465 6420 6f6e 2074 6865 200a 2020  anded on the .  
 00002190: 2020 2020 2020 7468 6520 6675 7475 7265        the future
 000021a0: 2074 6f20 616c 6c6f 7720 7772 6170 7069   to allow wrappi
 000021b0: 6e67 2074 6f20 6120 6d6f 7265 2073 7175  ng to a more squ
 000021c0: 6172 6520 7368 6170 650a 2020 2020 2020  are shape.      
-000021d0: 2020 7255 0000 0072 9800 0000 e904 0000    rU...r........
+000021d0: 2020 7256 0000 0072 9b00 0000 e904 0000    rV...r........
 000021e0: 0029 0372 0100 0000 7201 0000 00e9 ff00  .).r....r.......
-000021f0: 0000 2904 5a08 666f 6e74 4661 6365 5a09  ..).Z.fontFaceZ.
+000021f0: 0000 2904 da08 666f 6e74 4661 6365 da09  ..)...fontFace..
 00002200: 666f 6e74 5363 616c 65da 0563 6f6c 6f72  fontScale..color
 00002210: da09 7468 6963 6b6e 6573 734e 7201 0000  ..thicknessNr...
-00002220: 0029 1872 8900 0000 da03 6765 7472 3000  .).r......getr0.
+00002220: 0029 1872 8c00 0000 da03 6765 7472 3000  .).r......getr0.
 00002230: 0000 da13 6375 7272 656e 745f 7379 6e63  ....current_sync
-00002240: 5f70 6163 6b65 7472 8100 0000 da0d 6672  _packetr......fr
-00002250: 616d 655f 7061 636b 6574 7372 9700 0000  ame_packetsr....
-00002260: 72a0 0000 0072 aa00 0000 729b 0000 00da  r....r....r.....
+00002240: 5f70 6163 6b65 7472 8400 0000 da0d 6672  _packetr......fr
+00002250: 616d 655f 7061 636b 6574 7372 9a00 0000  ame_packetsr....
+00002260: 72a7 0000 0072 b100 0000 729e 0000 00da  r....r....r.....
 00002270: 0466 6c69 70da 0770 7574 5465 7874 725e  .flip..putTextr^
-00002280: 0000 0072 5800 0000 729a 0000 0072 8000  ...rX...r....r..
+00002280: 0000 0072 5900 0000 729d 0000 0072 8300  ...rY...r....r..
 00002290: 0000 da14 464f 4e54 5f48 4552 5348 4559  ....FONT_HERSHEY
-000022a0: 5f53 494d 504c 4558 725d 0000 0072 7500  _SIMPLEXr]...ru.
-000022b0: 0000 7291 0000 00da 0668 7374 6163 6b72  ..r......hstackr
-000022c0: 8700 0000 7283 0000 00da 0676 7374 6163  ....r......vstac
-000022d0: 6b29 1172 4400 0000 5a10 7468 756d 626e  k).rD...Z.thumbn
-000022e0: 6169 6c5f 6672 616d 6573 7276 0000 0072  ail_framesrv...r
-000022f0: 9500 0000 5a09 7261 775f 6672 616d 655a  ....Z.raw_frameZ
+000022a0: 5f53 494d 504c 4558 725d 0000 0072 7800  _SIMPLEXr]...rx.
+000022b0: 0000 7294 0000 00da 0668 7374 6163 6b72  ..r......hstackr
+000022c0: 8a00 0000 7286 0000 00da 0676 7374 6163  ....r......vstac
+000022d0: 6b29 1172 4500 0000 5a10 7468 756d 626e  k).rE...Z.thumbn
+000022e0: 6169 6c5f 6672 616d 6573 7279 0000 0072  ail_framesry...r
+000022f0: 9800 0000 5a09 7261 775f 6672 616d 655a  ....Z.raw_frameZ
 00002300: 0c73 7175 6172 655f 6672 616d 655a 0d72  .square_frameZ.r
 00002310: 6f74 6174 6564 5f66 7261 6d65 5a0d 666c  otated_frameZ.fl
 00002320: 6970 7065 645f 6672 616d 655a 0a74 6578  ipped_frameZ.tex
-00002330: 745f 6672 616d 6572 8800 0000 5a0b 6375  t_framer....Z.cu
+00002330: 745f 6672 616d 6572 8b00 0000 5a0b 6375  t_framer....Z.cu
 00002340: 7272 656e 745f 726f 775a 1263 7572 7265  rrent_rowZ.curre
 00002350: 6e74 5f72 6f77 5f6c 656e 6774 685a 0c66  nt_row_lengthZ.f
 00002360: 7261 6d65 735f 6164 6465 645a 1066 7261  rames_addedZ.fra
-00002370: 6d65 735f 7265 6d61 696e 696e 6772 9400  mes_remainingr..
+00002370: 6d65 735f 7265 6d61 696e 696e 6772 9700  mes_remainingr..
 00002380: 0000 5a0a 6d65 6761 5f66 7261 6d65 da03  ..Z.mega_frame..
 00002390: 726f 7772 2a00 0000 722a 0000 0072 2b00  rowr*...r*...r+.
 000023a0: 0000 da13 6765 745f 7265 636f 7264 696e  ....get_recordin
 000023b0: 675f 6672 616d 650a 0100 0073 5a00 0000  g_frame....sZ...
 000023c0: 0a08 0a01 0402 0a01 0c01 0a01 0a01 0c01  ................
 000023d0: 0c01 0603 0601 1e01 0401 0201 0201 0201  ................
 000023e0: 06fa 0a09 0402 0401 0401 0401 0a01 1001  ................
 000023f0: 0802 0601 0e02 0801 0801 0802 0a02 1401  ................
 00002400: 0801 0afe 0a04 0a01 0401 0401 0280 0402  ................
 00002410: 0801 0801 0601 1002 0403 7a28 556e 7061  ..........z(Unpa
 00002420: 6972 6564 4672 616d 6542 7569 6c64 6572  iredFrameBuilder
 00002430: 2e67 6574 5f72 6563 6f72 6469 6e67 5f66  .get_recording_f
-00002440: 7261 6d65 4e29 0172 7f00 0000 290a 7224  rameN).r....).r$
+00002440: 7261 6d65 4e29 0172 8200 0000 290a 7224  rameN).r....).r$
 00002450: 0000 0072 2500 0000 7226 0000 0072 1f00  ...r%...r&...r..
-00002460: 0000 722f 0000 0072 8d00 0000 7297 0000  ..r/...r....r...
-00002470: 0072 a000 0000 72aa 0000 0072 b800 0000  .r....r....r....
+00002460: 0000 722f 0000 0072 9000 0000 729a 0000  ..r/...r....r...
+00002470: 0072 a700 0000 72b1 0000 0072 c100 0000  .r....r....r....
 00002480: 722a 0000 0072 2a00 0000 722a 0000 0072  r*...r*...r*...r
 00002490: 2b00 0000 7231 0000 00b2 0000 0073 0e00  +...r1.......s..
 000024a0: 0000 0800 1001 0815 0805 080f 081f 0c0f  ................
 000024b0: 7231 0000 0063 0000 0000 0000 0000 0000  r1...c..........
 000024c0: 0000 0000 0000 0400 0000 0000 0000 733a  ..............s:
 000024d0: 0000 0065 005a 0164 005a 0265 0365 0483  ...e.Z.d.Z.e.e..
 000024e0: 015a 0565 0365 0683 015a 0764 0165 0866  .Z.e.e...Z.d.e.f
@@ -598,132 +598,132 @@
 00002550: 8302 a002 a100 0100 7c01 7c00 5f03 7404  ........|.|._.t.
 00002560: a005 6401 a101 0100 7406 8300 7c00 5f07  ..d.....t...|._.
 00002570: 6400 5300 2902 4e7a 2149 6e69 7469 6174  d.S.).Nz!Initiat
 00002580: 6564 2072 6563 6f72 6469 6e67 2066 7261  ed recording fra
 00002590: 6d65 2065 6d69 7474 6572 2908 722e 0000  me emitter).r...
 000025a0: 0072 3300 0000 722f 0000 00da 1772 6563  .r3...r/.....rec
 000025b0: 6f72 6469 6e67 5f66 7261 6d65 5f62 7569  ording_frame_bui
-000025c0: 6c64 6572 726f 0000 0072 7000 0000 7204  lderro...rp...r.
+000025c0: 6c64 6572 7273 0000 0072 7400 0000 7204  lderrs...rt...r.
 000025d0: 0000 00da 0f6b 6565 705f 636f 6c6c 6563  .....keep_collec
-000025e0: 7469 6e67 2902 7244 0000 0072 b900 0000  ting).rD...r....
-000025f0: 7245 0000 0072 2a00 0000 722b 0000 0072  rE...r*...r+...r
+000025e0: 7469 6e67 2902 7245 0000 0072 c200 0000  ting).rE...r....
+000025f0: 7246 0000 0072 2a00 0000 722b 0000 0072  rF...r*...r+...r
 00002600: 2f00 0000 5001 0000 7308 0000 000e 0206  /...P...s.......
 00002610: 010a 010c 017a 1d55 6e70 6169 7265 6446  .....z.UnpairedF
 00002620: 7261 6d65 456d 6974 7465 722e 5f5f 696e  rameEmitter.__in
 00002630: 6974 5f5f 6301 0000 0000 0000 0000 0000  it__c...........
 00002640: 0003 0000 0003 0000 0043 0000 0073 6400  .........C...sd.
 00002650: 0000 7c00 6a00 a001 a100 0100 7c00 6a00  ..|.j.......|.j.
 00002660: a002 a100 722b 7c00 6a03 a004 a100 7d01  ....r+|.j.....}.
 00002670: 7c01 6400 7501 7226 7405 7c01 8301 7d02  |.d.u.r&t.|...}.
 00002680: 7c00 6a06 a007 7c02 a101 0100 7c00 6a08  |.j...|.....|.j.
 00002690: a007 7c00 6a03 6a09 6a08 a101 0100 7c00  ..|.j.j.j.....|.
 000026a0: 6a00 a002 a100 730a 740a a00b 6401 a101  j.....s.t...d...
 000026b0: 0100 6400 5300 2902 4e7a 2753 7465 7265  ..d.S.).Nz'Stere
 000026c0: 6f66 7261 6d65 2065 6d69 7474 6572 2072  oframe emitter r
 000026d0: 756e 2074 6872 6561 6420 656e 6465 642e  un thread ended.
-000026e0: 2e2e 290c 72bb 0000 00da 0373 6574 da06  ..).r......set..
-000026f0: 6973 5f73 6574 72ba 0000 0072 b800 0000  is_setr....r....
+000026e0: 2e2e 290c 72c4 0000 00da 0373 6574 da06  ..).r......set..
+000026f0: 6973 5f73 6574 72c3 0000 0072 c100 0000  is_setr....r....
 00002700: da0d 6376 325f 746f 5f71 6c61 6265 6c72  ..cv2_to_qlabelr
-00002710: 6400 0000 da04 656d 6974 7268 0000 0072  d.....emitrh...r
-00002720: 3000 0000 726f 0000 0072 7000 0000 2903  0...ro...rp...).
-00002730: 7244 0000 005a 0f72 6563 6f72 6469 6e67  rD...Z.recording
+00002710: 6700 0000 da04 656d 6974 726c 0000 0072  g.....emitrl...r
+00002720: 3000 0000 7273 0000 0072 7400 0000 2903  0...rs...rt...).
+00002730: 7245 0000 005a 0f72 6563 6f72 6469 6e67  rE...Z.recording
 00002740: 5f66 7261 6d65 da05 696d 6167 6572 2a00  _frame..imager*.
 00002750: 0000 722a 0000 0072 2b00 0000 da03 7275  ..r*...r+.....ru
 00002760: 6e57 0100 0073 1200 0000 0a02 0a02 0a04  nW...s..........
 00002770: 0802 0801 0c01 1201 0af7 0e0b 7a18 556e  ............z.Un
 00002780: 7061 6972 6564 4672 616d 6545 6d69 7474  pairedFrameEmitt
 00002790: 6572 2e72 756e 290c 7224 0000 0072 2500  er.run).r$...r%.
 000027a0: 0000 7226 0000 0072 0800 0000 720a 0000  ..r&...r....r...
-000027b0: 0072 6400 0000 727d 0000 0072 6800 0000  .rd...r}...rh...
-000027c0: 7231 0000 0072 2f00 0000 72c1 0000 0072  r1...r/...r....r
-000027d0: 7e00 0000 722a 0000 0072 2a00 0000 7245  ~...r*...r*...rE
+000027b0: 0072 6700 0000 7280 0000 0072 6c00 0000  .rg...r....rl...
+000027c0: 7231 0000 0072 2f00 0000 72ca 0000 0072  r1...r/...r....r
+000027d0: 8100 0000 722a 0000 0072 2a00 0000 7246  ....r*...r*...rF
 000027e0: 0000 0072 2b00 0000 7233 0000 004c 0100  ...r+...r3...L..
 000027f0: 0073 0a00 0000 0800 0801 0801 1202 1007  .s..............
 00002800: 7233 0000 0063 0200 0000 0000 0000 0000  r3...c..........
 00002810: 0000 0300 0000 0300 0000 0300 0000 731a  ..............s.
 00002820: 0000 0087 0066 0164 0164 0284 087c 00a0  .....f.d.d...|..
 00002830: 00a1 0044 0083 017d 027c 0253 0029 034e  ...D...}.|.S.).N
 00002840: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
 00002850: 0004 0000 0013 0000 0073 1c00 0000 6700  .........s....g.
 00002860: 7c00 5d0a 5c02 7d01 7d02 7c02 8800 6b00  |.].\.}.}.|...k.
 00002870: 7202 7c01 9102 7102 5300 722a 0000 0072  r.|...q.S.r*...r
-00002880: 2a00 0000 2903 724c 0000 00da 036b 6579  *...).rL.....key
-00002890: 723a 0000 00a9 01da 0d6d 696e 5f74 6872  r:.......min_thr
+00002880: 2a00 0000 2903 724d 0000 00da 036b 6579  *...).rM.....key
+00002890: 723b 0000 00a9 01da 0d6d 696e 5f74 6872  r;.......min_thr
 000028a0: 6573 686f 6c64 722a 0000 0072 2b00 0000  esholdr*...r+...
-000028b0: 724e 0000 006b 0100 0072 5900 0000 7a23  rN...k...rY...z#
+000028b0: 724f 0000 006b 0100 0072 5a00 0000 7a23  rO...k...rZ...z#
 000028c0: 6765 745f 656d 7074 795f 7061 6972 732e  get_empty_pairs.
 000028d0: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-000028e0: 6d70 3e29 0172 7500 0000 2903 5a0c 626f  mp>).ru...).Z.bo
-000028f0: 6172 645f 636f 756e 7473 72c4 0000 005a  ard_countsr....Z
+000028e0: 6d70 3e29 0172 7800 0000 2903 da0c 626f  mp>).rx...)...bo
+000028f0: 6172 645f 636f 756e 7473 72cd 0000 00da  ard_countsr.....
 00002900: 0b65 6d70 7479 5f70 6169 7273 722a 0000  .empty_pairsr*..
-00002910: 0072 c300 0000 722b 0000 00da 0f67 6574  .r....r+.....get
+00002910: 0072 cc00 0000 722b 0000 00da 0f67 6574  .r....r+.....get
 00002920: 5f65 6d70 7479 5f70 6169 7273 6a01 0000  _empty_pairsj...
-00002930: 7304 0000 0016 0104 0172 c500 0000 6302  s........r....c.
+00002930: 7304 0000 0016 0104 0172 d000 0000 6302  s........r....c.
 00002940: 0000 0000 0000 0000 0000 0007 0000 0005  ................
 00002950: 0000 0043 0000 0073 4400 0000 7c00 6a00  ...C...sD...|.j.
 00002960: 6400 6401 8502 1900 5c02 7d02 7d03 7c01  d.d.....\.}.}.|.
 00002970: 7401 7c02 8301 1b00 7d04 7402 7c03 7c04  t.|.....}.t.|.|.
 00002980: 1400 8301 7c01 6602 7d05 7403 6a04 7c00  ....|.f.}.t.j.|.
 00002990: 7c05 7403 6a05 6402 8d03 7d06 7c06 5300  |.t.j.d...}.|.S.
-000029a0: 2903 4e72 9800 0000 2901 da0d 696e 7465  ).Nr....)...inte
-000029b0: 7270 6f6c 6174 696f 6e29 0672 9a00 0000  rpolation).r....
-000029c0: da05 666c 6f61 7472 5800 0000 729b 0000  ..floatrX...r...
-000029d0: 0072 7700 0000 da0a 494e 5445 525f 4152  .rw.....INTER_AR
-000029e0: 4541 2907 72c0 0000 0072 9900 0000 5a0e  EA).r....r....Z.
+000029a0: 2903 4e72 9b00 0000 2901 da0d 696e 7465  ).Nr....)...inte
+000029b0: 7270 6f6c 6174 696f 6e29 0672 9d00 0000  rpolation).r....
+000029c0: da05 666c 6f61 7472 5900 0000 729e 0000  ..floatrY...r...
+000029d0: 0072 7a00 0000 da0a 494e 5445 525f 4152  .rz.....INTER_AR
+000029e0: 4541 2907 72c9 0000 0072 9c00 0000 da0e  EA).r....r......
 000029f0: 6375 7272 656e 745f 6865 6967 6874 da0d  current_height..
 00002a00: 6375 7272 656e 745f 7769 6474 68da 0572  current_width..r
-00002a10: 6174 696f da03 6469 6d5a 0772 6573 697a  atio..dimZ.resiz
+00002a10: 6174 696f da03 6469 6dda 0772 6573 697a  atio..dim..resiz
 00002a20: 6564 722a 0000 0072 2a00 0000 722b 0000  edr*...r*...r+..
-00002a30: 0072 7700 0000 6e01 0000 730a 0000 0012  .rw...n...s.....
-00002a40: 010c 0110 0112 0104 0172 7700 0000 6301  .........rw...c.
+00002a30: 0072 7a00 0000 6e01 0000 730a 0000 0012  .rz...n...s.....
+00002a40: 010c 0110 0112 0104 0172 7a00 0000 6301  .........rz...c.
 00002a50: 0000 0000 0000 0000 0000 0003 0000 0005  ................
 00002a60: 0000 0043 0000 0073 3200 0000 7400 a001  ...C...s2...t...
 00002a70: 7c00 7400 6a02 a102 7d01 7403 7c01 6a04  |.t.j...}.t.|.j.
 00002a80: 7c01 6a05 6401 1900 7c01 6a05 6402 1900  |.j.d...|.j.d...
 00002a90: 7403 6a06 6a07 8304 7d02 7c02 5300 2903  t.j.j...}.|.S.).
-00002aa0: 4e72 5500 0000 7201 0000 0029 0872 9b00  NrU...r....).r..
+00002aa0: 4e72 5600 0000 7201 0000 0029 0872 9e00  NrV...r....).r..
 00002ab0: 0000 da08 6376 7443 6f6c 6f72 da0d 434f  ....cvtColor..CO
 00002ac0: 4c4f 525f 4247 5232 5247 4272 0a00 0000  LOR_BGR2RGBr....
-00002ad0: da04 6461 7461 729a 0000 00da 0646 6f72  ..datar......For
+00002ad0: da04 6461 7461 729d 0000 00da 0646 6f72  ..datar......For
 00002ae0: 6d61 74da 0d46 6f72 6d61 745f 5247 4238  mat..Format_RGB8
-00002af0: 3838 2903 7294 0000 0072 c000 0000 5a08  88).r....r....Z.
+00002af0: 3838 2903 7297 0000 0072 c900 0000 da08  88).r....r......
 00002b00: 7174 5f66 7261 6d65 722a 0000 0072 2a00  qt_framer*...r*.
-00002b10: 0000 722b 0000 0072 be00 0000 7701 0000  ..r+...r....w...
+00002b10: 0000 722b 0000 0072 c700 0000 7701 0000  ..r+...r....w...
 00002b20: 7310 0000 000e 0102 0204 0108 0108 0106  s...............
-00002b30: 0104 fc04 0672 be00 0000 6301 0000 0000  .....r....c.....
+00002b30: 0104 fc04 0672 c700 0000 6301 0000 0000  .....r....c.....
 00002b40: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
 00002b50: 0000 0073 4c00 0000 7400 7c00 8301 7d01  ...sL...t.|...}.
 00002b60: 7401 7c01 8301 7d02 7c02 a002 a100 0100  t.|...}.|.......
 00002b70: 7c02 a003 a100 0100 7404 7405 6a06 8301  |.......t.t.j...
 00002b80: 7d03 7407 7c02 8301 7d04 7c04 a008 a100  }.t.|...}.|.....
 00002b90: 0100 7405 a009 7c03 a00a a100 a101 0100  ..t...|.........
-00002ba0: 6400 5300 7263 0000 0029 0b72 2200 0000  d.S.rc...).r"...
+00002ba0: 6400 5300 7266 0000 0029 0b72 2200 0000  d.S.rf...).r"...
 00002bb0: 721e 0000 00da 116c 6f61 645f 7374 7265  r......load_stre
 00002bc0: 616d 5f74 6f6f 6c73 da13 5f61 646a 7573  am_tools.._adjus
 00002bd0: 745f 7265 736f 6c75 7469 6f6e 7372 0d00  t_resolutionsr..
 00002be0: 0000 da03 7379 73da 0461 7267 7672 2c00  ....sys..argvr,.
 00002bf0: 0000 da04 7368 6f77 da04 6578 6974 da04  ....show..exit..
 00002c00: 6578 6563 2905 da0c 7365 7373 696f 6e5f  exec)...session_
 00002c10: 7061 7468 da06 636f 6e66 6967 722d 0000  path..configr-..
-00002c20: 005a 0341 7070 5a10 7265 636f 7264 696e  .Z.AppZ.recordin
+00002c20: 00da 0341 7070 5a10 7265 636f 7264 696e  ...AppZ.recordin
 00002c30: 675f 6469 616c 6f67 722a 0000 0072 2a00  g_dialogr*...r*.
 00002c40: 0000 722b 0000 00da 176c 6175 6e63 685f  ..r+.....launch_
 00002c50: 7265 636f 7264 696e 675f 7769 6467 6574  recording_widget
 00002c60: 8301 0000 7310 0000 0008 0108 0108 0108  ....s...........
-00002c70: 010a 0208 0108 0112 0272 da00 0000 293e  .........r....)>
+00002c70: 010a 0208 0108 0112 0272 e900 0000 293e  .........r....)>
 00002c80: da0d 7079 7879 3364 2e6c 6f67 6765 72da  ..pyxy3d.logger.
-00002c90: 0670 7978 7933 6472 6f00 0000 72af 0000  .pyxy3dro...r...
-00002ca0: 0072 2400 0000 72d3 0000 0072 8500 0000  .r$...r....r....
+00002c90: 0670 7978 7933 6472 7300 0000 72b8 0000  .pyxy3drs...r...
+00002ca0: 0072 2400 0000 72e1 0000 0072 8800 0000  .r$...r....r....
 00002cb0: da07 7061 7468 6c69 6272 0200 0000 da09  ..pathlibr......
 00002cc0: 7468 7265 6164 696e 6772 0300 0000 7204  threadingr....r.
-00002cd0: 0000 00da 056e 756d 7079 7291 0000 00da  .....numpyr.....
+00002cd0: 0000 00da 056e 756d 7079 7294 0000 00da  .....numpyr.....
 00002ce0: 0571 7565 7565 7205 0000 00da 0465 6e75  .queuer......enu
-00002cf0: 6d72 0600 0000 729b 0000 00da 0c50 7951  mr....r......PyQ
+00002cf0: 6d72 0600 0000 729e 0000 00da 0c50 7951  mr....r......PyQ
 00002d00: 7436 2e51 7443 6f72 6572 0700 0000 7208  t6.QtCorer....r.
-00002d10: 0000 0072 0900 0000 da0b 5079 5174 362e  ...r......PyQt6.
+00002d10: 0000 0072 0900 0000 5a0b 5079 5174 362e  ...r....Z.PyQt6.
 00002d20: 5174 4775 6972 0a00 0000 720b 0000 0072  QtGuir....r....r
 00002d30: 0c00 0000 da0f 5079 5174 362e 5174 5769  ......PyQt6.QtWi
 00002d40: 6467 6574 7372 0d00 0000 720e 0000 0072  dgetsr....r....r
 00002d50: 0f00 0000 7210 0000 0072 1100 0000 7212  ....r....r....r.
 00002d60: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
 00002d70: 0000 7216 0000 0072 1700 0000 7218 0000  ..r....r....r...
 00002d80: 0072 1900 0000 721a 0000 0072 1b00 0000  .r....r....r....
@@ -733,15 +733,15 @@
 00002dc0: 6361 6d65 7261 732e 7379 6e63 6872 6f6e  cameras.synchron
 00002dd0: 697a 6572 721f 0000 0072 2000 0000 da1f  izerr....r .....
 00002de0: 7079 7879 3364 2e72 6563 6f72 6469 6e67  pyxy3d.recording
 00002df0: 2e76 6964 656f 5f72 6563 6f72 6465 7272  .video_recorderr
 00002e00: 2100 0000 da13 7079 7879 3364 2e63 6f6e  !.....pyxy3d.con
 00002e10: 6669 6775 7261 746f 7272 2200 0000 7223  figuratorr"...r#
 00002e20: 0000 0072 2c00 0000 7231 0000 0072 3300  ...r,...r1...r3.
-00002e30: 0000 72c5 0000 0072 7700 0000 72be 0000  ..r....rw...r...
-00002e40: 0072 da00 0000 722a 0000 0072 2a00 0000  .r....r*...r*...
+00002e30: 0000 72d0 0000 0072 7a00 0000 72c7 0000  ..r....rz...r...
+00002e40: 0072 e900 0000 722a 0000 0072 2a00 0000  .r....r*...r*...
 00002e50: 722a 0000 0072 2b00 0000 da08 3c6d 6f64  r*...r+.....<mod
 00002e60: 756c 653e 0100 0000 7338 0000 0008 020c  ule>....s8......
 00002e70: 0108 0208 010c 0110 0108 010c 010c 0108  ................
 00002e80: 0214 0114 014c 010c 140c 010c 010c 010c  .....L..........
 00002e90: 0110 0210 0600 7f0e 0200 7f10 1b08 1e08  ................
 00002ea0: 0408 090c 0c                             .....
```

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/calibrate_capture_volume_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/calibrate_capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/calibration_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/camera_summary_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/camera_summary_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/charuco_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/charuco_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/extrinsic_calibration_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/paired_frame_builder.py` & `pyxy3d-0.0.20/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.0.20/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.0.20/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.0.20/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/log_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/log_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/main_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/main_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/navigation_bars.py` & `pyxy3d-0.0.20/pyxy3d/gui/navigation_bars.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/playback_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/playback_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/post_processing_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/post_processing_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/progress_dialog.py` & `pyxy3d-0.0.20/pyxy3d/gui/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/recording_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/playback_triangulation_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/gui/vizualize/realtime_triangulation_widget.py` & `pyxy3d-0.0.20/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/helper.py` & `pyxy3d-0.0.20/pyxy3d/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/interface.py` & `pyxy3d-0.0.20/pyxy3d/interface.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/logger.py` & `pyxy3d-0.0.20/pyxy3d/logger.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/post_processor.py` & `pyxy3d-0.0.20/pyxy3d/post_processor.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.0.20/pyxy3d/recording/recorded_stream.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.0.20/pyxy3d/recording/video_recorder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/session/__pycache__/session.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/session/__pycache__/session.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Mon Jun 12 15:10:31 2023 UTC, .py size: 20797 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 6735 8764 3d51 0000  o.......g5.d=Q..
+00000000: 6f0d 0d0a 0000 0000 814c 8764 3d51 0000  o........L.d=Q..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3801 0000 6400  .....@...s8...d.
 00000030: 6401 6c00 5a01 6501 6a02 a003 6504 a101  d.l.Z.e.j...e...
 00000040: 5a02 6400 6402 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6403 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c0a 6d0b 5a0b 0100 6400 6405 6c0c  d.l.m.Z...d.d.l.
 00000070: 6d0d 5a0d 0100 6400 6406 6c0e 6d0f 5a0f  m.Z...d.d.l.m.Z.
@@ -193,15 +193,15 @@
 00000c00: 7d01 7c00 6a03 6a04 a005 a100 4400 5d10  }.|.j.j.....D.].
 00000c10: 5c02 7d02 7d03 7c03 6a06 6400 7500 7321  \.}.}.|.j.d.u.s!
 00000c20: 7c03 6a07 6400 7500 7223 6402 7d01 7113  |.j.d.u.r#d.}.q.
 00000c30: 7c01 5300 2903 4e54 4629 0872 2800 0000  |.S.).NTF).r(...
 00000c40: da11 7265 6672 6573 685f 6672 6f6d 5f74  ..refresh_from_t
 00000c50: 6f6d 6cda 1067 6574 5f63 616d 6572 615f  oml..get_camera_
 00000c60: 6172 7261 79da 0c63 616d 6572 615f 6172  array..camera_ar
-00000c70: 7261 7972 2f00 0000 723f 0000 00da 066d  rayr/...r?.....m
+00000c70: 7261 7972 2f00 0000 723f 0000 005a 066d  rayr/...r?...Z.m
 00000c80: 6174 7269 785a 0b64 6973 746f 7274 696f  atrixZ.distortio
 00000c90: 6e73 a904 723c 0000 0072 4b00 0000 7245  ns..r<...rK...rE
 00000ca0: 0000 0072 4700 0000 7225 0000 0072 2500  ...rG...r%...r%.
 00000cb0: 0000 7226 0000 00da 2169 735f 6578 7472  ..r&....!is_extr
 00000cc0: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
 00000cd0: 6e5f 656c 6967 6962 6c65 7300 0000 7310  n_eligibles...s.
 00000ce0: 0000 000a 020c 0104 0114 0114 0104 0102  ................
@@ -243,15 +243,15 @@
 00000f20: 756d 653f 2028 692e 652e 2066 756c 6c79  ume? (i.e. fully
 00000f30: 2063 616c 6962 7261 7465 6420 6578 7472   calibrated extr
 00000f40: 696e 7369 6373 293a 2029 0c72 2800 0000  insics): ).r(...
 00000f50: 724d 0000 0072 4e00 0000 724f 0000 0072  rM...rN...rO...r
 00000f60: 4a00 0000 722f 0000 0072 3f00 0000 da08  J...r/...r?.....
 00000f70: 726f 7461 7469 6f6e da0b 7472 616e 736c  rotation..transl
 00000f80: 6174 696f 6eda 066c 6f67 6765 72da 0469  ation..logger..i
-00000f90: 6e66 6fda 085f 5f64 6963 745f 5f72 5100  nfo..__dict__rQ.
+00000f90: 6e66 6fda 085f 5f64 6963 745f 5f72 5000  nfo..__dict__rP.
 00000fa0: 0000 7225 0000 0072 2500 0000 7226 0000  ..r%...r%...r&..
 00000fb0: 00da 1a69 735f 6361 7074 7572 655f 766f  ...is_capture_vo
 00000fc0: 6c75 6d65 5f65 6c69 6769 626c 657e 0000  lume_eligible~..
 00000fd0: 0073 2000 0000 0a08 0c01 0403 1001 0401  .s .............
 00000fe0: 1402 1401 0401 0401 1001 04ff 0280 0404  ................
 00000ff0: 0801 04ff 0404 7a22 5365 7373 696f 6e2e  ......z"Session.
 00001000: 6973 5f63 6170 7475 7265 5f76 6f6c 756d  is_capture_volum
@@ -266,25 +266,25 @@
 00001090: 6a09 6404 7500 723b 6403 7d01 740a a00b  j.d.u.r;d.}.t...
 000010a0: 6405 7c02 9b00 6406 9d03 a101 0100 711d  d.|...d.......q.
 000010b0: 7c01 7242 6401 7d01 7c01 5300 6403 7d01  |.rBd.}.|.S.d.}.
 000010c0: 7c01 5300 2907 7a44 0a20 2020 2020 2020  |.S.).zD.       
 000010d0: 2055 7365 6420 746f 2064 6574 6572 6d69   Used to determi
 000010e0: 6e65 2069 6620 7468 6520 5265 636f 7264  ne if the Record
 000010f0: 2042 7574 746f 6e20 6973 2065 6e61 626c   Button is enabl
-00001100: 6564 0a0a 2020 2020 2020 2020 5472 5300  ed..        TrS.
+00001100: 6564 0a0a 2020 2020 2020 2020 5472 5200  ed..        TrR.
 00001110: 0000 464e 7a34 4361 6d65 7261 2061 7272  ..FNz4Camera arr
 00001120: 6179 2069 7320 6e6f 7420 6675 6c6c 7920  ay is not fully 
 00001130: 6361 6c69 6272 6174 6564 2062 6563 6175  calibrated becau
 00001140: 7365 2063 616d 6572 6120 7a11 206c 6163  se camera z. lac
 00001150: 6b73 2065 7874 7269 6e73 6963 7329 0c72  ks extrinsics).r
 00001160: 2800 0000 724d 0000 0072 4e00 0000 724f  (...rM...rN...rO
 00001170: 0000 0072 4a00 0000 722f 0000 0072 3f00  ...rJ...r/...r?.
-00001180: 0000 da06 6967 6e6f 7265 7254 0000 0072  ....ignorerT...r
-00001190: 5500 0000 7256 0000 0072 5700 0000 2904  U...rV...rW...).
-000011a0: 723c 0000 0072 4b00 0000 7245 0000 00da  r<...rK...rE....
+00001180: 0000 da06 6967 6e6f 7265 7253 0000 0072  ....ignorerS...r
+00001190: 5400 0000 7255 0000 0072 5600 0000 2904  T...rU...rV...).
+000011a0: 723c 0000 0072 4b00 0000 7245 0000 005a  r<...rK...rE...Z
 000011b0: 0663 616d 6572 6172 2500 0000 7225 0000  .camerar%...r%..
 000011c0: 0072 2600 0000 da15 6973 5f72 6563 6f72  .r&.....is_recor
 000011d0: 6469 6e67 5f65 6c69 6769 626c 659b 0000  ding_eligible...
 000011e0: 0073 2a00 0000 0a07 0c01 0403 1001 0401  .s*.............
 000011f0: 1402 0a01 0801 02ff 0801 02ff 0403 0401  ................
 00001200: 0a01 04ff 0280 0403 0401 0404 04fe 0402  ................
 00001210: 7a1d 5365 7373 696f 6e2e 6973 5f72 6563  z.Session.is_rec
@@ -312,17 +312,17 @@
 00001370: 0072 2600 0000 da0a 3c6c 6973 7463 6f6d  .r&.....<listcom
 00001380: 703e c000 0000 7302 0000 001a 007a 3753  p>....s......z7S
 00001390: 6573 7369 6f6e 2e69 735f 706f 7374 5f70  ession.is_post_p
 000013a0: 726f 6365 7373 696e 675f 656c 6967 6962  rocessing_eligib
 000013b0: 6c65 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  le.<locals>.<lis
 000013c0: 7463 6f6d 703e 7201 0000 0054 4629 0372  tcomp>r....TF).r
 000013d0: 2d00 0000 da07 6974 6572 6469 7272 4a00  -.....iterdirrJ.
-000013e0: 0000 2904 723c 0000 00da 0766 6f6c 6465  ..).r<.....folde
+000013e0: 0000 2904 723c 0000 005a 0766 6f6c 6465  ..).r<...Z.folde
 000013f0: 7273 5a0f 7265 636f 7264 696e 675f 636f  rsZ.recording_co
-00001400: 756e 7472 4b00 0000 7225 0000 0072 6000  untrK...r%...r`.
+00001400: 756e 7472 4b00 0000 7225 0000 0072 5e00  untrK...r%...r^.
 00001410: 0000 7226 0000 00da 1b69 735f 706f 7374  ..r&.....is_post
 00001420: 5f70 726f 6365 7373 696e 675f 656c 6967  _processing_elig
 00001430: 6962 6c65 b900 0000 7310 0000 0008 0518  ible....s.......
 00001440: 0208 0108 0104 0104 0404 fe04 027a 2353  .............z#S
 00001450: 6573 7369 6f6e 2e69 735f 706f 7374 5f70  ession.is_post_p
 00001460: 726f 6365 7373 696e 675f 656c 6967 6962  rocessing_eligib
 00001470: 6c65 723b 0000 0063 0200 0000 0000 0000  ler;...c........
@@ -411,16 +411,16 @@
 000019a0: 0000 7220 0000 0072 3700 0000 7228 0000  ..r ...r7...r(..
 000019b0: 005a 1e73 6176 655f 6670 735f 696e 7472  .Z.save_fps_intr
 000019c0: 696e 7369 635f 6361 6c69 6272 6174 696f  insic_calibratio
 000019d0: 6e72 2100 0000 7236 0000 005a 1e73 6176  nr!...r6...Z.sav
 000019e0: 655f 6670 735f 6578 7472 696e 7369 635f  e_fps_extrinsic_
 000019f0: 6361 6c69 6272 6174 696f 6e72 2300 0000  calibrationr#...
 00001a00: 7235 0000 005a 1273 6176 655f 6670 735f  r5...Z.save_fps_
-00001a10: 7265 636f 7264 696e 6772 6500 0000 2902  recordingre...).
-00001a20: 723c 0000 0072 6e00 0000 7225 0000 0072  r<...rn...r%...r
+00001a10: 7265 636f 7264 696e 6772 6200 0000 2902  recordingrb...).
+00001a20: 723c 0000 0072 6b00 0000 7225 0000 0072  r<...rk...r%...r
 00001a30: 2500 0000 7226 0000 00da 1373 6574 5f61  %...r&.....set_a
 00001a40: 6374 6976 655f 6d6f 6465 5f66 7073 0101  ctive_mode_fps..
 00001a50: 0000 731e 0000 0004 050c 0102 010c 0102  ..s.............
 00001a60: 010c 0106 010e 010c 0106 010e 0108 0106  ................
 00001a70: 010c 010c 027a 1b53 6573 7369 6f6e 2e73  .....z.Session.s
 00001a80: 6574 5f61 6374 6976 655f 6d6f 6465 5f66  et_active_mode_f
 00001a90: 7073 da06 7265 7475 726e 6301 0000 0000  ps..returnc.....
@@ -444,71 +444,71 @@
 00001bb0: 0403 08fe 0601 0801 7a1b 5365 7373 696f  ........z.Sessio
 00001bc0: 6e2e 6765 745f 6163 7469 7665 5f6d 6f64  n.get_active_mod
 00001bd0: 655f 6670 7363 0100 0000 0000 0000 0000  e_fpsc..........
 00001be0: 0000 0400 0000 0400 0000 4300 0000 7336  ..........C...s6
 00001bf0: 0000 007c 00a0 00a1 007d 017c 0164 0075  ...|.....}.|.d.u
 00001c00: 0172 177c 006a 01a0 02a1 0044 005d 0b5c  .r.|.j.....D.].\
 00001c10: 027d 027d 037c 03a0 037c 01a1 0101 0071  .}.}.|...|.....q
-00001c20: 0d64 0053 0064 0053 0072 7100 0000 2904  .d.S.d.S.rq...).
-00001c30: 7272 0000 0072 3000 0000 723f 0000 005a  rr...r0...r?...Z
+00001c20: 0d64 0053 0064 0053 0072 6e00 0000 2904  .d.S.d.S.rn...).
+00001c30: 726f 0000 0072 3000 0000 723f 0000 005a  ro...r0...r?...Z
 00001c40: 0e73 6574 5f66 7073 5f74 6172 6765 7429  .set_fps_target)
 00001c50: 0472 3c00 0000 5a0f 6163 7469 7665 5f6d  .r<...Z.active_m
 00001c60: 6f64 655f 6670 7372 4500 0000 7246 0000  ode_fpsrE...rF..
 00001c70: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00001c80: 7265 0000 0026 0100 0073 0c00 0000 0801  re...&...s......
+00001c80: 7262 0000 0026 0100 0073 0c00 0000 0801  rb...&...s......
 00001c90: 0801 1201 0c01 04fe 0401 7a1a 5365 7373  ..........z.Sess
 00001ca0: 696f 6e2e 7570 6461 7465 5f73 7472 6561  ion.update_strea
 00001cb0: 6d73 5f66 7073 da0b 7472 6163 6b69 6e67  ms_fps..tracking
 00001cc0: 5f6f 6e63 0200 0000 0000 0000 0000 0000  _onc............
 00001cd0: 0400 0000 0400 0000 4300 0000 7322 0000  ........C...s"..
 00001ce0: 007c 006a 00a0 01a1 0044 005d 095c 027d  .|.j.....D.].\.}
 00001cf0: 027d 037c 03a0 027c 01a1 0101 0071 0564  .}.|...|.....q.d
-00001d00: 0053 0072 7100 0000 2903 7230 0000 0072  .S.rq...).r0...r
+00001d00: 0053 0072 6e00 0000 2903 7230 0000 0072  .S.rn...).r0...r
 00001d10: 3f00 0000 5a0f 7365 745f 7472 6163 6b69  ?...Z.set_tracki
-00001d20: 6e67 5f6f 6e29 0472 3c00 0000 7273 0000  ng_on).r<...rs..
+00001d20: 6e67 5f6f 6e29 0472 3c00 0000 7270 0000  ng_on).r<...rp..
 00001d30: 0072 4500 0000 7246 0000 0072 2500 0000  .rE...rF...r%...
-00001d40: 7225 0000 0072 2600 0000 726a 0000 002c  r%...r&...rj...,
+00001d40: 7225 0000 0072 2600 0000 7267 0000 002c  r%...r&...rg...,
 00001d50: 0100 0073 0600 0000 1201 0c01 04ff 7a1c  ...s..........z.
 00001d60: 5365 7373 696f 6e2e 7365 745f 7374 7265  Session.set_stre
 00001d70: 616d 735f 7472 6163 6b69 6e67 6301 0000  ams_trackingc...
 00001d80: 0000 0000 0000 0000 0003 0000 0004 0000  ................
 00001d90: 0043 0000 0073 3a00 0000 7400 a001 6401  .C...s:...t...d.
 00001da0: a101 0100 7402 7c00 6a03 8301 7c00 5f04  ....t.|.j...|._.
 00001db0: 7c00 6a05 a006 a100 4400 5d0a 5c02 7d01  |.j.....D.].\.}.
 00001dc0: 7d02 7c02 a007 7c00 6a04 a101 0100 7110  }.|...|.j.....q.
 00001dd0: 6400 5300 2902 4e7a 2275 7064 6174 696e  d.S.).Nz"updatin
 00001de0: 6720 6368 6172 7563 6f20 696e 2063 6173  g charuco in cas
-00001df0: 6520 6e65 6365 7373 6172 7929 0872 5600  e necessary).rV.
-00001e00: 0000 7257 0000 0072 0900 0000 7239 0000  ..rW...r....r9..
+00001df0: 6520 6e65 6365 7373 6172 7929 0872 5500  e necessary).rU.
+00001e00: 0000 7256 0000 0072 0900 0000 7239 0000  ..rV...r....r9..
 00001e10: 0072 3a00 0000 7230 0000 0072 3f00 0000  .r:...r0...r?...
 00001e20: 5a0e 7570 6461 7465 5f74 7261 636b 6572  Z.update_tracker
 00001e30: 2903 723c 0000 0072 4500 0000 7246 0000  ).r<...rE...rF..
 00001e40: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
-00001e50: 7269 0000 0030 0100 0073 0a00 0000 0a01  ri...0...s......
+00001e50: 7266 0000 0030 0100 0073 0a00 0000 0a01  rf...0...s......
 00001e60: 0c01 1201 0e01 04ff 7a1b 5365 7373 696f  ........z.Sessio
 00001e70: 6e2e 7365 745f 7374 7265 616d 735f 6368  n.set_streams_ch
 00001e80: 6172 7563 6f63 0100 0000 0000 0000 0000  arucoc..........
 00001e90: 0000 0100 0000 0300 0000 4300 0000 7318  ..........C...s.
 00001ea0: 0000 0074 00a0 0164 01a1 0101 007c 006a  ...t...d.....|.j
 00001eb0: 02a0 03a1 0001 0064 0053 0029 024e 7a14  .......d.S.).Nz.
 00001ec0: 7061 7573 696e 6720 7379 6e63 6872 6f6e  pausing synchron
-00001ed0: 697a 6572 2904 7256 0000 0072 5700 0000  izer).rV...rW...
-00001ee0: 7242 0000 0072 6600 0000 a901 723c 0000  rB...rf.....r<..
+00001ed0: 697a 6572 2904 7255 0000 0072 5600 0000  izer).rU...rV...
+00001ee0: 7242 0000 0072 6300 0000 a901 723c 0000  rB...rc.....r<..
 00001ef0: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
 00001f00: da12 7061 7573 655f 7379 6e63 6872 6f6e  ..pause_synchron
 00001f10: 697a 6572 3601 0000 7304 0000 000a 010e  izer6...s.......
 00001f20: 017a 1a53 6573 7369 6f6e 2e70 6175 7365  .z.Session.pause
 00001f30: 5f73 796e 6368 726f 6e69 7a65 7263 0100  _synchronizerc..
 00001f40: 0000 0000 0000 0000 0000 0100 0000 0300  ................
 00001f50: 0000 4300 0000 731e 0000 007c 006a 00a0  ..C...s....|.j..
 00001f60: 01a1 0001 007c 006a 00a0 027c 006a 006a  .....|.j...|.j.j
-00001f70: 03a1 0101 0064 0053 0072 7100 0000 2904  .....d.S.rq...).
-00001f80: 7242 0000 0072 6c00 0000 5a0e 7365 745f  rB...rl...Z.set_
-00001f90: 7374 7265 616d 5f66 7073 726e 0000 0072  stream_fpsrn...r
-00001fa0: 7400 0000 7225 0000 0072 2500 0000 7226  t...r%...r%...r&
+00001f70: 03a1 0101 0064 0053 0072 6e00 0000 2904  .....d.S.rn...).
+00001f80: 7242 0000 0072 6900 0000 5a0e 7365 745f  rB...ri...Z.set_
+00001f90: 7374 7265 616d 5f66 7073 726b 0000 0072  stream_fpsrk...r
+00001fa0: 7100 0000 7225 0000 0072 2500 0000 7226  q...r%...r%...r&
 00001fb0: 0000 00da 1475 6e70 6175 7365 5f73 796e  .....unpause_syn
 00001fc0: 6368 726f 6e69 7a65 723a 0100 0073 0400  chronizer:...s..
 00001fd0: 0000 0a01 1401 7a1c 5365 7373 696f 6e2e  ......z.Session.
 00001fe0: 756e 7061 7573 655f 7379 6e63 6872 6f6e  unpause_synchron
 00001ff0: 697a 6572 6301 0000 0000 0000 0000 0000  izerc...........
 00002000: 0004 0000 0004 0000 0043 0000 0073 3400  .........C...s4.
 00002010: 0000 6401 7d01 7c00 6a00 6a01 a002 a100  ..d.}.|.j.j.....
@@ -559,36 +559,36 @@
 000022e0: 0100 7400 a001 6406 7c00 9b00 9d02 a101  ..t...d.|.......
 000022f0: 0100 5900 6400 5300 2907 4e7a 0c54 7279  ..Y.d.S.).Nz.Try
 00002300: 696e 6720 706f 7274 207a 1053 7563 6365  ing port z.Succe
 00002310: 7373 2061 7420 706f 7274 207a 174c 6f61  ss at port z.Loa
 00002320: 6469 6e67 2073 7472 6561 6d20 6174 2070  ding stream at p
 00002330: 6f72 7420 7a25 2077 6974 6820 6368 6172  ort z% with char
 00002340: 7563 6f20 7472 6163 6b65 7220 666f 7220  uco tracker for 
-00002350: 6361 6c69 6272 6174 696f 6ea9 01da 0774  calibration....t
+00002350: 6361 6c69 6272 6174 696f 6ea9 015a 0774  calibration..Z.t
 00002360: 7261 636b 6572 7a12 4e6f 2063 616d 6572  rackerz.No camer
-00002370: 6120 6174 2070 6f72 7420 290a 7256 0000  a at port ).rV..
-00002380: 0072 5700 0000 720b 0000 0072 2f00 0000  .rW...r....r/...
+00002370: 6120 6174 2070 6f72 7420 290a 7255 0000  a at port ).rU..
+00002380: 0072 5600 0000 720b 0000 0072 2f00 0000  .rV...r....r/...
 00002390: 7228 0000 005a 0b73 6176 655f 6361 6d65  r(...Z.save_came
 000023a0: 7261 7216 0000 0072 0900 0000 7239 0000  rar....r....r9..
 000023b0: 0072 3000 0000 2902 7245 0000 0072 4700  .r0...).rE...rG.
-000023c0: 0000 7274 0000 0072 2500 0000 7226 0000  ..rt...r%...r&..
+000023c0: 0000 7271 0000 0072 2500 0000 7226 0000  ..rq...r%...r&..
 000023d0: 00da 0761 6464 5f63 616d 4b01 0000 731c  ...add_camK...s.
 000023e0: 0000 0002 0110 0108 0110 010a 010c 0104  ................
 000023f0: 010a 0104 ff02 030a 0112 ff06 0316 017a  ...............z
 00002400: 2653 6573 7369 6f6e 2e5f 6669 6e64 5f63  &Session._find_c
 00002410: 616d 6572 6173 2e3c 6c6f 6361 6c73 3e2e  ameras.<locals>.
-00002420: 6164 645f 6361 6d72 0100 0000 4eda 0673  add_camr....N..s
+00002420: 6164 645f 6361 6d72 0100 0000 4e5a 0673  add_camr....NZ.s
 00002430: 7465 7265 6f29 0a72 0400 0000 da05 7261  tereo).r......ra
 00002440: 6e67 65da 154d 4158 5f43 414d 4552 415f  nge..MAX_CAMERA_
 00002450: 504f 5254 5f43 4845 434b 722f 0000 00da  PORT_CHECKr/....
 00002460: 046b 6579 73da 0673 7562 6d69 7472 2800  .keys..submitr(.
-00002470: 0000 7278 0000 0072 7900 0000 727a 0000  ..rx...ry...rz..
-00002480: 0029 0572 3c00 0000 7281 0000 00da 0865  .).r<...r......e
-00002490: 7865 6375 746f 72da 0169 727c 0000 0072  xecutor..ir|...r
-000024a0: 2500 0000 7274 0000 0072 2600 0000 da0d  %...rt...r&.....
+00002470: 0000 7275 0000 0072 7600 0000 7277 0000  ..ru...rv...rw..
+00002480: 0029 0572 3c00 0000 727d 0000 00da 0865  .).r<...r}.....e
+00002490: 7865 6375 746f 72da 0169 7279 0000 0072  xecutor..iry...r
+000024a0: 2500 0000 7271 0000 0072 2600 0000 da0d  %...rq...r&.....
 000024b0: 5f66 696e 645f 6361 6d65 7261 7345 0100  _find_camerasE..
 000024c0: 0073 1a00 0000 0c06 0810 0e01 0e01 0202  .s..............
 000024d0: 0e02 02fb 1cff 1409 0a01 0a01 0280 04fe  ................
 000024e0: 7a15 5365 7373 696f 6e2e 5f66 696e 645f  z.Session._find_
 000024f0: 6361 6d65 7261 7363 0100 0000 0000 0000  camerasc........
 00002500: 0000 0000 0300 0000 0500 0000 4300 0000  ............C...
 00002510: 73d0 0000 0064 017c 005f 007c 006a 01a0  s....d.|._.|.j..
@@ -613,32 +613,32 @@
 00002640: 4265 6361 7573 6520 7468 6573 6520 7374  Because these st
 00002650: 7265 616d 7320 6172 6520 6176 6169 6c61  reams are availa
 00002660: 626c 652c 2074 6865 2073 796e 6368 726f  ble, the synchro
 00002670: 6e69 7a65 7220 6361 6e20 7468 656e 2062  nizer can then b
 00002680: 6520 696e 6974 6961 6c69 7a65 640a 2020  e initialized.  
 00002690: 2020 2020 2020 5472 0100 0000 7a18 4c6f        Tr....z.Lo
 000026a0: 6164 696e 6720 5374 7265 616d 2066 6f72  ading Stream for
-000026b0: 2070 6f72 7420 727f 0000 0046 7a2d 5369   port r....Fz-Si
+000026b0: 2070 6f72 7420 727c 0000 0046 7a2d 5369   port r|...Fz-Si
 000026c0: 676e 616c 6c69 6e67 2073 7563 6365 7373  gnalling success
 000026d0: 6675 6c20 6c6f 6164 696e 6720 6f66 2073  ful loading of s
 000026e0: 7472 6561 6d20 746f 6f6c 734e 2919 7231  tream toolsN).r1
 000026f0: 0000 0072 2800 0000 5a0b 6765 745f 6361  ...r(...Z.get_ca
 00002700: 6d65 7261 7372 2f00 0000 724a 0000 0072  merasr/...rJ...r
-00002710: 8900 0000 723f 0000 0072 3000 0000 7285  ....r?...r0...r.
-00002720: 0000 0072 5600 0000 7257 0000 0072 1600  ...rV...rW...r..
+00002710: 8400 0000 723f 0000 0072 3000 0000 7280  ....r?...r0...r.
+00002720: 0000 0072 5500 0000 7256 0000 0072 1600  ...rU...rV...r..
 00002730: 0000 723a 0000 00da 135f 6164 6a75 7374  ..r:....._adjust
 00002740: 5f72 6573 6f6c 7574 696f 6e73 da15 5f6c  _resolutions.._l
 00002750: 6f61 645f 6d6f 6e6f 6361 6c69 6272 6174  oad_monocalibrat
 00002760: 6f72 73da 036d 696e 7233 0000 0072 3400  ors..minr3...r4.
 00002770: 0000 720c 0000 0072 4200 0000 7232 0000  ..r....rB...r2..
 00002780: 00da 1a73 7472 6561 6d5f 746f 6f6c 735f  ...stream_tools_
 00002790: 6c6f 6164 6564 5f73 6967 6e61 6c72 4400  loaded_signalrD.
-000027a0: 0000 7267 0000 0072 7500 0000 a903 723c  ..rg...ru.....r<
+000027a0: 0000 7264 0000 0072 7200 0000 a903 723c  ..rd...rr.....r<
 000027b0: 0000 0072 4500 0000 7247 0000 0072 2500  ...rE...rG...r%.
-000027c0: 0000 7225 0000 0072 2600 0000 7268 0000  ..r%...r&...rh..
+000027c0: 0000 7225 0000 0072 2600 0000 7265 0000  ..r%...r&...re..
 000027d0: 0068 0100 0073 2a00 0000 0605 0c02 0e02  .h...s*.........
 000027e0: 0801 1202 0e01 0201 1002 1601 0802 0801  ................
 000027f0: 1003 0202 0401 06ff 0605 0601 0a01 0a01  ................
 00002800: 0802 0c01 7a19 5365 7373 696f 6e2e 6c6f  ....z.Session.lo
 00002810: 6164 5f73 7472 6561 6d5f 746f 6f6c 7363  ad_stream_toolsc
 00002820: 0100 0000 0000 0000 0000 0000 0300 0000  ................
 00002830: 0600 0000 4300 0000 735e 0000 007c 006a  ....C...s^...|.j
@@ -652,17 +652,17 @@
 000028b0: 6e6f 6361 6c69 6272 6174 6f72 2063 7265  nocalibrator cre
 000028c0: 6174 696f 6e20 666f 7220 706f 7274 207a  ation for port z
 000028d0: 1b20 6265 6361 7573 6520 6974 2061 6c72  . because it alr
 000028e0: 6561 6479 2065 7869 7374 732e 7a20 4c6f  eady exists.z Lo
 000028f0: 6164 696e 6720 4d6f 6e6f 6361 6c69 6272  ading Monocalibr
 00002900: 6174 6f72 2066 6f72 2070 6f72 7420 2908  ator for port ).
 00002910: 722f 0000 0072 3f00 0000 7233 0000 0072  r/...r?...r3...r
-00002920: 8500 0000 7256 0000 0072 5700 0000 720a  ....rV...rW...r.
-00002930: 0000 0072 3000 0000 728e 0000 0072 2500  ...r0...r....r%.
-00002940: 0000 7225 0000 0072 2600 0000 728b 0000  ..r%...r&...r...
+00002920: 8000 0000 7255 0000 0072 5600 0000 720a  ....rU...rV...r.
+00002930: 0000 0072 3000 0000 7289 0000 0072 2500  ...r0...r....r%.
+00002940: 0000 7225 0000 0072 2600 0000 7286 0000  ..r%...r&...r...
 00002950: 008e 0100 0073 1200 0000 1201 0e01 0401  .....s..........
 00002960: 0a01 04ff 0203 1002 1601 04f8 7a1d 5365  ............z.Se
 00002970: 7373 696f 6e2e 5f6c 6f61 645f 6d6f 6e6f  ssion._load_mono
 00002980: 6361 6c69 6272 6174 6f72 734e da0b 6163  calibratorsN..ac
 00002990: 7469 7665 5f70 6f72 7463 0200 0000 0000  tive_portc......
 000029a0: 0000 0000 0000 0200 0000 0500 0000 4300  ..............C.
 000029b0: 0000 7346 0000 007c 0164 0175 0172 0f74  ..sF...|.d.u.r.t
@@ -680,19 +680,19 @@
 00002a70: 726f 6365 7373 0a20 2020 2020 2020 204e  rocess.        N
 00002a80: 7a29 5365 7474 696e 6720 7365 7373 696f  z)Setting sessio
 00002a90: 6e20 6163 7469 7665 206d 6f6e 6f63 616c  n active monocal
 00002aa0: 6962 7261 746f 7220 746f 207a 1a41 6374  ibrator to z.Act
 00002ab0: 6976 6174 6520 7472 6163 6b69 6e67 206f  ivate tracking o
 00002ac0: 6e20 706f 7274 207a 1620 616e 6420 6465  n port z. and de
 00002ad0: 6163 7469 7661 7465 206f 7468 6572 7329  activate others)
-00002ae0: 0572 5600 0000 7257 0000 0072 3400 0000  .rV...rW...r4...
+00002ae0: 0572 5500 0000 7256 0000 0072 3400 0000  .rU...rV...r4...
 00002af0: 7233 0000 005a 1373 7562 7363 7269 6265  r3...Z.subscribe
 00002b00: 5f74 6f5f 7374 7265 616d 2902 723c 0000  _to_stream).r<..
-00002b10: 0072 8f00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
-00002b20: 7226 0000 0072 6b00 0000 9901 0000 730e  r&...rk.......s.
+00002b10: 0072 8a00 0000 7225 0000 0072 2500 0000  .r....r%...r%...
+00002b20: 7226 0000 0072 6800 0000 9901 0000 730e  r&...rh.......s.
 00002b30: 0000 0008 0510 0106 0104 010c 0104 ff14  ................
 00002b40: 037a 1f53 6573 7369 6f6e 2e61 6374 6976  .z.Session.activ
 00002b50: 6174 655f 6d6f 6e6f 6361 6c69 6272 6174  ate_monocalibrat
 00002b60: 6f72 6301 0000 0000 0000 0000 0000 0003  orc.............
 00002b70: 0000 0003 0000 0043 0000 0073 2a00 0000  .......C...s*...
 00002b80: 7400 a001 6401 a101 0100 7c00 6a02 a003  t...d.....|.j...
 00002b90: a100 4400 5d08 5c02 7d01 7d02 7c02 a004  ..D.].\.}.}.|...
@@ -704,19 +704,19 @@
 00002bf0: 2020 2020 6f72 2077 6865 6e20 7369 6c65      or when sile
 00002c00: 6e63 696e 6720 616c 6c20 696e 2070 7265  ncing all in pre
 00002c10: 7061 7261 7469 6f6e 2066 6f72 2061 6374  paration for act
 00002c20: 6976 6174 696e 6720 6f6e 6c79 206f 6e65  ivating only one
 00002c30: 0a20 2020 2020 2020 207a 2550 6175 7369  .        z%Pausi
 00002c40: 6e67 2061 6c6c 206d 6f6e 6f63 616c 6962  ng all monocalib
 00002c50: 7261 746f 7220 6c6f 6f70 696e 672e 2e2e  rator looping...
-00002c60: 4e29 0572 5600 0000 7257 0000 0072 3300  N).rV...rW...r3.
+00002c60: 4e29 0572 5500 0000 7256 0000 0072 3300  N).rU...rV...r3.
 00002c70: 0000 723f 0000 005a 1575 6e73 7562 7363  ..r?...Z.unsubsc
 00002c80: 7269 6265 5f74 6f5f 7374 7265 616d 2903  ribe_to_stream).
 00002c90: 723c 0000 0072 4500 0000 7248 0000 0072  r<...rE...rH...r
-00002ca0: 2500 0000 7225 0000 0072 2600 0000 7267  %...r%...r&...rg
+00002ca0: 2500 0000 7225 0000 0072 2600 0000 7264  %...r%...r&...rd
 00002cb0: 0000 00a6 0100 0073 0800 0000 0a05 1201  .......s........
 00002cc0: 0a01 04ff 7a21 5365 7373 696f 6e2e 7061  ....z!Session.pa
 00002cd0: 7573 655f 616c 6c5f 6d6f 6e6f 6361 6c69  use_all_monocali
 00002ce0: 6272 6174 6f72 7346 da15 6465 7374 696e  bratorsF..destin
 00002cf0: 6174 696f 6e5f 6469 7265 6374 6f72 79da  ation_directory.
 00002d00: 1373 746f 7265 5f70 6f69 6e74 5f68 6973  .store_point_his
 00002d10: 746f 7279 6303 0000 0000 0000 0000 0000  toryc...........
@@ -724,21 +724,21 @@
 00002d30: 0000 7400 a001 6401 a101 0100 7c01 6a02  ..t...d.....|.j.
 00002d40: 6402 6402 6403 8d02 0100 7403 7c00 6a04  d.d.d.....t.|.j.
 00002d50: 8301 7c00 5f05 7c00 6a05 6a06 7c01 7c02  ..|._.|.j.j.|.|.
 00002d60: 6404 8d02 0100 6402 7c00 5f07 6400 5300  d.....d.|._.d.S.
 00002d70: 2905 4e7a 1749 6e69 7469 6174 696e 6720  ).Nz.Initiating 
 00002d80: 7265 636f 7264 696e 672e 2e2e 5429 02da  recording...T)..
 00002d90: 0770 6172 656e 7473 da08 6578 6973 745f  .parents..exist_
-00002da0: 6f6b 2901 7291 0000 0029 0872 5600 0000  ok).r....).rV...
-00002db0: 7257 0000 00da 056d 6b64 6972 7217 0000  rW.....mkdirr...
+00002da0: 6f6b 2901 728c 0000 0029 0872 5500 0000  ok).r....).rU...
+00002db0: 7256 0000 00da 056d 6b64 6972 7217 0000  rV.....mkdirr...
 00002dc0: 0072 4200 0000 da0e 7669 6465 6f5f 7265  .rB.....video_re
 00002dd0: 636f 7264 6572 da0f 7374 6172 745f 7265  corder..start_re
 00002de0: 636f 7264 696e 6772 3800 0000 2903 723c  cordingr8...).r<
-00002df0: 0000 0072 9000 0000 7291 0000 0072 2500  ...r....r....r%.
-00002e00: 0000 7225 0000 0072 2600 0000 7296 0000  ..r%...r&...r...
+00002df0: 0000 0072 8b00 0000 728c 0000 0072 2500  ...r....r....r%.
+00002e00: 0000 7225 0000 0072 2600 0000 7291 0000  ..r%...r&...r...
 00002e10: 00af 0100 0073 0e00 0000 0a03 0e01 0c02  .....s..........
 00002e20: 0601 0401 06ff 0a03 7a17 5365 7373 696f  ........z.Sessio
 00002e30: 6e2e 7374 6172 745f 7265 636f 7264 696e  n.start_recordin
 00002e40: 6763 0100 0000 0000 0000 0000 0000 0100  gc..............
 00002e50: 0000 0300 0000 4300 0000 736a 0000 0074  ......C...sj...t
 00002e60: 00a0 0164 01a1 0101 007c 006a 02a0 03a1  ...d.....|.j....
 00002e70: 0001 007c 006a 026a 0472 1b74 00a0 0164  ...|.j.j.r.t...d
@@ -751,24 +751,24 @@
 00002ee0: 2e2e 2e7a 2e57 6169 7469 6e67 2066 6f72  ...z.Waiting for
 00002ef0: 2076 6964 656f 2072 6563 6f72 6465 7220   video recorder 
 00002f00: 746f 2073 6176 6520 6f75 7420 6461 7461  to save out data
 00002f10: 2e2e 2e67 0000 0000 0000 e03f 467a 3d52  ...g.......?Fz=R
 00002f20: 6563 6f72 6469 6e67 206f 6620 6672 616d  ecording of fram
 00002f30: 6573 2069 7320 636f 6d70 6c65 7465 2e2e  es is complete..
 00002f40: 2e73 6967 6e61 6c6c 696e 6720 6368 616e  .signalling chan
-00002f50: 6765 2069 6e20 7374 6174 7573 290b 7256  ge in status).rV
-00002f60: 0000 0072 5700 0000 7295 0000 00da 0e73  ...rW...r......s
+00002f50: 6765 2069 6e20 7374 6174 7573 290b 7255  ge in status).rU
+00002f60: 0000 0072 5600 0000 7290 0000 00da 0e73  ...rV...r......s
 00002f70: 746f 705f 7265 636f 7264 696e 675a 0972  top_recordingZ.r
 00002f80: 6563 6f72 6469 6e67 7206 0000 0072 3800  ecordingr....r8.
 00002f90: 0000 da19 7265 636f 7264 696e 675f 636f  ....recording_co
 00002fa0: 6d70 6c65 7465 5f73 6967 6e61 6c72 4400  mplete_signalrD.
-00002fb0: 0000 7264 0000 00da 1575 6e6c 6f63 6b5f  ..rd.....unlock_
-00002fc0: 706f 7374 7072 6f63 6573 7369 6e67 7274  postprocessingrt
+00002fb0: 0000 7261 0000 00da 1575 6e6c 6f63 6b5f  ..ra.....unlock_
+00002fc0: 706f 7374 7072 6f63 6573 7369 6e67 7271  postprocessingrq
 00002fd0: 0000 0072 2500 0000 7225 0000 0072 2600  ...r%...r%...r&.
-00002fe0: 0000 7297 0000 00bb 0100 0073 1800 0000  ..r........s....
+00002fe0: 0000 7292 0000 00bb 0100 0073 1800 0000  ..r........s....
 00002ff0: 0a01 0a01 0801 0a01 0801 08fe 0604 0a02  ................
 00003000: 0a01 0802 0e01 04ff 7a16 5365 7373 696f  ........z.Sessio
 00003010: 6e2e 7374 6f70 5f72 6563 6f72 6469 6e67  n.stop_recording
 00003020: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
 00003030: 0008 0000 0003 0000 0073 5400 0000 8700  .........sT.....
 00003040: 6601 6401 6402 8408 7d01 7400 8300 8f17  f.d.d...}.t.....
 00003050: 7d02 8800 6a01 a002 a100 4400 5d08 7d03  }...j.....D.].}.
@@ -794,39 +794,39 @@
 00003190: 6403 6407 8502 1900 9b00 6408 7c02 6403  d.d.......d.|.d.
 000031a0: 6407 8502 1900 9b00 9d06 a101 0100 7c01  d.............|.
 000031b0: a007 7c02 a101 0100 7405 a006 6409 7c00  ..|.....t...d.|.
 000031c0: 9b00 6406 7c03 6403 6407 8502 1900 9b00  ..d.|.d.d.......
 000031d0: 6408 7c02 6403 6407 8502 1900 9b00 9d06  d.|.d.d.........
 000031e0: a101 0100 6400 5300 6400 5300 290a 4e5a  ....d.S.d.S.).NZ
 000031f0: 0463 616d 5fda 0473 697a 6572 0100 0000  .cam_..sizer....
-00003200: 7277 0000 007a 2742 6567 696e 6e69 6e67  rw...z'Beginning
+00003200: 7274 0000 007a 2742 6567 696e 6e69 6e67  rt...z'Beginning
 00003210: 2074 6f20 6368 616e 6765 2072 6573 6f6c   to change resol
 00003220: 7574 696f 6e20 6174 2070 6f72 7420 7a06  ution at port z.
-00003230: 2066 726f 6d20 7253 0000 007a 0420 746f   from rS...z. to
+00003230: 2066 726f 6d20 7252 0000 007a 0420 746f   from rR...z. to
 00003240: 207a 2743 6f6d 706c 6574 6564 2063 6861   z'Completed cha
 00003250: 6e67 6520 6f66 2072 6573 6f6c 7574 696f  nge of resolutio
 00003260: 6e20 6174 2070 6f72 7420 2908 7230 0000  n at port ).r0..
-00003270: 0072 2800 0000 7278 0000 0072 2f00 0000  .r(...rx...r/...
+00003270: 0072 2800 0000 7275 0000 0072 2f00 0000  .r(...ru...r/...
 00003280: 5a12 6465 6661 756c 745f 7265 736f 6c75  Z.default_resolu
-00003290: 7469 6f6e 7256 0000 0072 5700 0000 5a11  tionrV...rW...Z.
+00003290: 7469 6f6e 7255 0000 0072 5600 0000 5a11  tionrU...rV...Z.
 000032a0: 6368 616e 6765 5f72 6573 6f6c 7574 696f  change_resolutio
-000032b0: 6e29 0472 4500 0000 7246 0000 0072 9a00  n).rE...rF...r..
+000032b0: 6e29 0472 4500 0000 7246 0000 0072 9500  n).rE...rF...r..
 000032c0: 0000 5a0c 6465 6661 756c 745f 7369 7a65  ..Z.default_size
-000032d0: 7274 0000 0072 2500 0000 7226 0000 00da  rt...r%...r&....
+000032d0: 7271 0000 0072 2500 0000 7226 0000 00da  rq...r%...r&....
 000032e0: 1161 646a 7573 745f 7265 735f 776f 726b  .adjust_res_work
 000032f0: 6572 ce01 0000 7318 0000 000a 0116 010c  er....s.........
 00003300: 0120 0204 0124 0104 ff0a 0304 0124 0108  . ...$.......$..
 00003310: ff04 fb7a 3653 6573 7369 6f6e 2e5f 6164  ...z6Session._ad
 00003320: 6a75 7374 5f72 6573 6f6c 7574 696f 6e73  just_resolutions
 00003330: 2e3c 6c6f 6361 6c73 3e2e 6164 6a75 7374  .<locals>.adjust
 00003340: 5f72 6573 5f77 6f72 6b65 724e 2904 7204  _res_workerN).r.
-00003350: 0000 0072 2f00 0000 7285 0000 0072 8600  ...r/...r....r..
-00003360: 0000 2904 723c 0000 0072 9b00 0000 7287  ..).r<...r....r.
-00003370: 0000 0072 4500 0000 7225 0000 0072 7400  ...rE...r%...rt.
-00003380: 0000 7226 0000 0072 8a00 0000 ca01 0000  ..r&...r........
+00003350: 0000 0072 2f00 0000 7280 0000 0072 8100  ...r/...r....r..
+00003360: 0000 2904 723c 0000 0072 9600 0000 7282  ..).r<...r....r.
+00003370: 0000 0072 4500 0000 7225 0000 0072 7100  ...rE...r%...rq.
+00003380: 0000 7226 0000 0072 8500 0000 ca01 0000  ..r&...r........
 00003390: 730c 0000 000c 0408 0e0e 010e 0102 ff22  s.............."
 000033a0: ff7a 1b53 6573 7369 6f6e 2e5f 6164 6a75  .z.Session._adju
 000033b0: 7374 5f72 6573 6f6c 7574 696f 6e73 6301  st_resolutionsc.
 000033c0: 0000 0000 0000 0000 0000 0001 0000 0004  ................
 000033d0: 0000 0043 0000 0073 7a00 0000 7c00 6a00  ...C...sz...|.j.
 000033e0: a001 a100 7c00 5f02 7c00 6a00 a003 a100  ....|._.|.j.....
 000033f0: 7c00 5f04 7405 7c00 6a04 7c00 6a02 8302  |._.t.|.j.|.j...
@@ -852,19 +852,19 @@
 00003530: 6f20 7468 726f 7567 6820 7468 6520 7374  o through the st
 00003540: 6570 730a 0a20 2020 2020 2020 20da 0e63  eps..        ..c
 00003550: 6170 7475 7265 5f76 6f6c 756d 65da 0573  apture_volume..s
 00003560: 7461 6765 da11 6f72 6967 696e 5f73 796e  tage..origin_syn
 00003570: 635f 696e 6465 7829 0172 3900 0000 4e29  c_index).r9...N)
 00003580: 0e72 2800 0000 7214 0000 00da 0f70 6f69  .r(...r......poi
 00003590: 6e74 5f65 7374 696d 6174 6573 724e 0000  nt_estimatesrN..
-000035a0: 0072 4f00 0000 7211 0000 0072 9c00 0000  .rO...r....r....
-000035b0: 7278 0000 0072 9d00 0000 7285 0000 0072  rx...r....r....r
-000035c0: 9e00 0000 7212 0000 0072 3900 0000 da12  ....r....r9.....
+000035a0: 0072 4f00 0000 7211 0000 0072 9700 0000  .rO...r....r....
+000035b0: 7275 0000 0072 9800 0000 7280 0000 0072  ru...r....r....r
+000035c0: 9900 0000 7212 0000 0072 3900 0000 da12  ....r....r9.....
 000035d0: 7175 616c 6974 795f 636f 6e74 726f 6c6c  quality_controll
-000035e0: 6572 7274 0000 0072 2500 0000 7225 0000  errt...r%...r%..
+000035e0: 6572 7271 0000 0072 2500 0000 7225 0000  errq...r%...r%..
 000035f0: 0072 2600 0000 da1d 6c6f 6164 5f65 7374  .r&.....load_est
 00003600: 696d 6174 6564 5f63 6170 7475 7265 5f76  imated_capture_v
 00003610: 6f6c 756d 65e0 0100 0073 1600 0000 0c07  olume....s......
 00003620: 0c01 1001 1402 1401 0a01 0201 08ff 0205  ................
 00003630: 0801 0cff 7a25 5365 7373 696f 6e2e 6c6f  ....z%Session.lo
 00003640: 6164 5f65 7374 696d 6174 6564 5f63 6170  ad_estimated_cap
 00003650: 7475 7265 5f76 6f6c 756d 6563 0100 0000  ture_volumec....
@@ -901,67 +901,67 @@
 00003840: 2070 6f69 6e74 7320 6672 6f6d 2074 6865   points from the
 00003850: 206d 6f64 656c 4e29 1572 0f00 0000 7228   modelN).r....r(
 00003860: 0000 005a 0974 6f6d 6c5f 7061 7468 722e  ...Z.toml_pathr.
 00003870: 0000 005a 1473 7465 7265 6f5f 6361 6c69  ...Z.stereo_cali
 00003880: 6272 6174 655f 616c 6c72 0d00 0000 5a15  brate_allr....Z.
 00003890: 6765 745f 6265 7374 5f63 616d 6572 615f  get_best_camera_
 000038a0: 6172 7261 7972 4f00 0000 7214 0000 0072  arrayrO...r....r
-000038b0: 9f00 0000 7211 0000 0072 9c00 0000 da08  ....r....r......
+000038b0: 9a00 0000 7211 0000 0072 9700 0000 da08  ....r....r......
 000038c0: 6f70 7469 6d69 7a65 7212 0000 0072 3900  optimizer....r9.
-000038d0: 0000 72a0 0000 0072 5600 0000 7257 0000  ..r....rV...rW..
+000038d0: 0000 729b 0000 0072 5500 0000 7256 0000  ..r....rU...rV..
 000038e0: 00da 1146 494c 5445 5245 445f 4652 4143  ...FILTERED_FRAC
 000038f0: 5449 4f4e 5a16 6669 6c74 6572 5f70 6f69  TIONZ.filter_poi
 00003900: 6e74 5f65 7374 696d 6174 6573 5a13 7361  nt_estimatesZ.sa
 00003910: 7665 5f63 6170 7475 7265 5f76 6f6c 756d  ve_capture_volum
 00003920: 6529 0272 3c00 0000 5a10 7374 6572 656f  e).r<...Z.stereo
 00003930: 6361 6c69 6272 6174 6f72 7225 0000 0072  calibratorr%...r
 00003940: 2500 0000 7226 0000 00da 1365 7374 696d  %...r&.....estim
 00003950: 6174 655f 6578 7472 696e 7369 6373 f601  ate_extrinsics..
 00003960: 0000 732a 0000 0002 060a 0104 ff0c 0302  ..s*............
 00003970: 0206 0102 ff04 0204 fe02 0408 0106 ff10  ................
 00003980: 040a 0110 0204 020e 0104 ff0c 030a 0112  ................
 00003990: 027a 1b53 6573 7369 6f6e 2e65 7374 696d  .z.Session.estim
-000039a0: 6174 655f 6578 7472 696e 7369 6373 7271  ate_extrinsicsrq
+000039a0: 6174 655f 6578 7472 696e 7369 6373 726e  ate_extrinsicsrn
 000039b0: 0000 0029 0146 2929 721b 0000 0072 1c00  ...).F))r....r..
-000039c0: 0000 721d 0000 0072 0300 0000 728d 0000  ..r....r....r...
-000039d0: 0072 4300 0000 7299 0000 0072 9800 0000  .rC...r....r....
+000039c0: 0000 721d 0000 0072 0300 0000 7288 0000  ..r....r....r...
+000039d0: 0072 4300 0000 7294 0000 0072 9300 0000  .rC...r....r....
 000039e0: 7219 0000 005a 136d 6f64 655f 6368 616e  r....Z.mode_chan
 000039f0: 6765 5f73 7563 6365 7373 7215 0000 0072  ge_successr....r
-00003a00: 2b00 0000 7249 0000 0072 4c00 0000 7252  +...rI...rL...rR
-00003a10: 0000 0072 5900 0000 725c 0000 0072 6400  ...rY...r\...rd.
-00003a20: 0000 726d 0000 00da 0369 6e74 726f 0000  ..rm.....intro..
-00003a30: 0072 7200 0000 7265 0000 00da 0462 6f6f  .rr...re.....boo
-00003a40: 6c72 6a00 0000 7269 0000 0072 7500 0000  lrj...ri...ru...
-00003a50: 7276 0000 0072 7e00 0000 7289 0000 0072  rv...r~...r....r
-00003a60: 6800 0000 728b 0000 0072 6b00 0000 7267  h...r....rk...rg
-00003a70: 0000 0072 0500 0000 7296 0000 0072 9700  ...r....r....r..
-00003a80: 0000 728a 0000 0072 a100 0000 72a5 0000  ..r....r....r...
+00003a00: 2b00 0000 7249 0000 0072 4c00 0000 7251  +...rI...rL...rQ
+00003a10: 0000 0072 5800 0000 725a 0000 0072 6100  ...rX...rZ...ra.
+00003a20: 0000 726a 0000 00da 0369 6e74 726c 0000  ..rj.....intrl..
+00003a30: 0072 6f00 0000 7262 0000 00da 0462 6f6f  .ro...rb.....boo
+00003a40: 6c72 6700 0000 7266 0000 0072 7200 0000  lrg...rf...rr...
+00003a50: 7273 0000 0072 7b00 0000 7284 0000 0072  rs...r{...r....r
+00003a60: 6500 0000 7286 0000 0072 6800 0000 7264  e...r....rh...rd
+00003a70: 0000 0072 0500 0000 7291 0000 0072 9200  ...r....r....r..
+00003a80: 0000 7285 0000 0072 9c00 0000 72a0 0000  ..r....r....r...
 00003a90: 00da 0d5f 5f63 6c61 7373 6365 6c6c 5f5f  ...__classcell__
 00003aa0: 7225 0000 0072 2500 0000 723d 0000 0072  r%...r%...r=...r
 00003ab0: 2600 0000 7227 0000 0030 0000 0073 4a00  &...r'...0...sJ.
 00003ac0: 0000 0800 0601 0601 0601 0601 0802 1202  ................
 00003ad0: 0822 0812 0807 080b 081d 081e 0e10 0e38  .".............8
 00003ae0: 0e16 080f 0e06 0804 0806 0804 0804 0807  ................
 00003af0: 0823 0826 100b 080d 020a 04ff 0201 02ff  .#.&............
 00003b00: 0201 0aff 080c 080f 0816 1016 7227 0000  ............r'..
 00003b10: 0029 33da 0d70 7978 7933 642e 6c6f 6767  .)3..pyxy3d.logg
-00003b20: 6572 da06 7079 7879 3364 7256 0000 00da  er..pyxy3drV....
+00003b20: 6572 da06 7079 7879 3364 7255 0000 00da  er..pyxy3drU....
 00003b30: 0367 6574 721b 0000 00da 0c50 7951 7436  .getr......PyQt6
 00003b40: 2e51 7443 6f72 6572 0200 0000 7203 0000  .QtCorer....r...
 00003b50: 005a 1263 6f6e 6375 7272 656e 742e 6675  .Z.concurrent.fu
 00003b60: 7475 7265 7372 0400 0000 da07 7061 7468  turesr......path
 00003b70: 6c69 6272 0500 0000 da04 7469 6d65 7206  libr......timer.
 00003b80: 0000 00da 0465 6e75 6d72 0700 0000 7208  .....enumr....r.
-00003b90: 0000 005a 1f70 7978 7933 642e 7472 6163  ...Z.pyxy3d.trac
+00003b90: 0000 00da 1f70 7978 7933 642e 7472 6163  .....pyxy3d.trac
 00003ba0: 6b65 7273 2e63 6861 7275 636f 5f74 7261  kers.charuco_tra
 00003bb0: 636b 6572 7209 0000 005a 2170 7978 7933  ckerr....Z!pyxy3
 00003bc0: 642e 6361 6c69 6272 6174 696f 6e2e 6d6f  d.calibration.mo
 00003bd0: 6e6f 6361 6c69 6272 6174 6f72 720a 0000  nocalibratorr...
 00003be0: 005a 1570 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
-00003bf0: 732e 6361 6d65 7261 720b 0000 00da 1b70  s.camerar......p
+00003bf0: 732e 6361 6d65 7261 720b 0000 005a 1b70  s.camerar....Z.p
 00003c00: 7978 7933 642e 6361 6d65 7261 732e 7379  yxy3d.cameras.sy
 00003c10: 6e63 6872 6f6e 697a 6572 720c 0000 005a  nchronizerr....Z
 00003c20: 2770 7978 7933 642e 6361 6d65 7261 732e  'pyxy3d.cameras.
 00003c30: 6361 6d65 7261 5f61 7272 6179 5f69 6e69  camera_array_ini
 00003c40: 7469 616c 697a 6572 720d 0000 005a 1070  tializerr....Z.p
 00003c50: 7978 7933 642e 696e 7465 7266 6163 6572  yxy3d.interfacer
 00003c60: 0e00 0000 5a23 7079 7879 3364 2e63 616c  ....Z#pyxy3d.cal
@@ -984,17 +984,17 @@
 00003d70: 6170 7475 7265 5f76 6f6c 756d 652e 6865  apture_volume.he
 00003d80: 6c70 6572 5f66 756e 6374 696f 6e73 2e67  lper_functions.g
 00003d90: 6574 5f70 6f69 6e74 5f65 7374 696d 6174  et_point_estimat
 00003da0: 6573 7214 0000 00da 1370 7978 7933 642e  esr......pyxy3d.
 00003db0: 636f 6e66 6967 7572 6174 6f72 7215 0000  configuratorr...
 00003dc0: 005a 1a70 7978 7933 642e 6361 6d65 7261  .Z.pyxy3d.camera
 00003dd0: 732e 6c69 7665 5f73 7472 6561 6d72 1600  s.live_streamr..
-00003de0: 0000 da1f 7079 7879 3364 2e72 6563 6f72  ....pyxy3d.recor
+00003de0: 0000 5a1f 7079 7879 3364 2e72 6563 6f72  ..Z.pyxy3d.recor
 00003df0: 6469 6e67 2e76 6964 656f 5f72 6563 6f72  ding.video_recor
-00003e00: 6465 7272 1700 0000 7284 0000 0072 a400  derr....r....r..
+00003e00: 6465 7272 1700 0000 727f 0000 0072 9f00  derr....r....r..
 00003e10: 0000 7219 0000 0072 2700 0000 7225 0000  ..r....r'...r%..
 00003e20: 0072 2500 0000 7225 0000 0072 2600 0000  .r%...r%...r&...
 00003e30: da08 3c6d 6f64 756c 653e 0100 0000 7334  ..<module>....s4
 00003e40: 0000 0008 010c 0210 020c 010c 010c 0110  ................
 00003e50: 010c 020c 010c 010c 010c 010c 010c 020c  ................
 00003e60: 010c 010c 010c 020c 010c 030c 010c 0104  ................
 00003e70: 0304 0110 0314 0b                        .......
```

### Comparing `pyxy3d-0.0.19/pyxy3d/session/session.py` & `pyxy3d-0.0.20/pyxy3d/session/session.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/charuco_tracker.py` & `pyxy3d-0.0.20/pyxy3d/trackers/charuco_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/hand_tracker.py` & `pyxy3d-0.0.20/pyxy3d/trackers/hand_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/helper.py` & `pyxy3d-0.0.20/pyxy3d/trackers/helper.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/holistic_opensim_tracker.py` & `pyxy3d-0.0.20/pyxy3d/trackers/holistic_opensim_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/holistic_tracker.py` & `pyxy3d-0.0.20/pyxy3d/trackers/holistic_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/pose_tracker.py` & `pyxy3d-0.0.20/pyxy3d/trackers/pose_tracker.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/trackers/tracker_enum.py` & `pyxy3d-0.0.20/pyxy3d/trackers/tracker_enum.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc` & `pyxy3d-0.0.20/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.0.20/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.0.20/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/pyxy3d/triangulate/sync_packet_triangulator.py` & `pyxy3d-0.0.20/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.19/README.md` & `pyxy3d-0.0.20/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,119 +2,134 @@
 
 <div align="center"><img src = "pyxy3d/gui/icons/pyxy_logo.svg" width = "150"></div>
 
 ## Description
 
 Pyxy3D is an open-source python tool for converting two-dimensional (x,y) coordinates obtained from multiple standard webcams into 3D point estimates. It provides an integrated system for camera calibration and point triangulation that enables the creation of cost-efficient small scale motion capture systems. When combined with markerless tracking algorithms such as Google's Mediapipe, it is possible to perform markerless 3D tracking with a standard computer and a couple webcams. 
 
+## Video Walkthrough
+
+### Installation
+
+
+
+### A complete session
+
+
+
+
 ## Key Features
 
 The project leans heavily upon OpenCV, SciPy, and PyQt to provide the following **key features**:
 
-- User-friendly GUI
-- Easy design and creation of charuco calibration board
+- User-friendly graphical user interface (GUI)
+- Easy creation and modification of the charuco calibration board
 - Both extrinsic and intrinsic camera parameters are estimated
-- optional double-sided charuco board for better positional estimates of cameras placed opposite each other
-- Visual feedback during the calibration process including corner tracking, distortion modelling, and camera position estimates
+- Optional double-sided charuco board for better positional estimates of cameras placed opposite each other
+- Visual feedback during the calibration process 
 - World origin setting using the calibration board 
 - Fast convergence during bundle adjustment due to parameter initializations based on daisy-chained stereopairs of cameras
 - Recording of synchronized frames from connected webcams for post-processing
 - Tracker API for future extensibility with included sample implementation using Mediapipe 
 - Triangulation of tracked landmarks
 - Visualization of triangulated points for quick confirmation of output quality
-- currently exporting to `.csv` and `.trc` file formats
+- Currently exporting to `.csv` and `.trc` file formats
 
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
 - MediaPipe is only configured to run on Windows
     - while the camera calibration will likely work on other systems, the markerless tracking will not (currently)
 - It does not support anything other than standard webcams. 
     - I currently have no intention of supporting mobile phones as cameras for the system
 - Based on recent testing, some webcams will deliver poor connection times/frame rates/calibrations. I'm currently using 4 EMEET SmartCam C960 cameras. These are inexpensive (~$25 each) and readily available. They deliver decent results at 30 fps and 720p. I welcome feedback about user experiences with other cameras
 - No real-time tracking
     - the underlying data processing pipeline was designed to accommodate real-time tracking but I want to make sure that everything works well with the simpler and more stable post-processing workflow before trying to get that implemented in an integrated way
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
+## Known Issues
 
+The main GUI allows for accessing of all of the package's functionality at once, though this imposes some additional processing overhead that can undermine recording, and switching between GUI modes can provoke crashes. Improvements are on the To Do list, but in the meantime can be sidestepped by launching individual widgets from the command line as [described below](#3-launch-from-the-command-line)
 
 ## Installation
 
 Pyxy3D is installable via pip and the GUI can be launched from the command line. It is **strongly** advised that you do so within a virtual environment. The package requires [Python 3.10](https://www.python.org/downloads/release/python-3100/)  or higher. Because the Mediapipe implementation only works on Windows currently, these steps assume you are installing on Windows 10.
 
 ### 1. Create a virtual environment
 
 Find the path to your python.exe file. You can install Python 3.10 from [here](https://www.python.org/downloads/release/python-3100/). For me the path is `C:\Python310\python.exe`
 
-Create a folder where you would like the code and virtual environment to live. This can be different from the folder where your motion capture calibration and recording data is stored. Open the folder and right click within it, select  ![[Pasted image 20230608102647.png]] from the context menu to launch a terminal. 
+Create a folder where you would like the code and virtual environment to live. This can be different from the folder where your motion capture calibration and recording data is stored. Open the folder and right click within it, select  ![Pasted image 20230608102647](https://github.com/mprib/pyxy3d/assets/31831778/5c0ad5a7-fa57-473b-a549-243d93628dd3)
+ from the context menu to launch a terminal. 
    
 Run the following at the command prompt. Substitute in the path to `python.exe` that is true for your machine
 ```
 C:\Python310\python.exe -m venv .venv
 ```
 
 This will create a fresh version of python within that folder which you will use to manage your project. Activate the environment using the following command (if this exact command doesn't work, then [some other variation will](https://docs.python.org/3/library/venv.html#how-venvs-work))
 ```
 .\.venv\Scripts\activate
 ```
 
 The terminal should now show the environment is activated with something like this green parenthetical:
-![[Pasted image 20230608095719.png]]
+![Pasted image 20230608095719](https://github.com/mprib/pyxy3d/assets/31831778/10a91524-9a81-41d1-b27b-0b6ba723cb27)
 
 You can confirm that your python path is set by running
 
 ```
 python -c "import sys; print(sys.executable)"
 ```
 which should point to the file in the virtual environment you created:
-![[Pasted image 20230608100059.png]]
+![Pasted image 20230608100059](https://github.com/mprib/pyxy3d/assets/31831778/e214ebae-692c-4b50-b6f4-f34dcb44df43)
 
 ### 2. Install pyxy3D via pip
 
-For extra caution, upgrade pip with the following command:
-```
-pip install --upgrade pip
-```
-
 You are now ready to install pyxy3D from the Python Package Index (PyPI) via pip:
 
 ```
 pip install pyxy3d
 ```
 
 Installation may take a moment...
 
 ### 3. Launch from the command line
-
-With the package installed and the virtual environment activated, run the following command to launch the tool:
+With the package installed and the virtual environment activated, the main GUI can be launched by running the following command to launch the tool:
 
 ```
 pyxy3d
 ```
 
-A window should pop up and you can proceed with the capture session
+A video walkthrough of a sample session is [here]()
+
+If you experience crashes after initializing the session folder, then you can launch the individual interface components one at a time as needed. **NAVIGATE TO THE FOLDER OF THE SESSION YOU WANT TO LAUNCH** and run one of the following as needed: `charuco`, `cameras`, `calibrate`, `record`, `process`
+
+For example, if you are getting crashes when trying to record, within the terminal navigate to the session folder you previously created and run:
+
+```
+pyxy3d record
+```
 
-### Example session
+A recording widget will open up that should be more efficient and stable than the complete GUI.
 
-For a detailed walkthrough, refer to the project's comprehensive [documentation](link_to_documentation).
 
 ## Reporting Issues and Requesting Features
 
-To report a bug or request a feature, please open an issue.
+To report a bug or request a feature, please [open an issue](https://github.com/mprib/pyxy3d/issues). Please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
 
 ## General Questions and Conversation
 
-Post any questions in the Discussions section of the repo. As you post your questions, please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
+Post any questions in the [Discussions](https://github.com/mprib/pyxy3d/discussions) section of the repo. 
 
 ## Acknowledgments
 
-This project was inspired by [FreeMoCap](https://github.com/freemocap/freemocap) (FMC), which is spearheaded by [Jon Matthis, PhD](https://jonmatthis.com/) of the HuMoN Research Lab. The FMC calibration and triangulation system is built upon [Anipose](https://github.com/lambdaloop/anipose), created by Lili Karushchek, PhD. Several lines of FMC/Anipose code are used in the triangulation methods of Pyxy3D. I'm grateful to Dr. Matthis' for his time developing FreeMoCap, discussing it with me, pointing out important code considerations, and providing a great deal of information regarding open-source project management.
+This project was inspired by [FreeMoCap](https://github.com/freemocap/freemocap) (FMC), which is spearheaded by [Jon Matthis, PhD](https://jonmatthis.com/) of the HuMoN Research Lab. The FMC calibration and triangulation system is built upon [Anipose](https://github.com/lambdaloop/anipose), created by Lili Karushchek, PhD. Several lines of FMC/Anipose code are used in the triangulation methods of Pyxy3D. Pyxy3D is my attempt at helping to move toward an open source tool for motion capture that can hopefully one day benefit scientists, clinicians, and artists alike. I'm grateful to Dr. Matthis for his time developing FreeMoCap, discussing it with me, pointing out important code considerations, and providing a great deal of information regarding open-source project management.
 
-I began my python programming journey in August 2022. Hoping to understand the Anipose code, I started learning the basics of OpenCV. [Murtaza Hassan's](https://www.youtube.com/watch?v=01sAkU_NvOY) computer vision course rapidly got me up to speed on performing basic frame reading and parsing of Mediapipe data. To get a grounding in the fundamentals of camera calibration and triangulation I followed the excellent blog posts of [Temuge Batpurev](https://temugeb.github.io/). At the conclusion of those tutorials I decided to try to "roll my own" calibration and triangulation system as a learning exercise (which slowly turned into this repository). Videos from [GetIntoGameDev](https://www.youtube.com/watch?v=nCWApy9gCQQ) helped me through some dark and confusing times when this Physical Therapist tried to wrap his head around projection transforms. The excellent YouTube lectures of [Cyrill Stachniss](https://www.youtube.com/watch?v=sobyKHwgB0Y) provided a foundation for understanding the bundle adjustment process, and the [SciPy Cookbook](https://scipy-cookbook.readthedocs.io/items/bundle_adjustment.html) held my hand when implementing the code for this optimization. Debugging the daisy-chain approach to parameter initialization would not have been possible without the highly usable 3D visualization features of [PyQtGraph](https://www.pyqtgraph.org/).
+I began my python programming journey in August 2022. Hoping to understand the Anipose code, I started learning the basics of OpenCV. [Murtaza Hassan's](https://www.youtube.com/watch?v=01sAkU_NvOY) computer vision course rapidly got me up to speed on performing basic frame reading and parsing of Mediapipe data. To get a grounding in the fundamentals of camera calibration and triangulation I followed the excellent blog posts of [Temuge Batpurev](https://temugeb.github.io/). At the conclusion of those tutorials I decided to try to "roll my own" calibration and triangulation system as a learning exercise (which slowly turned into this repository). Videos from [GetIntoGameDev](https://www.youtube.com/watch?v=nCWApy9gCQQ) helped me through projection transforms. The excellent YouTube lectures of [Cyrill Stachniss](https://www.youtube.com/watch?v=sobyKHwgB0Y) provided a foundation for understanding the bundle adjustment process, and the [SciPy Cookbook](https://scipy-cookbook.readthedocs.io/items/bundle_adjustment.html) held my hand when implementing the code for this optimization. Debugging the daisy-chain approach to parameter initialization would not have been possible without the highly usable 3D visualization features of [PyQtGraph](https://www.pyqtgraph.org/).
 
-[ArjanCodes](https://www.youtube.com/@ArjanCodes) has been a frequent touchstone in my coding journey and is an incredible source of Python knowledge, as is [Corey Schafer](https://www.youtube.com/channel/UCCezIgC97PvUuR4_gbFUs5g) whose videos on multithreading were invaluable at tackling early technical hurdles related to concurrent frame reading. 
+[ArjanCodes](https://www.youtube.com/@ArjanCodes) has been an excellent resource for Python knowledge, as has [Corey Schafer](https://www.youtube.com/channel/UCCezIgC97PvUuR4_gbFUs5g) whose videos on multithreading were invaluable at tackling early technical hurdles related to concurrent frame reading. 
 
 While Pyxy3D is not a fork of any pre-existing project, it would not exist without the considerable previous work of many people, and I'm grateful to them all.
 
 ## License
 
 Pyxy3D is licensed under AGPL-3.0.
```

### Comparing `pyxy3d-0.0.19/PKG-INFO` & `pyxy3d-0.0.20/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxy3d
-Version: 0.0.19
+Version: 0.0.20
 Summary: A package for calibrating standard webcams to enable 3d motion tracking
 License: AGPL-3.0-only
 Author: Mac Prible
 Author-email: prible@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -26,120 +26,135 @@
 
 <div align="center"><img src = "pyxy3d/gui/icons/pyxy_logo.svg" width = "150"></div>
 
 ## Description
 
 Pyxy3D is an open-source python tool for converting two-dimensional (x,y) coordinates obtained from multiple standard webcams into 3D point estimates. It provides an integrated system for camera calibration and point triangulation that enables the creation of cost-efficient small scale motion capture systems. When combined with markerless tracking algorithms such as Google's Mediapipe, it is possible to perform markerless 3D tracking with a standard computer and a couple webcams. 
 
+## Video Walkthrough
+
+### Installation
+
+
+
+### A complete session
+
+
+
+
 ## Key Features
 
 The project leans heavily upon OpenCV, SciPy, and PyQt to provide the following **key features**:
 
-- User-friendly GUI
-- Easy design and creation of charuco calibration board
+- User-friendly graphical user interface (GUI)
+- Easy creation and modification of the charuco calibration board
 - Both extrinsic and intrinsic camera parameters are estimated
-- optional double-sided charuco board for better positional estimates of cameras placed opposite each other
-- Visual feedback during the calibration process including corner tracking, distortion modelling, and camera position estimates
+- Optional double-sided charuco board for better positional estimates of cameras placed opposite each other
+- Visual feedback during the calibration process 
 - World origin setting using the calibration board 
 - Fast convergence during bundle adjustment due to parameter initializations based on daisy-chained stereopairs of cameras
 - Recording of synchronized frames from connected webcams for post-processing
 - Tracker API for future extensibility with included sample implementation using Mediapipe 
 - Triangulation of tracked landmarks
 - Visualization of triangulated points for quick confirmation of output quality
-- currently exporting to `.csv` and `.trc` file formats
+- Currently exporting to `.csv` and `.trc` file formats
 
 ## Limitations
 
 Please note that the system currently has the following **limitations**:
 - MediaPipe is only configured to run on Windows
     - while the camera calibration will likely work on other systems, the markerless tracking will not (currently)
 - It does not support anything other than standard webcams. 
     - I currently have no intention of supporting mobile phones as cameras for the system
 - Based on recent testing, some webcams will deliver poor connection times/frame rates/calibrations. I'm currently using 4 EMEET SmartCam C960 cameras. These are inexpensive (~$25 each) and readily available. They deliver decent results at 30 fps and 720p. I welcome feedback about user experiences with other cameras
 - No real-time tracking
     - the underlying data processing pipeline was designed to accommodate real-time tracking but I want to make sure that everything works well with the simpler and more stable post-processing workflow before trying to get that implemented in an integrated way
 - Data export is currently limited to .csv, and .trc files. Use in 3D animation tools like Blender, which require character rigging, will require additional processing.
 
+## Known Issues
 
+The main GUI allows for accessing of all of the package's functionality at once, though this imposes some additional processing overhead that can undermine recording, and switching between GUI modes can provoke crashes. Improvements are on the To Do list, but in the meantime can be sidestepped by launching individual widgets from the command line as [described below](#3-launch-from-the-command-line)
 
 ## Installation
 
 Pyxy3D is installable via pip and the GUI can be launched from the command line. It is **strongly** advised that you do so within a virtual environment. The package requires [Python 3.10](https://www.python.org/downloads/release/python-3100/)  or higher. Because the Mediapipe implementation only works on Windows currently, these steps assume you are installing on Windows 10.
 
 ### 1. Create a virtual environment
 
 Find the path to your python.exe file. You can install Python 3.10 from [here](https://www.python.org/downloads/release/python-3100/). For me the path is `C:\Python310\python.exe`
 
-Create a folder where you would like the code and virtual environment to live. This can be different from the folder where your motion capture calibration and recording data is stored. Open the folder and right click within it, select  ![[Pasted image 20230608102647.png]] from the context menu to launch a terminal. 
+Create a folder where you would like the code and virtual environment to live. This can be different from the folder where your motion capture calibration and recording data is stored. Open the folder and right click within it, select  ![Pasted image 20230608102647](https://github.com/mprib/pyxy3d/assets/31831778/5c0ad5a7-fa57-473b-a549-243d93628dd3)
+ from the context menu to launch a terminal. 
    
 Run the following at the command prompt. Substitute in the path to `python.exe` that is true for your machine
 ```
 C:\Python310\python.exe -m venv .venv
 ```
 
 This will create a fresh version of python within that folder which you will use to manage your project. Activate the environment using the following command (if this exact command doesn't work, then [some other variation will](https://docs.python.org/3/library/venv.html#how-venvs-work))
 ```
 .\.venv\Scripts\activate
 ```
 
 The terminal should now show the environment is activated with something like this green parenthetical:
-![[Pasted image 20230608095719.png]]
+![Pasted image 20230608095719](https://github.com/mprib/pyxy3d/assets/31831778/10a91524-9a81-41d1-b27b-0b6ba723cb27)
 
 You can confirm that your python path is set by running
 
 ```
 python -c "import sys; print(sys.executable)"
 ```
 which should point to the file in the virtual environment you created:
-![[Pasted image 20230608100059.png]]
+![Pasted image 20230608100059](https://github.com/mprib/pyxy3d/assets/31831778/e214ebae-692c-4b50-b6f4-f34dcb44df43)
 
 ### 2. Install pyxy3D via pip
 
-For extra caution, upgrade pip with the following command:
-```
-pip install --upgrade pip
-```
-
 You are now ready to install pyxy3D from the Python Package Index (PyPI) via pip:
 
 ```
 pip install pyxy3d
 ```
 
 Installation may take a moment...
 
 ### 3. Launch from the command line
-
-With the package installed and the virtual environment activated, run the following command to launch the tool:
+With the package installed and the virtual environment activated, the main GUI can be launched by running the following command to launch the tool:
 
 ```
 pyxy3d
 ```
 
-A window should pop up and you can proceed with the capture session
+A video walkthrough of a sample session is [here]()
+
+If you experience crashes after initializing the session folder, then you can launch the individual interface components one at a time as needed. **NAVIGATE TO THE FOLDER OF THE SESSION YOU WANT TO LAUNCH** and run one of the following as needed: `charuco`, `cameras`, `calibrate`, `record`, `process`
+
+For example, if you are getting crashes when trying to record, within the terminal navigate to the session folder you previously created and run:
+
+```
+pyxy3d record
+```
 
-### Example session
+A recording widget will open up that should be more efficient and stable than the complete GUI.
 
-For a detailed walkthrough, refer to the project's comprehensive [documentation](link_to_documentation).
 
 ## Reporting Issues and Requesting Features
 
-To report a bug or request a feature, please open an issue.
+To report a bug or request a feature, please [open an issue](https://github.com/mprib/pyxy3d/issues). Please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
 
 ## General Questions and Conversation
 
-Post any questions in the Discussions section of the repo. As you post your questions, please keep in mind that this is an open-source project supported by volunteer effort, so your patience is appreciated.
+Post any questions in the [Discussions](https://github.com/mprib/pyxy3d/discussions) section of the repo. 
 
 ## Acknowledgments
 
-This project was inspired by [FreeMoCap](https://github.com/freemocap/freemocap) (FMC), which is spearheaded by [Jon Matthis, PhD](https://jonmatthis.com/) of the HuMoN Research Lab. The FMC calibration and triangulation system is built upon [Anipose](https://github.com/lambdaloop/anipose), created by Lili Karushchek, PhD. Several lines of FMC/Anipose code are used in the triangulation methods of Pyxy3D. I'm grateful to Dr. Matthis' for his time developing FreeMoCap, discussing it with me, pointing out important code considerations, and providing a great deal of information regarding open-source project management.
+This project was inspired by [FreeMoCap](https://github.com/freemocap/freemocap) (FMC), which is spearheaded by [Jon Matthis, PhD](https://jonmatthis.com/) of the HuMoN Research Lab. The FMC calibration and triangulation system is built upon [Anipose](https://github.com/lambdaloop/anipose), created by Lili Karushchek, PhD. Several lines of FMC/Anipose code are used in the triangulation methods of Pyxy3D. Pyxy3D is my attempt at helping to move toward an open source tool for motion capture that can hopefully one day benefit scientists, clinicians, and artists alike. I'm grateful to Dr. Matthis for his time developing FreeMoCap, discussing it with me, pointing out important code considerations, and providing a great deal of information regarding open-source project management.
 
-I began my python programming journey in August 2022. Hoping to understand the Anipose code, I started learning the basics of OpenCV. [Murtaza Hassan's](https://www.youtube.com/watch?v=01sAkU_NvOY) computer vision course rapidly got me up to speed on performing basic frame reading and parsing of Mediapipe data. To get a grounding in the fundamentals of camera calibration and triangulation I followed the excellent blog posts of [Temuge Batpurev](https://temugeb.github.io/). At the conclusion of those tutorials I decided to try to "roll my own" calibration and triangulation system as a learning exercise (which slowly turned into this repository). Videos from [GetIntoGameDev](https://www.youtube.com/watch?v=nCWApy9gCQQ) helped me through some dark and confusing times when this Physical Therapist tried to wrap his head around projection transforms. The excellent YouTube lectures of [Cyrill Stachniss](https://www.youtube.com/watch?v=sobyKHwgB0Y) provided a foundation for understanding the bundle adjustment process, and the [SciPy Cookbook](https://scipy-cookbook.readthedocs.io/items/bundle_adjustment.html) held my hand when implementing the code for this optimization. Debugging the daisy-chain approach to parameter initialization would not have been possible without the highly usable 3D visualization features of [PyQtGraph](https://www.pyqtgraph.org/).
+I began my python programming journey in August 2022. Hoping to understand the Anipose code, I started learning the basics of OpenCV. [Murtaza Hassan's](https://www.youtube.com/watch?v=01sAkU_NvOY) computer vision course rapidly got me up to speed on performing basic frame reading and parsing of Mediapipe data. To get a grounding in the fundamentals of camera calibration and triangulation I followed the excellent blog posts of [Temuge Batpurev](https://temugeb.github.io/). At the conclusion of those tutorials I decided to try to "roll my own" calibration and triangulation system as a learning exercise (which slowly turned into this repository). Videos from [GetIntoGameDev](https://www.youtube.com/watch?v=nCWApy9gCQQ) helped me through projection transforms. The excellent YouTube lectures of [Cyrill Stachniss](https://www.youtube.com/watch?v=sobyKHwgB0Y) provided a foundation for understanding the bundle adjustment process, and the [SciPy Cookbook](https://scipy-cookbook.readthedocs.io/items/bundle_adjustment.html) held my hand when implementing the code for this optimization. Debugging the daisy-chain approach to parameter initialization would not have been possible without the highly usable 3D visualization features of [PyQtGraph](https://www.pyqtgraph.org/).
 
-[ArjanCodes](https://www.youtube.com/@ArjanCodes) has been a frequent touchstone in my coding journey and is an incredible source of Python knowledge, as is [Corey Schafer](https://www.youtube.com/channel/UCCezIgC97PvUuR4_gbFUs5g) whose videos on multithreading were invaluable at tackling early technical hurdles related to concurrent frame reading. 
+[ArjanCodes](https://www.youtube.com/@ArjanCodes) has been an excellent resource for Python knowledge, as has [Corey Schafer](https://www.youtube.com/channel/UCCezIgC97PvUuR4_gbFUs5g) whose videos on multithreading were invaluable at tackling early technical hurdles related to concurrent frame reading. 
 
 While Pyxy3D is not a fork of any pre-existing project, it would not exist without the considerable previous work of many people, and I'm grateful to them all.
 
 ## License
 
 Pyxy3D is licensed under AGPL-3.0.
```

