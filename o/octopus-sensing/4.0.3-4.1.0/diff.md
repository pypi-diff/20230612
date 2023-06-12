# Comparing `tmp/octopus-sensing-4.0.3.tar.gz` & `tmp/octopus-sensing-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octopus-sensing-4.0.3.tar", max compression
+gzip compressed data, was "octopus-sensing-4.1.0.tar", max compression
```

## Comparing `octopus-sensing-4.0.3.tar` & `octopus-sensing-4.1.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
--rw-r--r--   0        0        0    35149 2020-08-21 08:41:09.800625 octopus-sensing-4.0.3/LICENSE
--rw-r--r--   0        0        0     2863 2022-05-20 05:30:08.246089 octopus-sensing-4.0.3/README.md
--rw-r--r--   0        0        0    11168 2020-08-17 23:48:22.186902 octopus-sensing-4.0.3/octopus_sensing/OpenVibe/csv2edf.xml
--rw-r--r--   0        0        0    18650 2020-08-17 23:48:22.186902 octopus-sensing-4.0.3/octopus_sensing/OpenVibe/display-save-eeg-exp2.xml
--rw-r--r--   0        0        0    18648 2020-08-17 23:48:22.186902 octopus-sensing-4.0.3/octopus_sensing/OpenVibe/display-save-eeg.xml
--rw-r--r--   0        0        0      790 2023-06-04 11:08:26.293848 octopus-sensing-4.0.3/octopus_sensing/__init__.py
--rw-r--r--   0        0        0      768 2020-12-08 03:09:47.654520 octopus-sensing-4.0.3/octopus_sensing/common/__init__.py
--rw-r--r--   0        0        0     7612 2022-05-24 06:03:24.413484 octopus-sensing-4.0.3/octopus_sensing/common/endpoint_base.py
--rw-r--r--   0        0        0     2261 2021-11-16 00:47:29.106136 octopus-sensing-4.0.3/octopus_sensing/common/message.py
--rw-r--r--   0        0        0     3645 2021-11-16 00:47:29.110136 octopus-sensing-4.0.3/octopus_sensing/common/message_creators.py
--rw-r--r--   0        0        0     7923 2023-06-01 10:51:19.874106 octopus-sensing-4.0.3/octopus_sensing/device_coordinator.py
--rw-r--r--   0        0        0     4551 2021-11-28 21:09:44.826763 octopus-sensing-4.0.3/octopus_sensing/device_message_endpoint.py
--rw-r--r--   0        0        0     1301 2021-11-18 05:55:31.419363 octopus-sensing-4.0.3/octopus_sensing/devices/__init__.py
--rw-r--r--   0        0        0     8887 2023-03-15 02:47:16.173420 octopus-sensing-4.0.3/octopus_sensing/devices/audio_streaming.py
--rw-r--r--   0        0        0     7303 2023-03-29 00:01:35.111275 octopus-sensing-4.0.3/octopus_sensing/devices/brainflow_openbci_streaming.py
--rw-r--r--   0        0        0     9113 2023-03-24 06:35:43.977593 octopus-sensing-4.0.3/octopus_sensing/devices/brainflow_streaming.py
--rw-r--r--   0        0        0    10893 2023-06-01 10:51:11.242158 octopus-sensing-4.0.3/octopus_sensing/devices/camera_streaming.py
--rw-r--r--   0        0        0     1492 2021-11-16 00:47:29.126136 octopus-sensing-4.0.3/octopus_sensing/devices/common.py
--rw-r--r--   0        0        0     2474 2021-11-16 00:47:29.126136 octopus-sensing-4.0.3/octopus_sensing/devices/device.py
--rw-r--r--   0        0        0     6140 2021-12-15 06:55:13.533285 octopus-sensing-4.0.3/octopus_sensing/devices/network_devices/http_device.py
--rw-r--r--   0        0        0     5333 2021-12-15 06:55:13.537285 octopus-sensing-4.0.3/octopus_sensing/devices/network_devices/socket_device.py
--rw-r--r--   0        0        0     2970 2021-11-16 00:47:29.126136 octopus-sensing-4.0.3/octopus_sensing/devices/open_vibe_streaming.py
--rw-r--r--   0        0        0    10264 2022-06-12 22:45:14.581331 octopus-sensing-4.0.3/octopus_sensing/devices/openbci_streaming.py
--rw-r--r--   0        0        0     3798 2023-03-15 02:49:37.500908 octopus-sensing-4.0.3/octopus_sensing/devices/realtime_data_device.py
--rw-r--r--   0        0        0    16116 2023-06-04 10:57:02.953141 octopus-sensing-4.0.3/octopus_sensing/devices/shimmer3_streaming.py
--rw-r--r--   0        0        0      908 2021-06-15 00:46:08.788642 octopus-sensing-4.0.3/octopus_sensing/preprocessing/__init__.py
--rw-r--r--   0        0        0     9318 2021-12-15 06:55:04.229264 octopus-sensing-4.0.3/octopus_sensing/preprocessing/openbci.py
--rw-r--r--   0        0        0     5569 2021-12-15 06:55:04.229264 octopus-sensing-4.0.3/octopus_sensing/preprocessing/openbci_brainflow.py
--rw-r--r--   0        0        0     9782 2023-03-15 02:13:19.401919 octopus-sensing-4.0.3/octopus_sensing/preprocessing/preprocess_devices.py
--rw-r--r--   0        0        0     8107 2021-11-19 01:23:57.615641 octopus-sensing-4.0.3/octopus_sensing/preprocessing/shimmer3.py
--rw-r--r--   0        0        0     9498 2021-12-15 06:55:04.245264 octopus-sensing-4.0.3/octopus_sensing/preprocessing/utils.py
--rw-r--r--   0        0        0      838 2021-11-16 00:47:29.130136 octopus-sensing-4.0.3/octopus_sensing/questionnaire/__init__.py
--rw-r--r--   0        0        0     6179 2021-11-19 01:15:41.861895 octopus-sensing-4.0.3/octopus_sensing/questionnaire/opinion_question.py
--rw-r--r--   0        0        0     1354 2021-11-16 00:47:29.138136 octopus-sensing-4.0.3/octopus_sensing/questionnaire/question.py
--rw-r--r--   0        0        0     6003 2021-11-16 00:47:29.150137 octopus-sensing-4.0.3/octopus_sensing/questionnaire/questionnaire.py
--rw-r--r--   0        0        0     3618 2021-11-16 00:47:29.150137 octopus-sensing-4.0.3/octopus_sensing/questionnaire/text_question.py
--rw-r--r--   0        0        0     1599 2023-06-01 10:51:16.854124 octopus-sensing-4.0.3/octopus_sensing/realtime_data_endpoint.py
--rw-r--r--   0        0        0      899 2021-11-18 05:55:31.419363 octopus-sensing-4.0.3/octopus_sensing/stimuli/__init__.py
--rw-r--r--   0        0        0     2382 2022-02-10 21:29:39.565850 octopus-sensing-4.0.3/octopus_sensing/stimuli/image_stimulus.py
--rw-r--r--   0        0        0     1088 2021-11-18 05:55:31.423363 octopus-sensing-4.0.3/octopus_sensing/stimuli/stimulus.py
--rw-r--r--   0        0        0     1283 2022-02-16 02:37:26.325088 octopus-sensing-4.0.3/octopus_sensing/stimuli/video_stimulus.py
--rw-r--r--   0        0        0      768 2020-12-08 03:09:47.838518 octopus-sensing-4.0.3/octopus_sensing/tests/__init__.py
--rw-r--r--   0        0        0     1992 2021-08-18 05:02:38.831410 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-00.csv
--rw-r--r--   0        0        0     1989 2021-08-18 05:02:44.559379 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-01.csv
--rw-r--r--   0        0        0     1511 2021-08-18 05:02:49.691350 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-02.csv
--rw-r--r--   0        0        0     1993 2021-08-18 05:02:53.691328 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep01.csv
--rw-r--r--   0        0        0     1994 2021-08-18 05:02:57.979304 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep02.csv
--rw-r--r--   0        0        0     1021 2021-08-18 05:03:07.883250 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep03.csv
--rw-r--r--   0        0        0      998 2021-08-18 05:03:10.955233 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-00.csv
--rw-r--r--   0        0        0      997 2021-08-18 05:03:14.483213 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-01.csv
--rw-r--r--   0        0        0      758 2021-08-18 05:03:33.447109 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-02.csv
--rw-r--r--   0        0        0     1001 2021-08-18 05:03:33.447109 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv
--rw-r--r--   0        0        0      999 2021-08-18 05:03:33.447109 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv
--rw-r--r--   0        0        0      511 2021-08-18 05:03:33.451109 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:27.283000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-00.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:27.385000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-01.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:27.454000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-02.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:37.798000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-00.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:37.907000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-01.csv
--rw-r--r--   0        0        0      300 2021-08-30 23:56:37.960000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-02.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:15.466000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep01.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:19.915000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep02.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:25.104000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep03.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:32.339000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep01.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:36.544000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep02.csv
--rw-r--r--   0        0        0      300 2021-08-31 00:09:41.331000 octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep03.csv
--rw-r--r--   0        0        0    11792 2021-08-16 23:55:07.629704 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_16_continuous/OpenBCI-20-cont16.csv
--rw-r--r--   0        0        0     3462 2021-06-16 01:05:46.778365 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep01.csv
--rw-r--r--   0        0        0     3813 2021-06-16 01:06:29.534207 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep02.csv
--rw-r--r--   0        0        0     3171 2021-06-16 01:07:09.338061 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep03.csv
--rw-r--r--   0        0        0     6488 2021-06-15 23:59:28.010010 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_8_continuous/OpenBCI-20-cont8.csv
--rw-r--r--   0        0        0     1899 2021-06-16 00:59:03.303862 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv
--rw-r--r--   0        0        0     2086 2021-06-16 01:02:50.443017 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv
--rw-r--r--   0        0        0     1748 2021-06-16 01:02:34.947075 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv
--rw-r--r--   0        0        0     3445 2021-08-16 23:55:10.557787 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/Shimmer_continuous/Shimmer-20-cont.csv
--rw-r--r--   0        0        0     1019 2021-06-16 01:10:56.233228 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep01.csv
--rw-r--r--   0        0        0     1104 2021-06-16 01:11:42.117060 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep02.csv
--rw-r--r--   0        0        0      932 2021-06-16 01:12:15.200939 octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep03.csv
--rw-r--r--   0        0        0     6170 2023-03-15 02:08:36.075229 octopus-sensing-4.0.3/octopus_sensing/tests/integration.py
--rw-r--r--   0        0        0     4198 2022-05-24 06:50:46.622856 octopus-sensing-4.0.3/octopus_sensing/tests/test_audio_streaming.py
--rw-r--r--   0        0        0     3758 2022-05-20 05:30:08.250089 octopus-sensing-4.0.3/octopus_sensing/tests/test_brainflow_streaming.py
--rw-r--r--   0        0        0     3274 2022-05-24 06:49:26.962799 octopus-sensing-4.0.3/octopus_sensing/tests/test_camera_streaming.py
--rw-r--r--   0        0        0     1717 2022-05-20 05:30:08.250089 octopus-sensing-4.0.3/octopus_sensing/tests/test_device_coordinator.py
--rw-r--r--   0        0        0     5286 2021-12-15 06:55:04.273264 octopus-sensing-4.0.3/octopus_sensing/tests/test_device_message_endpoint.py
--rw-r--r--   0        0        0     3481 2021-12-15 06:55:04.273264 octopus-sensing-4.0.3/octopus_sensing/tests/test_http_network_device.py
--rw-r--r--   0        0        0     8005 2021-08-30 23:59:50.554899 octopus-sensing-4.0.3/octopus_sensing/tests/test_preprocess.py
--rw-r--r--   0        0        0     2958 2021-12-15 06:55:04.273264 octopus-sensing-4.0.3/octopus_sensing/tests/test_socket_network_device.py
--rw-r--r--   0        0        0      955 2021-11-18 05:55:31.423363 octopus-sensing-4.0.3/octopus_sensing/windows/__init__.py
--rw-r--r--   0        0        0     2259 2021-11-25 20:15:14.808514 octopus-sensing-4.0.3/octopus_sensing/windows/image_window.py
--rw-r--r--   0        0        0     3076 2021-11-25 20:18:03.811225 octopus-sensing-4.0.3/octopus_sensing/windows/message_window.py
--rw-r--r--   0        0        0     3681 2021-12-07 20:15:43.372977 octopus-sensing-4.0.3/octopus_sensing/windows/timer_window.py
--rw-r--r--   0        0        0     1519 2023-06-04 11:08:52.425718 octopus-sensing-4.0.3/pyproject.toml
--rw-r--r--   0        0        0     5445 2023-06-04 11:12:11.390278 octopus-sensing-4.0.3/setup.py
--rw-r--r--   0        0        0     4303 2023-06-04 11:12:11.390785 octopus-sensing-4.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2020-08-21 08:41:09.800625 octopus-sensing-4.1.0/LICENSE
+-rw-r--r--   0        0        0     2863 2022-05-20 05:30:08.246089 octopus-sensing-4.1.0/README.md
+-rw-r--r--   0        0        0    11168 2020-08-17 23:48:22.186902 octopus-sensing-4.1.0/octopus_sensing/OpenVibe/csv2edf.xml
+-rw-r--r--   0        0        0    18650 2020-08-17 23:48:22.186902 octopus-sensing-4.1.0/octopus_sensing/OpenVibe/display-save-eeg-exp2.xml
+-rw-r--r--   0        0        0    18648 2020-08-17 23:48:22.186902 octopus-sensing-4.1.0/octopus_sensing/OpenVibe/display-save-eeg.xml
+-rw-r--r--   0        0        0      790 2023-06-12 03:37:45.517060 octopus-sensing-4.1.0/octopus_sensing/__init__.py
+-rw-r--r--   0        0        0      768 2020-12-08 03:09:47.654520 octopus-sensing-4.1.0/octopus_sensing/common/__init__.py
+-rw-r--r--   0        0        0     7612 2022-05-24 06:03:24.413484 octopus-sensing-4.1.0/octopus_sensing/common/endpoint_base.py
+-rw-r--r--   0        0        0     2261 2021-11-16 00:47:29.106136 octopus-sensing-4.1.0/octopus_sensing/common/message.py
+-rw-r--r--   0        0        0     3645 2021-11-16 00:47:29.110136 octopus-sensing-4.1.0/octopus_sensing/common/message_creators.py
+-rw-r--r--   0        0        0     8304 2023-06-12 03:37:45.517060 octopus-sensing-4.1.0/octopus_sensing/device_coordinator.py
+-rw-r--r--   0        0        0     4551 2021-11-28 21:09:44.826763 octopus-sensing-4.1.0/octopus_sensing/device_message_endpoint.py
+-rw-r--r--   0        0        0     1301 2021-11-18 05:55:31.419363 octopus-sensing-4.1.0/octopus_sensing/devices/__init__.py
+-rw-r--r--   0        0        0     8887 2023-03-15 02:47:16.173420 octopus-sensing-4.1.0/octopus_sensing/devices/audio_streaming.py
+-rw-r--r--   0        0        0     7262 2023-06-12 03:37:45.517060 octopus-sensing-4.1.0/octopus_sensing/devices/brainflow_openbci_streaming.py
+-rw-r--r--   0        0        0     9363 2023-06-12 03:37:45.517060 octopus-sensing-4.1.0/octopus_sensing/devices/brainflow_streaming.py
+-rw-r--r--   0        0        0    11016 2023-06-12 03:37:45.525060 octopus-sensing-4.1.0/octopus_sensing/devices/camera_streaming.py
+-rw-r--r--   0        0        0     1492 2021-11-16 00:47:29.126136 octopus-sensing-4.1.0/octopus_sensing/devices/common.py
+-rw-r--r--   0        0        0     2474 2021-11-16 00:47:29.126136 octopus-sensing-4.1.0/octopus_sensing/devices/device.py
+-rw-r--r--   0        0        0     6140 2021-12-15 06:55:13.533285 octopus-sensing-4.1.0/octopus_sensing/devices/network_devices/http_device.py
+-rw-r--r--   0        0        0     5333 2021-12-15 06:55:13.537285 octopus-sensing-4.1.0/octopus_sensing/devices/network_devices/socket_device.py
+-rw-r--r--   0        0        0     2970 2021-11-16 00:47:29.126136 octopus-sensing-4.1.0/octopus_sensing/devices/open_vibe_streaming.py
+-rw-r--r--   0        0        0    10264 2022-06-12 22:45:14.581331 octopus-sensing-4.1.0/octopus_sensing/devices/openbci_streaming.py
+-rw-r--r--   0        0        0     3798 2023-03-15 02:49:37.500908 octopus-sensing-4.1.0/octopus_sensing/devices/realtime_data_device.py
+-rw-r--r--   0        0        0    16817 2023-06-12 03:37:45.525060 octopus-sensing-4.1.0/octopus_sensing/devices/shimmer3_streaming.py
+-rw-r--r--   0        0        0      908 2021-06-15 00:46:08.788642 octopus-sensing-4.1.0/octopus_sensing/preprocessing/__init__.py
+-rw-r--r--   0        0        0     9318 2021-12-15 06:55:04.229264 octopus-sensing-4.1.0/octopus_sensing/preprocessing/openbci.py
+-rw-r--r--   0        0        0     5569 2021-12-15 06:55:04.229264 octopus-sensing-4.1.0/octopus_sensing/preprocessing/openbci_brainflow.py
+-rw-r--r--   0        0        0     9782 2023-03-15 02:13:19.401919 octopus-sensing-4.1.0/octopus_sensing/preprocessing/preprocess_devices.py
+-rw-r--r--   0        0        0     8107 2023-06-05 09:20:43.339770 octopus-sensing-4.1.0/octopus_sensing/preprocessing/shimmer3.py
+-rw-r--r--   0        0        0     9498 2021-12-15 06:55:04.245264 octopus-sensing-4.1.0/octopus_sensing/preprocessing/utils.py
+-rw-r--r--   0        0        0      838 2021-11-16 00:47:29.130136 octopus-sensing-4.1.0/octopus_sensing/questionnaire/__init__.py
+-rw-r--r--   0        0        0     6179 2021-11-19 01:15:41.861895 octopus-sensing-4.1.0/octopus_sensing/questionnaire/opinion_question.py
+-rw-r--r--   0        0        0     1354 2021-11-16 00:47:29.138136 octopus-sensing-4.1.0/octopus_sensing/questionnaire/question.py
+-rw-r--r--   0        0        0     6003 2021-11-16 00:47:29.150137 octopus-sensing-4.1.0/octopus_sensing/questionnaire/questionnaire.py
+-rw-r--r--   0        0        0     3618 2021-11-16 00:47:29.150137 octopus-sensing-4.1.0/octopus_sensing/questionnaire/text_question.py
+-rw-r--r--   0        0        0     1599 2023-06-01 10:51:16.854124 octopus-sensing-4.1.0/octopus_sensing/realtime_data_endpoint.py
+-rw-r--r--   0        0        0      899 2021-11-18 05:55:31.419363 octopus-sensing-4.1.0/octopus_sensing/stimuli/__init__.py
+-rw-r--r--   0        0        0     2382 2022-02-10 21:29:39.565850 octopus-sensing-4.1.0/octopus_sensing/stimuli/image_stimulus.py
+-rw-r--r--   0        0        0     1088 2021-11-18 05:55:31.423363 octopus-sensing-4.1.0/octopus_sensing/stimuli/stimulus.py
+-rw-r--r--   0        0        0     1283 2022-02-16 02:37:26.325088 octopus-sensing-4.1.0/octopus_sensing/stimuli/video_stimulus.py
+-rw-r--r--   0        0        0      768 2020-12-08 03:09:47.838518 octopus-sensing-4.1.0/octopus_sensing/tests/__init__.py
+-rw-r--r--   0        0        0     1992 2021-08-18 05:02:38.831410 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-00.csv
+-rw-r--r--   0        0        0     1989 2021-08-18 05:02:44.559379 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-01.csv
+-rw-r--r--   0        0        0     1511 2021-08-18 05:02:49.691350 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-02.csv
+-rw-r--r--   0        0        0     1993 2021-08-18 05:02:53.691328 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep01.csv
+-rw-r--r--   0        0        0     1994 2021-08-18 05:02:57.979304 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep02.csv
+-rw-r--r--   0        0        0     1021 2021-08-18 05:03:07.883250 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep03.csv
+-rw-r--r--   0        0        0      998 2021-08-18 05:03:10.955233 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-00.csv
+-rw-r--r--   0        0        0      997 2021-08-18 05:03:14.483213 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-01.csv
+-rw-r--r--   0        0        0      758 2021-08-18 05:03:33.447109 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-02.csv
+-rw-r--r--   0        0        0     1001 2021-08-18 05:03:33.447109 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv
+-rw-r--r--   0        0        0      999 2021-08-18 05:03:33.447109 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv
+-rw-r--r--   0        0        0      511 2021-08-18 05:03:33.451109 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:27.283000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-00.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:27.385000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-01.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:27.454000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/gsr/gsr-20-cont-02.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:37.798000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-00.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:37.907000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-01.csv
+-rw-r--r--   0        0        0      300 2021-08-30 23:56:37.960000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_continuous/ppg/ppg-20-cont-02.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:15.466000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep01.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:19.915000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep02.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:25.104000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/gsr/gsr-20-sep03.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:32.339000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep01.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:36.544000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep02.csv
+-rw-r--r--   0        0        0      300 2021-08-31 00:09:41.331000 octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/Shimmer_sep/ppg/ppg-20-sep03.csv
+-rw-r--r--   0        0        0    11792 2021-08-16 23:55:07.629704 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_16_continuous/OpenBCI-20-cont16.csv
+-rw-r--r--   0        0        0     3462 2021-06-16 01:05:46.778365 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep01.csv
+-rw-r--r--   0        0        0     3813 2021-06-16 01:06:29.534207 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep02.csv
+-rw-r--r--   0        0        0     3171 2021-06-16 01:07:09.338061 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep03.csv
+-rw-r--r--   0        0        0     6488 2021-06-15 23:59:28.010010 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_8_continuous/OpenBCI-20-cont8.csv
+-rw-r--r--   0        0        0     1899 2021-06-16 00:59:03.303862 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv
+-rw-r--r--   0        0        0     2086 2021-06-16 01:02:50.443017 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv
+-rw-r--r--   0        0        0     1748 2021-06-16 01:02:34.947075 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv
+-rw-r--r--   0        0        0     3445 2021-08-16 23:55:10.557787 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/Shimmer_continuous/Shimmer-20-cont.csv
+-rw-r--r--   0        0        0     1019 2021-06-16 01:10:56.233228 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep01.csv
+-rw-r--r--   0        0        0     1104 2021-06-16 01:11:42.117060 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep02.csv
+-rw-r--r--   0        0        0      932 2021-06-16 01:12:15.200939 octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep03.csv
+-rw-r--r--   0        0        0     6218 2023-06-12 03:37:45.525060 octopus-sensing-4.1.0/octopus_sensing/tests/integration.py
+-rw-r--r--   0        0        0     4198 2022-05-24 06:50:46.622856 octopus-sensing-4.1.0/octopus_sensing/tests/test_audio_streaming.py
+-rw-r--r--   0        0        0     3794 2023-06-12 03:37:45.537060 octopus-sensing-4.1.0/octopus_sensing/tests/test_brainflow_streaming.py
+-rw-r--r--   0        0        0     3274 2022-05-24 06:49:26.962799 octopus-sensing-4.1.0/octopus_sensing/tests/test_camera_streaming.py
+-rw-r--r--   0        0        0     1717 2022-05-20 05:30:08.250089 octopus-sensing-4.1.0/octopus_sensing/tests/test_device_coordinator.py
+-rw-r--r--   0        0        0     5286 2021-12-15 06:55:04.273264 octopus-sensing-4.1.0/octopus_sensing/tests/test_device_message_endpoint.py
+-rw-r--r--   0        0        0     3481 2021-12-15 06:55:04.273264 octopus-sensing-4.1.0/octopus_sensing/tests/test_http_network_device.py
+-rw-r--r--   0        0        0     8005 2021-08-30 23:59:50.554899 octopus-sensing-4.1.0/octopus_sensing/tests/test_preprocess.py
+-rw-r--r--   0        0        0     2958 2021-12-15 06:55:04.273264 octopus-sensing-4.1.0/octopus_sensing/tests/test_socket_network_device.py
+-rw-r--r--   0        0        0      955 2021-11-18 05:55:31.423363 octopus-sensing-4.1.0/octopus_sensing/windows/__init__.py
+-rw-r--r--   0        0        0     2259 2021-11-25 20:15:14.808514 octopus-sensing-4.1.0/octopus_sensing/windows/image_window.py
+-rw-r--r--   0        0        0     3076 2021-11-25 20:18:03.811225 octopus-sensing-4.1.0/octopus_sensing/windows/message_window.py
+-rw-r--r--   0        0        0     3681 2021-12-07 20:15:43.372977 octopus-sensing-4.1.0/octopus_sensing/windows/timer_window.py
+-rw-r--r--   0        0        0     1519 2023-06-12 03:37:57.376986 octopus-sensing-4.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5445 2023-06-12 03:38:05.149981 octopus-sensing-4.1.0/setup.py
+-rw-r--r--   0        0        0     4303 2023-06-12 03:38:05.150285 octopus-sensing-4.1.0/PKG-INFO
```

### Comparing `octopus-sensing-4.0.3/LICENSE` & `octopus-sensing-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/README.md` & `octopus-sensing-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/OpenVibe/csv2edf.xml` & `octopus-sensing-4.1.0/octopus_sensing/OpenVibe/csv2edf.xml`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/OpenVibe/display-save-eeg-exp2.xml` & `octopus-sensing-4.1.0/octopus_sensing/OpenVibe/display-save-eeg-exp2.xml`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/OpenVibe/display-save-eeg.xml` & `octopus-sensing-4.1.0/octopus_sensing/OpenVibe/display-save-eeg.xml`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/__init__.py` & `octopus-sensing-4.1.0/octopus_sensing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 # Octopus Sensing is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY;
 # without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
 # See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with Octopus Sensing.
 # If not, see <https://www.gnu.org/licenses/>.
 
-__version__ = '4.0.3'
+__version__ = '4.1.0'
```

### Comparing `octopus-sensing-4.0.3/octopus_sensing/common/__init__.py` & `octopus-sensing-4.1.0/octopus_sensing/common/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/common/endpoint_base.py` & `octopus-sensing-4.1.0/octopus_sensing/common/endpoint_base.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/common/message.py` & `octopus-sensing-4.1.0/octopus_sensing/common/message.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/common/message_creators.py` & `octopus-sensing-4.1.0/octopus_sensing/common/message_creators.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/device_coordinator.py` & `octopus-sensing-4.1.0/octopus_sensing/device_coordinator.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,16 +44,16 @@
         self._cached_data = data
         self._time = time.time_ns()
 
 
 class DeviceCoordinator:
     '''
     Device coordinator is responsible for coordination, like start recording data
-    from all devices at once, stop recording, triggering (marking data at point), 
-    and terminating devices. 
+    from all devices at once, stop recording, triggering (marking data at point),
+    and terminating devices.
     When a device is added to the device coordinator, it will be initialized and prepared for data recording.
     '''
 
     def __init__(self):
         self.__devices = {}
         self.__queues: List[QueueType] = []
         self.__device_counter: int = 0
@@ -91,15 +91,15 @@
         '''
         Adds new device to the coordinator and starts it
 
         Parameters
         ----------
         device: Device
             a device object
-        
+
         Example
         --------
         >>> my_shimmer = Shimmer3Streaming(name="Shimmer3_sensor", output_path="./output")
         >>> device_coordinator.add_device(my_shimmer)
 
         See Also
         ---------
@@ -125,15 +125,15 @@
         '''
         Adds a list of new devices to the coordinator and starts them
 
         Parameters
         ----------
         devices: List[Device]
             a list of device objects
-    
+
         Example
         --------
         >>> my_shimmer = Shimmer3Streaming(name="Shimmer3_sensor",
                                            output_path="./output")
         >>> device_coordinator.add_devices([my_shimmer])
 
         See Also
@@ -147,30 +147,45 @@
         '''
         dispatches a new message to all devices
 
         Parameters
         ----------
         message: Message
             a message object
-        
+
         Example
-        --------     
+        --------
         >>> device_coordinator.dispatch(start_message(experiment_id,
                                                       stimuli_id))
         '''
 
         for message_queue in self.__queues:
             message_queue.put(message)
 
+    def health_check(self):
+        '''
+        Checks if all the devices are okay.
+
+        Returns
+        -----------
+        boolean
+            True if all are healthy, False otherwise
+        '''
+        for device_name, device, in self.__devices.items():
+            if not device.is_alive():
+                print("device [{0}] is not alive anymore.".format(device_name))
+                return False
+        return True
+
     def terminate(self):
         '''
-        sends terminate message to all devices and terminate all processes 
+        sends terminate message to all devices and terminate all processes
 
         Example
-        --------     
+        --------
         >>> device_coordinator.terminate()
         '''
         self.dispatch(terminate_message())
         for item in self.__devices.values():
             item.join()
 
     def get_realtime_data(self, duration: int, device_list: Optional[List[str]]) -> Dict[str, List[Any]]:
@@ -178,23 +193,23 @@
         Returns latest collected data from all devices.
         Device's data can be anything, depending on the device itself.
 
         Parameters
         ----------
         duration: int
             a time duration for getting realtime data in seconds
-        
+
         device_list: List[str]
             a list of device names. Only devices in this list will be monitored or processed in realtime
 
         Returns
         ---------
         data : dict[str, list[any]]
             The keys are device names and values are collected data from the device
-        
+
         Note
         ----
         This method is being used for getting data in real-time for monitoring or realtime processing
 
         '''
         cached = self.__realtime_data_cache.get_cache()
         if cached:
```

### Comparing `octopus-sensing-4.0.3/octopus_sensing/device_message_endpoint.py` & `octopus-sensing-4.1.0/octopus_sensing/device_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/__init__.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/audio_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/audio_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/brainflow_openbci_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/brainflow_openbci_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,73 +26,73 @@
 
     Attributes
     -----------
 
     Parameters
     ----------
     name: str, default: None
-        Device name. This name will be used in the output path to identify 
+        Device name. This name will be used in the output path to identify
         each device's data.
 
     output_path: str,  default: output
         The path for recording files.
         Audio files will be recorded in folder {output_path}/{name}
-    
+
     saving_mode: int, default: SavingModeEnum.CONTINIOUS_SAVING_MODE
         The way of saving data: saving continiously in a file or save data related to
-        each stimulus in a separate file. 
+        each stimulus in a separate file.
         SavingModeEnum is:
 
             0. CONTINIOUS_SAVING_MODE
             1. SEPARATED_SAVING_MODE
-    
+
     board_type: str, default: cyton-daisy
         The type of OpenBCI boards that connect by USB dongle.
         It can be:
 
             - cyton: for cyton board sampling rate is 250 and it has 8 channels
             - cyton-daisy: for cyton-daisy board sampling rate is 125 and it has 16 channels
             - ganglion: for Ganglion board sampling rate is 200 and it has 4 channels
-    
+
     serial_port: str, default: None
         The serial port for reading OpenBCI data. By default we set this as follows for various platforms:
 
             - Linux: /dev/ttyUSB0
             - Windows: Com3
             - MacOS: /dev/cu.*
 
     channels_order: List(str), default: None
         A list of channel names which specify the order and names of channels
 
     Example
     --------
-    Creating an instance of OpenBCI board with USB dongle using 
+    Creating an instance of OpenBCI board with USB dongle using
     `brainflow <https://brainflow.readthedocs.io/en/stable/SupportedBoards.html#openbci>`_,
     and adding it to the device coordinator. Device coordinator is responsible
     for triggerng the OpenBCI to start or stop recording  or to add markers to
     recorded data.
-    In this example, since the saving mode is continuous, all recorded data 
+    In this example, since the saving mode is continuous, all recorded data
     will be saved in a file. But, when an event happens, device coordinator will send
     a trigger message to the device and recorded data will be marked with the trigger
-    
+
     >>> my_openbci =
     ...     BrainFlowOpenBCIStreaming(name="OpenBCI",
     ...                               output_path="./output",
     ...                               board_type="cyton-daisy",
     ...                               saving_mode=SavingModeEnum.CONTINIOUS_SAVING_MODE,
-    ...                               channels_order=["Fp1", "Fp2", "F7", "F3", 
+    ...                               channels_order=["Fp1", "Fp2", "F7", "F3",
     ...                                               "F4", "F8", "T3", "C3",
-    ...                                               "C4", "T4", "T5", "P3", 
+    ...                                               "C4", "T4", "T5", "P3",
     ...                                               "P4", "T6", "O1", "O2"])
     >>> device_coordinator.add_device(my_openbci)
 
     Note
     -----
     Before running the code, turn on the OpenBCI, connect the dongle and make sure its port is free.
-  
+
 
     See Also
     -----------
     :class:`octopus_sensing.device_coordinator`
     :class:`octopus_sensing.devices.device`,
     :class:`octopus_sensing.devices.brainflow_streaming`
     '''
@@ -100,15 +100,15 @@
     def __init__(self,
                  channels_order: List[str]=None,
                  board_type:str ="cyton-daisy",
                  name: Optional[str] = None,
                  output_path: str = "output",
                  serial_port=None,
                  saving_mode: int=SavingModeEnum.CONTINIOUS_SAVING_MODE):
-        self.channels = channels_order      
+        self.channels = channels_order
         if board_type == "cyton-daisy":
             device_id = 2
             sampling_rate = 125
             if self.channels is None:
                 self.channels = \
                     ["ch1", "ch2", "ch3", "ch4", "ch5", "ch6", "ch7", "ch8", "ch9",
                     "ch10", "ch11", "ch12", "ch13", "ch14", "ch15", "ch16"]
@@ -143,14 +143,15 @@
         params.serial_port = serial_port
         super().__init__(device_id,
                          sampling_rate,
                          brain_flow_input_params=params,
                          name=name,
                          output_path=output_path,
                          saving_mode=saving_mode)
+
     def get_output_path(self):
         '''
         Gets the path that is used for data recording
 
         Returns
         -----------
         output_path: str
@@ -166,20 +167,20 @@
         -------
 
         channels_name: List[str]
             The list of channels' name
 
         '''
         return self.channels
-    
+
     def get_saving_mode(self):
         '''
         Gets saving mode
-        
+
         Returns
         -----------
         saving_mode: int
             The way of saving data: saving continiously in a file or save data related to
-            each stimulus in a separate file. 
+            each stimulus in a separate file.
             SavingModeEnum is CONTINIOUS_SAVING_MODE = 0 or SEPARATED_SAVING_MODE = 1
         '''
-        return self._saving_mode
+        return self._saving_mode
```

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/brainflow_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/brainflow_streaming.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,61 +29,61 @@
 class BrainFlowStreaming(RealtimeDataDevice):
     '''
     Manage brainflow streaming
 
     Attributes
     ----------
     device_id
-        Device ID. 
+        Device ID.
         Brainflow support a list of devices, to see supported device IDs go to:
         https://brainflow.readthedocs.io/en/stable/SupportedBoards.html
-    
+
     sampling_rate
         the sampling rate for recording data
-    
+
     brain_flow_input_params
         Each supported board in brainflow gets some parameters, to see the list
         of parameters for each board go to:
         https://brainflow.readthedocs.io/en/stable/SupportedBoards.html
-    
+
     name
         device name
         This name will be used in the output path to identify each device's data
-    
+
     output_path
                  The path for recording files.
                  Audio files will be recorded in folder {output_path}/{name}
 
     saving_mode
-        The way of saving data. It saves data continiously in a file 
-        or saves data which are related to various stimulus in separate files. 
+        The way of saving data. It saves data continiously in a file
+        or saves data which are related to various stimulus in separate files.
         default is SavingModeEnum.CONTINIOUS_SAVING_MODE
         SavingModeEnum is [CONTINIOUS_SAVING_MODE, SEPARATED_SAVING_MODE]
     ** kwargs:
        Extra optional arguments according to the board type
-    
+
     See Also
     -----------
     :class:`octopus_sensing.device_coordinator`
     :class:`octopus_sensing.devices.device`
-    
+
     Examples
     ---------
     Here is an example of using brainflow for reading cyton_daisy board data
 
     >>> params = BrainFlowInputParams()
     >>> params.serial_port = "/dev/ttyUSB0"
-    >>> my_brainflow = 
+    >>> my_brainflow =
     ...       BrainFlowStreaming(2,
     ...                          125,
     ...                          brain_flow_input_params=params,
     ...                          name="cyton_daisy",
     ...                          output_path="./output",
     ...                          saving_mode=SavingModeEnum.CONTINIOUS_SAVING_MODE)
-        
+
     '''
     def __init__(self,
                  device_id: int,
                  sampling_rate: int,
                  brain_flow_input_params: BrainFlowInputParams,
                  saving_mode: int=SavingModeEnum.CONTINIOUS_SAVING_MODE,
                  name: Optional[str] = None,
@@ -96,30 +96,38 @@
 
         self._board = None
         self._device_id = device_id
         self._brain_flow_input_params = brain_flow_input_params
         self._terminate = False
         self._trigger = None
         self._experiment_id = None
+        self.__loop_thread: Optional[threading.Thread] = None
 
         self.output_path = os.path.join(self.output_path, self.name)
         os.makedirs(self.output_path, exist_ok=True)
         self._state = ""
 
     def _run(self):
         self._board = BoardShim(self._device_id, self._brain_flow_input_params)
         self._board.set_log_level(0)
         self._board.prepare_session()
 
-        threading.Thread(target=self._stream_loop).start()
+        self.__loop_thread = threading.Thread(target=self._stream_loop)
+        self.__loop_thread.start()
 
         while True:
             message = self.message_queue.get()
+
+            if not self.__loop_thread.is_alive():
+                print("Brainflow streaming: The streaming thread is dead. Terminating.")
+                break
+
             if message is None:
                 continue
+
             if message.type == MessageType.START:
                 if self._state == "START":
                     print("Brainflow streaming has already recorded the START triger")
                 else:
                     print("Brainflow start")
                     self.__set_trigger(message)
                     self._experiment_id = message.experiment_id
@@ -150,21 +158,24 @@
                                                  self.name,
                                                  self._experiment_id)
                     self._save_to_file(file_name)
                 break
 
         self._board.stop_stream()
         self._board.release_session()
+        self.__loop_thread.join()
 
     def _stream_loop(self):
         self._board.start_stream()
         while True:
             if self._terminate is True:
                 break
+
             data = self._board.get_board_data()
+
             if np.array(data).shape[1] != 0:
                 self._stream_data.extend(list(np.transpose(data)))
                 last_record = self._stream_data.pop()
                 last_record = list(last_record)
                 now = str(datetime.now().time())
                 last_record.append(now)
                 last_record.append(time.time())
@@ -175,15 +186,15 @@
             else:
                 time.sleep(0.1)
             #    print("brainflow: didn't read any data")
 
     def __set_trigger(self, message):
         '''
         Takes a message and set the trigger using its data
-        
+
         Parameters
         ----------
         message: Message
             a message object
         '''
         self._trigger = \
             "{0}-{1}-{2}".format(message.type,
@@ -205,35 +216,35 @@
         -------
 
         channels_name: List[str]
             The list of channels' name
 
         '''
         raise NotImplementedError()
-    
+
     def _get_realtime_data(self, duration: int) -> Dict[str, Any]:
         '''
-        Returns n seconds (duration) of latest collected data for monitoring/visualizing or 
+        Returns n seconds (duration) of latest collected data for monitoring/visualizing or
         realtime processing purposes.
 
         Parameters
         ----------
         duration: int
             A time duration in seconds for getting the latest recorded data in realtime
 
         Returns
         -------
         data: Dict[str, Any]
-            The keys are `data` and `metadata`.  
+            The keys are `data` and `metadata`.
             `data` is a list of records, or empty list if there's nothing.
-            `metadata` is a dictionary of device metadata including `sampling_rate` and `channels` and `type` 
+            `metadata` is a dictionary of device metadata including `sampling_rate` and `channels` and `type`
 
         '''
         # Last seconds of data
-        
+
         data = self._stream_data[-1 * duration * self.sampling_rate:]
         metadata = {"sampling_rate": self.sampling_rate,
                     "channels": self.get_channels(),
                     "type": self.__class__.__name__}
 
         realtime_data = {"data": data,
                   "metadata": metadata}
```

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/camera_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/camera_streaming.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,51 +19,51 @@
 from octopus_sensing.devices.realtime_data_device import RealtimeDataDevice
 from octopus_sensing.common.message_creators import MessageType
 import time
 from typing import Any, Dict
 
 class CameraStreaming(RealtimeDataDevice):
     '''
-    Stream and Record video data. 
+    Stream and Record video data.
     If we have several stimuli, one vide file will be recorded for each stimuli.
     Device coordinator is responsible for triggerng the camera to start or stop recording.
     The content of recorded file is the recorded video between start and stop triggers
 
     Attributes
     ----------
 
     Parameters
     ----------
     name: str, default: None:
         The name of device
-    
+
     output_path: str, default: output
                 The path for recording files.
                 Audio files will be recorded in folder {output_path}/{name}
 
     camera_no: int, default:0
         The camera number. Default is 0  which is defaul camera in system
-    
+
     camera_path: str, default: None
         The physical path of camera device. It varies in different platforms.
         For Example in linux it can be something like this:
         `/dev/v4l/by-id/usb-046d_081b_97E6A7D0-video-index0`
-    
+
     image_width: int, default: 1280
         The width of recorded frame/frames
 
     image_height: int, default: 720
         The height of recorded frame/frames.
-    
+
 
     Notes
     -----
     - Only one of camera_no or camera_path should have value.
 
-    - There is no guarantee that we can set the camera resolution. 
+    - There is no guarantee that we can set the camera resolution.
       Because camera may not be able to support these resolution and it will change it
       based on its settings
 
 
     Example
     -----------
     Creating an instance of camera and adding it to the device coordinator.
@@ -103,41 +103,45 @@
         self._fps: int = 30
         self._capture_times: list = []
         self._frames: list = []
         self._counter = 0
         self._state = ""
 
     def _run(self):
-        print("self._camera_number", self._camera_number)
         self._video_capture = cv2.VideoCapture(self._camera_number)
         try:
             self._video_capture.set(cv2.CAP_PROP_FRAME_WIDTH, self._image_width)
             self._video_capture.set(cv2.CAP_PROP_FRAME_HEIGHT, self._image_height)
         except Exception as error:
             # Ignoring all errors
-            print("Could not set the camera resolution.")
+            print(f"[{self.name}] Could not set the camera resolution. Continuing.")
             print(error)
 
         # There's no guarantee that we can set the camera resolution. So, we
         # re-read the settings again from the camera.
         self._video_size = (int(self._video_capture.get(cv2.CAP_PROP_FRAME_WIDTH)),
                             int(self._video_capture.get(cv2.CAP_PROP_FRAME_HEIGHT)))
         self._video_capture.read()
 
+        if self._video_size[0] <= 0 or self._video_size[1] <= 0:
+            print(f"[{self.name}] Couldn't read the video size from the camera. Trying to terminate.")
+            self._video_capture.release()
+            raise RuntimeError(f"[{self.name}] Couldn't read the video size from the camera.")
+
         recording_thread = None
         recording_event = None
 
-        print(f"Initialized video device [{self.name}]: {self._video_size}")
+        print(f"[{self.name}] Initialized video device: video size: {self._video_size}")
 
         while True:
             message = self.message_queue.get()
             if message is None:
                 continue
             if message.type == MessageType.START:
-                print("start camera")
+                print(f"[{self.name}] start camera")
                 if self._state == "START":
                     print("Video streaming has already started")
                 else:
                     self._frames = []
                     self._capture_times = []
                     if recording_thread is not None:
                         raise RuntimeError(
@@ -145,68 +149,67 @@
                             "A STOP message should be send before trying "
                             "to start a new video recording.".format(self.name)))
 
                     file_name = "{0}/{1}-{2}-{3}.avi".format(self.output_path,
                                                             self.name,
                                                             message.experiment_id,
                                                             str(message.stimulus_id).zfill(2))
-                    print("Starting the thread")
+                    print(f"[{self.name}] Starting the recording thread")
                     recording_event = threading.Event()
                     recording_event.set()
-                    print("recording_event", recording_event)
                     recording_thread = threading.Thread(
                         target=self._stream_loop, args=(file_name, recording_event), daemon=True)
                     recording_thread.start()
                     self._state = "START"
 
             elif message.type == MessageType.STOP:
                 if self._state == "STOP":
-                    print("Video streaming has already started")
+                    print(f"[{self.name}] Video streaming has already stopped")
                 else:
                     if recording_event is not None:
                         recording_event.clear()
                     recording_thread = None
                     recording_event = None
                     self._state = "STOP"
 
             elif message.type == MessageType.TERMINATE:
                 if recording_event is not None:
                     recording_event.clear()
                 recording_thread = None
                 recording_event = None
                 break
 
-        print("video terminated")
+        print(f"[{self.name}] video terminated")
         self._video_capture.release()
 
     def _stream_loop(self, file_name: str, event: threading.Event):
-        print("Start stream camera")
+        print(f"[{self.name}] Start stream camera")
         codec = cv2.VideoWriter_fourcc(*'XVID')
         try:
             while self._video_capture.isOpened:
                 if event.is_set():
                     ret, frame = self._video_capture.read()
                     if ret:
                         self._counter += 1
                         self._capture_times.append(time.time())
                         self._frames.append(frame)
                 else:
                     fps = self._get_frame_rate()
-                    print("Recording frame per second", fps)
+                    print(f"[{self.name}] Recording frame per second", fps)
                     writer = cv2.VideoWriter(file_name,
                             codec,
                             fps,
                             self._video_size)
                     for frame in self._frames:
                         writer.write(frame)
                     writer.release()
                     break
 
         except Exception as error:
-            print("Error while recording video. Device: {0}".format(self.name))
+            print(f"[{self.name}] Error while recording video:")
             print(error)
 
     def _stream_loop_image(self, file_name: str, event: threading.Event):
         try:
             while self._video_capture.isOpened:
                 if event.is_set():
                     ret, frame = self._video_capture.read()
@@ -216,57 +219,56 @@
                         image_file_name = file_name[:-4] + "/" + str(a) + ".jpg"
                         print(image_file_name)
                         cv2.imwrite(image_file_name, frame)
                 else:
                     break
 
         except Exception as error:
-            print("Error while recording video. Device: {0}".format(self.name))
+            print(f"[{self.name}] Error while recording video.")
             print(error)
 
     def _get_realtime_data(self, duration: int) -> Dict[str, Any]:
         '''
-        Returns n seconds (duration) of latest collected data for monitoring/visualizing or 
+        Returns n seconds (duration) of latest collected data for monitoring/visualizing or
         realtime processing purposes.
 
         Parameters
         ----------
         duration: int
             A time duration in seconds for getting the latest recorded data in realtime
 
         Returns
         -------
         data: Dict[str, Any]
-            The keys are `data` and `metadata`.  
+            The keys are `data` and `metadata`.
             `data` is a list of records, or empty list if there's nothing.
-            `metadata` is a dictionary of device metadata including `frame_rate` and `type` 
+            `metadata` is a dictionary of device metadata including `frame_rate` and `type`
         '''
         fps = self._get_frame_rate()
-        print("len(self._frames)", len(self._frames))
+
         data = self._frames[-1 * duration * fps:]
         metadata = {"frame_rate": fps,
                     "type": self.__class__.__name__}
-        print("len(data)", len(data), fps, duration)
+
         if len(data) == 0:
             realtime_data = {"data": [],
                              "metadata": metadata}
         else:
             one_frame_per_seconds = []
             for i in range(duration):
                 if (i * fps) + 1 > len(data):
                     break
                 one_frame_per_seconds.append(data[i * fps])
-        
+
             realtime_data = {"data": one_frame_per_seconds,
                              "metadata": metadata}
         return realtime_data
 
     def _get_frame_rate(self):
         time_diff = 1
         i = 1
         while time_diff < 5 and len(self._capture_times) > i:
             time_diff = self._capture_times[-1] - self._capture_times[-(i+1)]
             i += 1
         fps = int(i/time_diff)
-        print("measured fps: ", fps)
-        return fps
 
+        return fps
```

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/common.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/common.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/device.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/network_devices/http_device.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/network_devices/http_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/network_devices/socket_device.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/network_devices/socket_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/open_vibe_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/open_vibe_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/openbci_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/openbci_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/realtime_data_device.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/realtime_data_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/devices/shimmer3_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/devices/shimmer3_streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,30 @@
 #
 # You should have received a copy of the GNU General Public License along with Octopus Sensing.
 # If not, see <https://www.gnu.org/licenses/>.
 
 import os
 import platform
 import threading
+import time
 import datetime
 import csv
 import math
 import struct
 import serial
 from typing import List, Optional, Any, Dict
 
 from octopus_sensing.devices.realtime_data_device import RealtimeDataDevice
 from octopus_sensing.common.message_creators import MessageType
 from octopus_sensing.common.message import Message
 from octopus_sensing.devices.common import SavingModeEnum
 
+# In seconds
+SERIAL_PORT_TIMEOUT = 0.6
+
 class Shimmer3Streaming(RealtimeDataDevice):
     '''
     Streams and Records Shimmer3 data.
     Data will be recorded in a csv file/files with the following column order:
     type, time stamp, Acc_x, Acc_y, Acc_z, GSR_ohm, PPG_mv, time, trigger
 
     Attributes
@@ -99,25 +103,26 @@
     This class is based on `ShimmerReader <https://github.com/nastaran62/ShimmerReader>`_
     which is an extended version of
     `LogAndStream python firmware <http://www.shimmersensing.com/images/uploads/docs/LogAndStream_for_Shimmer3_Firmware_User_Manual_rev0.11a.pdf>`_
     for Shimmer3 data streaming.
     '''
 
     def __init__(self,
-                 sampling_rate: int=128,
-                 saving_mode: int=SavingModeEnum.CONTINIOUS_SAVING_MODE,
-                 serial_port: Optional[str]=None,
+                 sampling_rate: int = 128,
+                 saving_mode: int = SavingModeEnum.CONTINIOUS_SAVING_MODE,
+                 serial_port: Optional[str] = None,
                  **kwargs):
         super().__init__(**kwargs)
 
         self._saving_mode = saving_mode
         self._stream_data: List[float] = []
         self._sampling_rate = sampling_rate
         self._trigger: Optional[str] = None
         self._break_loop = False
+        self._loop_thread: Optional[threading.Thread] = None
         self.output_path = self._make_output_path()
         self._state = ""
         if serial_port is None:
             if platform.system() == "Windows":
                 self._serial_port = "Com12"
             else:
                 self._serial_port = "/dev/rfcomm0"
@@ -129,15 +134,19 @@
         os.makedirs(output_path, exist_ok=True)
         return output_path
 
     def _inintialize_connection(self):
         '''
         Initializing connection with Simmer3 device
         '''
-        self._serial = serial.Serial(self._serial_port, 115200)
+        self._serial = serial.Serial(port=self._serial_port, baudrate=115200, timeout=SERIAL_PORT_TIMEOUT, write_timeout=SERIAL_PORT_TIMEOUT)
+        if not self._serial.is_open:
+            raise RuntimeError(
+                "shimmer3: Couldn't open the port for some reason.")
+
         self._serial.flushInput()
         print("port opening, done.")
         # send the set sensors command
         # 4 bytes command:
         #     0x08 is SET_SENSORS_COMMAND
         #     Each bit in the three following bytes are one sensor.
         self._serial.write(struct.pack(
@@ -197,32 +206,41 @@
         # send start streaming command
         self._serial.write(struct.pack('B', 0x07))
         self._wait_for_ack()
         print("start command sending, done.")
         self._experiment_id = 0
 
     def _wait_for_ack(self):
+        start_time = time.time()
         ddata = ""
         ack = struct.pack('B', 0xff)
         while ddata != ack:
+            if time.time() - start_time >= 1:
+                raise RuntimeError(f"[{self.name}] Did not receive 'ack' from Shimmer3 after one second")
             ddata = self._serial.read(1)
 
     def _run(self):
         '''
         Listening to the message queue and manage messages
         '''
         self._inintialize_connection()
 
-        loop_thread = threading.Thread(target=self._stream_loop)
-        loop_thread.start()
+        self._loop_thread = threading.Thread(target=self._stream_loop)
+        self._loop_thread.start()
 
         while True:
             message = self.message_queue.get()
+
+            if not self._loop_thread.is_alive():
+                print(f"[{self.name}] Shimmer3: Streaming loop is dead. Terminating.")
+                break
+
             if message is None:
                 continue
+
             if message.type == MessageType.START:
                 if self._state == "START":
                     print("Shimmer3 streaming has already recorded the START triger")
                 else:
                     print("Shimmer start")
                     self._experiment_id = message.experiment_id
                     self.__set_trigger(message)
@@ -231,17 +249,17 @@
                 if self._state == "STOP":
                     print("Shimmer3 streaming has already recorded the STOP triger")
                 else:
                     if self._saving_mode == SavingModeEnum.SEPARATED_SAVING_MODE:
                         self._experiment_id = message.experiment_id
                         file_name = \
                             "{0}/{1}-{2}-{3}.csv".format(self.output_path,
-                                                        self.name,
-                                                        self._experiment_id,
-                                                        message.stimulus_id)
+                                                         self.name,
+                                                         self._experiment_id,
+                                                         message.stimulus_id)
                         self._save_to_file(file_name)
                         self._stream_data = []
                     else:
                         print("Shimmer stop")
                         self._experiment_id = message.experiment_id
                         self.__set_trigger(message)
                     self._state = "STOP"
@@ -251,15 +269,15 @@
                         "{0}/{1}-{2}.csv".format(self.output_path,
                                                  self.name,
                                                  self._experiment_id)
                     self._save_to_file(file_name)
                 break
 
         self._break_loop = True
-        loop_thread.join()
+        self._loop_thread.join()
 
     def __set_trigger(self, message: Message):
         '''
         Takes a message and set the trigger using its data
 
         Parameters
         -----------
@@ -323,15 +341,15 @@
                 GSR_ohm = rf/((gsr_to_volts / 0.5) - 1.0)
 
                 # convert PPG to milliVolt value
                 PPG_mv = PPG_raw * (3000.0/4095.0)
 
                 timestamp = timestamp0 + timestamp1*256 + timestamp2*65536
 
-                #print([packettype[0], timestamp, GSR_ohm, PPG_mv] + self._trigger)
+                # print([packettype[0], timestamp, GSR_ohm, PPG_mv] + self._trigger)
 
                 if self._trigger is not None:
                     print("Shimmer trigger")
                     row = [packettype[0],
                            timestamp,
                            x, y, z,
                            GSR_ohm,
@@ -378,26 +396,26 @@
             writer = csv.writer(csv_file)
             for row in self._stream_data:
                 writer.writerow(row)
                 csv_file.flush()
 
     def _get_realtime_data(self, duration: int) -> Dict[str, Any]:
         '''
-        Returns n seconds (duration) of latest collected data for monitoring/visualizing or 
+        Returns n seconds (duration) of latest collected data for monitoring/visualizing or
         realtime processing purposes.
 
         Parameters
         ----------
         duration: int
             A time duration in seconds for getting the latest recorded data in realtime
 
         Returns
         -------
         data: Dict[str, Any]
-            The keys are `data` and `metadata`.  
+            The keys are `data` and `metadata`.
             `data` is a list of records, or empty list if there's nothing.
             `metadata` is a dictionary of device metadata including `sampling_rate` and `type`
         '''
         # Last recorded data
         data = self._stream_data[-1 * duration * self._sampling_rate:]
         metadata = {"sampling_rate": self._sampling_rate,
                     "channels": ["type", "time stamp", "Acc_x", "Acc_y", "Acc_z",
```

### Comparing `octopus-sensing-4.0.3/octopus_sensing/preprocessing/__init__.py` & `octopus-sensing-4.1.0/octopus_sensing/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/preprocessing/openbci.py` & `octopus-sensing-4.1.0/octopus_sensing/preprocessing/openbci.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/preprocessing/openbci_brainflow.py` & `octopus-sensing-4.1.0/octopus_sensing/preprocessing/openbci_brainflow.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/preprocessing/preprocess_devices.py` & `octopus-sensing-4.1.0/octopus_sensing/preprocessing/preprocess_devices.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/preprocessing/shimmer3.py` & `octopus-sensing-4.1.0/octopus_sensing/preprocessing/shimmer3.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/preprocessing/utils.py` & `octopus-sensing-4.1.0/octopus_sensing/preprocessing/utils.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/questionnaire/__init__.py` & `octopus-sensing-4.1.0/octopus_sensing/questionnaire/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/questionnaire/opinion_question.py` & `octopus-sensing-4.1.0/octopus_sensing/questionnaire/opinion_question.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/questionnaire/question.py` & `octopus-sensing-4.1.0/octopus_sensing/questionnaire/question.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/questionnaire/questionnaire.py` & `octopus-sensing-4.1.0/octopus_sensing/questionnaire/questionnaire.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/questionnaire/text_question.py` & `octopus-sensing-4.1.0/octopus_sensing/questionnaire/text_question.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/realtime_data_endpoint.py` & `octopus-sensing-4.1.0/octopus_sensing/realtime_data_endpoint.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/stimuli/__init__.py` & `octopus-sensing-4.1.0/octopus_sensing/stimuli/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/stimuli/image_stimulus.py` & `octopus-sensing-4.1.0/octopus_sensing/stimuli/image_stimulus.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/stimuli/stimulus.py` & `octopus-sensing-4.1.0/octopus_sensing/stimuli/stimulus.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/stimuli/video_stimulus.py` & `octopus-sensing-4.1.0/octopus_sensing/stimuli/video_stimulus.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/__init__.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-00.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-00.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-01.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-02.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_continuous/OpenBCI-20-cont16-02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep01.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep02.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep03.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_16_sep/OpenBCI-20-sep03.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-00.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-00.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-01.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-02.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_continuous/OpenBCI-20-cont8-02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/preprocess_expected/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_16_continuous/OpenBCI-20-cont16.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_16_continuous/OpenBCI-20-cont16.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep01.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep02.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep03.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_16_sep/OpenBCI-20-sep03.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_8_continuous/OpenBCI-20-cont8.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_8_continuous/OpenBCI-20-cont8.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/OpenBCI_8_sep/OpenBCI-20-sep8-03.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/Shimmer_continuous/Shimmer-20-cont.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/Shimmer_continuous/Shimmer-20-cont.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep01.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep01.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep02.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep02.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep03.csv` & `octopus-sensing-4.1.0/octopus_sensing/tests/data/recorded/Shimmer_sep/Shimmer-20-sep03.csv`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/integration.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,26 +53,29 @@
         for _ in range(4 * 128):
             callback(MockSample(self._channels))
             # Sample rate: 128 per second
             time.sleep(1 / 128)
 
 
 class MockedSerial:
-    def __init__(self, port, speed):
+    def __init__(self, *args, **kwargs):
         pass
 
     def flushInput(self):
         pass
 
     def write(self, data):
         pass
 
     def close(self):
         pass
 
+    def is_open(self):
+        return True
+
     def read(self, size):
         if size == 1:
             # Asking for ack
             return struct.pack('B', 0xff)
         elif size == 9:
             # Enquiry configurations
             # Only byte 7 (number of channels) and byte 8 (buffer size) is used by the app.
```

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/test_audio_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/test_audio_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/test_brainflow_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/test_brainflow_streaming.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,14 +38,16 @@
         pass
     def prepare_session(self):
         pass
     def start_stream(self):
         pass
     def stop_stream(self):
         pass
+    def release_session(self):
+        pass
 
     def get_board_data(self):
         return (np.array([ [1,1],[1,1],[1,1] ]))
 
 
 @pytest.fixture(scope="module")
 def mocked():
@@ -71,15 +73,15 @@
     params = board_shim.BrainFlowInputParams()
     params.serial_port = "/dev/ttyUSB0"
     device = \
         brainflow_streaming.BrainFlowStreaming(2,
                                                125,
                                                brain_flow_input_params=params,
                                                name="cyton_daisy",
-                                               output_path=output_dir)    
+                                               output_path=output_dir)
     msg_queue = queue.Queue()
     device.set_queue(msg_queue)
     realtime_data_queue_in = queue.Queue()
     realtime_data_queue_out = queue.Queue()
     device.set_realtime_data_queues(realtime_data_queue_in, realtime_data_queue_out)
 
     device.start()
@@ -106,8 +108,7 @@
     assert len(os.listdir(brain_output)) == 1
     assert os.listdir(brain_output)[0] == filename
 
     filecontent = open(os.path.join(brain_output, filename), 'r').read()
     assert len(filecontent) >= 375
     # TODO: Check if the triggers are there.
     # TODO: We can check data in realtime data queues as well.
-
```

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/test_camera_streaming.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/test_camera_streaming.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/test_device_coordinator.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/test_device_coordinator.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/test_device_message_endpoint.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/test_device_message_endpoint.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/test_http_network_device.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/test_http_network_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/test_preprocess.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/tests/test_socket_network_device.py` & `octopus-sensing-4.1.0/octopus_sensing/tests/test_socket_network_device.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/windows/__init__.py` & `octopus-sensing-4.1.0/octopus_sensing/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/windows/image_window.py` & `octopus-sensing-4.1.0/octopus_sensing/windows/image_window.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/windows/message_window.py` & `octopus-sensing-4.1.0/octopus_sensing/windows/message_window.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/octopus_sensing/windows/timer_window.py` & `octopus-sensing-4.1.0/octopus_sensing/windows/timer_window.py`

 * *Files identical despite different names*

### Comparing `octopus-sensing-4.0.3/pyproject.toml` & `octopus-sensing-4.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry]
 name = "octopus-sensing"
-version = "4.0.3"
+version = "4.1.0"
 description = "Library for recording data synchronously from different physiological sensors"
 authors = ["Nastaran Saffaryazdi <nsaffar@gmail.com>", "Aidin Gharibnavaz <aidin@aidinhut.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 homepage = "https://octopus-sensing.nastaran-saffar.me"
 repository = "https://github.com/octopus-sensing/octopus-sensing"
 keywords = ["sensors", "eeg", "gsr", "recorder"]
```

### Comparing `octopus-sensing-4.0.3/setup.py` & `octopus-sensing-4.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 extras_require = \
 {':sys_platform != "win32"': ['PyGObject==3.40.1'],
  ':sys_platform == "linux"': ['bluepy>=1.3.0,<2.0.0']}
 
 setup_kwargs = {
     'name': 'octopus-sensing',
-    'version': '4.0.3',
+    'version': '4.1.0',
     'description': 'Library for recording data synchronously from different physiological sensors',
     'long_description': '<h2 align="center">Octopus Sensing</h2>\n<p align="center">\n  <img src="https://octopus-sensing.nastaran-saffar.me/_static/octopus-sensing-logo-small.png" alt="Octopus Sensing Logo">\n</p>\n<p align="center">\n  <img src="https://img.shields.io/github/workflow/status/octopus-sensing/octopus-sensing/Python%20Check?label=checks" alt="GitHub Workflow Status">\n  <img src="https://img.shields.io/codecov/c/gh/octopus-sensing/octopus-sensing" alt="Codecov">\n  <img src="https://img.shields.io/pypi/v/octopus-sensing" alt="PyPI">\n  <img src="https://img.shields.io/pypi/l/octopus-sensing" alt="PyPI - License">\n</p>\n\nOctopus Sensing is a tool to help you run scientific experiments that involve recording data synchronously from\nmultiple sources in human-computer interaction studies. You write steps of an experiment scenario, for example showing a stimulus and then a questionnaire. The tool takes care of the rest.\n\nIt can collect data from multiple devices such as OpenBCI EEG headset, Shimmer sensor (GSR and PPG),\nVideo and Audio and so forth simultaneously. Data collection can be started and stopped synchronously across all devices.\nCollected data will be tagged with the timestamp of the start and stop of the experiment, the ID of\nthe experiment, etc.\n\nThe aim is to make the scripting interface so simple that people with minimum or no software\ndevelopment skills can define experiment scenarios with no effort.\nAlso, this tool can be used as the base structure for creating real-time data processing systems like systems with capabilities of recognizing emotions, stress, cognitive load, or analyzing human behaviors.\n\n\n**To see the full documentation visit the [Octopus Sensing website](https://octopus-sensing.nastaran-saffar.me/).**\n\nWhen using the package in your research, please cite:\n-----------------------------------------------------\n\nSaffaryazdi, N., Gharibnavaz, A., & Billinghurst, M. (2022). Octopus Sensing: A Python library for human behavior studies. Journal of Open Source Software, 7(71), 4045.\n\nMain features\n--------------\n\n* Controls data recording from multiple sources using a simple unified interface\n* Tags an event on collected data, such as the start of an experiment, and events during the experiment, etc.\n* Can show stimuli (images and videos) and questionnaires\n* Monitoring interface that visualizes collected data in real-time\n* Offline visualization of data from multiple sources simultanously\n\nCopyright\n---------\nCopyright © 2020-2022 Nastaran Saffaryazdi, Aidin Gharibnavaz\n\nThis program is free software: you can redistribute it and/or modify it under the terms of the GNU\nGeneral Public License as published by the Free Software Foundation, either version 3 of the\nLicense, or (at your option) any later version.\n\nSee [License file](https://github.com/nastaran62/octopus-sensing/blob/master/LICENSE) for full terms.\n',
     'author': 'Nastaran Saffaryazdi',
     'author_email': 'nsaffar@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://octopus-sensing.nastaran-saffar.me',
```

### Comparing `octopus-sensing-4.0.3/PKG-INFO` & `octopus-sensing-4.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octopus-sensing
-Version: 4.0.3
+Version: 4.1.0
 Summary: Library for recording data synchronously from different physiological sensors
 Home-page: https://octopus-sensing.nastaran-saffar.me
 License: GPL-3.0-or-later
 Keywords: sensors,eeg,gsr,recorder
 Author: Nastaran Saffaryazdi
 Author-email: nsaffar@gmail.com
 Requires-Python: >=3.7.1,<4.0
```

