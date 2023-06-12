# Comparing `tmp/pyxy3d-0.0.18.tar.gz` & `tmp/pyxy3d-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxy3d-0.0.18.tar", max compression
+gzip compressed data, was "pyxy3d-0.0.19.tar", max compression
```

## Comparing `pyxy3d-0.0.18.tar` & `pyxy3d-0.0.19.tar`

### file list

```diff
@@ -1,108 +1,233 @@
--rw-r--r--   0        0        0    35184 2023-03-13 23:46:36.918754 pyxy3d-0.0.18/LICENSE.md
--rw-r--r--   0        0        0      646 2023-04-13 21:25:14.507585 pyxy3d-0.0.18/pyproject.toml
--rw-r--r--   0        0        0     1296 2023-04-09 20:25:53.804486 pyxy3d-0.0.18/pyxy3d/__init__.py
--rw-r--r--   0        0        0       85 2023-03-16 18:13:11.443057 pyxy3d-0.0.18/pyxy3d/__main__.py
--rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
--rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
--rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
--rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
--rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
--rw-r--r--   0        0        0    11421 2023-04-10 23:04:25.621637 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/capture_volume.py
--rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
--rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
--rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
--rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
--rw-r--r--   0        0        0     4691 2023-04-13 14:11:20.703490 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
--rw-r--r--   0        0        0     4216 2023-04-09 20:25:53.808487 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/point_estimates.py
--rw-r--r--   0        0        0    15880 2023-04-13 20:26:58.536423 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/quality_controller.py
--rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/seaborn_summaries.py
--rw-r--r--   0        0        0    10803 2023-04-06 11:06:01.814527 pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/set_origin_functions.py
--rw-r--r--   0        0        0     9511 2023-04-13 20:26:58.537423 pyxy3d-0.0.18/pyxy3d/calibration/charuco.py
--rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.0.18/pyxy3d/calibration/draw_charuco.py
--rw-r--r--   0        0        0     8893 2023-04-13 20:26:58.538423 pyxy3d-0.0.18/pyxy3d/calibration/monocalibrator.py
--rw-r--r--   0        0        0    12363 2023-04-13 14:18:38.789544 pyxy3d-0.0.18/pyxy3d/calibration/stereocalibrator.py
--rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
--rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
--rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
--rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
--rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
--rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
--rw-r--r--   0        0        0    11547 2023-04-12 14:36:41.404217 pyxy3d-0.0.18/pyxy3d/cameras/camera.py
--rw-r--r--   0        0        0     8380 2023-04-09 20:25:53.809488 pyxy3d-0.0.18/pyxy3d/cameras/camera_array.py
--rw-r--r--   0        0        0    12850 2023-04-06 11:06:01.817527 pyxy3d-0.0.18/pyxy3d/cameras/camera_array_initializer.py
--rw-r--r--   0        0        0     3104 2023-04-13 20:26:58.539421 pyxy3d-0.0.18/pyxy3d/cameras/data_packets.py
--rw-r--r--   0        0        0    11568 2023-04-13 20:26:58.541422 pyxy3d-0.0.18/pyxy3d/cameras/live_stream.py
--rw-r--r--   0        0        0    14587 2023-04-13 20:26:58.542423 pyxy3d-0.0.18/pyxy3d/cameras/synchronizer.py
--rw-r--r--   0        0        0     7195 2023-04-10 23:04:25.624639 pyxy3d-0.0.18/pyxy3d/configurator.py
--rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.0.18/pyxy3d/gui/__pycache__/main.cpython-38.pyc
--rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.0.18/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
--rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.0.18/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
--rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.0.18/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
--rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.0.18/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
--rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.0.18/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
--rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.0.18/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
--rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.0.18/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
--rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.0.18/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
--rw-r--r--   0        0        0    19394 2023-03-28 23:02:56.662465 pyxy3d-0.0.18/pyxy3d/gui/camera_config/camera_config_dialogue.py
--rw-r--r--   0        0        0     4403 2023-03-20 15:38:55.652454 pyxy3d-0.0.18/pyxy3d/gui/camera_config/camera_tabs.py
--rw-r--r--   0        0        0     3364 2023-03-16 18:13:11.462059 pyxy3d-0.0.18/pyxy3d/gui/camera_config/frame_emitter.py
--rw-r--r--   0        0        0      708 2023-03-16 18:13:11.463060 pyxy3d-0.0.18/pyxy3d/gui/icons/orb.svg
--rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.0.18/pyxy3d/gui/icons/pyxy_logo.svg
--rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.0.18/pyxy3d/gui/icons/rotate-camera-left.svg
--rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.0.18/pyxy3d/gui/icons/rotate-camera-right.svg
--rw-r--r--   0        0        0     4979 2023-03-16 18:13:11.465059 pyxy3d-0.0.18/pyxy3d/gui/icons/rotate_right.svg
--rw-r--r--   0        0        0    11494 2023-04-11 10:48:05.433736 pyxy3d-0.0.18/pyxy3d/gui/main.py
--rw-r--r--   0        0        0     2211 2023-04-03 14:25:42.363308 pyxy3d-0.0.18/pyxy3d/gui/qt_logger.py
--rw-r--r--   0        0        0    12116 2023-04-12 14:36:41.410217 pyxy3d-0.0.18/pyxy3d/gui/recording_widget.py
--rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.0.18/pyxy3d/gui/stereoframe/__pycache__/omni_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.0.18/pyxy3d/gui/stereoframe/__pycache__/omni_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.0.18/pyxy3d/gui/stereoframe/__pycache__/stereo_frame_builder.cpython-38.pyc
--rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.0.18/pyxy3d/gui/stereoframe/__pycache__/stereo_frame_widget.cpython-38.pyc
--rw-r--r--   0        0        0    16495 2023-04-13 20:26:58.543422 pyxy3d-0.0.18/pyxy3d/gui/stereoframe/stereo_frame_builder.py
--rw-r--r--   0        0        0     9157 2023-04-13 20:26:58.545422 pyxy3d-0.0.18/pyxy3d/gui/stereoframe/stereo_frame_widget.py
--rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.0.18/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
--rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.0.18/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
--rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.0.18/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.0.18/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.0.18/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
--rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.0.18/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
--rw-r--r--   0        0        0     5231 2023-04-09 20:25:53.815487 pyxy3d-0.0.18/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
--rw-r--r--   0        0        0     6249 2023-04-13 20:26:58.546422 pyxy3d-0.0.18/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
--rw-r--r--   0        0        0     9110 2023-04-09 20:25:53.817485 pyxy3d-0.0.18/pyxy3d/gui/vizualize/camera_mesh.py
--rw-r--r--   0        0        0     4649 2023-04-11 13:54:56.764987 pyxy3d-0.0.18/pyxy3d/gui/vizualize/triangulation_widget.py
--rw-r--r--   0        0        0     3263 2023-03-31 14:27:43.762616 pyxy3d-0.0.18/pyxy3d/gui/widgets.py
--rw-r--r--   0        0        0    11152 2023-03-16 18:13:11.472057 pyxy3d-0.0.18/pyxy3d/gui/wizard_charuco.py
--rw-r--r--   0        0        0     6830 2023-03-30 21:33:42.816929 pyxy3d-0.0.18/pyxy3d/gui/wizard_directory.py
--rw-r--r--   0        0        0        0 2023-04-13 20:26:58.547423 pyxy3d-0.0.18/pyxy3d/img2xy/__init__.py
--rw-r--r--   0        0        0      149 2023-04-13 17:33:55.961380 pyxy3d-0.0.18/pyxy3d/img2xy/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     3376 2023-04-13 17:54:11.599140 pyxy3d-0.0.18/pyxy3d/img2xy/__pycache__/charuco_tracker.cpython-38.pyc
--rw-r--r--   0        0        0      835 2023-04-13 17:33:55.977597 pyxy3d-0.0.18/pyxy3d/img2xy/__pycache__/tracker_abc.cpython-38.pyc
--rw-r--r--   0        0        0     4847 2023-04-13 20:26:58.548423 pyxy3d-0.0.18/pyxy3d/img2xy/charuco_tracker.py
--rw-r--r--   0        0        0     2369 2023-04-13 20:26:58.549422 pyxy3d-0.0.18/pyxy3d/img2xy/mphands.py
--rw-r--r--   0        0        0      356 2023-04-13 20:26:58.550423 pyxy3d-0.0.18/pyxy3d/img2xy/tracker_abc.py
--rw-r--r--   0        0        0     2752 2023-03-30 21:33:42.818928 pyxy3d-0.0.18/pyxy3d/logger.py
--rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.0.18/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
--rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.0.18/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
--rw-r--r--   0        0        0    10748 2023-04-13 20:26:58.551422 pyxy3d-0.0.18/pyxy3d/recording/recorded_stream.py
--rw-r--r--   0        0        0     7941 2023-04-13 14:11:20.706490 pyxy3d-0.0.18/pyxy3d/recording/video_recorder.py
--rw-r--r--   0        0        0    24318 2023-04-13 20:26:58.552422 pyxy3d-0.0.18/pyxy3d/session.py
--rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
--rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
--rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
--rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
--rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
--rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
--rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
--rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
--rw-r--r--   0        0        0     8787 2023-04-13 20:26:58.553422 pyxy3d-0.0.18/pyxy3d/triangulate/array_stereo_triangulator.py
--rw-r--r--   0        0        0     6547 2023-04-10 23:04:25.629637 pyxy3d-0.0.18/pyxy3d/triangulate/real_time_triangulator.py
--rw-r--r--   0        0        0     5771 2023-04-13 20:26:58.554421 pyxy3d-0.0.18/pyxy3d/triangulate/stereo_points_builder.py
--rw-r--r--   0        0        0     1574 2023-04-12 14:36:41.399217 pyxy3d-0.0.18/README.md
--rw-r--r--   0        0        0     2431 1970-01-01 00:00:00.000000 pyxy3d-0.0.18/PKG-INFO
+-rw-r--r--   0        0        0    35184 2023-03-13 23:46:36.918754 pyxy3d-0.0.19/LICENSE.md
+-rw-r--r--   0        0        0      925 2023-06-12 17:18:54.002781 pyxy3d-0.0.19/pyproject.toml
+-rw-r--r--   0        0        0     2007 2023-05-20 12:18:55.240529 pyxy3d-0.0.19/pyxy3d/__init__.py
+-rw-r--r--   0        0        0      934 2023-06-12 16:51:54.169618 pyxy3d-0.0.19/pyxy3d/__main__.py
+-rw-r--r--   0        0        0     7201 2023-04-16 14:08:55.358491 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     7111 2023-04-13 18:16:32.164621 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 14:11:35.706111 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc
+-rw-r--r--   0        0        0     1525 2023-04-13 21:33:14.966692 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/draw_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     1517 2023-03-16 18:37:10.539737 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     7208 2023-06-12 15:03:14.886290 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/monocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7083 2023-04-13 18:16:59.718066 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0    11365 2023-03-16 18:37:11.887671 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7979 2023-06-08 18:19:03.652989 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-310.pyc
+-rw-r--r--   0        0        0     7845 2023-04-13 14:31:07.431535 pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc
+-rw-r--r--   0        0        0     7001 2023-06-12 12:22:25.787593 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-310.pyc
+-rw-r--r--   0        0        0     8147 2023-04-11 10:38:21.551689 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc
+-rw-r--r--   0        0        0     3205 2023-05-02 22:08:30.018323 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     3651 2023-04-09 20:26:50.741740 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     9626 2023-05-22 14:59:39.828020 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-310.pyc
+-rw-r--r--   0        0        0     9567 2023-04-13 18:47:12.691013 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc
+-rw-r--r--   0        0        0     7294 2023-05-22 14:59:39.817019 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-310.pyc
+-rw-r--r--   0        0        0     7172 2023-04-06 11:06:35.216555 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc
+-rw-r--r--   0        0        0    10148 2023-06-12 12:14:10.017140 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/capture_volume.py
+-rw-r--r--   0        0        0  1505952 2023-03-13 23:46:36.934749 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl
+-rw-r--r--   0        0        0     2813 2023-04-13 21:41:08.181971 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-310.pyc
+-rw-r--r--   0        0        0     2825 2023-03-16 18:37:13.420982 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc
+-rw-r--r--   0        0        0     2938 2023-04-16 14:08:57.590539 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-310.pyc
+-rw-r--r--   0        0        0     2963 2023-04-13 14:11:34.686199 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc
+-rw-r--r--   0        0        0     3898 2023-03-16 18:13:11.445058 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py
+-rw-r--r--   0        0        0     4680 2023-04-16 12:58:12.386690 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py
+-rw-r--r--   0        0        0     3631 2023-05-02 22:08:10.575286 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/point_estimates.py
+-rw-r--r--   0        0        0    15888 2023-05-22 13:44:00.083689 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/quality_controller.py
+-rw-r--r--   0        0        0     1766 2023-03-16 18:13:11.448058 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/seaborn_summaries.py
+-rw-r--r--   0        0        0    10868 2023-05-22 13:44:00.084688 pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/set_origin_functions.py
+-rw-r--r--   0        0        0     9510 2023-04-16 12:58:12.392689 pyxy3d-0.0.19/pyxy3d/calibration/charuco.py
+-rw-r--r--   0        0        0     1685 2023-03-16 18:13:11.451057 pyxy3d-0.0.19/pyxy3d/calibration/draw_charuco.py
+-rw-r--r--   0        0        0     9886 2023-06-12 16:49:05.518131 pyxy3d-0.0.19/pyxy3d/calibration/monocalibrator.py
+-rw-r--r--   0        0        0    12385 2023-06-08 18:18:45.456813 pyxy3d-0.0.19/pyxy3d/calibration/stereocalibrator.py
+-rw-r--r--   0        0        0     7119 2023-05-22 16:42:44.186443 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera.cpython-310.pyc
+-rw-r--r--   0        0        0     7171 2023-04-12 14:56:03.753093 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc
+-rw-r--r--   0        0        0     6788 2023-06-10 20:39:00.834305 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array.cpython-310.pyc
+-rw-r--r--   0        0        0     6811 2023-04-09 20:26:50.029740 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc
+-rw-r--r--   0        0        0     9199 2023-05-02 22:08:30.006322 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-310.pyc
+-rw-r--r--   0        0        0     9153 2023-04-06 11:06:35.358553 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc
+-rw-r--r--   0        0        0     3161 2023-04-13 21:33:14.970692 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/data_packets.cpython-310.pyc
+-rw-r--r--   0        0        0     3147 2023-04-13 17:33:55.370369 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc
+-rw-r--r--   0        0        0     8085 2023-06-10 20:05:09.584549 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/live_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     8585 2023-04-13 17:33:56.274500 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc
+-rw-r--r--   0        0        0    11255 2023-06-10 20:05:09.592548 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/synchronizer.cpython-310.pyc
+-rw-r--r--   0        0        0    11042 2023-04-13 18:30:26.417813 pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc
+-rw-r--r--   0        0        0    10631 2023-05-22 16:41:37.293000 pyxy3d-0.0.19/pyxy3d/cameras/camera.py
+-rw-r--r--   0        0        0     7710 2023-06-10 20:38:54.275345 pyxy3d-0.0.19/pyxy3d/cameras/camera_array.py
+-rw-r--r--   0        0        0    12868 2023-05-02 22:08:10.579286 pyxy3d-0.0.19/pyxy3d/cameras/camera_array_initializer.py
+-rw-r--r--   0        0        0    11935 2023-06-10 20:04:58.799532 pyxy3d-0.0.19/pyxy3d/cameras/live_stream.py
+-rw-r--r--   0        0        0    15573 2023-06-10 20:04:49.722607 pyxy3d-0.0.19/pyxy3d/cameras/synchronizer.py
+-rw-r--r--   0        0        0    13040 2023-06-12 12:14:10.019141 pyxy3d-0.0.19/pyxy3d/configurator.py
+-rw-r--r--   0        0        0     7036 2023-05-18 21:56:09.817280 pyxy3d-0.0.19/pyxy3d/export.py
+-rw-r--r--   0        0        0     3538 2023-06-12 15:03:16.496290 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibrate_capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5645 2023-06-10 20:05:11.196557 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8693 2023-05-06 16:11:05.603259 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/calibration_wizard.cpython-310.pyc
+-rw-r--r--   0        0        0     7124 2023-06-08 18:19:04.615289 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/charuco_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8098 2023-06-12 15:03:15.902289 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2110 2023-05-29 12:41:08.382954 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/log_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8811 2023-05-02 22:10:09.955994 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0        0        0     8445 2023-04-12 14:19:14.529651 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main.cpython-38.pyc
+-rw-r--r--   0        0        0    10204 2023-06-12 15:03:16.485299 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2664 2023-06-08 18:19:04.619290 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/navigation_bars.cpython-310.pyc
+-rw-r--r--   0        0        0     2468 2023-06-02 00:29:24.448977 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/playback_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9611 2023-06-10 20:31:20.063896 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/post_processing_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     1176 2023-05-29 13:25:02.424999 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/progress_dialog.cpython-310.pyc
+-rw-r--r--   0        0        0     2649 2023-05-22 15:00:23.510630 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/qt_logger.cpython-310.pyc
+-rw-r--r--   0        0        0     2623 2023-04-06 18:40:19.597418 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc
+-rw-r--r--   0        0        0    11941 2023-06-12 16:32:28.139452 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/recording_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     8798 2023-04-12 14:17:47.475386 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     2641 2023-04-13 21:41:10.861210 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/widgets.cpython-310.pyc
+-rw-r--r--   0        0        0     2969 2023-04-06 18:40:19.600418 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc
+-rw-r--r--   0        0        0     6864 2023-05-29 12:41:07.242642 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_charuco.cpython-310.pyc
+-rw-r--r--   0        0        0     6979 2023-04-06 18:40:19.594417 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc
+-rw-r--r--   0        0        0     4851 2023-05-02 13:40:54.299559 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_directory.cpython-310.pyc
+-rw-r--r--   0        0        0     4903 2023-04-06 18:40:19.608417 pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc
+-rw-r--r--   0        0        0     4052 2023-06-12 16:49:05.519131 pyxy3d-0.0.19/pyxy3d/gui/calibrate_capture_volume_widget.py
+-rw-r--r--   0        0        0     7438 2023-06-12 17:07:44.747202 pyxy3d-0.0.19/pyxy3d/gui/calibration_widget.py
+-rw-r--r--   0        0        0    13085 2023-06-02 16:06:24.614359 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-310.pyc
+-rw-r--r--   0        0        0    13777 2023-03-29 13:33:28.389797 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc
+-rw-r--r--   0        0        0     3658 2023-06-10 20:05:11.213579 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_summary_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4748 2023-06-01 14:22:06.839277 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-310.pyc
+-rw-r--r--   0        0        0     3850 2023-03-20 23:10:53.097964 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc
+-rw-r--r--   0        0        0     3155 2023-06-02 14:30:41.590277 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-310.pyc
+-rw-r--r--   0        0        0     2704 2023-03-16 18:37:13.513000 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc
+-rw-r--r--   0        0        0     3619 2023-06-10 20:39:01.831691 pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/intrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0    17771 2023-06-02 15:39:41.317656 pyxy3d-0.0.19/pyxy3d/gui/camera_config/camera_config_dialogue.py
+-rw-r--r--   0        0        0     5794 2023-06-10 20:04:49.727607 pyxy3d-0.0.19/pyxy3d/gui/camera_config/camera_summary_widget.py
+-rw-r--r--   0        0        0     3893 2023-06-02 00:28:42.145417 pyxy3d-0.0.19/pyxy3d/gui/camera_config/frame_emitter.py
+-rw-r--r--   0        0        0     3760 2023-06-10 20:38:54.278346 pyxy3d-0.0.19/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py
+-rw-r--r--   0        0        0    11157 2023-06-08 18:18:45.460813 pyxy3d-0.0.19/pyxy3d/gui/charuco_widget.py
+-rw-r--r--   0        0        0    10279 2023-06-12 16:49:05.520130 pyxy3d-0.0.19/pyxy3d/gui/extrinsic_calibration_widget.py
+-rw-r--r--   0        0        0     7468 2023-06-01 18:24:14.049008 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/extrinsic_calibration_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     9143 2023-03-16 18:37:13.553998 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5691 2023-03-16 18:37:13.539983 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     9807 2023-06-02 14:30:41.606273 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/paired_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     9881 2023-06-01 18:24:14.063003 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-310.pyc
+-rw-r--r--   0        0        0    11456 2023-04-13 17:55:04.283828 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     7359 2023-06-01 14:22:06.856278 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     7148 2023-04-13 18:41:31.149308 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc
+-rw-r--r--   0        0        0    14193 2023-06-02 00:29:03.392704 pyxy3d-0.0.19/pyxy3d/gui/frame_builders/paired_frame_builder.py
+-rw-r--r--   0        0        0    19878 2023-04-07 19:40:35.259432 pyxy3d-0.0.19/pyxy3d/gui/icons/pyxy_logo.svg
+-rw-r--r--   0        0        0      941 2023-03-16 18:13:11.463060 pyxy3d-0.0.19/pyxy3d/gui/icons/rotate-camera-left.svg
+-rw-r--r--   0        0        0      944 2023-03-16 18:13:11.464059 pyxy3d-0.0.19/pyxy3d/gui/icons/rotate-camera-right.svg
+-rw-r--r--   0        0        0     2460 2023-05-28 21:21:33.674553 pyxy3d-0.0.19/pyxy3d/gui/log_widget.py
+-rw-r--r--   0        0        0    14273 2023-06-12 16:49:05.521130 pyxy3d-0.0.19/pyxy3d/gui/main_widget.py
+-rw-r--r--   0        0        0     3292 2023-06-08 18:18:45.464814 pyxy3d-0.0.19/pyxy3d/gui/navigation_bars.py
+-rw-r--r--   0        0        0     1988 2023-06-02 00:28:42.150417 pyxy3d-0.0.19/pyxy3d/gui/playback_widget.py
+-rw-r--r--   0        0        0    11310 2023-06-10 20:29:24.686837 pyxy3d-0.0.19/pyxy3d/gui/post_processing_widget.py
+-rw-r--r--   0        0        0      950 2023-05-28 21:21:33.677553 pyxy3d-0.0.19/pyxy3d/gui/progress_dialog.py
+-rw-r--r--   0        0        0    14618 2023-06-12 16:49:05.522130 pyxy3d-0.0.19/pyxy3d/gui/recording_widget.py
+-rw-r--r--   0        0        0     6275 2023-05-13 12:35:31.914917 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-310.pyc
+-rw-r--r--   0        0        0     6278 2023-04-10 15:11:26.319020 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc
+-rw-r--r--   0        0        0     3198 2023-03-27 01:11:02.734179 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc
+-rw-r--r--   0        0        0     5013 2023-04-08 17:08:48.219160 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5850 2023-04-08 17:08:47.292159 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     4920 2023-06-12 12:22:29.640003 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/playback_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     4522 2023-04-16 14:08:58.474682 pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/realtime_triangulation_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     2999 2023-06-08 18:19:05.638538 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-310.pyc
+-rw-r--r--   0        0        0     3506 2023-04-10 15:11:26.253010 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc
+-rw-r--r--   0        0        0     5838 2023-06-12 12:22:27.405313 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-310.pyc
+-rw-r--r--   0        0        0     5615 2023-04-13 18:47:41.885491 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc
+-rw-r--r--   0        0        0     3404 2023-06-08 18:18:45.466812 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py
+-rw-r--r--   0        0        0     6843 2023-06-12 12:14:10.025140 pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py
+-rw-r--r--   0        0        0     9146 2023-05-12 22:51:00.876793 pyxy3d-0.0.19/pyxy3d/gui/vizualize/camera_mesh.py
+-rw-r--r--   0        0        0     5054 2023-06-12 12:14:10.027140 pyxy3d-0.0.19/pyxy3d/gui/vizualize/playback_triangulation_widget.py
+-rw-r--r--   0        0        0     5450 2023-05-22 13:44:00.101687 pyxy3d-0.0.19/pyxy3d/gui/vizualize/realtime_triangulation_widget.py
+-rw-r--r--   0        0        0     1135 2023-05-18 17:09:55.119648 pyxy3d-0.0.19/pyxy3d/helper.py
+-rw-r--r--   0        0        0     6646 2023-06-01 14:21:56.755811 pyxy3d-0.0.19/pyxy3d/interface.py
+-rw-r--r--   0        0        0     3111 2023-06-01 14:21:56.756810 pyxy3d-0.0.19/pyxy3d/logger.py
+-rw-r--r--   0        0        0     7100 2023-06-12 12:14:10.028141 pyxy3d-0.0.19/pyxy3d/post_processor.py
+-rw-r--r--   0        0        0     8482 2023-05-29 13:25:01.175649 pyxy3d-0.0.19/pyxy3d/recording/__pycache__/recorded_stream.cpython-310.pyc
+-rw-r--r--   0        0        0     7603 2023-04-13 17:33:56.707496 pyxy3d-0.0.19/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc
+-rw-r--r--   0        0        0     5928 2023-06-12 12:22:27.383610 pyxy3d-0.0.19/pyxy3d/recording/__pycache__/video_recorder.cpython-310.pyc
+-rw-r--r--   0        0        0     5376 2023-04-13 14:11:36.908257 pyxy3d-0.0.19/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc
+-rw-r--r--   0        0        0    11830 2023-05-28 21:21:33.684552 pyxy3d-0.0.19/pyxy3d/recording/recorded_stream.py
+-rw-r--r--   0        0        0     8730 2023-06-12 12:14:10.029141 pyxy3d-0.0.19/pyxy3d/recording/video_recorder.py
+-rw-r--r--   0        0        0     2818 2023-06-05 20:04:19.162433 pyxy3d-0.0.19/pyxy3d/session/__pycache__/get_stage.cpython-310.pyc
+-rw-r--r--   0        0        0    15991 2023-06-12 15:10:34.851320 pyxy3d-0.0.19/pyxy3d/session/__pycache__/session.cpython-310.pyc
+-rw-r--r--   0        0        0    20797 2023-06-12 16:49:05.524130 pyxy3d-0.0.19/pyxy3d/session/session.py
+-rw-r--r--   0        0        0        0 2023-04-16 12:58:12.408688 pyxy3d-0.0.19/pyxy3d/trackers/__init__.py
+-rw-r--r--   0        0        0      153 2023-04-16 14:08:55.370508 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3955 2023-05-13 12:35:24.878771 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/charuco_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3531 2023-05-13 12:35:26.254677 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1123 2023-05-13 12:35:28.030304 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     6774 2023-05-18 18:02:52.161100 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/holistic_opensim_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     6262 2023-05-13 12:35:28.041314 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/holistic_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3797 2023-05-13 12:35:28.036311 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/pose_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     3515 2023-05-12 22:32:19.505484 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/threaded_hand_tracker.cpython-310.pyc
+-rw-r--r--   0        0        0     1017 2023-05-18 18:02:48.968666 pyxy3d-0.0.19/pyxy3d/trackers/__pycache__/tracker_enum.cpython-310.pyc
+-rw-r--r--   0        0        0     5004 2023-05-12 22:51:00.882792 pyxy3d-0.0.19/pyxy3d/trackers/charuco_tracker.py
+-rw-r--r--   0        0        0     4651 2023-05-12 22:51:00.883791 pyxy3d-0.0.19/pyxy3d/trackers/hand_tracker.py
+-rw-r--r--   0        0        0     1330 2023-05-12 22:51:00.884792 pyxy3d-0.0.19/pyxy3d/trackers/helper.py
+-rw-r--r--   0        0        0    10677 2023-05-18 17:09:55.120646 pyxy3d-0.0.19/pyxy3d/trackers/holistic_opensim_tracker.py
+-rw-r--r--   0        0        0     9419 2023-05-12 22:51:00.885792 pyxy3d-0.0.19/pyxy3d/trackers/holistic_tracker.py
+-rw-r--r--   0        0        0     4239 2023-05-12 22:51:00.885792 pyxy3d-0.0.19/pyxy3d/trackers/pose_tracker.py
+-rw-r--r--   0        0        0      669 2023-05-18 17:09:55.121648 pyxy3d-0.0.19/pyxy3d/trackers/tracker_enum.py
+-rw-r--r--   0        0        0     5629 2023-04-16 14:08:57.598538 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     5656 2023-04-13 17:33:55.945379 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0      564 2023-04-24 13:44:16.864821 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/helper.cpython-310.pyc
+-rw-r--r--   0        0        0     5809 2023-05-03 19:22:07.093614 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-04-11 11:20:24.830020 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0   277847 2023-04-17 18:50:37.938076 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.1.nbc
+-rw-r--r--   0        0        0   278178 2023-04-17 18:47:53.733008 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.2.nbc
+-rw-r--r--   0        0        0     1853 2023-04-17 18:50:37.934076 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-135.py310.nbi
+-rw-r--r--   0        0        0   278065 2023-04-15 22:26:29.919720 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.1.nbc
+-rw-r--r--   0        0        0     1795 2023-04-15 22:26:29.916718 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py310.nbi
+-rw-r--r--   0        0        0   277525 2023-04-13 14:11:54.518242 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc
+-rw-r--r--   0        0        0     1794 2023-04-13 14:11:54.515242 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 16:24:55.484079 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 16:24:55.480077 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-138.py310.nbi
+-rw-r--r--   0        0        0   277847 2023-04-15 21:02:04.894614 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.1.nbc
+-rw-r--r--   0        0        0     1853 2023-04-15 21:02:04.889631 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-139.py310.nbi
+-rw-r--r--   0        0        0   277790 2023-04-09 20:05:59.716347 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:05:59.712345 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi
+-rw-r--r--   0        0        0   277795 2023-04-09 20:08:37.404028 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc
+-rw-r--r--   0        0        0     1793 2023-04-09 20:08:37.400042 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi
+-rw-r--r--   0        0        0    80840 2023-04-17 18:50:25.192073 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.1.nbc
+-rw-r--r--   0        0        0     1278 2023-04-17 18:50:25.189073 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.unique_with_counts-118.py310.nbi
+-rw-r--r--   0        0        0     4903 2023-04-16 14:08:57.603539 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-310.pyc
+-rw-r--r--   0        0        0     4910 2023-04-13 17:33:55.950369 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc
+-rw-r--r--   0        0        0     5522 2023-06-08 19:16:30.042145 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.cpython-310.pyc
+-rw-r--r--   0        0        0   277993 2023-06-10 20:35:53.847895 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.1.nbc
+-rw-r--r--   0        0        0   278337 2023-06-10 20:36:00.364127 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.2.nbc
+-rw-r--r--   0        0        0   275198 2023-06-10 20:36:15.587107 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.3.nbc
+-rw-r--r--   0        0        0     3826 2023-06-10 20:36:15.585108 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-168.py310.nbi
+-rw-r--r--   0        0        0   274936 2023-05-07 17:31:11.859065 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.1.nbc
+-rw-r--r--   0        0        0     1819 2023-05-07 17:31:11.856057 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-170.py310.nbi
+-rw-r--r--   0        0        0   280483 2023-05-11 20:37:44.633248 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.1.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 20:37:44.630243 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-186.py310.nbi
+-rw-r--r--   0        0        0   277957 2023-05-11 19:51:33.032983 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.1.nbc
+-rw-r--r--   0        0        0   278013 2023-05-11 17:55:35.449169 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.2.nbc
+-rw-r--r--   0        0        0   278357 2023-05-11 17:56:15.957610 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.3.nbc
+-rw-r--r--   0        0        0     1855 2023-05-11 19:51:33.028983 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-188.py310.nbi
+-rw-r--r--   0        0        0   277977 2023-05-11 20:58:46.910959 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.1.nbc
+-rw-r--r--   0        0        0   274956 2023-05-11 22:29:46.557422 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.2.nbc
+-rw-r--r--   0        0        0   280725 2023-05-12 22:34:01.184507 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.3.nbc
+-rw-r--r--   0        0        0     3913 2023-05-12 22:34:01.181521 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-189.py310.nbi
+-rw-r--r--   0        0        0   274956 2023-05-13 12:36:45.045739 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.1.nbc
+-rw-r--r--   0        0        0   277993 2023-05-14 17:03:11.852980 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.2.nbc
+-rw-r--r--   0        0        0   278337 2023-05-14 17:03:18.755882 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.3.nbc
+-rw-r--r--   0        0        0     3855 2023-05-14 17:03:18.752878 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-194.py310.nbi
+-rw-r--r--   0        0        0   278215 2023-05-12 22:36:41.576195 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.1.nbc
+-rw-r--r--   0        0        0     1797 2023-05-12 22:36:41.573185 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.triangulate_sync_index-195.py310.nbi
+-rw-r--r--   0        0        0    80914 2023-06-10 20:35:46.176596 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-06-10 20:36:11.729164 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-06-10 20:36:11.727174 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-152.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-10 14:04:48.307277 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-09 20:10:40.338051 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-10 14:04:48.305276 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-153.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:37:03.860602 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 20:37:03.857602 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-170.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 19:51:22.690984 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-11 17:55:29.550170 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.2.nbc
+-rw-r--r--   0        0        0     1280 2023-05-11 19:51:22.687981 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-172.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-11 20:58:36.790966 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.1.nbc
+-rw-r--r--   0        0        0    77589 2023-05-11 22:29:37.429700 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.2.nbc
+-rw-r--r--   0        0        0     2321 2023-05-11 22:29:37.426700 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-173.py310.nbi
+-rw-r--r--   0        0        0    77589 2023-05-13 12:36:36.027208 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.1.nbc
+-rw-r--r--   0        0        0    80894 2023-05-14 17:03:04.107988 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.2.nbc
+-rw-r--r--   0        0        0     2292 2023-05-14 17:03:04.102988 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-178.py310.nbi
+-rw-r--r--   0        0        0    80894 2023-05-12 22:36:32.819436 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.1.nbc
+-rw-r--r--   0        0        0     1280 2023-05-12 22:36:32.816430 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/sync_packet_triangulator.unique_with_counts-179.py310.nbi
+-rw-r--r--   0        0        0     5598 2023-04-04 19:53:34.784759 pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc
+-rw-r--r--   0        0        0     8778 2023-04-16 12:58:12.413689 pyxy3d-0.0.19/pyxy3d/triangulate/array_stereo_triangulator.py
+-rw-r--r--   0        0        0     5762 2023-04-16 12:58:12.416688 pyxy3d-0.0.19/pyxy3d/triangulate/stereo_points_builder.py
+-rw-r--r--   0        0        0     7616 2023-06-08 19:15:56.173904 pyxy3d-0.0.19/pyxy3d/triangulate/sync_packet_triangulator.py
+-rw-r--r--   0        0        0     8240 2023-06-12 17:10:55.916740 pyxy3d-0.0.19/README.md
+-rw-r--r--   0        0        0     9057 1970-01-01 00:00:00.000000 pyxy3d-0.0.19/PKG-INFO
```

### Comparing `pyxy3d-0.0.18/LICENSE.md` & `pyxy3d-0.0.19/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/corner_tracker.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/draw_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/monocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/omnicalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/__pycache__/stereocalibrator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/capture_volume.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/quality_controller.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/__pycache__/set_origin_functions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/capture_volume.py` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/capture_volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import pandas as pd
 from time import perf_counter
 
 
 from pyxy3d import get_config
 from pyxy3d.calibration.capture_volume.point_estimates import PointEstimates,load_point_estimates
 from pyxy3d.calibration.charuco import Charuco
-from pyxy3d.cameras.camera_array import CameraArray, get_camera_array
+from pyxy3d.cameras.camera_array import CameraArray
 from pyxy3d.calibration.capture_volume.set_origin_functions import (
     get_board_origin_transform,
 )
 
 CAMERA_PARAM_COUNT = 6
 
 
@@ -70,23 +70,21 @@
             rmse = rms_reproj_error(
                 xy_reproj_error, self.point_estimates.camera_indices
             )
 
         return rmse
 
     def get_rmse_summary(self):
-        
-        rmse_string = f"\nRMSE of Reprojection\n"
-        rmse_string+= f"    Overall: {round(self.rmse['overall'],2)}\n"
+        rmse_string = f"RMSE of Reprojection Overall: {round(self.rmse['overall'],2)}\n"
         rmse_string+= "    by camera:\n"
         for key, value in self.rmse.items():
             if key == "overall":
                 pass
             else:
-                rmse_string+=f"{key: >9}: {round(float(value),2)} \n"
+                rmse_string+=f"    {key: >9}: {round(float(value),2)}\n"
 
         return rmse_string
         
     def get_xy_reprojection_error(self):
         vectorized_params = self.get_vectorized_params()
         error = xy_reprojection_error(vectorized_params, self)
 
@@ -246,54 +244,18 @@
         camera_errors = euclidean_distance_error[camera_indices == port]
         rmse[str(port)] = np.sqrt(np.mean(camera_errors**2))
     # for port in camera_indices
     # logger.info(f"Optimization run with {xy_reproj_error.shape[0]} image points")
     # logger.info(f"RMSE of reprojection is {rmse}")
     return rmse
 
-def load_capture_volume(session_path:Path):
-    config = get_config(session_directory)
-
-    camera_array = get_camera_array(config)
-    point_estimates = load_point_estimates(config)
-    
-    capture_volume = CaptureVolume(camera_array, point_estimates)    
-    capture_volume.stage = config["capture_volume"]["stage"]
-    # capture_volume.origin_sync_index = config["capture_volume"]["origin_sync_index"]
+# def load_capture_volume(session_path:Path):
+#     config = get_config(session_directory)
 
-    return capture_volume
+#     camera_array = get_camera_array(config)
+#     point_estimates = load_point_estimates(config)
     
+#     capture_volume = CaptureVolume(camera_array, point_estimates)    
+#     capture_volume.stage = config["capture_volume"]["stage"]
+#     # capture_volume.origin_sync_index = config["capture_volume"]["origin_sync_index"]
 
-if __name__ == "__main__":
-    # if True:
-    from pyxy3d import __root__
-    from pyxy3d.cameras.camera_array_initializer import CameraArrayInitializer
-    from pyxy3d.calibration.capture_volume.helper_functions.get_point_estimates import (
-        get_point_estimates,
-    )
-    from pyxy3d.calibration.stereocalibrator import StereoCalibrator
-
-    session_directory = Path(__root__, "tests", "217")
-
-    point_data_path = Path(session_directory, "point_data.csv")
-
-    config_path = Path(session_directory, "config.toml")
-
-    stereocalibrator = StereoCalibrator(config_path, point_data_path)
-    stereocalibrator.stereo_calibrate_all(boards_sampled=10)
-
-    camera_array: CameraArray = CameraArrayInitializer(
-        config_path
-    ).get_best_camera_array()
-
-    point_estimates: PointEstimates = get_point_estimates(camera_array, point_data_path)
-
-    capture_volume = CaptureVolume(camera_array, point_estimates)
-    capture_volume.optimize()
-
-    rmse_string = "\nRMSE of Reprojection (overall and by camera)\n"
-    
-    for key, value in capture_volume.rmse.items():
-        rmse_string+=f"{key: >7}: {round(float(value),2)} \n"
-        
-    logger.info(rmse_string)    
-    
+#     return capture_volume
```

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/capture_volume_stage_1.pkl`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_point_estimates.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/__pycache__/get_stereotriangulated_table.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/get_point_estimates.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/helper_functions/get_stereotriangulated_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from itertools import combinations
 import pandas as pd
 import numpy as np
 from pathlib import Path
 import time
 
 from pyxy3d import __root__
-from pyxy3d.cameras.data_packets import PointPacket, FramePacket, SyncPacket
+from pyxy3d.interface import PointPacket, FramePacket, SyncPacket
 from pyxy3d.cameras.camera_array import CameraArray
 from pyxy3d.triangulate.array_stereo_triangulator import ArrayStereoTriangulator
 
 from pyxy3d.triangulate.stereo_points_builder import (
     StereoPointsBuilder,
     StereoPointsPacket,
     SynchedStereoPointsPacket,
```

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/point_estimates.py` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/point_estimates.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from pathlib import Path
 
 from scipy.sparse import lil_matrix
 
 import pandas as pd
 import numpy as np
 from dataclasses import dataclass
-from pyxy3d.cameras.camera_array import CameraArray, get_camera_array
 from pyxy3d.calibration.capture_volume.helper_functions.get_stereotriangulated_table import get_stereotriangulated_table
 
 CAMERA_PARAM_COUNT = 6  # this will evolve when moving from extrinsic to intrinsic
 
 
 @dataclass
 class PointEstimates:
@@ -91,24 +90,7 @@
 
     for key, value in point_estimates_dict.items():
         point_estimates_dict[key] = np.array(value)
 
     point_estimates = PointEstimates(**point_estimates_dict)
     return point_estimates
 
-
-
-#%%
-if __name__ == "__main__":
-    #%%
-    from pyxy3d import __root__
-    from pyxy3d.calibration.capture_volume.helper_functions.get_point_estimates import get_point_estimates 
-    session_directory = Path(__root__, "tests", "4_cameras_beginning")
-    point_data_path = Path(session_directory, "point_data.csv" )
-
-    camera_array = CameraArrayBuilder(Path(session_directory, "config.toml")).get_camera_array()
-
-    point_estimates = get_point_estimates(camera_array, point_data_path)
-
-
-
-# %%
```

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/quality_controller.py` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/quality_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
     for i, a in enumerate(np.ix_(*arrays)):
         arr[..., i] = a
     return arr.reshape(-1, la)
 
 
 if __name__ == "__main__":
 # if True:
-    from pyxy3d.session import Session
+    from pyxy3d.session.session import Session
     from pyxy3d import __root__
 
     session_directory = Path(__root__, "tests", "217")
     # config_path = Path(session_directory, "config.toml")  
     # capture_volume_name = "capture_volume_stage_0.pkl"
     
     # get the inputs for quality control (CaptureVolume and Charuco)
```

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/seaborn_summaries.py` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/seaborn_summaries.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/capture_volume/set_origin_functions.py` & `pyxy3d-0.0.19/pyxy3d/calibration/capture_volume/set_origin_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     note that the array is ordered according to the charuco id
     """
     sync_indices = point_estimates.sync_indices  # convienent shortening
     charuco_ids = point_estimates.point_id[sync_indices == sync_index]
     unique_charuco_id = np.unique(charuco_ids)
     unique_charuco_id.sort()
 
-    board_corners_xyz = charuco.board.chessboardCorners[unique_charuco_id]
+    board_corners_xyz = charuco.board.getChessboardCorners()[unique_charuco_id]
     return board_corners_xyz
 
 
 def get_anchor_cameras(
     camera_array: CameraArray, point_estimates: PointEstimates, sync_index: int
 ) -> list:
     """
@@ -93,15 +93,14 @@
 
 def get_rvec_tvec_from_board_pose(
     camera_array: CameraArray,
     point_estimates: PointEstimates,
     sync_index: int,
     charuco: Charuco,
 ):
-
     world_corners_xyz = get_world_corners_xyz(point_estimates, sync_index)
     board_corners_xyz = get_board_corners_xyz(point_estimates, sync_index, charuco)
     anchor_cameras = get_anchor_cameras(camera_array, point_estimates, sync_index)
 
     rvecs = []
     tvecs = []
 
@@ -165,15 +164,14 @@
     rot_matrix = transformation[0:3, 0:3]
     rvec = cv2.Rodrigues(rot_matrix)[0]
     tvec = np.expand_dims(transformation[0:3, 3], axis=1)
     return rvec, tvec
 
 
 def rvec_tvec_to_transform(rvec: np.ndarray, tvec: np.ndarray) -> np.ndarray:
-
     # might send a rotation matrix into here so check
     # that rvec is a rodrigues vector before converting
     if len(rvec.shape) == 1 or rvec.shape[1] == 1:
         rvec = cv2.Rodrigues(rvec)[0]
 
     # if tvec doesn't have the extra dimension, add it
     if len(tvec.shape) == 1:
@@ -183,15 +181,14 @@
     transform = np.vstack([transform, np.array([0, 0, 0, 1], np.float32)])
     return transform
 
 
 def world_board_distance(
     tvec_xyz: np.ndarray, good_rvec: np.ndarray, raw_world_xyz, board_corners_xyz
 ):
-
     scale = np.expand_dims(np.ones(raw_world_xyz.shape[0]), 1)
     raw_world_xyzh = np.hstack([raw_world_xyz, scale])
 
     origin_shift_transform = rvec_tvec_to_transform(good_rvec, tvec_xyz)
 
     new_origin_xyzh = np.matmul(
         np.linalg.inv(origin_shift_transform), raw_world_xyzh.T
@@ -235,19 +232,23 @@
     final_transform = rvec_tvec_to_transform(good_rvec, optimal_tvec)
 
     return final_transform
 
 
 if __name__ == "__main__":
     #
-    from pyxy3d.session import Session
+    from pyxy3d.session.session import Session
     from pyxy3d.cameras.camera_array_initializer import CameraArrayInitializer
     from pyxy3d.calibration.capture_volume.capture_volume import CaptureVolume
-    from pyxy3d.gui.vizualize.capture_volume_visualizer import CaptureVolumeVisualizer
-    from pyxy3d.gui.vizualize.capture_volume_widget import CaptureVolumeWidget
+    from pyxy3d.gui.vizualize.calibration.capture_volume_visualizer import (
+        CaptureVolumeVisualizer,
+    )
+    from pyxy3d.gui.vizualize.calibration.capture_volume_widget import (
+        CaptureVolumeWidget,
+    )
 
     # test_scenario = "4_cameras_nonoverlap"
     # test_scenario = "3_cameras_middle"
     # test_scenario = "2_cameras_linear"
     # test_scenario = "3_cameras_triangular"
     test_scenario = "4_cameras_beginning"  # initial translation off
     # test_scenario = "3_cameras_midlinear"
@@ -266,41 +267,39 @@
 
     session_directory = Path(__root__, "tests", test_scenario)
     point_data_csv_path = Path(session_directory, "point_data.csv")
     config_path = Path(session_directory, "config.toml")
 
     # need to get the charuco board that was used during the session for later
     session = Session(session_directory)
-    charuco = session.charuco
+    tracker = session.charuco
 
     REOPTIMIZE_CAPTURE_VOLUME = True
     # REOPTIMIZE_CAPTURE_VOLUME = False
 
     if REOPTIMIZE_CAPTURE_VOLUME:
-
         array_initializer = CameraArrayInitializer(config_path)
         camera_array = array_initializer.get_best_camera_array()
         point_estimates = get_point_estimates(camera_array, point_data_csv_path)
 
         print(f"Optimizing initial camera array configuration ")
 
         capture_volume = CaptureVolume(camera_array, point_estimates)
         capture_volume._save(session_directory, "initial")
         capture_volume.optimize()
         capture_volume._save(session_directory, "optimized")
     else:
-
         saved_CV_path = Path(session_directory, "capture_volume_stage_1_optimized.pkl")
         with open(saved_CV_path, "rb") as f:
             capture_volume: CaptureVolume = pickle.load(f)
 
     origin_sync_index = origin_sync_indices[test_scenario]
     logger.warning(f"New test sync index is {origin_sync_index}")
 
-    capture_volume.set_origin_to_board(origin_sync_index, charuco)
+    capture_volume.set_origin_to_board(origin_sync_index, tracker)
 
     app = QApplication(sys.argv)
     vizr = CaptureVolumeVisualizer(capture_volume=capture_volume)
 
     vizr_dialog = CaptureVolumeWidget(vizr)
     vizr_dialog.show()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/charuco.py` & `pyxy3d-0.0.19/pyxy3d/calibration/charuco.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     def save_image(self, path):
         cv2.imwrite(path, self.board_img)
 
     def save_mirror_image(self, path):
         mirror = cv2.flip(self.board_img, 1)
         cv2.imwrite(path, mirror)
 
-    def get_connected_corners(self):
+    def get_connected_points(self):
         """
         For a given board, returns a set of corner id pairs that will connect to form
         a grid pattern. This will provide the "object points" used by the calibration
         functions. It is the ground truth of how the points relate in the world.
 
         The return value is a *set* not a list
         """
```

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/draw_charuco.py` & `pyxy3d-0.0.19/pyxy3d/calibration/draw_charuco.py`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/monocalibrator.py` & `pyxy3d-0.0.19/pyxy3d/calibration/monocalibrator.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,51 +9,61 @@
 
 import cv2
 import numpy as np
 
 
 import pyxy3d.calibration.draw_charuco as draw_charuco
 from pyxy3d.calibration.charuco import Charuco
-from pyxy3d.img2xy.charuco_tracker import CharucoTracker
-from pyxy3d.cameras.data_packets import FramePacket
+from pyxy3d.trackers.charuco_tracker import CharucoTracker
+from pyxy3d.interface import FramePacket
 from pyxy3d.cameras.live_stream import LiveStream
 
 class MonoCalibrator():
 
     def __init__(
-        self, stream:LiveStream,  board_threshold=0.7, wait_time=0.5
+        self, stream:LiveStream,  board_threshold=0.7, wait_time=0.5, fps = 6
     ):
         self.stream = stream
         self.camera: Camera = stream.camera  # reference needed to update params
         self.port = self.camera.port
+        self.board_threshold = board_threshold
+                
+        # # this is strange but is done to allow the GUI an easy way to restore stream fps when switching between monocal/synchronizer
+        # # self.fps = fps # monocalibrator should not store fps...it's a stream prop. 
+        # self.set_stream_fps(fps)
+
         self.wait_time = wait_time
         self.capture_corners = Event()
         self.capture_corners.clear() # start out not doing anything
         self.stop_event = Event()
-        
+                
         self.frame_packet_in_q = Queue(-1)    
         self.subscribe_to_stream()
 
         self.grid_frame_ready_q = Queue()
-        self.connected_corners = self.stream.charuco.get_connected_corners()
 
-        board_corner_count = len(self.stream.charuco.board.getChessboardCorners())
-        self.min_points_to_process = int(board_corner_count * board_threshold)
 
         self.initialize_grid_history()
 
         self.last_calibration_time = (
             time.perf_counter()
         )  # need to initialize to *something*
 
         self.thread = Thread(target=self.collect_corners, args=(), daemon=True)
         self.thread.start()
 
         logger.info(f"Beginning monocalibrator for port {self.port}")
 
+    # def set_stream_fps(self, fps_target:int=None):
+    #     """
+    #     If new target, update monocal property, otherwise revert to previously stored
+    #     """
+    #     if fps_target is not None:
+    #         self.fps = fps_target
+    #     self.stream.set_fps_target(self.fps)
      
     @property
     def grid_count(self):
         """How many sets of corners have been collected up to this point"""
         return len(self.all_ids)
 
     @property
@@ -87,63 +97,71 @@
         """
         Input: opencv frame
 
         Primary Action: records corner ids, positions, and board positions provided
         that enough time has past since the last set was recorded
 
         """
-        logger.debug("Entering collect_corners thread loop")
-        
-        # self.stream.push_to_out_q.set()
+        logger.info(f"Entering collect_corners thread loop for port {self.port}")
+
+        # these values are getting initialized now because the stream may not have
+        # a tracker at the time the stream tools are loaded
+        self.connected_points = self.stream.tracker.get_connected_points()
+        board_corner_count = len(self.stream.tracker.board.getChessboardCorners())
+        self.min_points_to_process = int(board_corner_count * self.board_threshold)
         
         while not self.stop_event.is_set():
             
             self.frame_packet: FramePacket = self.frame_packet_in_q.get()
             self.frame = self.frame_packet.frame
 
             if self.capture_corners.is_set() and self.frame_packet.points is not None:
-                logger.info("Points found and being processed...")
                 self.ids = self.frame_packet.points.point_id
                 self.img_loc = self.frame_packet.points.img_loc
                 self.obj_loc = self.frame_packet.points.obj_loc
 
                 if self.ids.any():
                     enough_corners = len(self.ids) > self.min_points_to_process
                 else:
                     enough_corners = False
 
                 enough_time_from_last_cal = (
                     time.perf_counter() > self.last_calibration_time + self.wait_time
                 )
 
                 if enough_corners and enough_time_from_last_cal:
+                    logger.debug(f"Points found and being processed for port {self.port}")
 
                     # store the corners and IDs
                     self.all_ids.append(self.ids)
                     self.all_img_loc.append(self.img_loc)
                     self.all_obj_loc.append(self.obj_loc)
 
                     self.last_calibration_time = time.perf_counter()
                     self.update_grid_history()
-
+                else:
+                    logger.debug(f"No points collected for processing at port {self.port}")
+                    
+                    
             if self.frame_packet.frame is not None:
                 self.set_grid_frame()
 
         logger.info(f"Monocalibrator at port {self.port} successfully shutdown...")
         self.stream.push_to_out_q.clear()
         
     def update_grid_history(self):
         if len(self.ids) > 2:
             self.grid_capture_history = draw_charuco.grid_history(
                 self.grid_capture_history,
                 self.ids,
                 self.img_loc,
-                self.connected_corners,
+                self.connected_points,
             )
 
+
     def set_grid_frame(self):
         """Merges the current frame with the currently detected corners (red circles) 
         and a history of the stored grid information."""
 
         logger.debug(f"Frame Size is {self.frame.shape} at port {self.port}")
         logger.debug(
             f"camera resolution is {self.camera.size} at port {self.port}"
@@ -198,27 +216,30 @@
         logger.info(f"Setting calibration params on camera {self.camera.port}")
         # ret is RMSE of reprojection
         self.camera.error = round(self.error, 3)
         self.camera.matrix = self.mtx
         self.camera.distortions = self.dist
         self.camera.grid_count = len(self.all_ids)
 
+
 if __name__ == "__main__":
 
     from pyxy3d.cameras.camera import Camera
     from pyxy3d.cameras.synchronizer import Synchronizer
     from pyxy3d.cameras.live_stream import LiveStream
 
     charuco = Charuco(
-        4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
+        3, 4, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
     )
+    charuco_tracker = CharucoTracker(charuco)
+
 
     test_port = 0
     cam = Camera(0)
-    stream = LiveStream(cam, charuco=charuco)
+    stream = LiveStream(cam, tracker=charuco_tracker)
     stream._show_fps = True
     # syncr = Synchronizer(streams, fps_target=20)
 
     monocal = MonoCalibrator(stream)
 
     monocal.capture_corners.set()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/calibration/stereocalibrator.py` & `pyxy3d-0.0.19/pyxy3d/calibration/stereocalibrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         # group points into boards and get the total count for sample weighting below
         pair_points = self.all_point_data[self.all_point_data["in_pair"] == True]
         pair_boards = (
             pair_points.filter(["sync_index", "port", "point_id"])
             .groupby(["sync_index", "port"])
             .agg("count")
             .rename({"point_id": "point_count"}, axis=1)
-            .query("point_count > 4")  # a requirement of the stereocalibration function
+            .query("point_count >=6")  # a requirement of the stereocalibration function
             .reset_index()
             .query(f"port == {pair[0]}")  # will be the same..only need one copy
             .drop("port", axis=1)
         )
 
         # configure random sampling. If you have too few boards, then only take what you have
         board_count = pair_boards.shape[0]
@@ -303,18 +303,18 @@
 
 if __name__ == "__main__":
     # if True:
     from pathlib import Path
 
     # set inputs
     # session_path = Path(__root__, "tests", "4_cameras_nonoverlap")
-    session_path = Path(__root__, "tests", "4_cameras_endofday")
+    session_path = Path(__root__, "dev", "sample_sessions", "257")
 
     config_path = Path(session_path, "config.toml")
-    point_data_path = Path(session_path, "point_data.csv")
+    point_data_path = Path(session_path, "calibration", "extrinsic", "xy.csv")
 
     stereocal = StereoCalibrator(
         config_path,
         point_data_path,
     )
     
 # %%
```

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/camera_array_initializer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/data_packets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/live_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/cameras/__pycache__/synchronizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/camera.py` & `pyxy3d-0.0.19/pyxy3d/cameras/camera.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,18 +34,19 @@
     # see above for constants used to access properties
     def __init__(self, port, verified_resolutions = None):
 
         # get the platform in use:
         if platform.system() == "Windows":
             logger.debug(f"Windows machine detected - using backend `cv2.CAP_DSHOW`")
             self.device_connection = cv2.CAP_DSHOW
+            # self.device_connection = cv2.CAP_ANY
         else:
             logger.debug(f"Non-Windows machine detected - using backend `cv2.CAP_ANY`")
             self.device_connection = cv2.CAP_ANY
-
+        # self.device_connection = cv2.CAP_ANY
 
         # check if source has a data feed before proceeding...if not it is
         # either in use or fake
         logger.info(f"Attempting to connect video capure at port {port}")
         test_capture = cv2.VideoCapture(port,self.device_connection)
         for _ in range(0, TEST_FRAME_COUNT):
             good_read, frame = test_capture.read()
@@ -170,39 +171,14 @@
             logger.info(f"Checking resolution of {resolution} at port {self.port}")
             self.size = resolution
             
             # if it sticks, then that resolution is verified
             if resolution == self.size:
                 self.verified_resolutions.append(resolution)
                 
-        # min_res = self.get_nearest_resolution(MIN_RESOLUTION_CHECK)
-        # max_res = self.get_nearest_resolution(MAX_RESOLUTION_CHECK)
-
-        # min_width = min_res[0]
-        # max_width = max_res[0]
-
-        # STEPS_TO_CHECK = 20  # fast to check so cover your bases
-
-        # # the size of jump to make before checking on the resolution
-        # step_size = int((max_width - min_width) / STEPS_TO_CHECK)
-
-        # resolutions = {min_res, max_res}
-
-        # if max_width > min_width:  # i.e. only one size avaialable
-        #     for test_width in range(
-        #         int(min_width + step_size), int(max_width - step_size), int(step_size)
-        #     ):
-        #         new_res = self.get_nearest_resolution(test_width)
-        #         # print(new_res)
-        #         resolutions.add(new_res)
-        #     resolutions = list(resolutions)
-        #     resolutions.sort()
-        #     self.possible_resolutions = resolutions
-        # else:
-        #     self.possible_resolutions = self.default_resolution
 
     def rotate_CW(self):
         if self.rotation_count == 3:
             self.rotation_count = 0
         else:
             self.rotation_count = self.rotation_count + 1
 
@@ -280,15 +256,15 @@
     # (3840, 2160),
     # (7680, 4320),
 ]
 
 ######################### TEST FUNCTIONALITY OF CAMERAS ########################
 if __name__ == "__main__":
 
-    cam = Camera(0)
+    cam = Camera(0, verified_resolutions=[(640,480), (1280,720)])
     logger.info(f"Camera {cam.port} has possible resolutions: {cam.verified_resolutions}")
 
     for res in cam.verified_resolutions:
         logger.info(f"Testing Resolution {res}")
 
         cam.disconnect()
         cam.connect()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/camera_array.py` & `pyxy3d-0.0.19/pyxy3d/cameras/camera_array.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pyxy3d.logger
 logger = pyxy3d.logger.get(__name__)
 
 from pathlib import Path
 import numpy as np
 from dataclasses import dataclass
 import cv2
-
+from enum import Enum, auto
 
 CAMERA_PARAM_COUNT = 6
 
 @dataclass
 class CameraData:
     """
     A place to hold the calibration data associated with a camera that has been populated from a config file.
@@ -130,53 +130,39 @@
         new_camera_params = flat_camera_params.reshape(n_cameras, n_cam_param)
 
         # update camera array with new positional data
         for index in range(len(new_camera_params)):
             port = self.index_port[index]  # correct in case ignoring a camera
             cam_vec = new_camera_params[index, :]
             self.cameras[port].extrinsics_from_vector(cam_vec)
+        
+    @property
+    def extrinsics_calibrated(self)->bool:
+       
+        # assume extrinsics calibrated and provide otherwise
+        full_extrinsics = True 
+        for port, cam in self.cameras.items():
+            if cam.rotation is None or cam.translation is None:
+                full_extrinsics = False
 
+        return full_extrinsics
+        
+            
+            
 
-def get_camera_array(config:dict)->CameraArray:
+class CalibrationStage(Enum):
     """
-    Load camera array directly from config file. The results of capture volume
-    optimization and origin transformation will be reflected in this array
-    which can then be the basis for future 3d point estimation
-    """
-    all_camera_data = {}
-    for key, params in config.items():
-        if key.startswith("cam"):
-            if params["translation"] is not None:
-                port = params["port"]
-                size = params["size"]
-
-                logger.info(f"Adding camera {port} to calibrated camera array...")
-                cam_data = CameraData(
-                    port=port,
-                    size=params["size"],
-                    rotation_count=params["rotation_count"],
-                    error=params["error"],
-                    matrix=np.array(params["matrix"]),
-                    distortions=np.array(params["distortions"]),
-                    exposure=params["exposure"],
-                    grid_count=params["grid_count"],
-                    ignore=params["ignore"],
-                    verified_resolutions=params["verified_resolutions"],
-                    translation=np.array(params["translation"]),
-                    rotation=np.array(params["rotation"]),
-                )
-
-                all_camera_data[port] = cam_data
-
-    camera_array = CameraArray(all_camera_data)
-    return camera_array
-
-if __name__ == "__main__":
-    from pyxy3d.cameras.camera_array_initializer import CameraArrayInitializer  
-    from pyxy3d import __root__
-
-    session_directory = Path(__root__, "tests", "sessions", "217")
-    config_path = Path(session_directory, "config.toml")
-    array_builder = CameraArrayInitializer(config_path)
-    camera_array = array_builder.get_best_camera_array()
+    NOTE: this is not currently implemented. I was planning to set this up
+    in dev_post_process_eligible_check as a way to help manage the flow of the
+    GUI (it would be important to now the status of teh calibration in an easy way)
+    Unfortunately this begins to touch up on how/when the session loads the camera array,
+    and that's something that I'm not sure is fully relevant right now.
+    The camera array is not initialized until it is estimated via bundle adjustment.
+    Prior to that it is only a dictionary of cameras. 
+    
+    Consider removing...
 
-# %%
+    """
+    NO_INTRINSICS = auto()
+    PARTIAL_INTRINSICS = auto()
+    FULL_INTRINSICS = auto()
+    EXTRINSICS = auto()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/camera_array_initializer.py` & `pyxy3d-0.0.19/pyxy3d/cameras/camera_array_initializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,17 +314,17 @@
     config_path = Path(session_directory, "config.toml")
 
     initializer = CameraArrayInitializer(config_path)
         
     
     camera_array = initializer.get_best_camera_array()
 
-    point_data_path = Path(session_directory, "point_data.csv")
+    extrinsic_calibration_xy = Path(session_directory, "point_data.csv")
 
-    point_estimates: PointEstimates = get_point_estimates(camera_array, point_data_path)
+    point_estimates: PointEstimates = get_point_estimates(camera_array, extrinsic_calibration_xy)
 
     capture_volume = CaptureVolume(camera_array, point_estimates)
 
     pair_A_B = initializer.estimated_stereopairs[(0, 1)]
     pair_B_C = initializer.estimated_stereopairs[(1, 2)]
 
     bridged_pair = get_bridged_stereopair(pair_A_B, pair_B_C)
```

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/live_stream.py` & `pyxy3d-0.0.19/pyxy3d/cameras/live_stream.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,115 +11,110 @@
 from threading import Thread, Event
 
 import cv2
 import numpy as np
 from abc import ABC, abstractmethod
 
 from pyxy3d.cameras.camera import Camera
-from pyxy3d.cameras.data_packets import FramePacket
+from pyxy3d.interface import FramePacket, Stream, Tracker
 from pyxy3d.calibration.charuco import Charuco
-from pyxy3d.img2xy.charuco_tracker import CharucoTracker
+from pyxy3d.trackers.charuco_tracker import CharucoTracker
 import pyxy3d.calibration.draw_charuco as draw_charuco
 
-class Stream(ABC):
-    """
-    As much an exercise in better understanding ABC as it is anything...
-    """
-    @abstractmethod
-    def subscribe(self,queue:Queue):
-        pass
-    
-    @abstractmethod
-    def unsubscribe(self,queue:Queue):
-        pass
-    
-    def set_tracking_on(self,track:bool):
-        pass
-
-    
-    @abstractmethod
-    def worker(self):
-        pass
 
 class LiveStream(Stream):
-    def __init__(self, camera:Camera, fps_target=6, charuco=None):
-        self.camera:Camera = camera
+    def __init__(self, camera: Camera, fps_target: int = 6, tracker: Tracker = None):
+        self.camera: Camera = camera
         self.port = camera.port
         self.track_points = Event()
 
-        if charuco is not None:
-            self.charuco = charuco
-            self.tracker = CharucoTracker(charuco)
+        if tracker is not None:
+            self.tracker = tracker
             self.track_points.set()  # default to tracking points if the charuco is provided
+            self.draw_instructions = self.tracker.draw_instructions
         else:
             self.track_points.clear()  # just to be clear
+            self.draw_instructions = None
 
         self.stop_event = Event()
-        
+
         # list of queues that will have frame packets pushed to them
         self.subscribers = []
-        
+
         # make sure camera no longer reading before trying to change resolution
         self.stop_confirm = Queue()
 
         self._show_fps = False  # used for testing
-        self._show_charuco = False  # used for testing
+
+        self.show_points(False)
 
         self.set_fps_target(fps_target)
         self.FPS_actual = 0
         # Start the thread to read frames from the video stream
-        self.thread = Thread(target=self.worker, args=(), daemon=True)
+        self.thread = Thread(target=self.process_frames, args=(), daemon=True)
         self.thread.start()
 
         # initialize time trackers for actual FPS determination
         self.frame_time = perf_counter()
         self.avg_delta_time = 1  # initialize to something to avoid errors elsewhere
 
     def set_tracking_on(self, track: bool):
         if track:
             logger.info(f"Turning tracking on on stream {self.port}")
             self.track_points.set()
         else:
             logger.info(f"Turning tracking off on stream {self.port}")
             self.track_points.clear()
 
-    def subscribe(self,queue:Queue):
+    def show_points(self, show: bool):
+        if show:
+            self._show_points = True
+        else:
+            self._show_points = False
+
+    def subscribe(self, queue: Queue):
         if queue not in self.subscribers:
             logger.info(f"Adding queue to subscribers at stream {self.port}")
             self.subscribers.append(queue)
             logger.info(f"...now {len(self.subscribers)} subscriber(s) at {self.port}")
         else:
-            logger.warn(f"Attempted to subscribe to live stream at port {self.port} twice")
-
-    def unsubscribe(self, queue:Queue):
-        if queue in self.subscribers:
-            logger.info(f"Removing subscriber from queue at port {self.port}")
-            self.subscribers.remove(queue)
-            logger.info(f"{len(self.subscribers)} subscriber(s) remain at port {self.port}")
-        else:
-            logger.warn(f"Attempted to unsubscribe to live stream that was not subscribed to\
-                at port {self.port} twice")
-
+            logger.warn(
+                f"Attempted to subscribe to live stream at port {self.port} twice"
+            )
 
+    def unsubscribe(self, queue: Queue):
+        try:
+            if queue in self.subscribers:
+                logger.info(f"Removing subscriber from queue at port {self.port}")
+                self.subscribers.remove(queue)
+                logger.info(
+                    f"{len(self.subscribers)} subscriber(s) remain at port {self.port}"
+                )
+            else:
+                logger.warn(
+                    f"Attempted to unsubscribe to live stream that was not subscribed to\
+                    at port {self.port} twice"
+                )
+        except:
+            logger.warn("Attempted to remove queue that may have been removed twice at once")
     def set_fps_target(self, fps):
         """
         This is done through a method as it will also do a one-time determination of the times as which
         frames should be read (the milestones)
         """
 
         self.fps = fps
         milestones = []
         for i in range(0, fps):
             milestones.append(i / fps)
-        logger.info(f"Setting fps to {self.fps}")
+        logger.info(f"Setting fps to {self.fps} at port {self.port}")
         self.milestones = np.array(milestones)
 
-    def update_charuco(self, charuco: Charuco):
-        self.charuco = charuco
-        self.tracker = CharucoTracker(charuco)
+    def update_tracker(self, tracker: Tracker):
+        self.tracker = tracker
 
     def wait_to_next_frame(self):
         """
         based on the next milestone time, return the time needed to sleep so that
         a frame read immediately after would occur when needed
         """
 
@@ -141,97 +136,99 @@
         """
         self.delta_time = perf_counter() - self.start_time
         self.start_time = perf_counter()
         if not self.avg_delta_time:
             self.avg_delta_time = self.delta_time
 
         # folding in current frame rate to trailing average to smooth out
-        self.avg_delta_time = 0.5 * self.avg_delta_time + 0.5* self.delta_time
+        self.avg_delta_time = 0.5 * self.avg_delta_time + 0.5 * self.delta_time
         self.previous_time = self.start_time
         return 1 / self.avg_delta_time
 
-    def stop(self):
-        self.push_to_out_q.clear()
-        self.stop_event.set()
-        logger.info(f"Stop signal sent at stream {self.port}")
+    # def stop(self):
+    #     self.push_to_out_q.clear()
+    #     self.stop_event.set()
+    #     logger.info(f"Stop signal sent at stream {self.port}")
 
-    def worker(self):
+    def process_frames(self):
         """
         Worker function that is spun up by Thread. Reads in a working frame,
         calls various frame processing methods on it, and updates the exposed
         frame
         """
         self.start_time = perf_counter()  # used to get initial delta_t for FPS
         first_time = True
         while not self.stop_event.is_set():
             if first_time:
                 logger.info(f"Camera now rolling at port {self.port}")
                 first_time = False
 
             if self.camera.capture.isOpened():
-
-                # slow wait if not pushing frames                
+                # slow wait if not pushing frames
                 # this is a sub-optimal busy wait spin lock, but it works and I'm tired.
-                # stop_event condition added to allow loop to wrap up 
+                # stop_event condition added to allow loop to wrap up
                 # if attempting to change resolution
-                spinlock_looped = False 
+                spinlock_looped = False
                 while len(self.subscribers) == 0 and not self.stop_event.is_set():
                     if not spinlock_looped:
                         logger.info(f"Spinlock initiated at port {self.port}")
                         spinlock_looped = True
-                    sleep(.5)
+                    sleep(0.5)
                 if spinlock_looped == True:
                     logger.info(f"Spinlock released at port {self.port}")
-                    
-                
 
                 # Wait an appropriate amount of time to hit the frame rate target
                 sleep(self.wait_to_next_frame())
 
                 read_start = perf_counter()
-                self.success, self.frame = self.camera.capture.read()
+                grab_success = self.camera.capture.grab()
+                self.success, self.frame = self.camera.capture.retrieve()
 
                 read_stop = perf_counter()
-                point_data = None # Provide initial value here...may get overwritten
+                point_data = None  # Provide initial value here...may get overwritten
                 self.frame_time = (read_start + read_stop) / 2
 
                 if self.success and len(self.subscribers) > 0:
                     logger.debug(f"Pushing frame to reel at port {self.port}")
 
                     if self.track_points.is_set():
-                        point_data = self.tracker.get_points(self.frame)
-                    # else:
-                        # point_data = None
+                        point_data = self.tracker.get_points(
+                            frame = self.frame,
+                            port = self.port,
+                            rotation_count=self.camera.rotation_count,
+                        )
 
                     if self._show_fps:
                         self._add_fps()
 
                     frame_packet = FramePacket(
                         port=self.port,
                         frame_time=self.frame_time,
                         frame=self.frame,
                         points=point_data,
+                        draw_instructions=self.draw_instructions,
                     )
 
-                    if self._show_charuco:
-                        draw_charuco.corners(frame_packet)
-                        # self.out_q.put([self.frame_time, self.frame])
+                    # cv2.imshow(str(self.port), frame_packet.frame_with_points)
+                    # key = cv2.waitKey(1)
+                    # if key == ord("q"):
+                    #     cv2.destroyAllWindows()
+                    #     break
 
                     for q in self.subscribers:
                         q.put(frame_packet)
 
                     # Rate of calling recalc must be frequency of this loop
                     self.FPS_actual = self.get_FPS_actual()
 
         logger.info(f"Stream stopped at port {self.port}")
         self.stop_event.clear()
         self.stop_confirm.put("Successful Stop")
 
     def change_resolution(self, res):
-
         logger.info(f"About to stop camera at port {self.port}")
         self.stop_event.set()
         self.stop_confirm.get()
         logger.info(f"Roll camera stop confirmed at port {self.port}")
 
         self.FPS_actual = 0
         self.avg_delta_time = None
@@ -243,15 +240,15 @@
         self.camera.connect()
 
         self.camera.size = res
         # Spin up the thread again now that resolution is changed
         logger.info(
             f"Beginning roll_camera thread at port {self.port} with resolution {res}"
         )
-        self.thread = Thread(target=self.worker, args=(), daemon=True)
+        self.thread = Thread(target=self.process_frames, args=(), daemon=True)
         self.thread.start()
 
     def _add_fps(self):
         """NOTE: this is used in F5 test, not in external use"""
         self.fps_text = str(int(round(self.FPS_actual, 0)))
         cv2.putText(
             self.frame,
@@ -275,29 +272,28 @@
         cam.exposure = -7
         cams.append(cam)
 
     # standard inverted charuco
     charuco = Charuco(
         4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
     )
+    tracker = CharucoTracker(charuco)
 
     frame_packet_queues = {}
 
-
     streams = []
     for cam in cams:
-
         q = Queue(-1)
         frame_packet_queues[cam.port] = q
 
         print(f"Creating Video Stream for camera {cam.port}")
-        stream = LiveStream(cam, fps_target=5, charuco=charuco)
+        stream = LiveStream(cam, fps_target=5, tracker=tracker)
         stream.subscribe(frame_packet_queues[cam.port])
         stream._show_fps = True
-        stream._show_charuco = True
+        stream.show_points(True)
         streams.append(stream)
 
     while True:
         try:
             for port in ports:
                 frame_packet = frame_packet_queues[port].get()
 
@@ -317,14 +313,14 @@
                 stream.camera.capture.release()
             cv2.destroyAllWindows()
             exit(0)
 
         if key == ord("v"):
             for stream in streams:
                 print(f"Attempting to change resolution at port {stream.port}")
-                stream.change_resolution((640,480))
+                stream.change_resolution((640, 480))
 
         if key == ord("s"):
             for stream in streams:
                 stream.stop()
             cv2.destroyAllWindows()
             exit(0)
```

### Comparing `pyxy3d-0.0.18/pyxy3d/cameras/synchronizer.py` & `pyxy3d-0.0.19/pyxy3d/cameras/synchronizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pyxy3d.logger
 
 logger = pyxy3d.logger.get(__name__)
 import logging
 
-logger.setLevel(logging.DEBUG)
+# logger.setLevel(logging.DEBUG)
 
 import time
 from pathlib import Path
 from queue import Queue
 from threading import Thread, Event
 
 import cv2
 import numpy as np
-from pyxy3d.cameras.data_packets import SyncPacket
+from pyxy3d.interface import SyncPacket
 
 DROPPED_FRAME_TRACK_WINDOW = 100 # trailing frames tracked for reporting purposes
 
 class Synchronizer:
     def __init__(self, streams: dict, fps_target=6):
         self.streams = streams
         self.current_synched_frames = None
@@ -38,30 +38,26 @@
             self.ports.append(port)
             q = Queue(-1)
             self.frame_packet_queues[port] = q
 
         self.subscribed_to_streams = False # not subscribed yet
         self.subscribe_to_streams()
 
-        self._fps_target = fps_target
-        self.set_fps_target(self._fps_target)
+        self.set_stream_fps(fps_target)
         self.fps_mean = fps_target
         
         # place to store a recent history of dropped frames
         self.dropped_frame_history = {port:[] for port in sorted(self.ports)} 
         
         self.initialize_ledgers()
         self.start()
 
     def set_tracking_on_streams(self, track:bool):
         for port, stream in self.streams.items():
             stream.set_tracking_on(track)
-
-    def get_fps_target(self):
-        return self._fps_target
     
     def update_dropped_frame_history(self):
         current_dropped:dict = self.current_sync_packet.dropped    
         
         for port, dropped in current_dropped.items():
             self.dropped_frame_history[port].append(dropped)
             self.dropped_frame_history[port] = self.dropped_frame_history[port][-DROPPED_FRAME_TRACK_WINDOW:]
@@ -70,26 +66,26 @@
     def dropped_fps(self):
         """
         Averages dropped frame count across the observed history
         """
         return {port:np.mean(drop_history) for port,drop_history in self.dropped_frame_history.items()}        
 
         
-    def set_fps_target(self, target):
-        self._fps_target = target
-        logger.info(f"Attempting to change target fps in streams to {target}")
+    def set_stream_fps(self, fps_target):
+        self.fps_target = fps_target
+        logger.info(f"Attempting to change target fps in streams to {fps_target}")
         for port, stream in self.streams.items():
-            stream.set_fps_target(target)
+            stream.set_fps_target(fps_target)
 
     def subscribe_to_streams(self):
         for port, stream in self.streams.items():
             stream.subscribe(self.frame_packet_queues[port])
         self.subscribed_to_streams = True
 
-    def unsubscribe_to_streams(self):
+    def unsubscribe_from_streams(self):
         for port, stream in self.streams.items():
             logger.info(f"unsubscribe synchronizer from port {port}")
             stream.unsubscribe(self.frame_packet_queues[port])
         self.subscribed_to_streams = False
 
     def stop(self):
         self.stop_event.set()
@@ -172,22 +168,26 @@
             while frame_data_key not in self.all_frame_packets.keys():
                 logger.debug(
                     f"Waiting in a loop for frame data to populate with key: {frame_data_key}"
                 )
                 if self.subscribed_to_streams:
                     time.sleep(0.1)
                 else:
+                    # provide infrequent updates of busy waiting
+                    if int(time.time()) % 10 ==0:
+                        logger.info("Synchronizer not subscribed to any streams and busy waiting...")
                     time.sleep(1)
                     
             next_frame_time = self.all_frame_packets[frame_data_key].frame_time
 
             if next_frame_time == -1:
                 logger.info(
                     f"End of frames at port {p} detected; ending synchronization"
                 )
+                
                 self.frames_complete = True
                 self.stop_event.set()
 
             if p != port:
                 times_of_next_frames.append(next_frame_time)
 
         return min(times_of_next_frames)
@@ -291,64 +291,74 @@
             if self.stop_event.is_set():
                 logger.info("Sending `None` on queue to signal end of synced frames.")
                 self.current_sync_packet = None
 
             # notify other processes that the new frames are ready for processing
             # only for tasks that can risk missing frames (i.e. only for gui purposes)
             for q in self.sync_notice_subscribers:
-                logger.debug(f"Giving notice of new synched frames packet via {q}")
+                logger.debug(f"Giving notice of new synched frames packet via queue")
                 q.put("new synched frames available")
 
             for q in self.synched_frames_subscribers:
-                logger.debug(f"Placing new synched frames packet on queue: {q}")
                 q.put(self.current_sync_packet)
-
+                if self.current_sync_packet is not None:
+                    logger.debug(f"Placing new synched frames packet on queue with {self.current_sync_packet.frame_packet_count} frames")
+                    logger.debug(f"Placing new synched frames with index {self.current_sync_packet.sync_index}")
+                    
+                    # provide infrequent notice of synchronizer activity
+                    if self.current_sync_packet.sync_index % 100 ==0:
+                        logger.info(f"Placing new synched frames with index {self.current_sync_packet.sync_index}")
+                else:
+                    logger.info(f"signaling end of frames with `None` packet on subscriber queue.")
+                    for port, q in self.frame_packet_queues.items():
+                        logger.info(f"Currently {q.qsize()} frame packets unprocessed for port {port}")
+                    
             self.fps_mean = self.average_fps()
 
         logger.info("Frame synch worker successfully ended")
 
 
 if __name__ == "__main__":
     from pyxy3d.calibration.charuco import Charuco
-    from pyxy3d.img2xy.charuco_tracker import CharucoTracker
+    from pyxy3d.trackers.charuco_tracker import CharucoTracker
     from pyxy3d.recording.recorded_stream import RecordedStream, RecordedStreamPool
 
-    from pyxy3d.session import Session
+    from pyxy3d.session.session import Session
     import time
 
     from pyxy3d import __root__
     
 
     # test_live = True
     test_live = False
 
     if test_live:
 
         session_directory = Path(__root__, "tests", "217")
         # config = Path(session_directory, "config.toml")
         session = Session(session_directory)
-        session.load_cameras()
-        session.load_streams()
+        # session.load_cameras()
+        session.load_stream_tools()
         # session.adjust_resolutions()
 
         for port, stream in session.streams.items():
             stream._show_fps = True
             stream._show_charuco = True
 
         logger.info("Creating Synchronizer")
         syncr = Synchronizer(session.streams, fps_target=5)
     else:
         ports = [0, 1, 2, 3, 4]
         # ports = [0,1]
         recording_directory = Path(__root__, "tests","sessions", "217")
-        charuco = Charuco(
+        tracker = Charuco(
                 4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
             )
         recorded_stream_pool = RecordedStreamPool(
-            ports, recording_directory, charuco=charuco
+            ports, recording_directory, charuco=tracker
         )
         logger.info("Creating Synchronizer")
         syncr = Synchronizer(recorded_stream_pool.streams, fps_target=20)
         recorded_stream_pool.play_videos()
 
     notification_q = Queue()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/__pycache__/main.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/main.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/qt_logger.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/recording_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/widgets.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_charuco.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/__pycache__/wizard_directory.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_config_dialogue.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/camera_tabs.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/camera_config/__pycache__/frame_emitter.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/camera_config/camera_config_dialogue.py` & `pyxy3d-0.0.19/pyxy3d/gui/camera_config/camera_config_dialogue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pyxy3d.logger
+
 logger = pyxy3d.logger.get(__name__)
 
 import sys
 from pathlib import Path
 from threading import Thread
 import time
 
@@ -25,331 +26,332 @@
     QVBoxLayout,
 )
 
 # Append main repo to top of path to allow import of backend
 from pyxy3d.gui.camera_config.frame_emitter import FrameEmitter
 from pyxy3d.calibration.monocalibrator import MonoCalibrator
 from pyxy3d.cameras.camera import Camera
-from pyxy3d.cameras.live_stream import LiveStream 
-from pyxy3d.session import Session
+from pyxy3d.cameras.live_stream import LiveStream
+from pyxy3d.session.session import Session
+from pyxy3d.gui.camera_config.camera_summary_widget import SummaryWidget
 from pyxy3d import __root__
 
 
-class CameraConfigDialog(QDialog):
-    
+class CameraConfigTab(QDialog):
     def __init__(self, session, port):
-        super(CameraConfigDialog, self).__init__()
+        super(CameraConfigTab, self).__init__()
 
         # set up variables for ease of reference
         self.session = session
         self.monocal = session.monocalibrators[port]
         self.port = port
         self.stream = self.monocal.stream
         self.camera = self.stream.camera
 
-        # need frame emitter to create actual frames and track FPS/grid count 
+        # need frame emitter to create actual frames and track FPS/grid count
         App = QApplication.instance()
         DISPLAY_WIDTH = App.primaryScreen().size().width()
         DISPLAY_HEIGHT = App.primaryScreen().size().height()
 
         self.pixmap_edge = min(DISPLAY_WIDTH / 3, DISPLAY_HEIGHT / 3)
         self.frame_emitter = FrameEmitter(self.monocal, self.pixmap_edge)
         self.frame_emitter.start()
 
         self.setWindowTitle("Camera Configuration and Calibration")
         self.setContentsMargins(0, 0, 0, 0)
 
         ################### BUILD SUB WIDGETS #############################
-        
+
         ###################################################################
-        
+
         self.setLayout(QHBoxLayout())
         ##########################################################
         ###################### CALIBRATION  ################################
-        self.calibrate_grp = CalibrationControls(self.session, self.port, self.frame_emitter)
+        self.calibrate_grp = CalibrationControls(
+            self.session, self.port, self.frame_emitter
+        )
 
         # self.build_calibrate_grp()
         self.layout().addWidget(self.calibrate_grp)
 
-
         self.frame_controls_layout = QVBoxLayout(self)
         self.layout().addLayout(self.frame_controls_layout)
-        self.basic_frame_control = FrameControlWidget(self.session, self.port, self.frame_emitter)
-       
-        
+        self.basic_frame_control = FrameControlWidget(
+            self.session, self.port, self.frame_emitter
+        )
+
         self.frame_controls_layout.addWidget(self.basic_frame_control)
 
         self.frame_controls_layout.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         self.frame_controls_layout.setContentsMargins(0, 0, 0, 0)
 
         self.advanced_controls_toggle = QPushButton("Advanced Settings")
         self.advanced_controls_toggle.setCheckable(True)
         self.advanced_controls_toggle.clicked.connect(self.toggle_advanced_controls)
 
         self.frame_controls_layout.addWidget(self.advanced_controls_toggle)
-    
-        self.advanced_controls = AdvancedControls(self.session, self.port, self.frame_emitter)
+
+        self.advanced_controls = AdvancedControls(
+            self.session, self.port, self.frame_emitter
+        )
         self.advanced_controls.hide()
         self.frame_controls_layout.addWidget(self.advanced_controls)
 
         self.connect_widgets()
 
     def toggle_advanced_controls(self):
         if self.advanced_controls_toggle.isChecked():
             self.advanced_controls.show()
         else:
             self.advanced_controls.hide()
-   
+
     def connect_widgets(self):
-        self.basic_frame_control.resolution_combo.currentTextChanged.connect(self.calibrate_grp.clear_camera_calibration)
+        self.basic_frame_control.resolution_combo.currentTextChanged.connect(
+            self.calibrate_grp.clear_camera_calibration
+        )
         self.calibrate_grp.signal_calibration_lock.connect(self.lock_resolution_combo)
-    
-    def lock_resolution_combo(self, lock:bool):
+
+    def lock_resolution_combo(self, lock: bool):
         # note, the is locking, so the signal meaning gets reversed when setting "enable"
         enabled = not lock
         self.basic_frame_control.resolution_combo.setEnabled(enabled)
-        
+
     def save_camera(self):
         self.session.save_camera(self.port)
 
-    
 
 class CalibrationControls(QGroupBox):
     signal_calibration_lock = pyqtSignal(bool)
     calibration_change = pyqtSignal()
 
-    def __init__(self, session:Session, port, frame_emitter:FrameEmitter):
-        super(CalibrationControls,self).__init__("Calibration Summary")
+    def __init__(self, session: Session, port, frame_emitter: FrameEmitter):
+        super(CalibrationControls, self).__init__("Calibration Summary")
 
         self.session: Session = session
         self.port = port
         self.monocal: MonoCalibrator = self.session.monocalibrators[port]
         self.stream: LiveStream = self.monocal.stream
         self.camera: Camera = self.stream.camera
         self.frame_emitter = frame_emitter
-        self.setLayout(QVBoxLayout())        
+        self.setLayout(QVBoxLayout())
 
         self.place_widgets()
         self.connect_widgets()
 
-
     def place_widgets(self):
-
-        self.start_stop_calibration_btn = QPushButton("Collect Data")
+        self.start_stop_calibration_btn = QPushButton("&Collect Data")
         self.layout().addWidget(self.start_stop_calibration_btn)
-        self.undistort_btn = QPushButton("Undistort")    
+        self.undistort_btn = QPushButton("Un&distort")
         self.layout().addWidget(self.undistort_btn)
-         
+
         if self.camera.matrix is None and self.camera.distortions is None:
             self.undistort_btn.setEnabled(False)
-        
-        self.cal_output = QLabel()
-        self.cal_output.setWordWrap(True)
-        self.cal_output.setText(self.monocal.camera.calibration_summary())
-        self.layout().addWidget(self.cal_output)
+
+        self.camera_summary = SummaryWidget(self.camera)
+        self.layout().addWidget(self.camera_summary)
 
     def connect_widgets(self):
         self.start_stop_calibration_btn.clicked.connect(self.capture_control)
         self.undistort_btn.clicked.connect(self.undistort)
+        self.calibration_change.connect(self.update_camera_data)
 
     def capture_control(self):
         """change to turn on/off"""
 
-        if self.start_stop_calibration_btn.text() == "Collect Data":
+        if self.start_stop_calibration_btn.text() == "&Collect Data":
             self.signal_calibration_lock.emit(True)
             self.clear_camera_calibration()
             self.calibration_change.emit()
             self.monocal.capture_corners.set()
             self.undistort_btn.setEnabled(False)
-            self.start_stop_calibration_btn.setText("Calibrate")
-        
-        if self.start_stop_calibration_btn.text() == "Calibrate":
+            self.start_stop_calibration_btn.setText("&Calibrate")
+
+        elif self.start_stop_calibration_btn.text() == "&Calibrate":
             self.signal_calibration_lock.emit(True)
             if len(self.monocal.all_ids) > 0:
-                self.cal_output.setText("Calibration can take a moment...")
+                # stop the colletion of more data
                 self.monocal.capture_corners.clear()
-                self.calibrate()    
+                self.calibrate()
             else:
-                self.cal_output.setText("Need to Collect Grids")
+                # no data collected
+                self.monocal.capture_corners.clear()
+                self.update_camera_data()
+                self.start_stop_calibration_btn.setText("&Collect Data")
 
-        if self.start_stop_calibration_btn.text() == "Re-Collect":
+        elif self.start_stop_calibration_btn.text() == "Re-&Collect":
             self.signal_calibration_lock.emit(True)
             self.clear_camera_calibration()
             self.calibration_change.emit()
             self.monocal.initialize_grid_history()
             self.undistort_btn.setEnabled(False)
             self.monocal.capture_corners.set()
-            self.start_stop_calibration_btn.setText("Calibrate")
-    
+            self.start_stop_calibration_btn.setText("&Calibrate")
+
     def clear_camera_calibration(self):
         self.camera.matrix = None
         self.camera.distortions = None
         self.camera.error = None
         self.camera.grid_count = None
-        self.session.save_camera(self.port)
-        self.cal_output.setText("Need to collect data....")
+        self.session.config.save_camera(self.camera)
+        # self.camera_summary.place_widgets()
+        self.update_camera_data()
         self.undistort_btn.setEnabled(False)
-       
+
     def calibrate(self):
+        def wrker():
+            self.start_stop_calibration_btn.setText("---processing---")
+            self.start_stop_calibration_btn.setEnabled(False)
+
+            self.monocal.calibrate()
+            self.session.config.save_camera(self.camera)
+            self.calibration_change.emit()
 
-            def wrker():
-                self.start_stop_calibration_btn.setText("---processing---")
-                self.start_stop_calibration_btn.setEnabled(False)
-
-                self.monocal.calibrate()
-                self.cal_output.setText(self.monocal.camera.calibration_summary())
-                self.session.save_camera(self.port)
-
-                # signal to camera tabs to check on total session calibration status
-                self.calibration_change.emit() 
-
-                self.undistort_btn.setEnabled(True)
-                self.start_stop_calibration_btn.setText("Re-Collect")
-                self.start_stop_calibration_btn.setEnabled(True)
-                self.signal_calibration_lock.emit(False)
+            self.undistort_btn.setEnabled(True)
+            self.start_stop_calibration_btn.setText("Re-&Collect")
+            self.start_stop_calibration_btn.setEnabled(True)
+            self.signal_calibration_lock.emit(False)
 
-            self.calib_thread = Thread(target=wrker, args=(), daemon=True)
-            self.calib_thread.start()
+        self.calib_thread = Thread(target=wrker, args=(), daemon=True)
+        self.calib_thread.start()
 
     def undistort(self):
-        def undistort_worker():
-            # create thread for timer to play out
+        if self.undistort_btn.text() == "Un&distort":
             self.signal_calibration_lock.emit(True)
             self.start_stop_calibration_btn.setEnabled(False)
-            self.undistort_btn.setEnabled(False)
             self.frame_emitter.undistort = True
-            for i in range(5,0,-1):
-                self.undistort_btn.setText(f"Reverting in {i}")
-                time.sleep(1)
-            self.undistort_btn.setEnabled(True)
+            self.undistort_btn.setText("Revert &Distortion")
+
+        elif self.undistort_btn.text() == "Revert &Distortion":
             self.start_stop_calibration_btn.setEnabled(True)
-                    
             self.frame_emitter.undistort = False
-            self.undistort_btn.setText("Undistort")
+            self.undistort_btn.setText("Un&distort")
             self.signal_calibration_lock.emit(False)
-            
-        undistort_thread = Thread(target=undistort_worker,args=(),daemon=True)
-        undistort_thread.start()
 
-        
+    def update_camera_data(self):
+        self.layout().removeWidget(self.camera_summary)
+        self.camera_summary.deleteLater()
+        self.camera_summary = None
+        self.camera_summary = SummaryWidget(self.camera)
+        self.layout().addWidget(self.camera_summary)
+
+
 class AdvancedControls(QWidget):
-    def __init__(self,session:Session, port, frame_emitter:FrameEmitter):
+    def __init__(self, session: Session, port, frame_emitter: FrameEmitter):
         super(AdvancedControls, self).__init__()
         self.session: Session = session
         self.port = port
         self.monocal: MonoCalibrator = self.session.monocalibrators[port]
         self.stream: LiveStream = self.monocal.stream
         self.camera: Camera = self.stream.camera
         self.frame_emitter = frame_emitter
-        self.setLayout(QHBoxLayout())        
+        self.setLayout(QHBoxLayout())
 
         self.place_widgets()
         self.connect_widgets()
-        
-    def place_widgets(self):        
 
+    def place_widgets(self):
         self.fps_grp = QGroupBox("FPS")
         self.layout().addWidget(self.fps_grp)
         self.fps_grp.setLayout(QHBoxLayout())
 
         logger.debug("Building FPS Control")
         self.fps_grp.layout().addWidget(QLabel("Target:"))
 
         self.frame_rate_spin = QSpinBox()
         self.frame_rate_spin.setValue(self.stream.fps)
         self.fps_grp.layout().addWidget(self.frame_rate_spin)
 
         self.fps_display = QLabel()
-        # self.fps_display.setAlignment(Qt.AlignmentFlag.AlignHCenter)
         self.fps_grp.layout().addWidget(self.fps_display)
         self.grid_grp = QGroupBox("Grid Collection")
         self.layout().addWidget(self.grid_grp)
         self.grid_grp.setLayout(QHBoxLayout())
 
         self.grid_grp.layout().addWidget(QLabel("Wait Time:"))
 
         self.wait_time_spin = QDoubleSpinBox()
         self.wait_time_spin.setValue(self.monocal.wait_time)
         self.wait_time_spin.setSingleStep(0.1)
 
         self.wait_time_spin.valueChanged.connect(self.on_wait_time_spin)
         self.grid_grp.layout().addWidget(self.wait_time_spin)
 
-        logger.debug("Building Grid Count Display")
-        self.grid_count_display = QLabel()
-        self.grid_grp.layout().addWidget(self.grid_count_display)
-        self.grid_count_display.setAlignment(Qt.AlignmentFlag.AlignHCenter)
-
-        def grid_count_update_slot(grid_count):
-            self.grid_count_display.setText(f"Count: {grid_count}")
-        # self.frame_emitter.FPSBroadcast.connect(FPSUpdateSlot)
+        self.ignore_box = QCheckBox("Ignore", self)
+        self.layout().addWidget(self.ignore_box)
 
     def connect_widgets(self):
         self.frame_rate_spin.valueChanged.connect(self.on_frame_rate_spin)
-        
-        
+
         def FPSUpdateSlot(fps):
             if self.monocal.camera.capture.isOpened():
                 # rounding to nearest integer should be close enough for our purposes
                 self.fps_display.setText("Actual: " + str(round(fps, 1)))
             else:
                 self.fps_display.setText("reconnecting to camera...")
 
         self.frame_emitter.FPSBroadcast.connect(FPSUpdateSlot)
-        
+        self.ignore_box.stateChanged.connect(self.ignore_cam)
+
+    def ignore_cam(self, signal):
+        if signal == 0:  # not checked
+            logger.info(f"Don't ignore camera at port {self.port}")
+            self.camera.ignore = False
+        else:  # value of checkState() might be 2?
+            logger.info(f"Ignore camera at port {self.port}")
+            self.camera.ignore = True
+        self.session.config.save_camera(self.camera)
+
     def on_wait_time_spin(self, wait_time):
-        self.monocal.wait_time = wait_time
+        self.session.wait_time_intrinsic = wait_time
+        self.session.config.save_intrinsic_wait_time(wait_time)
 
-        
-    def on_frame_rate_spin(self,fps_rate):
-        self.stream.set_fps_target(fps_rate)
+    def on_frame_rate_spin(self, fps_rate):
+        self.session.set_active_mode_fps(fps_rate)
         logger.info(f"Changing monocalibrator frame rate for port{self.port}")
 
-    def FPSUpdateSlot(self,fps):
+    def FPSUpdateSlot(self, fps):
         if self.monocal.camera.capture.isOpened():
             # rounding to nearest integer should be close enough for our purposes
             self.fps_display.setText("Actual: " + str(round(fps, 1)))
         else:
             self.fps_display.setText("reconnecting to camera...")
 
+
 class FrameControlWidget(QWidget):
-    def __init__(self, session: Session, port, frame_emitter:FrameEmitter):
+    def __init__(self, session: Session, port, frame_emitter: FrameEmitter):
         super(FrameControlWidget, self).__init__()
-        self.session:Session = session
-        self.monocal:MonoCalibrator  = session.monocalibrators[port]
+        self.session: Session = session
+        self.monocal: MonoCalibrator = session.monocalibrators[port]
         self.port = port
         self.camera: Camera = self.monocal.stream.camera
         self.frame_emitter = frame_emitter
-       
+
         self.place_widgets()
         self.connect_widgets()
-         
-    def place_widgets(self):
 
+    def place_widgets(self):
         self.setLayout(QVBoxLayout())
         ###### FRAME ####################################
         # return a QLabel that is linked to the constantly changing image
         self.frame_display = QLabel()
         self.layout().addWidget(self.frame_display)
 
-        # self.build_ignore_checkbox()
-
         self.rotation_resolution_hbox = QHBoxLayout()
         self.layout().addLayout(self.rotation_resolution_hbox)
-        ###################### Rotation Buttons  ###################################      
+        ###################### Rotation Buttons  ###################################
         # icons from https://iconoir.com
         self.cw_rotation_btn = QPushButton(
             QIcon(str(Path(__root__, "pyxy3d/gui/icons/rotate-camera-right.svg"))), ""
         )
-        self.cw_rotation_btn.setMaximumSize(35,35)
+        self.cw_rotation_btn.setMaximumSize(35, 35)
         self.ccw_rotation_btn = QPushButton(
             QIcon(str(Path(__root__, "pyxy3d/gui/icons/rotate-camera-left.svg"))), ""
         )
 
-        self.ccw_rotation_btn.setMaximumSize(35,35)
+        self.ccw_rotation_btn.setMaximumSize(35, 35)
         self.rotation_resolution_hbox.addWidget(self.cw_rotation_btn)
         self.rotation_resolution_hbox.addWidget(self.ccw_rotation_btn)
 
         ##################### RESOLUTION DROP DOWN ##############################
         self.resolution_combo = QComboBox()
 
         resolutions_text = []
@@ -357,143 +359,92 @@
             resolutions_text.append(f"{int(w)} x {int(h)}")
 
         self.resolution_combo.addItems(resolutions_text)
         self.resolution_combo.setMaximumSize(100, 35)
 
         w, h = self.monocal.camera.size
         self.resolution_combo.setCurrentText(f"{int(w)} x {int(h)}")
-    
-        self.rotation_resolution_hbox.addWidget(self.resolution_combo)    
+
+        self.rotation_resolution_hbox.addWidget(self.resolution_combo)
 
         ######################## EXPOSURE BOX #############################
-        
+
         self.exposure_hbox = QHBoxLayout()
         self.layout().addLayout(self.exposure_hbox)
-    
+
         # construct a horizontal widget with label: slider: value display
         self.exposure_label = QLabel("Exposure")
         self.exposure_label.setAlignment(Qt.AlignmentFlag.AlignRight)
 
         self.exp_slider = QSlider(Qt.Orientation.Horizontal)
         self.exp_slider.setRange(-10, 0)
         self.exp_slider.setSliderPosition(int(self.monocal.camera.exposure))
         self.exp_slider.setPageStep(1)
         self.exp_slider.setSingleStep(1)
         self.exp_slider.setMaximumWidth(200)
         self.exposure_number = QLabel()
         self.exposure_number.setText(str(int(self.monocal.camera.exposure)))
 
-
         self.exposure_hbox.addWidget(self.exposure_label)
         self.exposure_hbox.addWidget(self.exp_slider)
         self.exposure_hbox.addWidget(self.exposure_number)
 
         self.exposure_hbox.setAlignment(Qt.AlignmentFlag.AlignCenter)
-    
-        self.ignore_box = QCheckBox("Ignore", self)
-        self.layout().addWidget(self.ignore_box)
 
     def connect_widgets(self):
         def ImageUpdateSlot(QPixmap):
             self.frame_display.setPixmap(QPixmap)
 
         self.frame_emitter.ImageBroadcast.connect(ImageUpdateSlot)
 
         # Counter Clockwise rotation called because the display image is flipped
         self.cw_rotation_btn.clicked.connect(self.monocal.camera.rotate_CCW)
         self.cw_rotation_btn.clicked.connect(self.save_camera)
 
         # Clockwise rotation called because the display image is flipped
         self.ccw_rotation_btn.clicked.connect(self.monocal.camera.rotate_CW)
         self.ccw_rotation_btn.clicked.connect(self.save_camera)
-        
+
         # resolution combo box
         self.resolution_combo.currentTextChanged.connect(self.change_resolution)
 
-        # exposure slider 
+        # exposure slider
         self.exp_slider.valueChanged.connect(self.update_exposure)
-        self.ignore_box.stateChanged.connect(self.ignore_cam)
+        # self.ignore_box.stateChanged.connect(self.ignore_cam)
+
+    def save_camera(self):
+        # normally wouldn't bother with a one-liner function, but it makes connecting
+        # to the signal more straightforward
+        self.session.config.save_camera(self.camera)
 
-    def ignore_cam(self,signal):
-        if signal == 0:  # not checked
-            logger.info(f"Don't ignore camera at port {self.port}")
-            self.camera.ignore = False
-        else:  # value of checkState() might be 2?
-            logger.info(f"Ignore camera at port {self.port}")
-            self.camera.ignore = True
-        self.save_camera()
 
     def update_exposure(self, exp):
         self.monocal.camera.exposure = exp
         self.exposure_number.setText(str(exp))
         self.save_camera()
 
     def change_resolution(self, res_text):
         # call the cam_cap widget to change the resolution, but do it in a
         # thread so that it doesn't halt your progress
 
         w, h = res_text.split("x")
         w, h = int(w), int(h)
         new_res = (w, h)
-        # self.cam_cap.change_resolution(new_res)
-        logger.info(
-            f"Attempting to change resolution of camera at port {self.port}"
-        )
+        logger.info(f"Attempting to change resolution of camera at port {self.port}")
 
         def change_res_worker(new_res):
             self.monocal.stream.change_resolution(new_res)
-            
+
             # clear out now irrelevant params
-            self.camera.matrix=None
-            self.camera.distortions=None
-            self.camera.error=None
-            self.camera.grid_count=None
+            self.camera.matrix = None
+            self.camera.distortions = None
+            self.camera.error = None
+            self.camera.grid_count = None
             self.save_camera()
 
-
         self.change_res_thread = Thread(
             target=change_res_worker,
             args=(new_res,),
             daemon=True,
         )
         self.change_res_thread.start()
 
-    def save_camera(self):
-        self.session.save_camera(self.port)
-
-
-if __name__ == "__main__":
-    App = QApplication(sys.argv)
-    from pyxy3d import __root__
-    config_path = Path(__root__, "tests", "why breaking")
-
-    print(config_path)
-    session = Session(config_path)
-    session.load_cameras()
-    session.load_streams()
-    # session.adjust_resolutions()
-    session.load_monocalibrators()
-
-    test_port = 0
-
-    logger.info("Creating Camera Config Dialog")
-    cam_dialog = CameraConfigDialog(session, test_port)
-    cam_dialog.show()
-    
-    # frame_control = FrameControlWidget(session, test_port)
-    # frame_control.show()
-
-    # adv_control = AdvancedControls(session, test_port)
-    # adv_control.show()
-
-    # DISPLAY_WIDTH = App.primaryScreen().size().width()
-    # DISPLAY_HEIGHT = App.primaryScreen().size().height()
-
-    # pixmap_edge = min(DISPLAY_WIDTH / 3, DISPLAY_HEIGHT / 3)
-    # frame_emitter = FrameEmitter(session.monocalibrators[test_port], pixmap_edge)
-    
-    # frame_emitter.start()
-    # cal_controls = CalibrationControls(session, test_port,frame_emitter)
-    # cal_controls.show()
-    logger.info("About to show camera config dialog")
-
-    sys.exit(App.exec())
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/camera_config/camera_tabs.py` & `pyxy3d-0.0.19/pyxy3d/gui/camera_config/intrinsic_calibration_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,60 +1,82 @@
 
 import pyxy3d.logger
 logger = pyxy3d.logger.get(__name__)
 
 import sys
 from pathlib import Path
 
-from PyQt6.QtCore import pyqtSignal
+from PyQt6.QtCore import pyqtSignal, Qt
 from PyQt6.QtWidgets import (
     QApplication,
     QVBoxLayout,
     QWidget,
     QTabWidget,
 )
 
-from pyxy3d.gui.camera_config.camera_config_dialogue import CameraConfigDialog
-from pyxy3d.session import Session, Stage
-from pyxy3d.gui.widgets import NavigationBarBackNext
-
-class CameraWizard(QWidget):
-    def __init__(self, session):
-        super(CameraWizard, self).__init__()
+from pyxy3d.gui.camera_config.camera_config_dialogue import CameraConfigTab
+from pyxy3d.session.session import Session
+from pyxy3d.gui.navigation_bars import NavigationBarBackNext
+
+class IntrinsicCalibrationWidget(QWidget):
+    """ 
+    This is basically just the camera tabs plus the navigation bar
+    """
+    def __init__(self, session: Session):
+        super(IntrinsicCalibrationWidget, self).__init__()
         self.setLayout(QVBoxLayout())    
         self.camera_tabs = CameraTabs(session)
-        self.navigation_bar = NavigationBarBackNext()
         self.layout().addWidget(self.camera_tabs)
-        self.layout().addWidget(self.navigation_bar)
     
-        self.camera_tabs.stereoframe_ready.connect(self.set_next_enabled)
-        self.camera_tabs.check_session_calibration()
-         
-    def set_next_enabled(self, stereoframe_ready:bool):
-        logger.info(f"Setting camera tab next button enabled status to {stereoframe_ready}")
-        self.navigation_bar.next_btn.setEnabled(stereoframe_ready)
+        self.session = session
             
 class CameraTabs(QTabWidget):
     
     stereoframe_ready = pyqtSignal(bool)
 
     def __init__(self, session: Session):
         super(CameraTabs, self).__init__()
         self.session = session
 
         self.setTabPosition(QTabWidget.TabPosition.North)
         self.add_cam_tabs()
-        self.currentChanged.connect(self.toggle_tracking)
+        # self.session.set_mode(SessionMode.IntrinsicCalibration)
+        self.currentChanged.connect(self.activate_current_tab)
+        self.session.active_monocalibrator = self.currentWidget().stream.port
+        self.session.activate_monocalibrator()
+
+    def keyPressEvent(self, event):
+        """
+        Override the keyPressEvent method to allow navigation via PgUp/PgDown
+        """
+
+        if event.key() == Qt.Key.Key_PageUp:
+            current_index = self.currentIndex()
+            if current_index > 0:
+                self.setCurrentIndex(current_index - 1)
+        elif event.key() == Qt.Key.Key_PageDown:
+            current_index = self.currentIndex()
+            if current_index < self.count() - 1:
+                self.setCurrentIndex(current_index + 1)
+        else:
+            super().keyPressEvent(event)
         
         
-    def toggle_tracking(self, index):
+    def activate_current_tab(self, index):
 
         logger.info(f"Toggle tracking to activate {self.tabText(index)}")
-        self.session.set_active_monocalibrator(self.widget(index).stream.port)
+        self.session.pause_all_monocalibrators()
+        self.session.activate_monocalibrator(self.widget(index).stream.port)
+
+        # this is where you can update the spin boxes to align with the session values
+        monocal_fps = self.session.get_active_mode_fps()
+        self.widget(index).advanced_controls.frame_rate_spin.setValue(monocal_fps)
 
+        wait_time_intrinsic = self.session.wait_time_intrinsic
+        self.widget(index).advanced_controls.wait_time_spin.setValue(wait_time_intrinsic)
 
     def add_cam_tabs(self):
         tab_names = [self.tabText(i) for i in range(self.count())]
         logger.info(f"Current tabs are: {tab_names}")
 
         if len(self.session.monocalibrators) > 0:
             
@@ -62,64 +84,19 @@
             tab_widgets = {}
             for port, monocal in self.session.monocalibrators.items():
                 tab_name = f"Camera {port}"
                 logger.info(f"Potentially adding {tab_name}")
                 if tab_name in tab_names:
                     pass  # already here, don't bother
                 else:
-                    cam_tab = CameraConfigDialog(self.session, port)
-                    
-                    # when new camera calibrated, check to see if all cameras calibrated
-                    cam_tab.calibrate_grp.calibration_change.connect(self.check_session_calibration)
-
+                    cam_tab = CameraConfigTab(self.session, port)
                     tab_widgets[port] = cam_tab
 
             # add the widgets to the tab bar in order
             ordered_ports = list(tab_widgets.keys())
             ordered_ports.sort()
             for port in ordered_ports:
                 self.insertTab(port, tab_widgets[port], f"Camera {port}")
             
-            # session may be pre-calibrated and ready to proceed...or not
-            self.check_session_calibration()
-            
         else:
             logger.info("No cameras available")
-        
-        self.toggle_tracking(self.currentIndex())
-
-    def check_session_calibration(self):
-        logger.info(f"Checking session stage....")
-      
-        if self.session.get_stage() == Stage.MONOCALIBRATED_CAMERAS:
-            logger.info("Ready for stereoframe")
-            self.stereoframe_ready.emit(True)       
-        elif self.session.get_stage() == Stage.UNCALIBRATED_CAMERAS:
-            logger.info("Not ready for stereoframe")
-            self.stereoframe_ready.emit(False)
-            
-if __name__ == "__main__":
-    from pyxy3d import __root__
-    
-    App = QApplication(sys.argv)
-
-    
-    config_path = Path(__root__, "tests", "laptop")
-    # config_path = Path(__root__, "tests", "pyxy3d")
-    # config_path = Path(repo, "sessions", "high_res_session")
-    print(config_path)
-    session = Session(config_path)
-    session.load_cameras()
-    session.load_streams()
-    # session.adjust_resolutions()
-    session.load_monocalibrators()
-
-    test_port = 0
-
-    # cam_dialog = CameraConfigDialog(session, test_port)
-    # cam_tabs = CameraTabs(session)
-    # cam_tabs.show()
-    cam_wizard = CameraWizard(session)
-    cam_wizard.show()
-
-    sys.exit(App.exec())
-
+
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/camera_config/frame_emitter.py` & `pyxy3d-0.0.19/pyxy3d/gui/camera_config/frame_emitter.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
         while self.ThreadActive:
             # Grab a frame from the queue and broadcast to displays
             self.monocalibrator.grid_frame_ready_q.get()
 
             self.frame = self.monocalibrator.grid_frame
             self.apply_undistortion()
+            self.frame = resize_to_square(self.frame)
             self.apply_rotation()
 
             image = self.cv2_to_qlabel(self.frame)
             pixmap = QPixmap.fromImage(image)
 
             if self.pixmap_edge_length:
                 pixmap = pixmap.scaled(
@@ -86,11 +87,34 @@
             self.frame = cv2.undistort(
                 self.frame,
                 self.monocalibrator.camera.matrix,
                 self.monocalibrator.camera.distortions,
             )
 
 
+def resize_to_square(frame):
+
+    height = frame.shape[0]
+    width = frame.shape[1]
+
+    padded_size = max(height, width)
+
+    height_pad = int((padded_size - height) / 2)
+    width_pad = int((padded_size - width) / 2)
+    pad_color = [0, 0, 0]
+
+    frame = cv2.copyMakeBorder(
+        frame,
+        height_pad,
+        height_pad,
+        width_pad,
+        width_pad,
+        cv2.BORDER_CONSTANT,
+        value=pad_color,
+    )
+
+    return frame
+
 if __name__ == "__main__":
     pass
 
     # not much to look at here... go to camera_config_dialogue.py for test
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/icons/pyxy_logo.svg` & `pyxy3d-0.0.19/pyxy3d/gui/icons/pyxy_logo.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/icons/rotate-camera-left.svg` & `pyxy3d-0.0.19/pyxy3d/gui/icons/rotate-camera-left.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/icons/rotate-camera-right.svg` & `pyxy3d-0.0.19/pyxy3d/gui/icons/rotate-camera-right.svg`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/qt_logger.py` & `pyxy3d-0.0.19/pyxy3d/gui/log_widget.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,69 +1,80 @@
+import logging
+from pyxy3d.logger import get, XStream
+logger = get(__name__)
+
 import sys
 from PyQt6.QtCore import pyqtSlot, Qt
-from PyQt6.QtWidgets import QDialog, QApplication, QTextBrowser, QPushButton, QVBoxLayout
-import logging
+from PyQt6.QtWidgets import (
+    QWidget,
+    QDialog,
+    QApplication,
+    QTextBrowser,
+    QPushButton,
+    QVBoxLayout,
+)
 
-from pyxy3d.session import Session
+from pyxy3d.session.session import Session
 from pathlib import Path
-from threading  import Thread
+from threading import Thread
+
+# def test():
+#     def worker():
+#         session = Session(Path(r"C:\Users\Mac Prible\repos\pyxy3d\tests\217"))
+#         session.find_cameras()
+#     thread = Thread(target=worker, args=(), daemon=True)
+#     thread.start()
 
-def test():
-    def worker():
-        session = Session(Path(r"C:\Users\Mac Prible\repos\pyxy3d\tests\217"))
-        session.find_cameras()
-    thread = Thread(target=worker, args=(), daemon=True)
-    thread.start()
 
-from pyxy3d.logger import get, XStream
-logger = get(__name__)
 
-class QtLogger(QDialog):
-    def __init__( self, message:str = None):
-        super(QtLogger, self).__init__()
+class LogWidget(QWidget):
+    def __init__(self, message: str = None):
+        super(LogWidget, self).__init__()
         self.setWindowTitle(message)
         self._console = LogMessageViewer(self)
 
         self.setWindowFlags(Qt.WindowType.WindowTitleHint)
 
         layout = QVBoxLayout()
 
         layout.addWidget(self._console)
-        
-        if __name__ == "__main__":
-            self._button  = QPushButton(self)
-            self._button.setText('Test Me')
-            layout.addWidget(self._button)
-            self._button.clicked.connect(test)
+
+        # if __name__ == "__main__":
+        #     self._button = QPushButton(self)
+        #     self._button.setText("Test Me")
+        #     layout.addWidget(self._button)
+        #     self._button.clicked.connect(test)
 
         self.setLayout(layout)
-        XStream.stdout().messageWritten.connect( self._console.appendLogMessage)
-        XStream.stderr().messageWritten.connect( self._console.appendLogMessage)
+        XStream.stdout().messageWritten.connect(self._console.appendLogMessage)
+        XStream.stderr().messageWritten.connect(self._console.appendLogMessage)
 
 
 class LogMessageViewer(QTextBrowser):
-
     def __init__(self, parent=None):
-        super(LogMessageViewer,self).__init__(parent)
+        super(LogMessageViewer, self).__init__(parent)
         self.setReadOnly(True)
-        #self.setLineWrapMode(QtGui.QTextEdit.NoWrap)
-        self.setEnabled(False)
-        self.verticalScrollBar().setVisible(False)
+        # self.setLineWrapMode(QtGui.QTextEdit.NoWrap)
+        self.setEnabled(True)
+        self.verticalScrollBar().setVisible(True)
 
     @pyqtSlot(str)
     def appendLogMessage(self, msg):
         horScrollBar = self.horizontalScrollBar()
         verScrollBar = self.verticalScrollBar()
-        scrollIsAtEnd = verScrollBar.maximum() - verScrollBar.value() <= 10
+        # scrollIsAtEnd = verScrollBar.maximum() - verScrollBar.value() <= 10
 
+        verScrollBar.setValue(verScrollBar.maximum())  # Scrolls to the bottom
+        horScrollBar.setValue(0)  # scroll to the left  
         self.insertPlainText(msg)
 
-        if scrollIsAtEnd:
-            verScrollBar.setValue(verScrollBar.maximum()) # Scrolls to the bottom
-            horScrollBar.setValue(0) # scroll to the left
-    
-if __name__ == '__main__':
+        # if scrollIsAtEnd:
+        #     verScrollBar.setValue(verScrollBar.maximum())  # Scrolls to the bottom
+        #     self.insertPlainText(msg)
+        #     horScrollBar.setValue(0)  # scroll to the left  
+
+if __name__ == "__main__":
     app = QApplication([])
-    dlg = QtLogger("This is only a test")
+    dlg = LogWidget("This is only a test")
     dlg.show()
-        
-    app.exec()
+
+    app.exec()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/recording_widget.py` & `pyxy3d-0.0.19/pyxy3d/gui/recording_widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,116 +4,191 @@
 logger = pyxy3d.logger.get(__name__)
 
 import sys
 import math
 from pathlib import Path
 from threading import Thread, Event
 import numpy as np
-import time
 from queue import Queue
+from enum import Enum
 
 import cv2
 from PyQt6.QtCore import Qt, pyqtSignal, QThread
 from PyQt6.QtGui import QImage, QPixmap, QIcon
 from PyQt6.QtWidgets import (
     QApplication,
     QSizePolicy,
     QWidget,
     QSpinBox,
     QScrollArea,
     QComboBox,
     QCheckBox,
+    QTextEdit,
+    QLineEdit,
     QDialog,
     QGroupBox,
     QDoubleSpinBox,
     QHBoxLayout,
     QLabel,
     QPushButton,
     QSlider,
     QVBoxLayout,
 )
 
-from pyxy3d.session import Session
-from pyxy3d.gui.stereoframe.stereo_frame_builder import StereoFrameBuilder
+from pyxy3d.session.session import Session
 from pyxy3d.cameras.synchronizer import Synchronizer
 from pyxy3d import __root__
-from pyxy3d.gui.qt_logger import QtLogger
-from pyxy3d.gui.widgets import NavigationBarBackFinish
-
+from pyxy3d.recording.video_recorder import VideoRecorder
+from pyxy3d.configurator import Configurator
 
+class NextRecordingActions(Enum):
+    StartRecording = "Start Recording"
+    StopRecording = "Stop Recording"
+    AwaitSave = "--Saving Frames--"
+    
+ 
 class RecordingWidget(QWidget):
      
     def __init__(self,session:Session):
 
         super(RecordingWidget, self).__init__()
         self.session = session
-        self.synchronizer:Synchronizer = self.session.get_synchronizer()
+        self.synchronizer:Synchronizer = self.session.synchronizer
         
         # don't let point tracking slow down the frame reading
-        self.synchronizer.set_tracking_on_streams(False)
+        # self.synchronizer.set_tracking_on_streams(False)
+
         # create tools to build and emit the displayed frame
-        self.frame_builder = RecordingFrameBuilder(self.synchronizer)
-        self.frame_emitter = RecordingFrameEmitter(self.frame_builder)
+        self.frame_builder = UnpairedFrameBuilder(self.synchronizer)
+        self.frame_emitter = UnpairedFrameEmitter(self.frame_builder)
         self.frame_emitter.start()
 
+        self.video_recorder = VideoRecorder(self.synchronizer)
+        
         self.frame_rate_spin = QSpinBox()
-        self.frame_rate_spin.setValue(self.synchronizer.get_fps_target())
+        self.frame_rate_spin.setValue(self.session.fps_recording)
 
+        self.next_action = NextRecordingActions.StartRecording
+        self.start_stop = QPushButton(self.next_action.value)
+        self.destination_label = QLabel("Recording Destination:")
+        self.recording_directory = QLineEdit(self.get_next_recording_directory())
+        
         self.dropped_fps_label = QLabel()
                 
         self.recording_frame_display = QLabel()
         
         self.place_widgets()
         self.connect_widgets()        
+        self.update_btn_eligibility()
+    
+    def update_btn_eligibility(self):
+        if self.session.is_recording_eligible():
+            self.start_stop.setEnabled(True)
+        else:
+            self.start_stop.setEnabled(False)
+            
+
+    def get_next_recording_directory(self):
 
+        folders = [item.name for item in self.session.path.iterdir() if item.is_dir()]
+        recording_folders = [folder for folder in folders if folder.startswith("recording_")]
+        recording_counts = [folder.split("_")[1] for folder in recording_folders]
+        recording_counts = [int(rec_count) for rec_count in recording_counts if rec_count.isnumeric()]
+
+        if len(recording_counts) == 0:
+            next_directory = "recording_1"
+        
+        else:
+            next_directory = "recording_" + str(max(recording_counts)+1)
+       
+        return next_directory 
+        
+        
 
     def place_widgets(self):
         self.setLayout(QVBoxLayout())
         self.settings_group = QGroupBox("Settings")
         self.settings_group.setLayout(QHBoxLayout())
         self.settings_group.layout().addWidget(QLabel("Frame Rate:"))
         self.settings_group.layout().addWidget(self.frame_rate_spin)       
         self.layout().addWidget(self.settings_group)
+
+        self.record_controls = QGroupBox()
+        self.record_controls.setLayout(QHBoxLayout())
+        self.record_controls.layout().addWidget(self.start_stop)
+        self.record_controls.layout().addWidget(self.destination_label)
+        self.record_controls.layout().addWidget(self.recording_directory)
+
+        self.layout().addWidget(self.record_controls)
         self.layout().addWidget(self.dropped_fps_label)
 
         self.layout().addWidget(self.recording_frame_display)
 
 
     def connect_widgets(self):
     
         self.frame_emitter.ImageBroadcast.connect(self.ImageUpdateSlot)
-        self.frame_rate_spin.valueChanged.connect(self.synchronizer.set_fps_target)
+        self.frame_rate_spin.valueChanged.connect(self.session.set_active_mode_fps)
         self.frame_emitter.dropped_fps.connect(self.update_dropped_fps)
-        
+        self.start_stop.clicked.connect(self.toggle_start_stop)
+        self.session.recording_complete_signal.connect(self.on_recording_complete)
+
+    def toggle_start_stop(self):
+        if self.next_action == NextRecordingActions.StartRecording:
+            self.next_action = NextRecordingActions.StopRecording
+            self.start_stop.setText(self.next_action.value)
+            self.recording_directory.setEnabled(False)
+
+            logger.info("Initiate recording")
+            recording_path:Path = Path(self.session.path, self.recording_directory.text()) 
+            self.session.start_recording(recording_path)
+
+        elif self.next_action == NextRecordingActions.StopRecording:
+            self.start_stop.setEnabled(False)
+            # need to wait for session to signal that recording is complete
+            self.next_action = NextRecordingActions.AwaitSave
+            # self.start_stop.setText("HELLO")
+            self.start_stop.setText(self.next_action.value)
+            self.session.stop_recording()
+
+            self.recording_directory.setEnabled(True)
+            logger.info("Stop recording and initiate final save of file") 
+            self.recording_directory.setText(self.get_next_recording_directory())
+
+    def on_recording_complete(self):
+        logger.info("Recording complete signal received...updating next action and button")
+        self.next_action = NextRecordingActions.StartRecording
+        self.start_stop.setText(self.next_action.value)
+        self.start_stop.setEnabled(True)
+        logger.info("Enabling start/stop recording button")
+                    
     def update_dropped_fps(self, dropped_fps:dict):
         "Unravel dropped fps dictionary to a more readable string"
         text = "Rate of Frame Dropping by Port:    "
-        
-        
         for port, drop_rate in dropped_fps.items():
             text += f"{port}: {drop_rate:.0%}        "
 
         self.dropped_fps_label.setText(text)
          
         
     def ImageUpdateSlot(self, q_image):
         self.recording_frame_display.resize(self.recording_frame_display.sizeHint())
         qpixmap = QPixmap.fromImage(q_image)
         self.recording_frame_display.setPixmap(qpixmap)
         
-class RecordingFrameBuilder:
+class UnpairedFrameBuilder:
     def __init__(self, synchronizer: Synchronizer, single_frame_height=250):
         self.synchronizer = synchronizer 
         self.single_frame_height = single_frame_height
 
-        self.rotation_counts = {}
+        # self.rotation_counts = {}
         self.ports = []        
         for port, stream in self.synchronizer.streams.items():
             # override here while testing this out with pre-recorded video
-            self.rotation_counts[port] = stream.camera.rotation_count
+            # self.rotation_counts[port] = stream.camera.rotation_count
             self.ports.append(port)
         self.ports.sort()
         
         # reasonable default for the shape of the all-cameras frame
         # make it as square as you can get it
         camera_count = len(self.ports)
         self.frame_columns = int(math.ceil(camera_count**.5))
@@ -143,15 +218,15 @@
 
 
     def resize_to_square(self, frame):
         """To make sure that frames align well, scale them all to thumbnails
         squares with black borders."""
         logger.debug("resizing square")
 
-        frame = cv2.flip(frame, 1)
+        # frame = cv2.flip(frame, 1)
 
         height = frame.shape[0]
         width = frame.shape[1]
 
         padded_size = max(height, width)
 
         height_pad = int((padded_size - height) / 2)
@@ -170,15 +245,16 @@
         )
 
         frame = resize(frame, new_height=self.single_frame_height)
         return frame
 
 
     def apply_rotation(self, frame, port):
-        rotation_count = self.rotation_counts[port]
+        # rotation_count = self.rotation_counts[port]
+        rotation_count = self.synchronizer.streams[port].camera.rotation_count
         if rotation_count == 0:
             pass
         elif rotation_count in [1, -3]:
             frame = cv2.rotate(frame, cv2.ROTATE_90_CLOCKWISE)
         elif rotation_count in [2, -2]:
             frame = cv2.rotate(frame, cv2.ROTATE_180)
         elif rotation_count in [-1, 3]:
@@ -200,19 +276,20 @@
         
         thumbnail_frames = {} 
         for port in self.ports:
             frame_packet = self.current_sync_packet.frame_packets[port]
             raw_frame = self.get_frame_or_blank(frame_packet)
             square_frame = self.resize_to_square(raw_frame)
             rotated_frame = self.apply_rotation(square_frame,port)
+            flipped_frame = cv2.flip(rotated_frame, 1)
             
             # put the port number on the top of the frame
-            text_frame = cv2.putText(rotated_frame,
+            text_frame = cv2.putText(flipped_frame,
                                 str(port),
-                                (int(rotated_frame.shape[1]/2), int(self.single_frame_height / 4)),
+                                (int(flipped_frame.shape[1]/2), int(self.single_frame_height / 4)),
                                 fontFace=cv2.FONT_HERSHEY_SIMPLEX,
                                 fontScale=1,
                                 color=(0, 0, 255),
                                 thickness=2,
                             )
             
             thumbnail_frames[port] = text_frame
@@ -248,22 +325,22 @@
                 mega_frame = row
             else:
                 mega_frame = np.vstack([mega_frame,row]) 
                          
          
         return mega_frame
 
-class RecordingFrameEmitter(QThread):
+class UnpairedFrameEmitter(QThread):
     ImageBroadcast = pyqtSignal(QImage)
     dropped_fps = pyqtSignal(dict)
     
-    def __init__(self, recording_frame_builder:RecordingFrameBuilder):
+    def __init__(self, unpaired_frame_builder:UnpairedFrameBuilder):
         
-        super(RecordingFrameEmitter,self).__init__()
-        self.recording_frame_builder = recording_frame_builder
+        super(UnpairedFrameEmitter,self).__init__()
+        self.recording_frame_builder = unpaired_frame_builder
         logger.info("Initiated recording frame emitter")        
         self.keep_collecting = Event() 
         
     def run(self):
 
         self.keep_collecting.set()
         
@@ -293,61 +370,28 @@
     resized = cv2.resize(image, dim, interpolation=cv2.INTER_AREA)
     return resized
         
         
         
 def cv2_to_qlabel(frame):
     image = cv2.cvtColor(frame, cv2.COLOR_BGR2RGB)
-
+    
     qt_frame = QImage(
         image.data,
         image.shape[1],
         image.shape[0],
         QImage.Format.Format_RGB888,
     )
     return qt_frame
 
-# Trying to get away from these F5 tests and move toward working scripts in /dev that can 
-# more easily be reconfigured into /tests  
-# if __name__ == "__main__":
-        # App = QApplication(sys.argv)
-
-        # session_path = Path(__root__, "dev", "sample_sessions", "post_optimization")
-
-        # session = Session(session_path)
-        # session.load_cameras()
-        # session.load_streams()
-        
-        # toggle off tracking for max frame rate
-        # for port, stream in session.streams.items():
-        #     stream.track_points.clear()
-            
-        # session.adjust_resolutions()
-        # syncr = Synchronizer(session.streams, fps_target=24)
-
-        # frame_builder = RecordingFrameBuilder(syncr)
-        
-        # while True:
-        #     recording_frame = frame_builder.get_recording_frame()
-        #     cv2.imshow("Recording Frame", recording_frame)
-            
-        #     key = cv2.waitKey(1)
-
-        #     if key == ord("q"):
-        #         cv2.destroyAllWindows()
-        #         break
-
-        # sys.exit(App.exec())
-
-        # App = QApplication(sys.argv)
-
-
-        # session = Session(session_path)
-        # session.load_cameras()
-        # session.load_streams()
-        # session.adjust_resolutions()
-
 
-        # recording_dialog = RecordingWidget(session)
-        # recording_dialog.show()
+def launch_recording_widget(session_path):
+            config = Configurator(session_path)
+            session = Session(config)
+            session.load_stream_tools()
+            session._adjust_resolutions()
+
+            App = QApplication(sys.argv)
+            recording_dialog = RecordingWidget(session)
+            recording_dialog.show()
 
-        # sys.exit(App.exec())
+            sys.exit(App.exec())
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/stereoframe/__pycache__/omni_frame_builder.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/omni_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/stereoframe/__pycache__/omni_frame_widget.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/omni_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/stereoframe/__pycache__/stereo_frame_builder.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/stereoframe/__pycache__/stereo_frame_widget.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/__pycache__/stereo_frame_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/stereoframe/stereo_frame_builder.py` & `pyxy3d-0.0.19/pyxy3d/gui/frame_builders/paired_frame_builder.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import numpy as np
 
 from pyxy3d.cameras.synchronizer import Synchronizer
 from itertools import combinations
 from queue import Queue
 from threading import Event
 
-COMMON_CORNER_TARGET = 5 # how many shared corners must be present to be recorded...
+COMMON_CORNER_TARGET = 4 # how many shared corners must be present to be recorded...
 
-class StereoFrameBuilder:
+class PairedFrameBuilder:
     def __init__(self, synchronizer: Synchronizer, single_frame_height=250,board_count_target=50):
         self.synchronizer = synchronizer 
         self.single_frame_height = single_frame_height
 
         # used to determine sort order. Should this be in the stereo_tracker?
         self.board_count_target = board_count_target 
         self.common_corner_target = COMMON_CORNER_TARGET
         
-        self.rotation_counts = {}
-        for port, stream in self.synchronizer.streams.items():
-            # override here while testing this out with pre-recorded video
-            self.rotation_counts[port] = stream.camera.rotation_count
+        # self.rotation_counts = {}
+        # for port, stream in self.synchronizer.streams.items():
+        #     # override here while testing this out with pre-recorded video
+        #     self.rotation_counts[port] = stream.camera.rotation_count
 
         self.pairs = self.get_pairs()
 
         self.new_sync_packet_notice = Queue()
         self.synchronizer.subscribe_to_notice(self.new_sync_packet_notice)
         self.store_points = Event()
     
@@ -110,15 +110,15 @@
             img_loc_A = frame_packet_A.points.img_loc
             img_loc_B = frame_packet_B.points.img_loc
 
             # bit of an important side effect in here. Not best practice,
             # but the convenience is hard to pass up...
             # if there are enough corners in common, then store the corner locations
             # in the stereo history and update the board counts
-            if len(common_ids) > self.common_corner_target and self.store_points.is_set():
+            if len(common_ids) >= self.common_corner_target and self.store_points.is_set():
                 # logger.info("Storing common ids..")
                 # logger.info("Stereo History:")
                 # logger.info(self.stereo_history)
                 self.stereo_history[(portA,portB)]['img_loc_A'].extend(img_loc_A.tolist())
                 self.stereo_history[(portA,portB)]['img_loc_B'].extend(img_loc_B.tolist())
                 self.board_counts[(portA,portB)]+=1
                 
@@ -153,16 +153,14 @@
         return frameA, frameB
 
     def resize_to_square(self, frame):
         """To make sure that frames align well, scale them all to thumbnails
         squares with black borders."""
         logger.debug("resizing square")
 
-        frame = cv2.flip(frame, 1)
-
         height = frame.shape[0]
         width = frame.shape[1]
 
         padded_size = max(height, width)
 
         height_pad = int((padded_size - height) / 2)
         width_pad = int((padded_size - width) / 2)
@@ -180,15 +178,18 @@
         )
 
         frame = resize(frame, new_height=self.single_frame_height)
         return frame
 
 
     def apply_rotation(self, frame, port):
-        rotation_count = self.rotation_counts[port]
+        # rotation_count = self.rotation_counts[port]
+        rotation_count = self.synchronizer.streams[port].camera.rotation_count
+        # logger.info(f"stream is {self.synchronizer.streams[port].camera}")
+        # logger.info(f"Applying rotation {rotation_count} at port {port}")
         if rotation_count == 0:
             pass
         elif rotation_count in [1, -3]:
             frame = cv2.rotate(frame, cv2.ROTATE_90_CLOCKWISE)
         elif rotation_count in [2, -2]:
             frame = cv2.rotate(frame, cv2.ROTATE_180)
         elif rotation_count in [-1, 3]:
@@ -210,14 +211,16 @@
 
         frameA = self.resize_to_square(frameA)
         frameB = self.resize_to_square(frameB)
 
         frameA = self.apply_rotation(frameA, portA)
         frameB = self.apply_rotation(frameB, portB)
 
+        frameA = cv2.flip(frameA, 1)
+        frameB = cv2.flip(frameB, 1)
 
         frameA = cv2.putText(frameA,
                              str(portA),
                             (int(frameA.shape[1]/2), int(self.single_frame_height / 4)),
                             fontFace=cv2.FONT_HERSHEY_SIMPLEX,
                             fontScale=1,
                             color=(0, 0, 255),
@@ -354,85 +357,7 @@
 
 def resize(image, new_height):
     (current_height, current_width) = image.shape[:2]
     ratio = new_height / float(current_height)
     dim = (int(current_width * ratio), new_height)
     resized = cv2.resize(image, dim, interpolation=cv2.INTER_AREA)
     return resized
-
-if __name__ == "__main__":
-    from pyxy3d.img2xy.charuco_tracker import CharucoTracker
-    from pyxy3d.recording.recorded_stream import RecordedStreamPool,RecordedStream
-    from pyxy3d.recording.video_recorder import VideoRecorder
-    from pyxy3d.session import Session
-    from pyxy3d.calibration.charuco import Charuco
-    
-    from pyxy3d import __root__
-    
-    ports = [0, 1, 2, 3]
-    # ports = [1,2, 3]
-
-    test_live = True
-    record = True
-    # test_live = False
-    
-    if test_live:
-
-        session_directory = Path(__root__, "tests", "4_cameras_beginning")
-        session = Session(session_directory)
-        session.load_cameras()
-        session.load_streams()
-        logger.info("Creating Synchronizer")
-        syncr = Synchronizer(session.streams, fps_target=3)
-    else:
-        recording_directory = Path(__root__, "tests", "mimic_anipose")
-        charuco = Charuco(
-            4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
-        )
-        recorded_stream_pool = RecordedStreamPool(ports, recording_directory, charuco=charuco)
-        logger.info("Creating Synchronizer")
-        syncr = Synchronizer(recorded_stream_pool.streams, fps_target=3)
-        recorded_stream_pool.play_videos()
-
-    frame_builder = StereoFrameBuilder(synchronizer=syncr, board_count_target=20)
-
-    if record:
-        video_path = Path(__root__, "tests", "please work")
-        video_recorder = VideoRecorder(syncr)
-        video_recorder.start_recording(video_path)
-
-    
-    while not syncr.stop_event.is_set():
-
-        stereo_frame = frame_builder.get_stereo_frame()
-        if stereo_frame is None:
-            cv2.destroyAllWindows()
-            break
-
-        cv2.imshow("stereo frame", stereo_frame)
-
-        key = cv2.waitKey(1)
-
-        if key == ord("q"):
-            cv2.destroyAllWindows()
-            break
-        
-        if key == ord("s"): # as in `s`tore
-            if frame_builder.store_points.is_set():
-                frame_builder.store_points.clear()
-            else: 
-                frame_builder.store_points.set()
-
-        if key == ord("r"): # as in `s`tore
-            frame_builder.reset()
-
-        if key == ord("u"):
-            frame_builder.synchronizer.unsubscribe_to_streams() 
-            
-        if frame_builder.possible_to_initialize_array(5):
-            logger.info("possible to initialize array now")
-
-    # recorder.stop_recording()
-    cv2.destroyAllWindows()
-    
-    if record:
-        video_recorder.stop_recording()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/stereoframe/stereo_frame_widget.py` & `pyxy3d-0.0.19/pyxy3d/gui/extrinsic_calibration_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import pyxy3d.logger
 logger = pyxy3d.logger.get(__name__)
 
 import sys
 from pathlib import Path
 from threading import Thread, Event
 import time
+from enum import Enum
 
 import cv2
 from PyQt6.QtCore import Qt, pyqtSignal, QThread
 from PyQt6.QtGui import QImage, QPixmap, QIcon
 from PyQt6.QtWidgets import (
     QApplication,
     QSizePolicy,
@@ -25,55 +26,68 @@
     QLabel,
     QPushButton,
     QSlider,
     QVBoxLayout,
 )
 
 # Append main repo to top of path to allow import of backend
-from pyxy3d.session import Session
-from pyxy3d.gui.stereoframe.stereo_frame_builder import StereoFrameBuilder
+from pyxy3d.session.session import Session
+from pyxy3d.gui.frame_builders.paired_frame_builder import PairedFrameBuilder
 from pyxy3d.cameras.synchronizer import Synchronizer
 from pyxy3d import __root__
-from pyxy3d.gui.qt_logger import QtLogger
-from pyxy3d.gui.widgets import NavigationBarBackFinish
+from pyxy3d.gui.navigation_bars import NavigationBarNext
 
-# the boards needed to before a pair could be used to bridge pairs without common corners
+# the boards needed before a pair could be used to bridge pairs without common corners
 MIN_THRESHOLD_FOR_EARLY_CALIBRATE = 5
 
 
-class StereoFrameWidget(QWidget):
+class PossibleActions(Enum):
+    CollectData = "Collect Data"
+    Terminate = "Terminate"
+    Calibrate = "Calibrate"
+
+class ExtrinsicCalibrationWidget(QWidget):
     calibration_complete = pyqtSignal()
     calibration_initiated = pyqtSignal()
     terminate = pyqtSignal()
      
     def __init__(self,session:Session):
 
-        super(StereoFrameWidget, self).__init__()
+        super(ExtrinsicCalibrationWidget, self).__init__()
         self.session = session
-        self.synchronizer:Synchronizer = self.session.get_synchronizer()
+        self.synchronizer:Synchronizer = self.session.synchronizer
 
         self.create_stereoframe_tools()
 
         self.frame_rate_spin = QSpinBox()
-        self.frame_rate_spin.setValue(self.synchronizer.get_fps_target())
+        self.frame_rate_spin.setValue(self.synchronizer.fps_target)
         self.board_count_spin = QSpinBox()
         self.board_count_spin.setValue(self.frame_builder.board_count_target)
         
         self.stereo_frame_display = QLabel()
-        self.navigation_bar = NavigationBarBackFinish() 
-        self.calibrate_collect_btn = self.navigation_bar.calibrate_collect_btn
-
+        # self.navigation_bar = NavigationBarNext() 
+        self.possible_action = PossibleActions.CollectData
+        self.calibrate_collect_btn = QPushButton(self.possible_action.value)
         
         self.place_widgets()
         self.connect_widgets()        
 
+        self.update_btn_eligibility()
+    
+    def update_btn_eligibility(self):
+        if self.session.is_extrinsic_calibration_eligible():
+            self.calibrate_collect_btn.setEnabled(True)
+        else:
+            self.calibrate_collect_btn.setEnabled(False)
+    
+
     def create_stereoframe_tools(self):
 
-        self.frame_builder = StereoFrameBuilder(self.synchronizer, board_count_target=30)
-        self.frame_emitter = StereoFrameEmitter(self.frame_builder)
+        self.frame_builder = PairedFrameBuilder(self.synchronizer, board_count_target=30)
+        self.frame_emitter = PairedFrameEmitter(self.frame_builder)
         self.frame_emitter.start()
 
     def place_widgets(self):
         self.setLayout(QVBoxLayout())
         
         self.settings_group = QGroupBox("Settings")
         self.settings_group.setLayout(QHBoxLayout())
@@ -89,56 +103,60 @@
         self.scroll_area = QScrollArea()
         self.scroll_area.setVerticalScrollBarPolicy(Qt.ScrollBarPolicy.ScrollBarAlwaysOn)
         # self.scroll_area.setLayout(QVBoxLayout())
         self.layout().addWidget(self.scroll_area)
 
         self.scroll_area.setWidget(self.stereo_frame_display)
        
-        self.layout().addWidget(self.navigation_bar)
+        self.layout().addWidget(self.calibrate_collect_btn)
 
 
 
     def connect_widgets(self):
         
-        self.calibrate_collect_btn.clicked.connect(self.on_calibrate_connect_click)
+        self.calibrate_collect_btn.clicked.connect(self.on_calibrate_collect_click)
         self.frame_emitter.ImageBroadcast.connect(self.ImageUpdateSlot)
         self.frame_emitter.possible_to_initialize_array.connect(self.enable_calibration)
-        self.frame_rate_spin.valueChanged.connect(self.synchronizer.set_fps_target)
+        self.frame_rate_spin.valueChanged.connect(self.synchronizer.set_stream_fps)
         self.board_count_spin.valueChanged.connect(self.update_board_count_target)
         self.frame_emitter.calibration_data_collected.connect(self.initiate_calibration)
     
     def update_board_count_target(self, target):
         self.frame_builder.board_count_target = target
         
-    def on_calibrate_connect_click(self):
-        if self.calibrate_collect_btn.text() == "Collect Data":
+    def on_calibrate_collect_click(self):
+        if self.possible_action == PossibleActions.CollectData:
             logger.info("Begin collecting calibration data")
             # by default, data saved to session folder
             self.frame_builder.store_points.set()
-            self.session.start_recording()
-            self.calibrate_collect_btn.setText("Terminate")
+            extrinsic_calibration_path = Path(self.session.path, "calibration", "extrinsic")
+            self.session.start_recording(extrinsic_calibration_path,store_point_history=True)
+            self.possible_action = PossibleActions.Terminate
+            self.calibrate_collect_btn.setText(self.possible_action.value)
             self.calibrate_collect_btn.setEnabled(True)
             self.navigation_bar.back_btn.setEnabled(False)
 
-        elif self.calibrate_collect_btn.text() == "Terminate":
+        elif self.possible_action == PossibleActions.Terminate:
             logger.info("Terminating current data collection")
             self.terminate.emit()
             # self.session.stop_recording()
             # self.frame_builder.reset()
-            self.calibrate_collect_btn.setText("Collect Data")
+            self.possible_action = PossibleActions.CollectData
+            self.calibrate_collect_btn.setText(self.possible_action.value)
 
-        elif self.calibrate_collect_btn.text() == "Calibrate":
-            logger.info("Prematurely end data collection")
+        elif self.possible_action == PossibleActions.Calibrate:
+            logger.info("Prematurely end data collection to initiate calibration")
             self.frame_builder.store_points.clear()
             self.initiate_calibration()
             
 
 
     def enable_calibration(self):
-        self.calibrate_collect_btn.setText("Calibrate")
+        self.possible_action = PossibleActions.Calibrate
+        self.calibrate_collect_btn.setText(self.possible_action.value)
         self.calibrate_collect_btn.setEnabled(True)
         
         
     def ImageUpdateSlot(self, q_image):
         self.stereo_frame_display.resize(self.stereo_frame_display.sizeHint())
 
         qpixmap = QPixmap.fromImage(q_image)
@@ -156,32 +174,33 @@
             # self.stereo_frame_display.hide()
             logger.info("Stop recording video")
             self.session.stop_recording()
             logger.info("Begin calibration")
             logger.info("Pause synchronizer")
             self.session.pause_synchronizer()
             self.session.estimate_extrinsics()
-            self.navigation_bar.back_btn.setEnabled(True)
-            self.calibrate_collect_btn.setText("Collect Data")
+
+            self.possible_action = PossibleActions.CollectData
+            self.calibrate_collect_btn.setText(self.possible_action.value)
             self.calibrate_collect_btn.setEnabled(True)
             self.calibration_complete.emit()
             logger.info("Calibration Complete signal sent...")
             
         self.init_calibration_thread = Thread(target=worker,args=(), daemon=True)
         self.init_calibration_thread.start()
 
-class StereoFrameEmitter(QThread):
+class PairedFrameEmitter(QThread):
     ImageBroadcast = pyqtSignal(QImage)
     calibration_data_collected = pyqtSignal() 
     possible_to_initialize_array = pyqtSignal()
     
-    def __init__(self, stereoframe_builder:StereoFrameBuilder):
+    def __init__(self, paired_frame_builder:PairedFrameBuilder):
         
-        super(StereoFrameEmitter,self).__init__()
-        self.stereoframe_builder = stereoframe_builder
+        super(PairedFrameEmitter,self).__init__()
+        self.paired_frame_builder = paired_frame_builder
         logger.info("Initiated frame emitter")        
         self.keep_collecting = Event() 
         self.collection_complete = False
         
     def run(self):
 
         self.keep_collecting.set()
@@ -189,29 +208,29 @@
 
         possible_to_initialize = False
         
         while self.keep_collecting.is_set():
             
             # that that it is important to make sure that this signal is sent only once
             # to avoid multiple calibration attempts 
-            if len(self.stereoframe_builder.stereo_list) == 0 and not self.collection_complete:
+            if len(self.paired_frame_builder.stereo_list) == 0 and not self.collection_complete:
                 logger.info("Signalling that calibration data is fully collected.")
                 self.collection_complete = True
                 self.calibration_data_collected.emit()
         
                 # break
             
             if not possible_to_initialize:
                 # check to see if it is now
-                if self.stereoframe_builder.possible_to_initialize_array(MIN_THRESHOLD_FOR_EARLY_CALIBRATE):
+                if self.paired_frame_builder.possible_to_initialize_array(MIN_THRESHOLD_FOR_EARLY_CALIBRATE):
                     logger.info("Signaling that it is possible to initialize array based on collected data.")
                     possible_to_initialize = True
                     self.possible_to_initialize_array.emit()
                       
-            stereo_frame = self.stereoframe_builder.get_stereo_frame()
+            stereo_frame = self.paired_frame_builder.get_stereo_frame()
 
             if stereo_frame is not None:
                 image = cv2_to_qlabel(stereo_frame)
                 self.ImageBroadcast.emit(image)
 
         logger.info("Stereoframe emitter run thread ended...") 
             
@@ -231,21 +250,25 @@
         image.shape[0],
         QImage.Format.Format_RGB888,
     )
     return qt_frame
 
     
 if __name__ == "__main__":
+        from pyxy3d.configurator import Configurator
+        from pyxy3d.trackers.charuco_tracker import CharucoTracker
+
         App = QApplication(sys.argv)
 
-        config_path = Path(__root__, "tests", "217")
+        session_path = Path(__root__, "dev","sample_sessions", "257")
+        configurator = Configurator(session_path)
 
-        session = Session(config_path)
-        session.load_cameras()
-        session.load_streams()
-        session.adjust_resolutions()
+        session = Session(configurator)
+        # session.load_cameras()
+        tracker = CharucoTracker(session.charuco)
+        session.load_stream_tools(tracker=tracker)
 
 
-        stereo_dialog = StereoFrameWidget(session)
+        stereo_dialog = ExtrinsicCalibrationWidget(session)
         stereo_dialog.show()
 
         sys.exit(App.exec())
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/camera_mesh.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_dialog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_visualizer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/__pycache__/capture_volume_widget.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/calibration/capture_volume_visualizer.py` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/realtime_triangulation_widget.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,145 +1,169 @@
+#%%
+
 import pyxy3d.logger
 
 logger = pyxy3d.logger.get(__name__)
 
-import math
 import sys
-import time
 from pathlib import Path
-from threading import Thread
-from queue import Queue
-import pandas as pd
 import numpy as np
+import pandas as pd
+from queue import Queue
+from threading import Thread
 import pyqtgraph.opengl as gl
 
-from random import random
-
+from PyQt6.QtCore import Qt, pyqtSignal
+from PyQt6.QtWidgets import (
+    QApplication,
+    QSlider,
+    QVBoxLayout,
+    QWidget,
+)
+from pyxy3d.session.session import Session
 from pyxy3d.gui.vizualize.camera_mesh import CameraMesh, mesh_from_camera
+from pyxy3d.interface import XYZPacket
 from pyxy3d.cameras.camera_array import CameraArray
-from pyxy3d.calibration.capture_volume.capture_volume import CaptureVolume
 
+class RealTimeTriangulationWidget(QWidget):
+    def __init__(self, camera_array:CameraArray, xyz_packet_q:Queue):
+        super(RealTimeTriangulationWidget, self).__init__()
+
+        self.camera_array = camera_array
+        self.xyz_packet_q = xyz_packet_q #place to receive xyz_packets from Triangulator or similar...
+
+        self.visualizer = TriangulationVisualizer(self.camera_array)
+
+        self.setMinimumSize(500, 500)
+
+        self.place_widgets()
+        self.connect_widgets()
+
+        self.thread = Thread(target=self.process_incoming,args=[],daemon=True)
+        self.thread.start()
+
+    def place_widgets(self):
+        self.setLayout(QVBoxLayout())
+        self.layout().addWidget(self.visualizer.scene)
 
-class CaptureVolumeVisualizer:
+    def connect_widgets(self):
+        pass
+        # self.slider.valueChanged.connect(self.visualizer.display_points)
+
+    def process_incoming(self):
+        
+        while True:
+            xyz_packet = self.xyz_packet_q.get()
+            self.visualizer.display_points(xyz_packet)
+            
+
+class TriangulationVisualizer:
     """
     Can except either a single camera array or a capture volume that includes
     point_estimates. If a capture volume is supplied, point positions can
     be played back.
     """
 
     def __init__(
-        self, capture_volume: CaptureVolume = None, camera_array: CameraArray = None
+        self, camera_array: CameraArray
     ):
 
-        if camera_array is not None and capture_volume is None:
-            self.camera_array = camera_array
-            self.point_estimates = None
-        else:
-            self.capture_volume = capture_volume
-            self.camera_array = capture_volume.camera_array
-            self.point_estimates = self.capture_volume.point_estimates
+        self.camera_array = camera_array
 
+        # self.min_sync_index = np.min(self.sync_indices)
+        # self.max_sync_index = np.max(self.sync_indices)
+        # self.sync_index = self.min_sync_index
+
+        # x_coord = self.xyz_history["x_coord"]
+        # y_coord = self.xyz_history["y_coord"]
+        # z_coord = self.xyz_history["z_coord"]
+        # self.xyz_coord = np.vstack([x_coord,y_coord,z_coord]).T
+        
         # constuct a scene
         self.scene = gl.GLViewWidget()
         self.scene.setCameraPosition(distance=4)  # the scene camera, not a real Camera
-        self.sync_index = None
-
-        self.refresh_scene()
-
-    def refresh_scene(self):
-        self.scene.clear()
 
         axis = gl.GLAxisItem()
         self.scene.addItem(axis)
 
         # build meshes for all cameras
         self.meshes = {}
         for port, cam in self.camera_array.cameras.items():
             print(port)
             print(cam)
             mesh:CameraMesh = mesh_from_camera(cam)
             self.meshes[port] = mesh
             self.scene.addItem(mesh)
 
-        # self.scene.show()
-
-        if self.point_estimates is not None:
-            self.scatter = gl.GLScatterPlotItem(
-                pos=np.array([0, 0, 0]),
-                color=[1, 1, 1, 1],
-                size=0.01,
-                pxMode=False,
-            )
-            self.scene.addItem(self.scatter)
-
-            self.sync_indices = np.unique(self.point_estimates.sync_indices)
-            self.sync_indices = np.sort(self.sync_indices)
-
-            self.min_sync_index = np.min(self.sync_indices)
-            self.max_sync_index = np.max(self.sync_indices)
-   
-            if self.sync_index is not None:
-                self.display_points(self.sync_index)
-                 
-    def display_points(self, sync_index):
-        """
-        sync_index is provided from the dialog and linked to the slider
-        it is initially set to the minimum viable sync index
-        """
-        self.sync_index = sync_index
-        current_sync_index_flag = self.point_estimates.sync_indices == sync_index
-        single_board_indices = np.unique(
-            self.point_estimates.obj_indices[current_sync_index_flag]
+        self.scatter = gl.GLScatterPlotItem(
+            pos=np.array([0, 0, 0]),
+            color=[1, 1, 1, 1],
+            size=0.01,
+            pxMode=False,
         )
+        self.scene.addItem(self.scatter)
 
+        # self.display_points(self.sync_index)
+                 
+    def display_points(self, xyz_packet:XYZPacket):
+        # self.sync_index = sync_index
+        # current_sync_index_flag = self.sync_indices == self.sync_index
+        # self.single_board_points = self.xyz_coord[current_sync_index_flag]
+        # logger.info(f"Displaying xyz points for sync index {sync_index}")
+        self.scatter.setData(pos=xyz_packet.point_xyz)
 
-        self.single_board_points = self.point_estimates.obj[single_board_indices]
-        self.mean_board_position = np.mean(self.single_board_points,axis=0)
-        logger.debug(f"Mean Board Position at sync index {sync_index}: {self.mean_board_position}")
-
-        self.scatter.setData(pos=self.single_board_points)
-
-
-
-
-# %%
 if __name__ == "__main__":
 
     from PyQt6.QtWidgets import QApplication
-
+    import time
     from pyxy3d import __root__
     from pyxy3d.calibration.capture_volume.helper_functions.get_point_estimates import (
         get_point_estimates,
     )
 
     from pyxy3d.calibration.capture_volume.capture_volume import CaptureVolume
-    import pickle
+    
+    test_sessions = [
+        # Path(__root__, "dev", "sample_sessions", "post_triangulation"),
+        Path(__root__, "dev", "sample_sessions", "triangulated_hands", )
+    ]
+
+    test_session_index = 0
+    session_path = test_sessions[test_session_index]
+    logger.info(f"Loading session {session_path}")
+    session = Session(session_path)
 
-    # session_directory = Path(__root__,  "tests", "2_cameras_linear")
-    # session_directory = Path(__root__,  "tests", "tripod")
-    # session_directory = Path(__root__,  "tests", "2_cameras_90_deg")
-    # session_directory = Path(__root__,  "tests", "2_cameras_180_deg")
-    # session_directory = Path(__root__,  "tests", "3_cameras_triangular")
-    # session_directory = Path(__root__,  "tests", "3_cameras_middle")
-    # session_directory = Path(__root__, "tests", "4_cameras_beginning")
-    # session_directory = Path(__root__, "tests", "4_cameras_endofday")
-    session_directory = Path(__root__,  "tests", "4_cameras_nonoverlap")
-    # session_directory = Path(__root__,  "tests", "3_cameras_linear")
-    # session_directory = Path(__root__,  "tests", "3_cameras_midlinear")
-    # session_directory = Path(__root__,  "tests", "just_checking")
-
-    saved_CV_path = Path(session_directory, "capture_volume_stage_1_optimized.pkl")
-    # saved_CV_path = Path(session_directory, "capture_volume_stage_1_new_origin.pkl")
-    with open(saved_CV_path, "rb") as f:
-        capture_volume: CaptureVolume = pickle.load(f)
+    session.load_estimated_capture_volume()
 
     app = QApplication(sys.argv)
-    with open(saved_CV_path, "rb") as f:
-        capture_volume: CaptureVolume = pickle.load(f)
+    
+    xyz_queue = Queue()
+    
+    vizr_dialog = RealTimeTriangulationWidget(session.capture_volume.camera_array, xyz_queue)
+
+#%%   
+    def send_packets_from_history():
+        xyz_history_path = Path(session_path,"xyz_history.csv")
+        
+        xyz_data = pd.read_csv(xyz_history_path)
+        sync_indices = np.unique(xyz_data["sync_index"])
+        sync_indices.sort()
+        
+        for sync_index in sync_indices:
+            current_xyz = xyz_data[xyz_data["sync_index"]==sync_index] 
+            points = current_xyz["point_id"].to_numpy()
+            xyz = current_xyz[["x_coord", "y_coord", "z_coord"]].to_numpy()
+            
+            xyz_packet = XYZPacket(sync_index,points,xyz )
+            xyz_queue.put(xyz_packet)
+            time.sleep(.01)  
+        logger.info("attempting to quit application")
+        # vizr_dialog.close()
+        # app.quit()
+        # sys.exit()
+         
+    thread = Thread(target=send_packets_from_history,args=[],daemon=True)
+    thread.start()        
 
-    app = QApplication(sys.argv)
-    vizr = CaptureVolumeVisualizer(capture_volume=capture_volume)
-    # vizr.display_points(28)
-    # vizr.scene.show()
-    # vizr = CaptureVolumeVisualizer(camera_array = capture_volume.camera_array)
+    vizr_dialog.show()
 
     sys.exit(app.exec())
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/calibration/capture_volume_widget.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,28 @@
     QScrollArea,
     QSlider,
     QSpinBox,
     QVBoxLayout,
     QWidget,
 )
 
-from pyxy3d.session import Session
+from pyxy3d.session.session import Session
 from pyxy3d.gui.vizualize.calibration.capture_volume_visualizer import CaptureVolumeVisualizer
-from pyxy3d.gui.widgets import NavigationBarBackFinish
+from pyxy3d.gui.navigation_bars import NavigationBarBack
 
 
 class CaptureVolumeWidget(QWidget):
     def __init__(self, session: Session):
         super(CaptureVolumeWidget, self).__init__()
 
         self.session = session
+
+        if not hasattr(self.session, "capture_volume"):
+            self.session.load_estimated_capture_volume()
+            
         self.visualizer = CaptureVolumeVisualizer(self.session.capture_volume)
         # self.visualizer.scene.show()
         self.slider = QSlider(Qt.Orientation.Horizontal)
         self.slider.setMinimum(self.visualizer.min_sync_index)
         self.slider.setMaximum(self.visualizer.max_sync_index)
         self.set_origin_btn = QPushButton("Set Origin")
 
@@ -51,49 +55,54 @@
         self.rotate_x_plus_btn = QPushButton("X+")
         self.rotate_x_minus_btn = QPushButton("X-")
         self.rotate_y_plus_btn = QPushButton("Y+")
         self.rotate_y_minus_btn = QPushButton("Y-")
         self.rotate_z_plus_btn = QPushButton("Z+")
         self.rotate_z_minus_btn = QPushButton("Z-")
 
-        self.distance_error_summary = QLabel(self.session.quality_controller.distance_error_summary.to_string(index=False))
+        # self.distance_error_summary = QLabel(self.session.quality_controller.distance_error_summary.to_string(index=False))
         self.rmse_summary = QLabel(self.session.capture_volume.get_rmse_summary())
-        
-
-        self.navigation_bar = NavigationBarBackFinish()
+       
+        self.recalibrate_btn = QPushButton("Recalibrate") 
 
         self.place_widgets()
         self.connect_widgets()
 
         self.visualizer.display_points(self.visualizer.min_sync_index)
 
     def place_widgets(self):
         self.setLayout(QVBoxLayout())
-        self.layout().addWidget(self.visualizer.scene)
+        self.layout().addWidget(self.visualizer.scene, stretch=2)
         self.layout().addWidget(self.slider)
-        self.layout().addWidget(self.set_origin_btn)
-        # self.visualizer.begin()
+    
 
         self.grid = QGridLayout()
-        self.layout().addLayout(self.grid)
         self.grid.addWidget(self.rotate_x_plus_btn, 0, 0)
         self.grid.addWidget(self.rotate_x_minus_btn, 1, 0)
         self.grid.addWidget(self.rotate_y_plus_btn, 0, 1)
         self.grid.addWidget(self.rotate_y_minus_btn, 1, 1)
         self.grid.addWidget(self.rotate_z_plus_btn, 0, 2)
         self.grid.addWidget(self.rotate_z_minus_btn, 1, 2)
 
-        # thie distance error summary here is ugly and needs to be in a table,
-        # But thats out of scope for my current objectives.
-        self.hbox_summary = QHBoxLayout()
-        self.hbox_summary.addWidget(self.rmse_summary)  
-        self.hbox_summary.addWidget(self.distance_error_summary)  
-        self.layout().addLayout(self.hbox_summary)
-
-        self.layout().addWidget(self.navigation_bar)
+        self.world_origin_group = QGroupBox()
+        self.world_origin_group.setLayout(QVBoxLayout())
+        self.world_origin_group.layout().addWidget(self.set_origin_btn)
+        self.world_origin_group.layout().addLayout(self.grid)
+        
+        self.calibrate_group = QGroupBox()
+        self.calibrate_group.setLayout(QVBoxLayout())
+        self.calibrate_group.layout().addWidget(self.rmse_summary)
+        self.calibrate_group.layout().addWidget(self.recalibrate_btn)
+        
+        self.hbox = QHBoxLayout()
+        self.hbox.addWidget(self.calibrate_group)
+        self.hbox.addWidget(self.world_origin_group)
+        self.layout().addLayout(self.hbox)
+        
+        # self.layout().addWidget(self.recalibrate_btn)
 
 
     def connect_widgets(self):
         self.slider.valueChanged.connect(self.visualizer.display_points)
         self.set_origin_btn.clicked.connect(self.set_origin_to_board)
         self.rotate_x_plus_btn.clicked.connect(lambda: self.rotate_capture_volume("x+"))
         self.rotate_x_minus_btn.clicked.connect(
@@ -103,22 +112,27 @@
         self.rotate_y_minus_btn.clicked.connect(
             lambda: self.rotate_capture_volume("y-")
         )
         self.rotate_z_plus_btn.clicked.connect(lambda: self.rotate_capture_volume("z+"))
         self.rotate_z_minus_btn.clicked.connect(
             lambda: self.rotate_capture_volume("z-")
         )
+        
 
     def set_origin_to_board(self):
+
+        logger.info("Setting origin to board...")
+        origin_index = self.slider.value()
+        logger.info(f"Charuco board is {self.session.charuco}")
         self.session.capture_volume.set_origin_to_board(
-            self.slider.value(), self.session.charuco
+            origin_index, self.session.charuco
         )
         self.visualizer.refresh_scene()
-        self.session.save_capture_volume()
-
+        self.session.config.save_capture_volume(self.session.capture_volume)
+        
     def rotate_capture_volume(self, direction):
         transformations = {
             "x+": np.array(
                 [[1, 0, 0, 0], [0, 0, 1, 0], [0, -1, 0, 0], [0, 0, 0, 1]], dtype=float
             ),
             "x-": np.array(
                 [[1, 0, 0, 0], [0, 0, -1, 0], [0, 1, 0, 0], [0, 0, 0, 1]], dtype=float
@@ -135,15 +149,15 @@
             "z-": np.array(
                 [[0, -1, 0, 0], [1, 0, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]], dtype=float
             ),
         }
 
         self.session.capture_volume.shift_origin(transformations[direction])
         self.visualizer.refresh_scene()
-        self.session.save_capture_volume()
+        self.session.config.save_capture_volume(self.session.capture_volume)
 
     def update_board(self, sync_index):
 
         logger.info(f"Updating board to sync index {sync_index}")
 
         self.visualizer.display_points(sync_index)
 
@@ -157,15 +171,15 @@
         get_point_estimates,
     )
 
     from pyxy3d.calibration.capture_volume.capture_volume import CaptureVolume
     import pickle
 
     test_sessions = [
-        Path(__root__, "dev", "sample_sessions", "mediapipe_calibration"),
+        Path(__root__, "dev", "sample_sessions", "test_calibration")
     ]
 
     test_session_index = 0
     session_path = test_sessions[test_session_index]
     logger.info(f"Loading session {session_path}")
     session = Session(session_path)
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/camera_mesh.py` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/camera_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -230,23 +230,23 @@
                         x,y,z = [t/translation_scale for t in translation]
                         cams[other_port].mesh.translate(x,y,z)
                         logger.info(f"Translation: x: {x}, y: {y}, z: {z}")
                         # cams[other_port].mesh.setGLOptions('additive')
 
                         scene.addItem(cams[other_port].mesh)
                     if "rotation" in param_key:
-                        rotation = rotation_to_float(value) # feeding in 3x3 rotation matrix  from config file
-                        rotation = rotationMatrixToEulerAngles(rotation) # convert to angles
+                        rotation_count = rotation_to_float(value) # feeding in 3x3 rotation matrix  from config file
+                        rotation_count = rotationMatrixToEulerAngles(rotation_count) # convert to angles
                         if origin_port == pair[1]:
-                            rotation = -rotation
+                            rotation_count = -rotation_count
                             other_port = pair[0]
                         else:
                             other_port = pair[1]
 
-                        rot_deg = [x*(180/math.pi) for x in rotation] # convert to degrees
+                        rot_deg = [x*(180/math.pi) for x in rotation_count] # convert to degrees
                         print(f"Rotation (deg) for port {other_port}: {rot_deg}")
                         x = rot_deg[0]
                         y = rot_deg[1]
                         z = rot_deg[2]
 
                         logger.info(f"ROTATION: x: {x}, y: {y}, z: {z}")
                         cams[other_port].mesh.rotate(x,1,0,0, local=True)
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/vizualize/triangulation_widget.py` & `pyxy3d-0.0.19/pyxy3d/gui/vizualize/playback_triangulation_widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,136 +12,134 @@
 from PyQt6.QtCore import Qt, pyqtSignal
 from PyQt6.QtWidgets import (
     QApplication,
     QSlider,
     QVBoxLayout,
     QWidget,
 )
-from pyxy3d.session import Session
+from pyxy3d.session.session import Session
 from pyxy3d.gui.vizualize.camera_mesh import CameraMesh, mesh_from_camera
 from pyxy3d.cameras.camera_array import CameraArray
 
-class TriangulationWidget(QWidget):
-    def __init__(self, camera_array:CameraArray, xyz_history_path:Path):
-        super(TriangulationWidget, self).__init__()
+
+class PlaybackTriangulationWidget(QWidget):
+    def __init__(self, camera_array: CameraArray, xyz_history_path: Path = None):
+        super(PlaybackTriangulationWidget, self).__init__()
 
         self.camera_array = camera_array
-        self.xyz_history = pd.read_csv(xyz_history_path)
 
-        self.visualizer = TriangulationVisualizer(self.camera_array, self.xyz_history)
+        self.visualizer = TriangulationVisualizer(self.camera_array)
         # self.visualizer.scene.show()
         self.slider = QSlider(Qt.Orientation.Horizontal)
-        self.slider.setMinimum(self.visualizer.min_sync_index)
-        self.slider.setMaximum(self.visualizer.max_sync_index)
 
-        self.setMinimumSize(500, 500)
+        # these defaults mean nothing right now without xyz data. Just placeholders
 
+        self.setMinimumSize(500, 500)
 
         self.place_widgets()
         self.connect_widgets()
-
-        # self.visualizer.display_points(self.visualizer.min_sync_index)
+        if xyz_history_path is not None:
+            xyz_history = pd.read_csv(xyz_history_path)
+            self.set_xyz(xyz_history)
 
     def place_widgets(self):
         self.setLayout(QVBoxLayout())
         self.layout().addWidget(self.visualizer.scene)
         self.layout().addWidget(self.slider)
 
-
     def connect_widgets(self):
         self.slider.valueChanged.connect(self.visualizer.display_points)
 
+    def set_xyz(self, xyz: pd.DataFrame):
+        # self.xyz_history = pd.read_csv(xyz_history)
+        self.visualizer.set_xyz(xyz)
+        if xyz is not None:
+            self.slider.setMinimum(self.visualizer.min_sync_index)
+            self.slider.setMaximum(self.visualizer.max_sync_index)
+        else:
+            self.slider.setMinimum(0)
+            self.slider.setMaximum(100)
 
+    def update_camera_array(self, camera_array:CameraArray):
+        self.visualizer.update_camera_array(camera_array)
 class TriangulationVisualizer:
     """
     Can except either a single camera array or a capture volume that includes
     point_estimates. If a capture volume is supplied, point positions can
     be played back.
     """
 
-    def __init__(
-        self, camera_array: CameraArray, xyz_history:pd.DataFrame
-    ):
-
+    def __init__(self, camera_array: CameraArray):
         self.camera_array = camera_array
-        self.xyz_history = xyz_history
-
-        self.sync_indices = self.xyz_history["sync_index"]
-        self.min_sync_index = np.min(self.sync_indices)
-        self.max_sync_index = np.max(self.sync_indices)
-        self.sync_index = self.min_sync_index
-
-        x_coord = self.xyz_history["x_coord"]
-        y_coord = self.xyz_history["y_coord"]
-        z_coord = self.xyz_history["z_coord"]
-        self.xyz_coord = np.vstack([x_coord,y_coord,z_coord]).T
-        
-        # constuct a scene
-        self.scene = gl.GLViewWidget()
-        self.scene.setCameraPosition(distance=4)  # the scene camera, not a real Camera
+        self.build_scene()
 
+    def build_scene(self):
+        # constuct a scene if not yet there
+        if hasattr(self, "scene"):
+            logger.info("Clearing scene in capture volume visualizer")
+            self.scene.clear()
+        else:
+            logger.info("Creating initial scene in capture volume visualizer")
+            self.scene = gl.GLViewWidget()
+            self.scene.setCameraPosition(distance=4)  # the scene camera, not a real Camera
         axis = gl.GLAxisItem()
         self.scene.addItem(axis)
 
-        # build meshes for all cameras
-        self.meshes = {}
-        for port, cam in self.camera_array.cameras.items():
-            print(port)
-            print(cam)
-            mesh:CameraMesh = mesh_from_camera(cam)
-            self.meshes[port] = mesh
-            self.scene.addItem(mesh)
+        if self.camera_array.extrinsics_calibrated:
+            self.meshes = {}
+            for port, cam in self.camera_array.cameras.items():
+                mesh: CameraMesh = mesh_from_camera(cam)
+                self.meshes[port] = mesh
+                self.scene.addItem(mesh)
 
         self.scatter = gl.GLScatterPlotItem(
             pos=np.array([0, 0, 0]),
             color=[1, 1, 1, 1],
             size=0.01,
             pxMode=False,
         )
         self.scene.addItem(self.scatter)
+        self.scatter.setData(pos=None)
+    
+    def update_camera_array(self, camera_array:CameraArray):
+        self.camera_array = camera_array
+        self.build_scene()
+
+
+    def set_xyz(self, xyz_history: pd.DataFrame):
+        logger.info(f"Updating xyz history in playback widget")
+        self.xyz_history = xyz_history
+
+        if self.xyz_history is not None:
+            self.sync_indices = self.xyz_history["sync_index"]
+            self.min_sync_index = np.min(self.sync_indices)
+            self.max_sync_index = np.max(self.sync_indices)
+            self.sync_index = self.min_sync_index
+
+            x_coord = self.xyz_history["x_coord"]
+            y_coord = self.xyz_history["y_coord"]
+            z_coord = self.xyz_history["z_coord"]
+            self.xyz_coord = np.vstack([x_coord, y_coord, z_coord]).T
+
+        else:
+            self.xyz_coord = None
+            self.sync_index=0
+            # self.scatter.setData(pos=None)
 
         self.display_points(self.sync_index)
-                 
+
     def display_points(self, sync_index):
         """
         sync_index is provided from the dialog and linked to the slider
         it is initially set to the minimum viable sync index
         """
-        self.sync_index = sync_index
-
-        current_sync_index_flag = self.sync_indices == self.sync_index
-
-        self.single_board_points = self.xyz_coord[current_sync_index_flag]
-        logger.info(f"Displaying xyz points for sync index {sync_index}")
-
-        self.scatter.setData(pos=self.single_board_points)
-
-if __name__ == "__main__":
 
-    from PyQt6.QtWidgets import QApplication
+        if self.xyz_coord is not None:
+            self.sync_index = sync_index
 
-    from pyxy3d import __root__
-    from pyxy3d.calibration.capture_volume.helper_functions.get_point_estimates import (
-        get_point_estimates,
-    )
-
-    from pyxy3d.calibration.capture_volume.capture_volume import CaptureVolume
-    import pickle
-
-    test_sessions = [
-        Path(__root__, "dev", "sample_sessions", "post_triangulation"),
-    ]
-
-    test_session_index = 0
-    session_path = test_sessions[test_session_index]
-    logger.info(f"Loading session {session_path}")
-    session = Session(session_path)
-
-    session.load_estimated_capture_volume()
-
-    app = QApplication(sys.argv)
-    
-    xyz_history_path = Path(session_path,"xyz_history.csv")
-    vizr_dialog = TriangulationWidget(session.capture_volume.camera_array,xyz_history_path)
-    vizr_dialog.show()
+            current_sync_index_flag = self.sync_indices == self.sync_index
+            self.points = self.xyz_coord[current_sync_index_flag]
+            logger.debug(f"Displaying xyz points for sync index {sync_index}")
+            self.scatter.setData(pos=self.points)
 
-    sys.exit(app.exec())
+        else: 
+            self.scatter.setData(pos=None)
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/widgets.py` & `pyxy3d-0.0.19/pyxy3d/gui/navigation_bars.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,82 +12,85 @@
 )
 
 NAV_BAR_HEIGHT = 75
 class NavigationBarNext(QWidget):
     def __init__(self):
         super().__init__()
         self.setLayout(QHBoxLayout())
-        self.next_wizard_step_btn = QPushButton("Next")
-        self.next_wizard_step_btn.setMaximumWidth(50)
+
+        self.calibrate_collect_btn = QPushButton("&Collect Data")
+        self.calibrate_collect_btn.setMaximumWidth(120)
+
         self.layout().setAlignment(Qt.AlignmentFlag.AlignRight)
-        self.layout().addWidget(self.next_wizard_step_btn)
+        self.layout().addWidget(self.calibrate_collect_btn)
         self.setMaximumHeight(NAV_BAR_HEIGHT)
+
 class NavigationBarBackNext(QWidget):
     def __init__(self):
         super().__init__()
         self.setLayout(QHBoxLayout())
         self.left_box = QHBoxLayout()
         self.right_box = QHBoxLayout()
 
         self.layout().addLayout(self.left_box)
         self.layout().addLayout(self.right_box)
 
-        self.back_btn = QPushButton("Back")
+        self.back_btn = QPushButton("&Back")
         self.back_btn.setMaximumWidth(50)
         self.left_box.addWidget(self.back_btn)
         
-        self.next_btn = QPushButton("Next")
+        self.next_btn = QPushButton("&Next")
         self.next_btn.setMaximumWidth(50)
         self.right_box.addWidget(self.next_btn)
         
         self.right_box.setAlignment(Qt.AlignmentFlag.AlignRight)
         self.left_box.setAlignment(Qt.AlignmentFlag.AlignLeft)
         self.setMaximumHeight(NAV_BAR_HEIGHT)
 
         
-class NavigationBarBackFinish(QWidget):
+class NavigationBarBack_deprecate(QWidget):
     def __init__(self):
         super().__init__()
         self.setLayout(QHBoxLayout())
         self.left_box = QHBoxLayout()
         self.right_box = QHBoxLayout()
 
         self.layout().addLayout(self.left_box)
         self.layout().addLayout(self.right_box)
 
-        self.back_btn = QPushButton("Back")
+        self.back_btn = QPushButton("&Back")
         self.back_btn.setMaximumWidth(50)
         self.left_box.addWidget(self.back_btn)
         
-        self.finish_btn = QPushButton("Finish")
+        self.finish_btn = QPushButton("&Finish")
         self.finish_btn.setMaximumWidth(50)
         self.right_box.addWidget(self.finish_btn)
         
         self.right_box.setAlignment(Qt.AlignmentFlag.AlignRight)
         self.left_box.setAlignment(Qt.AlignmentFlag.AlignLeft)
         self.setMaximumHeight(NAV_BAR_HEIGHT)
 
         
-class NavigationBarBackFinish(QWidget):
+class NavigationBarBack(QWidget):
     def __init__(self):
         super().__init__()
         self.setLayout(QHBoxLayout())
         self.left_box = QHBoxLayout()
         self.right_box = QHBoxLayout()
 
         self.layout().addLayout(self.left_box)
         self.layout().addLayout(self.right_box)
 
-        self.back_btn = QPushButton("Back")
+        self.back_btn = QPushButton("&Back")
         self.back_btn.setMaximumWidth(50)
         self.left_box.addWidget(self.back_btn)
         
-        self.calibrate_collect_btn = QPushButton("Collect Data")
-        self.calibrate_collect_btn.setMaximumWidth(100)
-        self.right_box.addWidget(self.calibrate_collect_btn)
+        # self.calibrate_collect_btn = qpushbutton("&collect data")
+        # self.calibrate_collect_btn.setmaximumwidth(120)
+        # self.right_box.addwidget(self.calibrate_collect_btn)
         
         self.right_box.setAlignment(Qt.AlignmentFlag.AlignRight)
         self.left_box.setAlignment(Qt.AlignmentFlag.AlignLeft)
         self.setMaximumHeight(NAV_BAR_HEIGHT)
 
 if __name__ == "__main__":
     import sys
```

### Comparing `pyxy3d-0.0.18/pyxy3d/gui/wizard_charuco.py` & `pyxy3d-0.0.19/pyxy3d/gui/charuco_widget.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,74 +24,73 @@
     QWidget,
     QWizard,
     QWizardPage,
 )
 
 from pyxy3d import __app_dir__
 from pyxy3d.calibration.charuco import ARUCO_DICTIONARIES, Charuco
-from pyxy3d.session import Session
-from pyxy3d.gui.qt_logger import QtLogger
-from pyxy3d.gui.widgets import NavigationBarNext
+from pyxy3d.session.session import Session
+from pyxy3d.gui.navigation_bars import NavigationBarNext
 
-class WizardCharuco(QWidget):
+
+class CharucoWidget(QWidget):
     def __init__(self, session):
         super().__init__()
 
         logger.info("Charuco Wizard initializing")
         self.session = session
-        self.params = self.session.config["charuco"]
-        
+        self.params = self.session.config.dict["charuco"]
+
         # add group to do initial configuration of the charuco board
-        self.configurator = CharucoConfigurator(self.session)
-        self.configurator.row_spin.valueChanged.connect(self.build_charuco)
-        self.configurator.column_spin.valueChanged.connect(self.build_charuco)
-        self.configurator.width_spin.valueChanged.connect(self.build_charuco)
-        self.configurator.length_spin.valueChanged.connect(self.build_charuco)
-        self.configurator.units.currentIndexChanged.connect(self.build_charuco)
-        self.configurator.invert_checkbox.stateChanged.connect(self.build_charuco)
+        self.charuco_config = CharucoConfigGroup(self.session)
+        self.charuco_config.row_spin.valueChanged.connect(self.build_charuco)
+        self.charuco_config.column_spin.valueChanged.connect(self.build_charuco)
+        self.charuco_config.width_spin.valueChanged.connect(self.build_charuco)
+        self.charuco_config.length_spin.valueChanged.connect(self.build_charuco)
+        self.charuco_config.units.currentIndexChanged.connect(self.build_charuco)
+        self.charuco_config.invert_checkbox.stateChanged.connect(self.build_charuco)
 
         # Build primary actions
         self.build_save_png_group()
         self.build_true_up_group()
-        # self.build_save_config()
+
         # Build display of board
         self.charuco_added = False  # track to handle redrawing of board
         self.build_charuco()
         self.charuco_added = True
 
         #################### ESTABLISH LARGELY VERTICAL LAYOUT ##############
         self.setLayout(QVBoxLayout())
         self.setWindowTitle("Charuco Board Builder")
 
-        self.layout().addWidget(self.configurator)
-        self.layout().addWidget(self.charuco_display)
-        self.layout().addSpacing(20)
+        self.layout().addWidget(self.charuco_config)
+        self.layout().setAlignment(self.charuco_config, Qt.AlignmentFlag.AlignHCenter)
+        self.layout().addWidget(QLabel("<i>Top left corner is point (0,0,0) when setting capture volume origin</i>"))
+        self.layout().addWidget(self.charuco_display,2)
+        self.layout().addSpacing(10)
         self.layout().addLayout(self.save_png_hbox)
-        self.layout().addSpacing(20)
-
-        self.layout().addWidget(self.true_up_group)
-        self.layout().addSpacing(20)
-        for w in self.children():
-            self.layout().setAlignment(w, Qt.AlignmentFlag.AlignHCenter)
-        
-        # add navigation bar at the end so as to not mess up alignment
-        self.navigation_bar = NavigationBarNext()
-        self.layout().addWidget(self.navigation_bar)
+        self.layout().addSpacing(10)
+        self.layout().addLayout(self.true_up_hbox)
+        self.layout().addWidget(QLabel("<i>Printed square size will set the scale of the capture volume</i>"))
+
+        # self.layout().addSpacing(10)
+        # for w in self.children():
+        #     self.layout().setAlignment(w, Qt.AlignmentFlag.AlignHCenter)
 
-
-        
-        
     def build_save_png_group(self):
         # basic png save button
         self.png_btn = QPushButton("Save &png")
         self.png_btn.setMaximumSize(100, 30)
 
         def save_png():
             save_file_tuple = QFileDialog.getSaveFileName(
-                self, "Save As", str(Path(self.session.path,"charuco.png")), "PNG (*.png)"
+                self,
+                "Save As",
+                str(Path(self.session.path, "charuco.png")),
+                "PNG (*.png)",
             )
             print(save_file_tuple)
             save_file_name = str(Path(save_file_tuple[0]))
             if len(save_file_name) > 1:
                 print(f"Saving board to {save_file_name}")
                 self.charuco.save_image(save_file_name)
 
@@ -99,72 +98,68 @@
 
         # additional mirror image option
         self.png_mirror_btn = QPushButton("Save &mirror png")
         self.png_mirror_btn.setMaximumSize(100, 30)
 
         def save_mirror_png():
             save_file_tuple = QFileDialog.getSaveFileName(
-                self, "Save As", str(Path(self.session.path,"charuco_mirror.png")), "PNG (*.png)"
+                self,
+                "Save As",
+                str(Path(self.session.path, "charuco_mirror.png")),
+                "PNG (*.png)",
             )
             print(save_file_tuple)
             save_file_name = str(Path(save_file_tuple[0]))
             if len(save_file_name) > 1:
                 print(f"Saving board to {save_file_name}")
                 self.charuco.save_mirror_image(save_file_name)
 
         self.png_mirror_btn.clicked.connect(save_mirror_png)
 
         self.save_png_hbox = QHBoxLayout()
         self.save_png_hbox.addWidget(self.png_btn)
         self.save_png_hbox.addWidget(self.png_mirror_btn)
 
     def build_true_up_group(self):
-        self.true_up_group = QGroupBox("&True-Up Printed Square Edge")
-        self.true_up_group.setLayout(QHBoxLayout())
-        self.true_up_group.layout().addWidget(QLabel("Actual Length (cm):"))
+        self.true_up_hbox = QHBoxLayout()
+        self.true_up_hbox.addWidget(QLabel("Actual Printed Square Edge Length (cm):"))
 
         self.printed_edge_length = QDoubleSpinBox()
-        self.printed_edge_length.setSingleStep(.01)
+        self.printed_edge_length.setSingleStep(0.01)
         self.printed_edge_length.setMaximumWidth(100)
         # self.set_true_edge_length()
-        overide = self.session.config["charuco"]["square_size_overide_cm"]
+        overide = self.session.config.dict["charuco"]["square_size_overide_cm"]
         self.printed_edge_length.setValue(overide)
 
         def update_charuco():
-            self.charuco.square_size_overide_cm = round(self.printed_edge_length.value(),2)
+            self.charuco.square_size_overide_cm = round(
+                self.printed_edge_length.value(), 2
+            )
 
-            logger.info(f"Updated Square Size Overide to {self.printed_edge_length.value}")
+            logger.info(
+                f"Updated Square Size Overide to {self.printed_edge_length.value}"
+            )
             self.session.charuco = self.charuco
-            self.session.save_charuco()
+            self.session.config.save_charuco(self.charuco)
 
         self.printed_edge_length.valueChanged.connect(update_charuco)
 
-        self.true_up_group.layout().addWidget(self.printed_edge_length)
-
-    # def build_save_config(self):
-    #     self.save_btn = QPushButton("&Save Charuco")
-    #     self.save_btn.setMaximumSize(100, 30)
-
-    #     def save_charuco():
-    #         self.session.charuco = self.charuco
-    #         self.session.save_charuco()
-    #     self.save_btn.clicked.connect(save_charuco)
-
+        self.true_up_hbox.layout().addWidget(self.printed_edge_length)
 
     def build_charuco(self):
-        columns = self.configurator.column_spin.value()
-        rows = self.configurator.row_spin.value()
-        board_height = self.configurator.length_spin.value()
-        board_width = self.configurator.width_spin.value()
+        columns = self.charuco_config.column_spin.value()
+        rows = self.charuco_config.row_spin.value()
+        board_height = self.charuco_config.length_spin.value()
+        board_width = self.charuco_config.width_spin.value()
         aruco_scale = 0.75
-        units = self.configurator.units.currentText()
+        units = self.charuco_config.units.currentText()
         square_edge_length = self.printed_edge_length.value()
-
-        inverted = self.configurator.invert_checkbox.isChecked()
-        dictionary_str = "DICT_4X4_1000"
+        # a
+        inverted = self.charuco_config.invert_checkbox.isChecked()
+        dictionary_str = "DICT_4X4_50"
 
         self.charuco = Charuco(
             columns,
             rows,
             board_height,
             board_width,
             units=units,
@@ -173,51 +168,47 @@
             square_size_overide_cm=square_edge_length,
             inverted=inverted,
         )
 
         if not self.charuco_added:
             self.charuco_display = QLabel()
             self.charuco_display.setAlignment(Qt.AlignmentFlag.AlignHCenter)
-            # self.charuco_display.setMaximumSize(
-            #     int(self.height() / 2), int(self.width() / 2)
-            # )
-        
-        
+
         # interesting problem comes up when scaling this... I want to switch between scaling the width and height
         # based on how these two things relate....
-        if board_height>board_width:
+        if board_height > board_width:
             charuco_height = int(self.height() / 2)
-            charuco_width = int(charuco_height*(board_width/board_height))
+            charuco_width = int(charuco_height * (board_width / board_height))
         else:
             charuco_width = int(self.width() / 2)
-            charuco_height = int(charuco_width*(board_height/board_width))
+            charuco_height = int(charuco_width * (board_height / board_width))
 
         logger.info("Building charuco thumbnail...")
         charuco_img = self.charuco.board_pixmap(charuco_width, charuco_height)
         self.charuco_display.setPixmap(charuco_img)
 
         self.session.charuco = self.charuco
-        self.session.save_charuco()
+        self.session.config.save_charuco(self.charuco)
+
 
-class CharucoConfigurator(QWidget):
-   
-    def __init__(self, session): 
+class CharucoConfigGroup(QWidget):
+    def __init__(self, session):
         super().__init__()
         self.session = session
-        self.params = self.session.config["charuco"]
-  
+        self.params = self.session.config.dict["charuco"]
+
         self.column_spin = QSpinBox()
-        self.column_spin.setMinimum(2)
+        self.column_spin.setMinimum(3)
         self.column_spin.setValue(self.params["columns"])
-        self.column_spin.setMaximumWidth(50)
+        # self.column_spin.setMaximumWidth(50)
 
         self.row_spin = QSpinBox()
-        self.row_spin.setMinimum(2)
+        self.row_spin.setMinimum(4)
         self.row_spin.setValue(self.params["rows"])
-        self.row_spin.setMaximumWidth(50)
+        # self.row_spin.setMaximumWidth(50)
 
         self.width_spin = QDoubleSpinBox()
         self.width_spin.setMinimum(1)
         self.width_spin.setValue(self.params["board_width"])
         self.width_spin.setMaximumWidth(50)
 
         self.length_spin = QDoubleSpinBox()
@@ -267,34 +258,38 @@
 
         ####################################### UPDATE CHARUCO #################
 
         # self.charuco_build_btn = QPushButton("&Update")
         # self.charuco_build_btn.setMaximumSize(50, 30)
         # self.charuco_build_btn.clicked.connect(self.build_charuco)
         # self.config_options.addWidget(self.charuco_build_btn)
-        
+
     def update_charuco(self):
-        
         columns = self.column_spin.value()
         rows = self.row_spin.value()
         board_height = self.length_spin.value()
         board_width = self.width_spin.value()
         aruco_scale = 0.75
         units = self.units.currentText()
 
 
 if __name__ == "__main__":
-    
-    from pyxy3d import __root__
-    config_path = Path(__root__, "tests", "pyxy3d")
+    from pyxy3d.configurator import Configurator
+    import toml
+
+    app_settings = toml.load(Path(__app_dir__, "settings.toml"))
+    recent_projects: list = app_settings["recent_projects"]
 
-    session = Session(config_path)
+    recent_project_count = len(recent_projects)
+    session_path = Path(recent_projects[recent_project_count - 1])
+    config = Configurator(session_path)
+    session = Session(config)
 
     app = QApplication(sys.argv)
 
-    charuco_page = WizardCharuco(session)
+    charuco_page = CharucoWidget(session)
     charuco_page.show()
 
     # configurator = CharucoConfigurator(session)
     # configurator.show()
 
     sys.exit(app.exec())
```

### Comparing `pyxy3d-0.0.18/pyxy3d/logger.py` & `pyxy3d-0.0.19/pyxy3d/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 import sys
 import os
 from pathlib import Path
 from pyxy3d import __log_dir__
 
 # only one file handler accross package so all messages logged to one file
 
-file_handler = logging.FileHandler(Path(__log_dir__,'calibration.log'), "w+")
-file_handler.setLevel(logging.INFO)
+app_dir_file_handler = logging.FileHandler(Path(__log_dir__,'calibration.log'), "w+")
+app_dir_file_handler.setLevel(logging.INFO)
 
 file_log_format = " %(levelname)8s| %(name)30s| %(lineno)3d|  %(message)s"
 file_formatter = logging.Formatter(file_log_format)
-file_handler.setFormatter(file_formatter)
+app_dir_file_handler.setFormatter(file_formatter)
 
 
 console_handler = logging.StreamHandler()
 console_handler.setLevel(logging.INFO)
 
 console_log_format =" %(levelname)8s| %(name)30s| %(lineno)3d|  %(message)s"
 console_formatter = logging.Formatter(console_log_format)
@@ -35,17 +35,22 @@
     splash screen to show users that something is happening during big processing moments like:
     - loading/finding cameras
     - building / unbuilding synchronizer
     - performing stereocalibration
     """
     def __init__(self):
         logging.Handler.__init__(self)
+        # qt_log_format =" %(levelname)s| %(name)s |%(message)s"
+        qt_log_format =" %(name)s|%(message)s"
+        qt_formatter = logging.Formatter(qt_log_format)
+        self.setFormatter(qt_formatter)
+
     def emit(self, record):
         record = self.format(record)
-        if record: XStream.stdout().write('%s\n'%record)
+        if record: XStream.stdout().write(f"{record} \n")
 
 
 class XStream(QtCore.QObject):
     _stdout = None
     _stderr = None
     messageWritten = QtCore.pyqtSignal(str)
     def flush( self ):
@@ -74,15 +79,19 @@
     logger = logging.getLogger(name)
 
     if name in log_level_overides.keys():
         logger.setLevel(log_level_overides[name])
     else:
         logger.setLevel(logging.INFO) 
 
-    qt_handler = QtHandler()
     
-    logger.addHandler(file_handler)
+    logger.addHandler(app_dir_file_handler)
     logger.addHandler(console_handler)
-    logger.addHandler(qt_handler)
+   
+    # avoid stepping through XStream object if in debug 
+    if os.getenv("DEBUG") != '1':
+        qt_handler = QtHandler()
+        logger.addHandler(qt_handler)
+    
 
     return logger
```

### Comparing `pyxy3d-0.0.18/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/recording/__pycache__/recorded_stream.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/recording/__pycache__/video_recorder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/recording/recorded_stream.py` & `pyxy3d-0.0.19/pyxy3d/recording/recorded_stream.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,34 +17,38 @@
 import toml
 
 import cv2
 from time import perf_counter, sleep
 import pandas as pd
 import numpy as np
 
-from pyxy3d.img2xy.charuco_tracker import CharucoTracker
-from pyxy3d.cameras.data_packets import FramePacket
+from pyxy3d.interface import FramePacket, Tracker, Stream
+from pyxy3d.trackers.tracker_enum import TrackerEnum
 from pyxy3d.cameras.live_stream import Stream
 from pyxy3d.cameras.camera_array import CameraData
+from pyxy3d.configurator import Configurator
+
 
 class RecordedStream(Stream):
     """
-    Analogous to the live stream, this will place frames on a queue 
+    Analogous to the live stream, this will place frames on a queue
     These can then be harvested and synchronized by a Synchronizer
     Within the stream, point detection occurs.
     """
 
-    def __init__(self, camera:CameraData, directory, fps_target=6, charuco=None):
+    def __init__(
+        self, camera: CameraData, directory: Path, fps_target:int=6, tracker: Tracker = None
+    ):
         # self.port = port
         self.directory = directory
         self.camera = camera
         self.port = camera.port
 
-        if charuco is not None:
-            self.tracker = CharucoTracker(charuco)
+        if tracker is not None:
+            self.tracker = tracker
             self.track_points = True
         else:
             self.track_points = False
 
         video_path = str(Path(self.directory, f"port_{self.port}.mp4"))
         self.capture = cv2.VideoCapture(video_path)
 
@@ -64,30 +68,46 @@
         self.last_frame_index = self.port_history["frame_index"].max()
 
         # initializing to something to avoid errors elsewhere
         self.frame_index = 0
         self.frame_time = 0
         self.set_fps_target(fps_target)
 
-    def subscribe(self,queue:Queue):
+    def set_tracking_on(self, track: bool):
+        if track:
+            logger.info(f"Turning tracking on for recorded stream {self.port}")
+            self.track_points.set()
+        else:
+            logger.info(f"Turning tracking off for recorded stream {self.port}")
+            self.track_points.clear()
+
+    def subscribe(self, queue: Queue):
         if queue not in self.subscribers:
             logger.info(f"Adding queue to subscribers at recorded stream {self.port}")
             self.subscribers.append(queue)
             logger.info(f"...now {len(self.subscribers)} subscriber(s) at {self.port}")
         else:
-            logger.warn(f"Attempted to subscribe to recorded stream at port {self.port} twice")
+            logger.warn(
+                f"Attempted to subscribe to recorded stream at port {self.port} twice"
+            )
 
-    def unsubscribe(self, queue:Queue):
+    def unsubscribe(self, queue: Queue):
         if queue in self.subscribers:
-            logger.info(f"Removing subscriber from queue at recorded stream {self.port}")
+            logger.info(
+                f"Removing subscriber from queue at recorded stream {self.port}"
+            )
             self.subscribers.remove(queue)
-            logger.info(f"{len(self.subscribers)} subscriber(s) remain at recorded stream {self.port}")
+            logger.info(
+                f"{len(self.subscribers)} subscriber(s) remain at recorded stream {self.port}"
+            )
         else:
-            logger.warn(f"Attempted to unsubscribe to recorded stream that was not subscribed to\
-                at port {self.port} twice")
+            logger.warn(
+                f"Attempted to unsubscribe to recorded stream that was not subscribed to\
+                at port {self.port} twice"
+            )
 
     def set_fps_target(self, fps):
         self.fps = fps
         if self.fps is None:
             self.milestones = None
         else:
             milestones = []
@@ -109,59 +129,66 @@
 
         if len(future_wait_times) == 0:
             return 1 - fractional_time
         else:
             return future_wait_times[0]
 
     def play_video(self):
-
-        self.thread = Thread(target=self.worker, args=[], daemon=True)
+        self.thread = Thread(target=self.process_frames, args=[], daemon=True)
         self.thread.start()
 
-    def worker(self):
+    def process_frames(self):
         """
         Places FramePacket on the out_q, mimicking the behaviour of the LiveStream.
         """
 
         self.frame_index = self.start_frame_index
         logger.info(f"Beginning playback of video for port {self.port}")
         while not self.stop_event.is_set():
             current_frame = self.port_history["frame_index"] == self.frame_index
             self.frame_time = self.port_history[current_frame]["frame_time"]
             self.frame_time = float(self.frame_time)
-                
-            spinlock_looped = False 
+
+            spinlock_looped = False
             while len(self.subscribers) == 0 and not self.stop_event.is_set():
                 if not spinlock_looped:
                     logger.info(f"Spinlock initiated at port {self.port}")
                     spinlock_looped = True
-                sleep(.5)
+                sleep(0.5)
             if spinlock_looped == True:
                 logger.info(f"Spinlock released at port {self.port}")
 
             if self.milestones is not None:
                 sleep(self.wait_to_next_frame())
 
             success, self.frame = self.capture.read()
 
             if not success:
                 break
 
             if self.track_points:
-                self.point_data = self.tracker.get_points(self.frame)
+                self.point_data = self.tracker.get_points(self.frame, self.port, self.camera.rotation_count)
             else:
                 self.point_data = None
 
             frame_packet = FramePacket(
                 port=self.port,
                 frame_time=self.frame_time,
                 frame=self.frame,
                 frame_index=self.frame_index,
                 points=self.point_data,
+                draw_instructions=self.tracker.draw_instructions,
             )
+            
+            
+            # cv2.imshow(str(self.port), frame_packet.frame_with_points)
+            # key = cv2.waitKey(1)
+            # if key == ord("q"):
+            #     cv2.destroyAllWindows()
+            #     break
 
             logger.debug(
                 f"Placing frame on reel {self.port} for frame time: {self.frame_time} and frame index: {self.frame_index}"
             )
 
             for q in self.subscribers:
                 q.put(frame_packet)
@@ -176,120 +203,129 @@
 
                 for q in self.subscribers:
                     q.put(frame_packet)
                 break
 
 
 class RecordedStreamPool:
-    def __init__(self, directory, fps_target=6, charuco=None):
-
+    def __init__(
+        self,
+        directory: Path,
+        config: Configurator,
+        fps_target=6,
+        tracker: Tracker = None,
+    ):
         self.streams = {}
-        self.cameras = get_configured_camera_data(directory)
-        # self.ports = ports
+        self.camera_array = config.get_camera_array()
 
-        for port, camera in self.cameras.items():
-            self.streams[port] = RecordedStream(camera, directory, fps_target=fps_target, charuco=charuco)
+        for port, camera in self.camera_array.cameras.items():
+            # tracker: Tracker = tracker.value()
+            self.streams[port] = RecordedStream(
+                camera, directory, fps_target=fps_target, tracker=tracker
+            )
 
     def play_videos(self):
         for port, stream in self.streams.items():
             stream.play_video()
 
 
-def get_configured_camera_data(directory, intrinsics_only =True):
+def get_configured_camera_data(config_path, intrinsics_only=True):
     """
     return a list of CameraData objects that is built from the config
     file that is found in the directory. This will be the same
     file where the mp4 files are located.
-    """  
-
-    # load config 
-    config_path = Path(directory,"config.toml")    
+    """
 
     with open(config_path, "r") as f:
         config = toml.load(config_path)
 
     all_camera_data = {}
     for key, params in config.items():
         if key.startswith("cam"):
             if not params["ignore"]:
                 port = params["port"]
-                
+
                 if intrinsics_only:
-                    logger.info(f"Adding intrinisic camera {port} to calibrated camera array...")
+                    logger.info(
+                        f"Adding intrinisic camera {port} to calibrated camera array..."
+                    )
 
                     cam_data = CameraData(
                         port=port,
                         size=params["size"],
                         rotation_count=params["rotation_count"],
                         error=params["error"],
                         matrix=np.array(params["matrix"]),
                         distortions=np.array(params["distortions"]),
                         exposure=params["exposure"],
                         grid_count=params["grid_count"],
                         ignore=params["ignore"],
                         verified_resolutions=params["verified_resolutions"],
                     )
                 else:
-                    
-                    logger.info(f"Adding intrinsic and extrinsic camera {port} to calibrated camera array...")
+                    logger.info(
+                        f"Adding intrinsic and extrinsic camera {port} to calibrated camera array..."
+                    )
                     cam_data = CameraData(
                         port=port,
                         size=params["size"],
                         rotation_count=params["rotation_count"],
                         error=params["error"],
                         matrix=np.array(params["matrix"]),
                         distortions=np.array(params["distortions"]),
                         exposure=params["exposure"],
                         grid_count=params["grid_count"],
                         ignore=params["ignore"],
                         verified_resolutions=params["verified_resolutions"],
                         translation=np.array(params["translation"]),
                         rotation=np.array(params["rotation"]),
                     )
-                    
+
                 all_camera_data[port] = cam_data
-                
+
     return all_camera_data
 
-    
+
 if __name__ == "__main__":
+    from pyxy3d.trackers.charuco_tracker import CharucoTracker
     from pyxy3d.cameras.synchronizer import Synchronizer
     from pyxy3d.calibration.charuco import Charuco
-    
-    
+
     from pyxy3d import __root__
 
-    recording_directory = Path(__root__, "tests", "sessions","217")
+    recording_directory = Path(__root__, "tests", "sessions", "post_monocal")
 
     charuco = Charuco(
         4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
     )
 
-            
+    tracker = CharucoTracker(charuco)
+
     cameras = get_configured_camera_data(recording_directory)
-        
-    recorded_stream_pool = RecordedStreamPool(recording_directory, charuco=charuco)
+
+    recorded_stream_pool = RecordedStreamPool(
+        recording_directory, tracker_factory=tracker
+    )
     syncr = Synchronizer(recorded_stream_pool.streams, fps_target=None)
     recorded_stream_pool.play_videos()
 
     syncr.subscribe_to_streams()
-    
+
     in_q = Queue(-1)
     syncr.subscribe_to_sync_packets(in_q)
-    
+
     while not syncr.frames_complete:
-        sync_packet =in_q.get()
+        sleep(0.03)
+        sync_packet = in_q.get()
         for port, frame_packet in sync_packet.frame_packets.items():
             if frame_packet:
-                cv2.imshow(f"Port {port}", frame_packet.frame)
+                if frame_packet.frame_time == -1:
+                    break  # end of frames
+                cv2.imshow(f"Port {port}", frame_packet.frame_with_points)
 
         key = cv2.waitKey(1)
 
-        # if key == ord("q"):
-        #     cv2.destroyAllWindows()
-        #     break
-
-        # if syncr.frames_complete:
-        #     cv2.destroyAllWindows()
-        #     break
+        if key == ord("q"):
+            # cv2.destroyAllWindows()
+            break
 
     cv2.destroyAllWindows()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/recording/video_recorder.py` & `pyxy3d-0.0.19/pyxy3d/recording/video_recorder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,208 +1,208 @@
 import pyxy3d.logger
 
 logger = pyxy3d.logger.get(__name__)
 
+from PyQt6.QtCore import QObject, pyqtSignal
 from pathlib import Path
 from queue import Queue
 from threading import Thread, Event
 import cv2
 import sys
 import pandas as pd
+import shutil
 
 from pyxy3d.cameras.synchronizer import Synchronizer
 from pyxy3d.cameras.live_stream import LiveStream
+from pyxy3d.interface import FramePacket, SyncPacket
 
-class VideoRecorder:
-    def __init__(self, synchronizer:Synchronizer):
+
+class VideoRecorder(QObject):
+    recording_stop_signal = pyqtSignal()
+    all_frames_saved_signal = pyqtSignal()
+
+    def __init__(self, synchronizer: Synchronizer, suffix: str = None):
+        super().__init__()
         self.synchronizer = synchronizer
 
+        # set text to be appended as port_X_{suffix}.mp4
+        # will also be appended to xy_{suffix}
+        if suffix is not None:
+            self.suffix = "_" + suffix
+        else:
+            self.suffix = ""
+
         self.recording = False
+        self.sync_index = 0  # no sync packets at init... absence of initialized value can cause errors elsewhere
         # build dict that will be stored to csv
         self.trigger_stop = Event()
 
     def build_video_writers(self):
-
+        """
+        suffix provides a way to provide additional labels to the mp4 file name
+        This would be relevant when performing post-processing and saving out frames with points
+        """
         # create a dictionary of videowriters
         self.video_writers = {}
         for port, stream in self.synchronizer.streams.items():
-
-            path = str(Path(self.destination_folder, f"port_{port}.mp4"))
+            path = str(Path(self.destination_folder, f"port_{port}{self.suffix}.mp4"))
             logger.info(f"Building video writer for port {port}; recording to {path}")
             fourcc = cv2.VideoWriter_fourcc(*"MP4V")
-            fps = self.synchronizer.get_fps_target()
             frame_size = stream.camera.size
 
-            writer = cv2.VideoWriter(path, fourcc, fps, frame_size)
+            writer = cv2.VideoWriter(path, fourcc, stream.fps, frame_size)
             self.video_writers[port] = writer
 
-    def save_data_worker(self, include_video):
+    def save_data_worker(self, include_video: bool, show_points: bool, store_point_history:bool):
         # connect video recorder to synchronizer via an "in" queue
+
         if include_video:
             self.build_video_writers()
 
-            # I think I put this here so that it will get reset if you reuse the same recorder..
-            self.frame_history = {
-                "sync_index": [],
-                "port": [],
-                "frame_index": [],
-                "frame_time": [],
-            }
+        # I think I put this here so that it will get reset if you reuse the same recorder..
+        self.frame_history = {
+            "sync_index": [],
+            "port": [],
+            "frame_index": [],
+            "frame_time": [],
+        }
 
         self.point_data_history = {
-                    "sync_index":[],
-                    "port":[],
-                    "frame_index":[],
-                    "frame_time":[],
-                    "point_id":[],
-                    "img_loc_x":[],
-                    "img_loc_y":[],
-                    "obj_loc_x":[],
-                    "obj_loc_y":[],
+            "sync_index": [],
+            "port": [],
+            "frame_index": [],
+            "frame_time": [],
+            "point_id": [],
+            "img_loc_x": [],
+            "img_loc_y": [],
+            "obj_loc_x": [],
+            "obj_loc_y": [],
         }
-        
+
         self.sync_packet_in_q = Queue(-1)
         self.synchronizer.subscribe_to_sync_packets(self.sync_packet_in_q)
+        syncronizer_subscription_released = False
         
-        # reset in case recording a second time
-        # self.trigger_stop.clear() 
-        
-        while not self.trigger_stop.is_set():
-            sync_packet = self.sync_packet_in_q.get()
-            logger.debug("Pulling sync packet from queue")
+        # this is where the issue is... need to figure out when the queue is empty...
+        while self.sync_packet_in_q.qsize() > 0 or not self.trigger_stop.is_set(): 
+            sync_packet: SyncPacket = self.sync_packet_in_q.get()
+
+            # provide periodic updates of recording queue
+            backlog = self.sync_packet_in_q.qsize()
+            if backlog % 25 == 0 and backlog !=0:
+                logger.info(f"Size of unsaved frames on the recording queue is {self.sync_packet_in_q.qsize()}")
+
             if sync_packet is None:
+                # relenvant when 
                 logger.info("End of sync packets signaled...breaking record loop")
                 break
 
-            sync_index = sync_packet.sync_index
-            
+            self.sync_index = sync_packet.sync_index
+
             for port, frame_packet in sync_packet.frame_packets.items():
                 if frame_packet is not None:
                     # logger.info("Processiong frame packet...")
                     # read in the data for this frame for this port
-                    frame = frame_packet.frame
+                    if show_points:
+                        frame = frame_packet.frame_with_points
+                    else:
+                        frame = frame_packet.frame
+
                     frame_index = frame_packet.frame_index
                     frame_time = frame_packet.frame_time
 
                     if include_video:
                         # store the frame
                         self.video_writers[port].write(frame)
 
                         # store to assocated data in the dictionary
-                        self.frame_history["sync_index"].append(sync_index)
+                        self.frame_history["sync_index"].append(self.sync_index)
                         self.frame_history["port"].append(port)
                         self.frame_history["frame_index"].append(frame_index)
                         self.frame_history["frame_time"].append(frame_time)
-                    
-                    new_tidy_table = frame_packet.to_tidy_table(sync_index)
-                    if new_tidy_table is not None: # i.e. it has data
+
+                    new_tidy_table = frame_packet.to_tidy_table(self.sync_index)
+                    if new_tidy_table is not None:  # i.e. it has data
                         for key, value in self.point_data_history.copy().items():
                             self.point_data_history[key].extend(new_tidy_table[key])
-                        print(new_tidy_table)
-
-        logger.info("Save frame worker winding down...")
-        self.synchronizer.release_sync_packet_q(self.sync_packet_in_q)
+                        
+            if not syncronizer_subscription_released and self.trigger_stop.is_set():
+                logger.info("Save frame worker winding down...")
+                syncronizer_subscription_released = True
+                self.synchronizer.release_sync_packet_q(self.sync_packet_in_q)
+                self.recording_stop_signal.emit()
 
         # a proper release is strictly necessary to ensure file is readable
         if include_video:
             logger.info("releasing video writers...")
-            for port, frame_packet in sync_packet.frame_packets.items():
+            for port in self.synchronizer.ports:
                 self.video_writers[port].release()
 
             del self.video_writers
 
             logger.info("Initiate storing of frame history")
             self.store_frame_history()
 
-
         logger.info("Initiate storing of point history")
-        self.store_point_history()
+        if store_point_history:
+            self.store_point_history()
         self.trigger_stop.clear()  # reset stop recording trigger
         self.recording = False
-                
+        self.all_frames_saved_signal.emit()
+
+
     def store_point_history(self):
         df = pd.DataFrame(self.point_data_history)
-        # TODO: #25 if file exists then change the name
-        point_data_path = str(Path(self.destination_folder, "point_data.csv"))
+        point_data_path = str(Path(self.destination_folder, f"xy{self.suffix}.csv"))
         logger.info(f"Storing point data in {point_data_path}")
         df.to_csv(point_data_path, index=False, header=True)
 
     def store_frame_history(self):
         df = pd.DataFrame(self.frame_history)
-        # TODO: #25 if file exists then change the name
         frame_hist_path = str(Path(self.destination_folder, "frame_time_history.csv"))
         logger.info(f"Storing frame history to {frame_hist_path}")
         df.to_csv(frame_hist_path, index=False, header=True)
-
-    def start_recording(self, destination_folder:Path, include_video=True):
-
+    
+    def store_active_config(self):
+        pass
+
+    def start_recording(
+        self,
+        destination_folder: Path,
+        include_video=True,
+        show_points=False,
+        store_point_history=True,
+    ):
+        """
+        Option exists to not store video if only interested in getting points from original video
+        
+        Parent of destination folder will be the source of the config file that will be stored with the video
+        This enables the nested processing of videos (i.e. Recording_1 will store the main config.toml,
+        then POSE subfolder will store config.toml from Recording_1). Each folder should largely become self
+        contained and portable for analysis / reconstruction.
+        """
         logger.info(f"All video data to be saved to {destination_folder}")
 
         self.destination_folder = destination_folder
         # create the folder if it doesn't already exist
         self.destination_folder.mkdir(exist_ok=True, parents=True)
+       
+        # Because calibration files are nested in a calibration directory, need to go 
+        # to parent.parent to get the config.toml file      
+        if self.destination_folder.parent.stem == "calibration":
+            source_config_path = Path(self.destination_folder.parent.parent, "config.toml")
+        else:   # just a regular recording
+            source_config_path = Path(self.destination_folder.parent, "config.toml")
+
+        duplicate_config_path = Path(self.destination_folder,"config.toml")
+        
+        shutil.copy2(source_config_path,duplicate_config_path)
 
         self.recording = True
         self.recording_thread = Thread(
-            target=self.save_data_worker, args=[include_video], daemon=True
+            target=self.save_data_worker, args=[include_video, show_points, store_point_history], daemon=True
         )
         self.recording_thread.start()
 
     def stop_recording(self):
         logger.info("Stop recording initiated within VideoRecorder")
         self.trigger_stop.set()
-
-
-if __name__ == "__main__":
-
-    import time
-
-    from pyxy3d.cameras.camera import Camera
-    from pyxy3d.cameras.live_stream import LiveStream
-    from pyxy3d.session import Session
-    from pyxy3d.calibration.charuco import Charuco
-
-    from pyxy3d.recording.recorded_stream import RecordedStream, RecordedStreamPool
-    from pyxy3d import __root__
-
-
-    ports = [0, 1, 2, 3, 4]
-    # ports = [0,1]
-
-    test_live = True
-    # test_live = False
-
-    if test_live:
-
-        session_directory = Path(__root__, "tests", "please work")
-        session = Session(session_directory)
-        session.load_cameras()
-        session.load_streams()
-        session.adjust_resolutions()
-
-        for port, stream in session.streams.items():
-            stream._show_fps = True
-            # stream._show_charuco = True
-
-        logger.info("Creating Synchronizer")
-        syncr = Synchronizer(session.streams, fps_target=30)
-        video_path = Path(session_directory, "recording2")
-    else:
-        recording_directory = Path(__root__, "sessions", "5_cameras", "recording")
-        charuco = Charuco(
-            4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
-        )
-        stream_pool = RecordedStreamPool(ports, recording_directory, charuco=charuco)
-        logger.info("Creating Synchronizer")
-        syncr = Synchronizer(stream_pool.streams, fps_target=3)
-        stream_pool.play_videos()
-        new_recording_directory = Path(__root__, "sessions", "5_cameras", "recording2")
-        video_path = Path(new_recording_directory)
-
-    video_recorder = VideoRecorder(syncr)
-
-    video_recorder.start_recording(video_path)
-    time.sleep(20)
-    # while not syncr.stop_event.is_set():
-    #     time.sleep(1)
-
-    video_recorder.stop_recording()
```

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/array_stereo_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-137.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-86.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.1.nbc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/real_time_triangulator.triangulate_sync_index-88.py38.nbi`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/stereo_points_builder.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc` & `pyxy3d-0.0.19/pyxy3d/triangulate/__pycache__/triangulator.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/array_stereo_triangulator.py` & `pyxy3d-0.0.19/pyxy3d/triangulate/array_stereo_triangulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import cv2
 import numpy as np
 import pandas as pd
 from pathlib import Path
 from itertools import combinations
 
 from pyxy3d.triangulate.stereo_points_builder import StereoPointsBuilder, StereoPointsPacket
-from pyxy3d.cameras.data_packets import PointPacket, FramePacket, SyncPacket
+from pyxy3d.interface import PointPacket, FramePacket, SyncPacket
 from pyxy3d.triangulate.stereo_points_builder import StereoPointsPacket, SynchedStereoPointsPacket
 
 
 from pyxy3d.cameras.camera_array import CameraData, CameraArray
 
 
 class ArrayStereoTriangulator:
@@ -157,15 +157,15 @@
 
 
 if __name__ == "__main__":
 
     from pyxy3d.recording.recorded_stream import RecordedStreamPool
     from pyxy3d.cameras.synchronizer import Synchronizer
     from pyxy3d.calibration.charuco import Charuco
-    from pyxy3d.img2xy.charuco_tracker import CharucoTracker
+    from pyxy3d.trackers.charuco_tracker import CharucoTracker
     from pyxy3d.cameras.camera_array import CameraArrayBuilder, CameraArray, CameraData
 
     repo = Path(str(Path(__file__)).split("pyxy")[0],"pyxy")
 
     config_path = Path(repo, "sessions", "iterative_adjustment", "config.toml")
     camera_array = CameraArrayBuilder(config_path).get_camera_array()
 
@@ -175,18 +175,18 @@
     recorded_stream_pool = RecordedStreamPool(ports, recorded_data)
     syncr = Synchronizer(
         recorded_stream_pool.streams, fps_target=None
     )  # no fps target b/c not playing back for visual display
     recorded_stream_pool.play_videos()
 
     # create a corner tracker to locate board corners
-    charuco = Charuco(
+    tracker = Charuco(
         4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
     )
-    trackr = CharucoTracker(charuco)
+    trackr = CharucoTracker(tracker)
 
     # create a commmon point finder to grab charuco corners shared between the pair of ports
     pairs = [(0, 1)]
     point_stream = StereoPointsBuilder(
         synchronizer=syncr,
         pairs=pairs,
         tracker=trackr,
```

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/real_time_triangulator.py` & `pyxy3d-0.0.19/pyxy3d/triangulate/sync_packet_triangulator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,143 +1,174 @@
-
-
 import pyxy3d.logger
-logger = pyxy3d.logger.get(__name__)
 
+logger = pyxy3d.logger.get(__name__)
+import os
 from numba import jit
 from numba.typed import Dict, List
 import numpy as np
 import pandas as pd
 from pyxy3d.cameras.camera_array import CameraArray
 from pyxy3d.cameras.synchronizer import Synchronizer, SyncPacket
 from queue import Queue
 from threading import Thread, Event
 from pathlib import Path
-from pyxy3d.cameras.data_packets import XYZPacket
+from pyxy3d.interface import XYZPacket, Tracker
 
 
-class RealTimeTriangulator:
+class SyncPacketTriangulator:
     """
     Will place 3d packets on subscribed queues and save consolidated data in csv
     format to output_path if provided
-    """    
-    def __init__(self,camera_array:CameraArray, synchronizer:Synchronizer, output_directory:Path=None):
+    """
+
+    def __init__(
+        self,
+        camera_array: CameraArray,
+        synchronizer: Synchronizer,
+        recording_directory: Path = None,
+        tracker_name:str = None,  # used only for getting the point names and tracker name
+    ):
         self.camera_array = camera_array
         self.synchronizer = synchronizer
-        self.output_directory = output_directory
+        self.recording_directory = recording_directory
 
         self.stop_thread = Event()
         self.stop_thread.clear()
-        # self._sync_packet_history = []     
-        self.xyz_history = []
-        self.sync_packet_in_q = Queue(-1) 
+
+        self.tracker_name = tracker_name
+
+        self.xyz_history = {
+            "sync_index": [],
+            "point_id": [],
+            "x_coord": [],
+            "y_coord": [],
+            "z_coord": [],
+        }
+
+        self.sync_packet_in_q = Queue(-1)
         self.synchronizer.subscribe_to_sync_packets(self.sync_packet_in_q)
-        
+
         # assemble numba compatible dictionary
-        self.projection_matrices = Dict() 
+        self.projection_matrices = Dict()
         # self.projection_matrices = {}
         for port, cam in self.camera_array.cameras.items():
             self.projection_matrices[port] = cam.projection_matrix
 
         self.subscribers = []
+        self.running = True
         self.thread = Thread(target=self.process_incoming, args=(), daemon=True)
         self.thread.start()
-        
-    def subscribe(self, queue:Queue):
+
+    def subscribe(self, queue: Queue):
         self.subscribers.append(queue)
-        
-    def unsubscriber(self,queue:Queue):
-        self.subscribers.remove(queue)
 
+    def unsubscriber(self, queue: Queue):
+        self.subscribers.remove(queue)
 
     def process_incoming(self):
-        self.running = True
-        while not self.stop_thread.is_set():
+        # waiting to set running property here was causing issues with identifying state of thread.
+        # set property to true then start thread...
 
-            sync_packet:SyncPacket = self.sync_packet_in_q.get()
+        # self.running = True
+        while not self.stop_thread.is_set():
+            sync_packet: SyncPacket = self.sync_packet_in_q.get()
 
             if sync_packet is None:
                 # No more sync packets after this... wind down
                 self.stop_thread.set()
-                logger.info("End processing of incoming sync packets...end signaled with `None` packet")
-
-            else:    
-                logger.info(f"Sync Packet {sync_packet.sync_index} acquired...")     
-                # self._sync_packet_history.append(sync_packet)
-    
-                cameras, point_ids, imgs_xy = sync_packet.triangulation_inputs
-
+                logger.info(
+                    "End processing of incoming sync packets...end signaled with `None` packet"
+                )
+            else:
+                logger.debug(
+                    f"Sync Packet {sync_packet.sync_index} acquired with {sync_packet.frame_packet_count} frames"
+                )
                 # only attempt to process if data exists
-                if len(cameras) > 2:
-
+                if sync_packet.frame_packet_count >= 2:
+                    cameras, point_ids, imgs_xy = sync_packet.triangulation_inputs
+                    logger.debug("Attempting to triangulate synced frames")
                     # prepare for jit
                     cameras = np.array(cameras)
                     point_ids = np.array(point_ids)
                     imgs_xy = np.array(imgs_xy)
-                    # only attempt to process points with multiple views
-                    # iterated across the current points to find those with multiple views
 
-                    point_id_xyz, points_xyz = triangulate_sync_index(
-                        self.projection_matrices, cameras, point_ids, imgs_xy
-                    )
-            
-                    logger.info(f"Synch Packet {sync_packet.sync_index} | Point ID: {point_id_xyz} | xyz: {points_xyz}")
+                    logger.debug(f"Cameras are {cameras} and point_ids are {point_ids}")
+                    if len(np.unique(cameras)) >= 2:
+                        logger.debug(f"Points observed on cameras {np.unique(cameras)}")
+                        point_id_xyz, points_xyz = triangulate_sync_index(
+                            self.projection_matrices, cameras, point_ids, imgs_xy
+                        )
+
+                        logger.debug(
+                            f"Synch Packet {sync_packet.sync_index} | Point ID: {point_id_xyz} | xyz: {points_xyz}"
+                        )
+
+                        xyz_packet = XYZPacket(
+                            sync_packet.sync_index, point_id_xyz, points_xyz
+                        )
+                        logger.info(
+                            f"Placing xyz pacKet for index {sync_packet.sync_index} with {len(xyz_packet.point_ids)} points"
+                        )
+                        for q in self.subscribers:
+                            q.put(xyz_packet)
+
+                        # if self.output_path is not None:
+                        self.add_packet_to_history(xyz_packet)
 
-                    xyz_packet = XYZPacket(sync_packet.sync_index,point_id_xyz,points_xyz)
-                    for q in self.subscribers:
-                        q.put(xyz_packet)
-                    
-                    # if self.output_path is not None:
-                    self.xyz_history.append(xyz_packet)
-                              
-        self.running = False 
+        self.running = False
 
-        if self.output_directory is not None:
-            logger.info(f"Saving xyz point data to {self.output_directory}")
+        if self.recording_directory is not None:
+            logger.info(f"Saving xyz point data to {self.recording_directory}")
             self.save_history()
+
+    def add_packet_to_history(self, xyz_packet: XYZPacket):
+        point_count = len(xyz_packet.point_ids)
+
+        if point_count > 0:
+            self.xyz_history["sync_index"].extend([xyz_packet.sync_index] * point_count)
+            xyz_array = np.array(xyz_packet.point_xyz)
+            self.xyz_history["point_id"].extend(xyz_packet.point_ids)
+            self.xyz_history["x_coord"].extend(xyz_array[:, 0].tolist())
+            self.xyz_history["y_coord"].extend(xyz_array[:, 1].tolist())
+            self.xyz_history["z_coord"].extend(xyz_array[:, 2].tolist())
             
-    def save_history(self):
-        
-        xyz_history = {"sync_index":[], 
-                        "point_id":[], 
-                        "x_coord":[],
-                        "y_coord":[], 
-                        "z_coord":[]}
-
-        for packet in self.xyz_history:
-            point_count = len(packet.point_ids)
-            if point_count>0:
-                xyz_history["sync_index"].extend([packet.sync_index]*point_count)
-                xyz_array = np.array(packet.point_xyz)
-                xyz_history["point_id"].extend(packet.point_ids)
-                xyz_history["x_coord"].extend(xyz_array[:,0].tolist())
-                xyz_history["y_coord"].extend(xyz_array[:,1].tolist())
-                xyz_history["z_coord"].extend(xyz_array[:,2].tolist())
+    
+
+    def save_history(self)->None:
+        """
+        If a recording directory is provided, then save the xyz directory into it
+        If a tracker name is provided, then base name on the tracker name
+        """
+        df_xyz: pd.DataFrame = pd.DataFrame(self.xyz_history)
        
-        xyz_history:pd.DataFrame = pd.DataFrame(xyz_history)
-        xyz_history.to_csv(Path(self.output_directory,"xyz_history.csv"))
-        
+        if self.recording_directory is not None: 
+            if self.tracker_name is None:
+                filename = "xyz.csv"
+            else:
+                filename = f"xyz_{self.tracker_name}.csv"
+                df_xyz.to_csv(Path(self.recording_directory,filename))
+
+
 # helper function to avoid use of np.unique(return_counts=True) which doesn't work with jit
-@jit(nopython=True)
+@jit(nopython=True, cache=True)
 def unique_with_counts(arr):
     sorted_arr = np.sort(arr)
     unique_values = [sorted_arr[0]]
     counts = [1]
 
     for i in range(1, len(sorted_arr)):
         if sorted_arr[i] != sorted_arr[i - 1]:
             unique_values.append(sorted_arr[i])
             counts.append(1)
         else:
             counts[-1] += 1
 
     return np.array(unique_values), np.array(counts)
 
-# NOTE: jit does not appear to improve processing time even after first compilation.
-# Test difference in the future with more points...
+
 @jit(nopython=True, parallel=True, cache=True)
 def triangulate_sync_index(
     projection_matrices, current_camera_indices, current_point_id, current_img
 ):
     # sync_indices_xyz = List()
     point_indices_xyz = List()
     obj_xyz = List()
@@ -160,8 +191,8 @@
             u, s, vh = np.linalg.svd(A, full_matrices=True)
             point_xyzw = vh[-1]
             point_xyz = point_xyzw[:3] / point_xyzw[3]
 
             point_indices_xyz.append(point)
             obj_xyz.append(point_xyz)
 
-    return point_indices_xyz, obj_xyz
+    return point_indices_xyz, obj_xyz
```

### Comparing `pyxy3d-0.0.18/pyxy3d/triangulate/stereo_points_builder.py` & `pyxy3d-0.0.19/pyxy3d/triangulate/stereo_points_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import sys
 from pathlib import Path
 import pandas as pd
 import numpy as np
 from dataclasses import dataclass
 from itertools import combinations
 from pyxy3d.cameras.synchronizer import Synchronizer
-from pyxy3d.img2xy.charuco_tracker import CharucoTracker
-from pyxy3d.cameras.data_packets import SyncPacket
+from pyxy3d.trackers.charuco_tracker import CharucoTracker
+from pyxy3d.interface import SyncPacket
 
 
 class StereoPointsBuilder:
     def __init__(self, ports: list):
 
         self.ports = ports
         self.pairs = [(i, j) for i, j in combinations(self.ports, 2) if i < j]
@@ -157,19 +157,19 @@
     from pyxy3d import __root__
 
     session_directory = Path(__root__, "tests", "5_cameras", "recording")
     csv_output = Path(session_directory, "paired_point_data.csv")
 
     ports = [0, 1, 2, 3, 4]
 
-    charuco = Charuco(
+    tracker = Charuco(
         4, 5, 11, 8.5, aruco_scale=0.75, square_size_overide_cm=5.25, inverted=True
     )
 
-    recorded_stream_pool = RecordedStreamPool(ports, session_directory, charuco=charuco)
+    recorded_stream_pool = RecordedStreamPool(ports, session_directory, charuco=tracker)
     syncr = Synchronizer(recorded_stream_pool.streams, fps_target=200)
     recorded_stream_pool.play_videos()
 
     point_stream = StereoPointsBuilder(synchronizer=syncr, csv_output_path=csv_output)
 
     # I think that EOF needs to propogate up
     while not point_stream.frames_complete:
```

