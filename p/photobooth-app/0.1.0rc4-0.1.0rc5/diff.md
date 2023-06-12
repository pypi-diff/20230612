# Comparing `tmp/photobooth_app-0.1.0rc4.tar.gz` & `tmp/photobooth_app-0.1.0rc5.tar.gz`

## Comparing `photobooth_app-0.1.0rc4.tar` & `photobooth_app-0.1.0rc5.tar`

### file list

```diff
@@ -1,138 +1,138 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/__init__.py
--rw-r--r--   0        0        0     3726 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/__main__.py
--rw-r--r--   0        0        0    17065 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/appconfig.py
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/application.py
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/containers.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/__init__.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/aquisition.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/config.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/home.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/log.py
--rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/mediacollection.py
--rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/mediaprocessing.py
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/processing.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/sse.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/routers/system.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/__init__.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/aquisitionservice.py
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/baseservice.py
--rw-r--r--   0        0        0     3207 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/containers.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/informationservice.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/keyboardservice.py
--rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/loggingservice.py
--rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/mediacollectionservice.py
--rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/mediaprocessingservice.py
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/processingservice.py
--rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/systemservice.py
--rw-r--r--   0        0        0     5647 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/wledservice.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/assets/systemservice/boothupload.service
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/assets/systemservice/boothupload.sh
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/assets/systemservice/photobooth-app.service
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/__init__.py
--rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/abstractbackend.py
--rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/containers.py
--rw-r--r--   0        0        0    10517 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/gphoto2.py
--rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/picamera2.py
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/picamera2_libcamafcontinuous.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/picamera2_libcamafinterval.py
--rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/simulated.py
--rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/webcamcv2.py
--rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/webcamv4l.py
--rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
--rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
--rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
--rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
--rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
--rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
--rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/mediacollection/__init__.py
--rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/mediacollection/mediaitem.py
--rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/services/mediaprocessing/image_pipelinestages.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/utils/exceptions.py
--rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/utils/fastapi_get_openapi.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/utils/helper.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/utils/repeatedtimer.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/utils/stoppablethread.py
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/LICENSE.txt
--rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
--rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
--rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
--rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
--rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
--rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
--rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
--rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
--rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
--rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
--rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
--rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/.gitattributes
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/.gitignore
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/CHANGES.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/LICENSE.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/MANIFEST.in
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/Makefile
--rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/README.md
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/make_release.py
--rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/setup.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/write.py
--rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/__init__.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/__main__.py
--rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
--rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
--rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_generic.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
--rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
--rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
--rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
--rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
--rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/mouse.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/index.html
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/css/31.363e41a9.css
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/css/706.42cb67d0.css
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/css/71.0be6c807.css
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/css/app.f5a22106.css
--rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/css/vendor.46e03c42.css
--rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
--rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/icons/favicon-128x128.png
--rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/icons/logo-notext-black-transparent.png
--rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/icons/logo-text-black-transparent.png
--rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/icons/logo-text-white-transparent.png
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/247.74c0e45d.js
--rw-r--r--   0        0        0     9915 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/31.51d7e662.js
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/391.70a80bd8.js
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/429.76096bfa.js
--rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/546.92b02def.js
--rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/705.fc48b137.js
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/706.f32434a0.js
--rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/71.3aaf5d7d.js
--rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/862.525f2f13.js
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/863.e0c5ac02.js
--rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/954.7419ae78.js
--rw-r--r--   0        0        0    12591 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/app.3153eea4.js
--rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/photobooth/web_spa/js/vendor.c9e02ba9.js
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/LICENSE.md
--rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/README.md
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/pyproject.toml
--rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc4/PKG-INFO
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/__init__.py
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/__main__.py
+-rw-r--r--   0        0        0    17072 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/appconfig.py
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/application.py
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/containers.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/__init__.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/aquisition.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/config.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/home.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/log.py
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/mediacollection.py
+-rw-r--r--   0        0        0     3390 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/mediaprocessing.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/processing.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/sse.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/routers/system.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/__init__.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/aquisitionservice.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/baseservice.py
+-rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/containers.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/informationservice.py
+-rw-r--r--   0        0        0     2528 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/keyboardservice.py
+-rw-r--r--   0        0        0     6280 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/loggingservice.py
+-rw-r--r--   0        0        0     6010 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediacollectionservice.py
+-rw-r--r--   0        0        0    10102 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediaprocessingservice.py
+-rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/processingservice.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/systemservice.py
+-rw-r--r--   0        0        0     5687 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/wledservice.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/assets/systemservice/boothupload.service
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/assets/systemservice/boothupload.sh
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/assets/systemservice/photobooth-app.service
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/__init__.py
+-rw-r--r--   0        0        0     7195 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/abstractbackend.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/containers.py
+-rw-r--r--   0        0        0    11212 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/gphoto2.py
+-rw-r--r--   0        0        0    16283 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2.py
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2_libcamafcontinuous.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2_libcamafinterval.py
+-rw-r--r--   0        0        0     6965 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/simulated.py
+-rw-r--r--   0        0        0    10084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/webcamcv2.py
+-rw-r--r--   0        0        0     7595 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/webcamv4l.py
+-rw-r--r--   0        0        0    43739 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg
+-rw-r--r--   0        0        0    11560 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   710982 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg
+-rw-r--r--   0        0        0   585221 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg
+-rw-r--r--   0        0        0   865667 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg
+-rw-r--r--   0        0        0  2314332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg
+-rw-r--r--   0        0        0  2126411 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediacollection/__init__.py
+-rw-r--r--   0        0        0     6853 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediacollection/mediaitem.py
+-rw-r--r--   0        0        0     1934 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/services/mediaprocessing/image_pipelinestages.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/exceptions.py
+-rw-r--r--   0        0        0      430 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/fastapi_get_openapi.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/helper.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/repeatedtimer.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/utils/stoppablethread.py
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/LICENSE.txt
+-rw-r--r--   0        0        0   168060 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf
+-rw-r--r--   0        0        0   174108 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf
+-rw-r--r--   0        0        0   167336 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf
+-rw-r--r--   0        0        0   171508 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf
+-rw-r--r--   0        0        0   170504 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf
+-rw-r--r--   0        0        0   167000 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf
+-rw-r--r--   0        0        0   173172 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf
+-rw-r--r--   0        0        0   168644 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf
+-rw-r--r--   0        0        0   173416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf
+-rw-r--r--   0        0        0   168260 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf
+-rw-r--r--   0        0        0   168488 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf
+-rw-r--r--   0        0        0   172860 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/.gitattributes
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/.gitignore
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/CHANGES.md
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/LICENSE.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/MANIFEST.in
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/Makefile
+-rw-r--r--   0        0        0    29447 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/README.md
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/make_release.py
+-rw-r--r--   0        0        0     1333 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/setup.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/10_second_macro.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/customizable_hotkey.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/pressed_keys.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/segmented_macro.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/simulate_held_down.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/write.py
+-rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/__main__.py
+-rw-r--r--   0        0        0    29387 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py
+-rw-r--r--   0        0        0    19352 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py
+-rw-r--r--   0        0        0     6457 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py
+-rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_generic.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py
+-rw-r--r--   0        0        0    36792 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_mouse_event.py
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py
+-rw-r--r--   0        0        0     5947 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py
+-rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py
+-rw-r--r--   0        0        0     3384 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py
+-rw-r--r--   0        0        0    20549 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py
+-rw-r--r--   0        0        0     5804 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/mouse.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/index.html
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/272.0be6c807.css
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/706.28b224d0.css
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/835.eb55e979.css
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/app.f5a22106.css
+-rw-r--r--   0        0        0   208939 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/css/vendor.46e03c42.css
+-rw-r--r--   0        0        0    20436 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+-rw-r--r--   0        0        0    20544 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-r--r--   0        0        0    20416 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-r--r--   0        0        0    20408 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-r--r--   0        0        0    20424 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-r--r--   0        0        0    20344 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-r--r--   0        0        0   164912 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/icons/favicon-128x128.png
+-rw-r--r--   0        0        0     4844 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-notext-black-transparent.png
+-rw-r--r--   0        0        0    10435 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-text-black-transparent.png
+-rw-r--r--   0        0        0     8328 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-text-white-transparent.png
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/247.74c0e45d.js
+-rw-r--r--   0        0        0     5553 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/272.a73245eb.js
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/391.70a80bd8.js
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/429.76096bfa.js
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/546.92b02def.js
+-rw-r--r--   0        0        0     3924 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/705.fc48b137.js
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/706.1c5cc1da.js
+-rw-r--r--   0        0        0     9742 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/835.70f6a199.js
+-rw-r--r--   0        0        0      778 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/862.525f2f13.js
+-rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/863.e0c5ac02.js
+-rw-r--r--   0        0        0     7393 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/954.7419ae78.js
+-rw-r--r--   0        0        0    12636 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/app.64608eed.js
+-rw-r--r--   0        0        0  1417500 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/photobooth/web_spa/js/vendor.c9e02ba9.js
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/LICENSE.md
+-rw-r--r--   0        0        0     3392 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/README.md
+-rw-r--r--   0        0        0     3332 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     5147 2020-02-02 00:00:00.000000 photobooth_app-0.1.0rc5/PKG-INFO
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/__main__.py` & `photobooth_app-0.1.0rc5/photobooth/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -58,51 +58,45 @@
 
     # adjust logging after uvicorn setup
     logging_service.uvicorn()
 
     return server
 
 
-def _guard(ip: str, port: int):
+def main(run_server: bool = True):
     # guard to start only one instance at a time.
     try:
         s = socket.socket()
-        s.bind((ip, port))  # bind fails on second instance, raising OSError
-        s.close()
+        s.bind(("localhost", 19988))  # bind fails on second instance, raising OSError
     except OSError as exc:
         print("startup aborted. another instance is running. exiting.")
         logger.critical("startup aborted. another instance is running. exiting.")
-        raise SystemExit("webserver port not avail") from exc
-
+        raise SystemExit("only one instance allowed") from exc
 
-def main(run_server: bool = True):
     application_container = ApplicationContainer()
 
     # use to construct paths in app referring to assets
     logger.info(f"photobooth directory: {Path(__file__).parent.resolve()}")
     # use to construct paths to user data
     logger.info(f"working directory: {Path.cwd().resolve()}")
     # __version__ = importlib.metadata.version("photobooth-app")
     # logger.info(f"{__version__=}")
 
-    # allow one instance at a time, set whether webserver port is avail as sign it's good or not
-    _guard(
-        application_container.config().common.webserver_bind_ip,
-        application_container.config().common.webserver_port,
-    )
-
     application_container.init_resources()
     application_container.wire(modules=[__name__], packages=[".routers"])
 
     # start main application
     server = _server()
 
     # serve, loops endless
     # this one is not executed in tests because it's not stoppable from within
     if run_server:
         server.run()
 
+    # close single instance port
+    s.close()
+
     application_container.shutdown_resources()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/appconfig.py` & `photobooth_app-0.1.0rc5/photobooth/appconfig.py`

 * *Files 3% similar despite different names*

```diff
@@ -251,33 +251,47 @@
 class EnumPilgramFilter(str, Enum):
     """enum to choose image filter from, pilgram filter"""
 
     original = "original"
 
     _1977 = "_1977"
     aden = "aden"
+    ashby = "ashby"
+    amaro = "amaro"
     brannan = "brannan"
     brooklyn = "brooklyn"
+    charmes = "charmes"
     clarendon = "clarendon"
+    crema = "crema"
+    dogpatch = "dogpatch"
     earlybird = "earlybird"
     gingham = "gingham"
+    ginza = "ginza"
+    hefe = "hefe"
+    helena = "helena"
     hudson = "hudson"
     inkwell = "inkwell"
+    juno = "juno"
     kelvin = "kelvin"
     lark = "lark"
     lofi = "lofi"
+    ludwig = "ludwig"
     maven = "maven"
     mayfair = "mayfair"
     moon = "moon"
     nashville = "nashville"
     perpetua = "perpetua"
+    poprocket = "poprocket"
     reyes = "reyes"
     rise = "rise"
+    sierra = "sierra"
+    skyline = "skyline"
     slumber = "slumber"
     stinson = "stinson"
+    sutro = "sutro"
     toaster = "toaster"
     valencia = "valencia"
     walden = "walden"
     willow = "willow"
     xpro2 = "xpro2"
 
 
@@ -297,48 +311,54 @@
     class Config:
         title = "Process media after capture"
 
     pic1_enable_pipeline: bool = Field(
         default=False,
         description="Enable/Disable 1pic processing pipeline completely",
     )
-
     pic1_filter: EnumPilgramFilter = Field(
         title="Pic1 Filter",
         default=EnumPilgramFilter.original,
         description="Instagram-like filter to apply per default. 'original' applies no filter.",
     )
-    """#TODO:
-    pic1_filter_userselectable: list[EnumPilgramFilter] = Field(
-        title="Pic1 Filter Userselectable",
-        default=[EnumPilgramFilter.original, EnumPilgramFilter._1977],
-        description="Filter the user may choose from in the gallery. 'original' applies no filter.",
-    )
-    """
     pic1_text_overlay: list[TextStageConfig] = Field(
         default=[],
         description="Text to overlay on images after capture. Pos_x/Pos_y measure in pixel starting 0/0 at top-left in image. Font to use in text stages. File needs to be located in DATA_DIR/fonts/",
     )
 
 
-class GroupHardwareInput(BaseModel):
-    """Configure GPIO, keyboard and more."""
+class GroupHardwareInputOutput(BaseModel):
+    """
+    Configure hardware GPIO, keyboard and more. Find integration information in the documentation.
+    """
 
     class Config:
         title = "Hardware Input/Output Config"
 
+    # keyboardservice config
     keyboard_input_enabled: bool = Field(
         default=False,
         description="Enable keyboard input globally",
     )
     keyboard_input_keycode_takepic: str = Field(
         default="down",
         description="Keycode triggers capture of one image",
     )
 
+    # WledService Config
+    wled_enabled: bool = Field(
+        default=False,
+        description="Enable WLED integration for user feedback during countdown and capture by LEDs.",
+    )
+    wled_serial_port: str = Field(
+        default="",
+        description="Serial port the WLED device is connected to.",
+    )
+
+
 
 class GroupUiSettings(BaseModel):
     """Personalize the booth's UI."""
 
     class Config:
         title = "Personalize the User Interface"
 
@@ -371,56 +391,36 @@
         description="Show link to admin center, usually only during setup.",
     )
     EXT_DOWNLOAD_URL: str = Field(
         default="http://dl.qbooth.net/{filename}",
         description="URL encoded by QR code to download images from onlineservice. {filename} is replaced by actual filename",
     )
     gallery_show_filter: bool = Field(
-        default=False,
+        default=True,
         description="",
     )
+    gallery_filter_userselectable: list[EnumPilgramFilter] = Field(
+        title="Pic1 Filter Userselectable",
+        default=[EnumPilgramFilter.original, EnumPilgramFilter.clarendon, EnumPilgramFilter.moon],
+        description="Filter the user may choose from in the gallery. 'original' applies no filter.",
+    )
     gallery_show_download: bool = Field(
-        default=False,
+        default=True,
         description="",
     )
     gallery_show_delete: bool = Field(
-        default=False,
+        default=True,
         description="",
     )
     gallery_show_print: bool = Field(
-        default=False,
+        default=True,
         description="",
     )
 
 
-class GroupWled(BaseModel):
-    """
-    WLED integration for countdown led / shoot animation
-    needs WLED module connected via USB serial port and
-    three presets:
-    1: standby (usually LEDs off)
-    2: countdown (animates countdown)
-    3: shoot (imitate a flash)
-    Please define presets on your own in WLED webfrontend
-    """
-
-    class Config:
-        title = "WLED Integration Config"
-
-    # WledService Config
-    ENABLED: bool = Field(
-        default=False,
-        description="Enable WLED integration for user feedback during countdown and capture by LEDs.",
-    )
-    SERIAL_PORT: str = Field(
-        default="",
-        description="Serial port the WLED device is connected to.",
-    )
-
-
 class GroupMisc(BaseModel):
     """
     Quite advanced, usually not necessary to touch.
     """
 
     class Config:
         title = "Miscellaneous Config"
@@ -458,16 +458,15 @@
     _processed_at: datetime = PrivateAttr(default_factory=datetime.now)  # private attributes
 
     # groups -> setting items
     common: GroupCommon = GroupCommon()
     mediaprocessing: GroupMediaprocessing = GroupMediaprocessing()
     uisettings: GroupUiSettings = GroupUiSettings()
     backends: GroupBackends = GroupBackends()
-    wled: GroupWled = GroupWled()
-    hardwareinput: GroupHardwareInput = GroupHardwareInput()
+    hardwareinputoutput: GroupHardwareInputOutput = GroupHardwareInputOutput()
     misc: GroupMisc = GroupMisc()
 
     class Config:
         """
         pydantic config class modified
         """
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/application.py` & `photobooth_app-0.1.0rc5/photobooth/application.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/containers.py` & `photobooth_app-0.1.0rc5/photobooth/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/aquisition.py` & `photobooth_app-0.1.0rc5/photobooth/routers/aquisition.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/config.py` & `photobooth_app-0.1.0rc5/photobooth/routers/config.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/home.py` & `photobooth_app-0.1.0rc5/photobooth/routers/home.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/log.py` & `photobooth_app-0.1.0rc5/photobooth/routers/log.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/mediacollection.py` & `photobooth_app-0.1.0rc5/photobooth/routers/mediacollection.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/mediaprocessing.py` & `photobooth_app-0.1.0rc5/photobooth/routers/mediaprocessing.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/processing.py` & `photobooth_app-0.1.0rc5/photobooth/routers/processing.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
 from dependency_injector.wiring import Provide, inject
 from fastapi import APIRouter, Depends, HTTPException
 
 from ..containers import ApplicationContainer
 from ..services.processingservice import ProcessingService
+from ..utils.exceptions import ProcessMachineOccupiedError
 
 logger = logging.getLogger(__name__)
 processing_router = APIRouter(
     prefix="/processing",
     tags=["processing"],
 )
 
@@ -18,20 +19,20 @@
 @inject
 def api_chose_1pic_get(
     processing_service: ProcessingService = Depends(Provide[ApplicationContainer.services.processing_service]),
 ):
     try:
         processing_service.evt_chose_1pic_get()
         return "OK"
-    except RuntimeError as exc:
+    except ProcessMachineOccupiedError as exc:
         # raised if processingservice not idle
         raise HTTPException(
             status_code=400,
             detail=f"only one capture at a time allowed: {exc}",
         ) from exc
     except Exception as exc:
         # other errors
-        logger.exception(exc)
+        logger.critical(exc)
         raise HTTPException(
             status_code=500,
             detail=f"something went wrong, Exception: {exc}",
         ) from exc
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/sse.py` & `photobooth_app-0.1.0rc5/photobooth/routers/sse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/routers/system.py` & `photobooth_app-0.1.0rc5/photobooth/routers/system.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/aquisitionservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/aquisitionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/containers.py` & `photobooth_app-0.1.0rc5/photobooth/services/containers.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         primary=primary,
         secondary=secondary,
     )
     try:
         resource.start()
     except Exception as exc:
         logger.critical(f"failed to start acquisition {exc}")
+        raise RuntimeError(f"cannot start backend, app fails, check configuration {exc}") from exc
     else:
         yield resource
         resource.stop()
     finally:
         pass
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/informationservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/informationservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/keyboardservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/keyboardservice.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 sshkeyboard: ?
 """
 import json
 
 from pymitter import EventEmitter
 
 from ..appconfig import AppConfig
+from ..utils.exceptions import ProcessMachineOccupiedError
 from ..vendor.packages.keyboard import keyboard
 from .baseservice import BaseService
 from .processingservice import ProcessingService
 
 
 class KeyboardService(BaseService):
     """_summary_"""
@@ -29,15 +30,15 @@
         config: AppConfig,
         processing_service: ProcessingService,
     ):
         super().__init__(evtbus=evtbus, config=config)
 
         self._processing_service = processing_service
 
-        if self._config.hardwareinput.keyboard_input_enabled:
+        if self._config.hardwareinputoutput.keyboard_input_enabled:
             self._logger.info("keyboardservice enabled - listeners installed")
             keyboard.on_press(self._on_key_callback)
         else:
             self._logger.info("keyboardservice not enabled - enable for keyboard triggers")
 
     def _on_key_callback(self, key):
         """_summary_
@@ -50,10 +51,21 @@
         # log to http sse helps finding the right key watching live logs
         self._evtbus.emit(
             "publishSSE",
             sse_event="information",
             sse_data=json.dumps({"lastkeycode": key.name}),
         )
 
-        if key.name == self._config.hardwareinput.keyboard_input_keycode_takepic:
-            self._logger.info(f"{self._config.hardwareinput.keyboard_input_keycode_takepic=}")
-            self._processing_service.evt_chose_1pic_get()
+        if key.name == self._config.hardwareinputoutput.keyboard_input_keycode_takepic:
+            self._logger.info(f"got key.name={self._config.hardwareinputoutput.keyboard_input_keycode_takepic}")
+            self._logger.info("trigger evt_chose_1pic_get")
+
+            try:
+                self._processing_service.evt_chose_1pic_get()
+            except ProcessMachineOccupiedError as exc:
+                # raised if processingservice not idle
+                self._logger.warning(f"only one capture at a time allowed, request ignored: {exc}")
+            except Exception as exc:
+                # other errors
+                self._logger.critical(exc)
+
+
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/loggingservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/loggingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/mediacollectionservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/mediacollectionservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/mediaprocessingservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/mediaprocessingservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/processingservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/processingservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from dataclasses import asdict, dataclass
 from threading import Thread
 
 from pymitter import EventEmitter
 from statemachine import State, StateMachine
 
 from ..appconfig import AppConfig
+from ..utils.exceptions import ProcessMachineOccupiedError
 from .aquisitionservice import AquisitionService
 from .mediacollection.mediaitem import MediaItem, MediaItemTypes, get_new_filename
 from .mediacollectionservice import (
     MediacollectionService,
 )
 from .mediaprocessingservice import MediaprocessingService
 
@@ -212,37 +213,41 @@
             except TimeoutError:
                 logger.error(f"error capture image. timeout expired {attempt=}/{MAX_ATTEMPTS}, retrying")
                 # can we do additional error handling here?
             else:
                 break
         else:
             # we failed finally all the attempts - deal with the consequences.
-            logger.critical(
-                "critical error capture image. " f"failed to get image after {MAX_ATTEMPTS} attempts. giving up!"
-            )
+            logger.critical(f"finally failed after {MAX_ATTEMPTS} attempts to capture image!")
             raise RuntimeError(f"finally failed after {MAX_ATTEMPTS} attempts to capture image!")
 
         logger.info(f"-- process time: {round((time.time() - start_time_capture), 2)}s to capture still")
 
     def on_exit_capture_still(self):
         """_summary_"""
         self._evtbus.emit("statemachine/on_exit_capture_still")
 
     ### some external functions
 
     def evt_chose_1pic_get(self):
         logger.info("evt_chose_1pic_get called to take picture")
         if not self.idle.is_active:
-            raise RuntimeError("bad request, only one request at a time!")
+            raise ProcessMachineOccupiedError("bad request, only one request at a time!")
+
+        try:
+            self.thrill()
+            self.countdown()
+            self.shoot()
+            self.postprocess()
+            self.finalize()
+        except Exception as exc:
+            logger.critical(f"something went wrong :( {exc}")
+            self._reset()
+            raise RuntimeError(f"something went wrong :( {exc}") from exc
 
-        self.thrill()
-        self.countdown()
-        self.shoot()
-        self.postprocess()
-        self.finalize()
 
     ### some custom helper
 
     def _sse_initial_processinfo(self):
         """_summary_"""
         self._sse_processinfo(__class__.Stateinfo(state=self.current_state.id))
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/systemservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/systemservice.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/wledservice.py` & `photobooth_app-0.1.0rc5/photobooth/services/wledservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 class WledService(BaseService):
     """_summary_"""
 
     def __init__(self, evtbus: EventEmitter, config: AppConfig):
         super().__init__(evtbus, config=config)
 
-        self._enabled = config.wled.ENABLED
-        self._serial_port = config.wled.SERIAL_PORT
+        self._enabled = config.hardwareinputoutput.wled_enabled
+        self._serial_port = config.hardwareinputoutput.wled_serial_port
 
         self._serial: serial.Serial = None
 
     def start(self):
         """_summary_
 
         Returns:
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/assets/systemservice/photobooth-app.service` & `photobooth_app-0.1.0rc5/photobooth/services/assets/systemservice/photobooth-app.service`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/abstractbackend.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/abstractbackend.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/containers.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/containers.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/gphoto2.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/gphoto2.py`

 * *Files 3% similar despite different names*

```diff
@@ -258,30 +258,48 @@
                     logger.info("disable viewfinder before capture")
                     self._viewfinder(0)
 
                 self._evtbus.emit("frameserver/onCapture")
 
                 # capture hq picture
                 logger.info("taking hq picture")
-                file_path = self._camera.capture(gp.GP_CAPTURE_IMAGE)
-                logger.info(f"Camera file path: {file_path.folder}/{file_path.name}")
+                try:
+                    file_path = self._camera.capture(gp.GP_CAPTURE_IMAGE)
 
-                if self._config.backends.gphoto2_wait_event_after_capture_trigger:
-                    self._camera.wait_for_event(1000)
+                    logger.info(f"Camera file path: {file_path.folder}/{file_path.name}")
 
-                camera_file = self._camera.file_get(
-                    file_path.folder,
-                    file_path.name,
-                    gp.GP_FILE_TYPE_NORMAL,
-                )
+                except gp.GPhoto2Error as exc:
+                    logger.critical(f"error capture! check logs for errors. {exc}")
+
+                    # inform finished anyway to signal WLED turn off lights
+                    self._evtbus.emit("frameserver/onCaptureFinished")
+
+                    # try again in next loop
+                    continue
 
                 self._evtbus.emit("frameserver/onCaptureFinished")
 
-                file_data = camera_file.get_data_and_size()
-                img_bytes = memoryview(file_data).tobytes()
+                # read from camera
+                try:
+                    if self._config.backends.gphoto2_wait_event_after_capture_trigger:
+                        self._camera.wait_for_event(1000)
+
+                    camera_file = self._camera.file_get(
+                        file_path.folder,
+                        file_path.name,
+                        gp.GP_FILE_TYPE_NORMAL,
+                    )
+
+                    file_data = camera_file.get_data_and_size()
+                    img_bytes = memoryview(file_data).tobytes()
+                except gp.GPhoto2Error as exc:
+                    logger.critical(f"error reading camera file! check logs for errors. {exc}")
+
+                    # try again in next loop
+                    continue
 
                 with self._hires_data.condition:
                     self._hires_data.data = img_bytes
 
                     self._hires_data.condition.notify_all()
 
             # self._count += 1
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/picamera2.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/picamera2_libcamafcontinuous.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2_libcamafcontinuous.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/picamera2_libcamafinterval.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/picamera2_libcamafinterval.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/simulated.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/simulated.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/webcamcv2.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/webcamcv2.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/webcamv4l.py` & `photobooth_app-0.1.0rc5/photobooth/services/backends/webcamv4l.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg` & `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/simulated_background.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt` & `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/fonts/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg` & `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/13-2500x1667.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg` & `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/21-3008x2008.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg` & `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/27-3264x1836.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg` & `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/28-4928x3264.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg` & `photobooth_app-0.1.0rc5/photobooth/services/backends/assets/backend_simulated/hq_img/29-4000x2670.jpg`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/mediacollection/mediaitem.py` & `photobooth_app-0.1.0rc5/photobooth/services/mediacollection/mediaitem.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/services/mediaprocessing/image_pipelinestages.py` & `photobooth_app-0.1.0rc5/photobooth/services/mediaprocessing/image_pipelinestages.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/utils/repeatedtimer.py` & `photobooth_app-0.1.0rc5/photobooth/utils/repeatedtimer.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/utils/stoppablethread.py` & `photobooth_app-0.1.0rc5/photobooth/utils/stoppablethread.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/LICENSE.txt` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-BlackItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Italic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Medium.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-MediumItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-Thin.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf` & `photobooth_app-0.1.0rc5/photobooth/vendor/fonts/Roboto/Roboto-ThinItalic.ttf`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/.gitignore` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/.gitignore`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/CHANGES.md` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/CHANGES.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/LICENSE.txt` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/Makefile` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/Makefile`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/README.md` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/make_release.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/make_release.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/setup.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/setup.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/push_to_talk_ubuntu.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/segmented_macro.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/segmented_macro.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/examples/stdin_stdout_events.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/__init__.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_canonical_names.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_darwinkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_darwinmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_generic.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_generic.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_event.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_keyboard_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_mouse_tests.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixcommon.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_nixmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_winkeyboard.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/_winmouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/vendor/packages/keyboard/keyboard/mouse.py` & `photobooth_app-0.1.0rc5/photobooth/vendor/packages/keyboard/keyboard/mouse.py`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/index.html` & `photobooth_app-0.1.0rc5/photobooth/web_spa/index.html`

 * *Files 4% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>qPhotobooth</title><meta charset=utf-8><meta name=description content=qPhotobooth><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><script defer src=js/vendor.c9e02ba9.js></script><script defer src=js/app.3153eea4.js></script><link href=css/vendor.46e03c42.css rel=stylesheet><link href=css/app.f5a22106.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>qPhotobooth</title><meta charset=utf-8><meta name=description content=qPhotobooth><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><script defer src=js/vendor.c9e02ba9.js></script><script defer src=js/app.64608eed.js></script><link href=css/vendor.46e03c42.css rel=stylesheet><link href=css/app.f5a22106.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/css/vendor.46e03c42.css` & `photobooth_app-0.1.0rc5/photobooth/web_spa/css/vendor.46e03c42.css`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2` & `photobooth_app-0.1.0rc5/photobooth/web_spa/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.c5371cfb.woff2`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/icons/favicon-128x128.png` & `photobooth_app-0.1.0rc5/photobooth/web_spa/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/icons/logo-notext-black-transparent.png` & `photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-notext-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/icons/logo-text-black-transparent.png` & `photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-text-black-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/icons/logo-text-white-transparent.png` & `photobooth_app-0.1.0rc5/photobooth/web_spa/icons/logo-text-white-transparent.png`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/247.74c0e45d.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/247.74c0e45d.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/31.51d7e662.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/835.70f6a199.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,119 +1,119 @@
 "use strict";
 (globalThis["webpackChunkqPhotobooth"] = globalThis["webpackChunkqPhotobooth"] || []).push([
-    [31], {
-        666: (e, t, i) => {
+    [835], {
+        9815: (e, t, i) => {
             i.d(t, {
                 Z: () => W
             });
             var l = i(9835),
-                a = i(6970);
-            const r = {
+                r = i(6970);
+            const a = {
                     class: "q-mr-sm"
                 },
                 o = {
                     class: "q-mr-sm"
                 },
                 n = {
                     class: "absolute-bottom-left text-subtitle2"
                 },
                 s = {
                     class: "q-gutter-sm"
                 };
 
-            function d(e, t, i, d, m, g) {
-                const c = (0, l.up)("q-btn"),
+            function d(e, t, i, d, g, c) {
+                const m = (0, l.up)("q-btn"),
                     u = (0, l.up)("q-space"),
                     h = (0, l.up)("q-icon"),
                     p = (0, l.up)("q-toolbar"),
-                    w = (0, l.up)("q-linear-progress"),
-                    y = (0, l.up)("q-header"),
+                    y = (0, l.up)("q-linear-progress"),
+                    w = (0, l.up)("q-header"),
                     S = (0, l.up)("q-img"),
                     I = (0, l.up)("q-drawer"),
                     f = (0, l.up)("q-carousel-slide"),
                     v = (0, l.up)("q-carousel"),
                     b = (0, l.up)("vue-qrcode"),
-                    k = (0, l.up)("q-page-sticky"),
+                    _ = (0, l.up)("q-page-sticky"),
                     q = (0, l.up)("q-page-container"),
-                    _ = (0, l.up)("q-layout"),
-                    x = (0, l.Q2)("close-popup"),
-                    D = (0, l.Q2)("touch-swipe");
-                return (0, l.wg)(), (0, l.j4)(_, {
+                    k = (0, l.up)("q-layout"),
+                    D = (0, l.Q2)("close-popup"),
+                    x = (0, l.Q2)("touch-swipe");
+                return (0, l.wg)(), (0, l.j4)(k, {
                     view: "hhh Lpr ffr",
-                    onClick: g.abortTimer
+                    onClick: c.abortTimer
                 }, {
-                    default: (0, l.w5)((() => [(0, l.Wm)(y, {
+                    default: (0, l.w5)((() => [(0, l.Wm)(w, {
                         elevated: "",
                         class: "bg-primary text-white"
                     }, {
                         default: (0, l.w5)((() => [(0, l.Wm)(p, null, {
-                            default: (0, l.w5)((() => [(0, l.wy)((0, l.Wm)(c, {
+                            default: (0, l.w5)((() => [(0, l.wy)((0, l.Wm)(m, {
                                 dense: "",
                                 flat: "",
                                 icon: "close"
                             }, null, 512), [
-                                [x]
-                            ]), (0, l.Wm)(u), d.uiSettingsStore.uiSettings.gallery_show_delete ? (0, l.wy)(((0, l.wg)(), (0, l.j4)(c, {
+                                [D]
+                            ]), (0, l.Wm)(u), d.uiSettingsStore.uiSettings.gallery_show_delete ? (0, l.wy)(((0, l.wg)(), (0, l.j4)(m, {
                                 key: 0,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "delete",
                                 label: "Delete",
-                                onClick: t[0] || (t[0] = e => g.deleteImage(d.currentSlideId))
+                                onClick: t[0] || (t[0] = e => c.deleteImage(d.currentSlideId))
                             }, null, 512)), [
-                                [x]
-                            ]) : (0, l.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_download ? ((0, l.wg)(), (0, l.j4)(c, {
+                                [D]
+                            ]) : (0, l.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_download ? ((0, l.wg)(), (0, l.j4)(m, {
                                 key: 1,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "download",
                                 label: "Download",
                                 onClick: t[1] || (t[1] = e => {
                                     d.openURL(i.itemRepository[d.currentSlideIndex]["full"])
                                 })
-                            })) : (0, l.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_print ? ((0, l.wg)(), (0, l.j4)(c, {
+                            })) : (0, l.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_print ? ((0, l.wg)(), (0, l.j4)(m, {
                                 key: 2,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "print",
                                 label: "Print"
-                            })) : (0, l.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_filter ? ((0, l.wg)(), (0, l.j4)(c, {
+                            })) : (0, l.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_filter && d.uiSettingsStore.uiSettings.gallery_filter_userselectable.length > 0 ? ((0, l.wg)(), (0, l.j4)(m, {
                                 key: 3,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "filter",
                                 label: "Filter",
                                 onClick: d.toggleRightDrawer
-                            }, null, 8, ["onClick"])) : (0, l.kq)("", !0), (0, l.Wm)(u), (0, l._)("div", r, [(0, l.Wm)(h, {
+                            }, null, 8, ["onClick"])) : (0, l.kq)("", !0), (0, l.Wm)(u), (0, l._)("div", a, [(0, l.Wm)(h, {
                                 name: "tag"
-                            }), (0, l._)("span", null, (0, a.zw)(d.currentSlideIndex + 1) + " of " + (0, a.zw)(i.itemRepository.length) + " total", 1)]), (0, l.Wm)(u), (0, l._)("div", o, [(0, l.Wm)(h, {
+                            }), (0, l._)("span", null, (0, r.zw)(d.currentSlideIndex + 1) + " of " + (0, r.zw)(i.itemRepository.length) + " total", 1)]), (0, l.Wm)(u), (0, l._)("div", o, [(0, l.Wm)(h, {
                                 name: "image"
-                            }), (0, l.Uk)(" " + (0, a.zw)(i.itemRepository[d.currentSlideIndex]["caption"]), 1)])])),
+                            }), (0, l.Uk)(" " + (0, r.zw)(i.itemRepository[d.currentSlideIndex]["caption"]), 1)])])),
                             _: 1
-                        }), m.displayLinearProgressBar && m.remainingSeconds > 0 ? ((0, l.wg)(), (0, l.j4)(w, {
+                        }), g.displayLinearProgressBar && g.remainingSeconds > 0 ? ((0, l.wg)(), (0, l.j4)(y, {
                             key: 0,
-                            value: m.remainingSecondsNormalized,
+                            value: g.remainingSecondsNormalized,
                             "animation-speed": "200",
                             color: "grey"
                         }, null, 8, ["value"])) : (0, l.kq)("", !0)])),
                         _: 1
                     }), d.uiSettingsStore.uiSettings.gallery_show_filter ? ((0, l.wg)(), (0, l.j4)(I, {
                         key: 0,
                         modelValue: d.rightDrawerOpen,
                         "onUpdate:modelValue": t[2] || (t[2] = e => d.rightDrawerOpen = e),
                         side: "right",
                         elevated: "",
                         overlay: ""
                     }, {
-                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(m.availableFilter, (e => ((0, l.wg)(), (0, l.j4)(S, {
+                        default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(d.uiSettingsStore.uiSettings.gallery_filter_userselectable, (e => ((0, l.wg)(), (0, l.j4)(S, {
                             src: `/mediaprocessing/preview/${d.currentSlideId}/${e}`,
                             key: e,
-                            onClick: t => g.applyFilter(d.currentSlideId, e)
+                            onClick: t => c.applyFilter(d.currentSlideId, e)
                         }, {
-                            default: (0, l.w5)((() => [(0, l._)("div", n, (0, a.zw)(e), 1)])),
+                            default: (0, l.w5)((() => [(0, l._)("div", n, (0, r.zw)(e), 1)])),
                             _: 2
                         }, 1032, ["src", "onClick"])))), 128))])),
                         _: 1
                     }, 8, ["modelValue"])) : (0, l.kq)("", !0), (0, l.Wm)(q, {
                         class: "q-pa-none galleryimagedetail full-height"
                     }, {
                         default: (0, l.w5)((() => [(0, l.wy)(((0, l.wg)(), (0, l.j4)(v, {
@@ -131,55 +131,55 @@
                             thumbnails: "",
                             autoplay: d.autoplay,
                             draggable: "false",
                             arrows: "",
                             "transition-prev": "slide-right",
                             "transition-next": "slide-left",
                             onTransition: t[4] || (t[4] = (e, t) => {
-                                d.currentSlideIndex = i.itemRepository.findIndex((t => t.id === e)), g.abortTimer()
+                                d.currentSlideIndex = i.itemRepository.findIndex((t => t.id === e)), c.abortTimer()
                             })
                         }, {
-                            default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(g.slicedImages, (e => ((0, l.wg)(), (0, l.j4)(f, {
+                            default: (0, l.w5)((() => [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(c.slicedImages, (e => ((0, l.wg)(), (0, l.j4)(f, {
                                 "img-src": e.preview,
                                 key: e.id,
                                 name: e.id
                             }, null, 8, ["img-src", "name"])))), 128))])),
                             _: 1
                         }, 8, ["modelValue", "autoplay"])), [
-                            [D, d.handleSwipeDown, void 0, {
+                            [x, d.handleSwipeDown, void 0, {
                                 mouse: !0,
                                 down: !0
                             }]
-                        ]), (0, l.Wm)(k, {
+                        ]), (0, l.Wm)(_, {
                             position: "top-right",
                             offset: [30, 30]
                         }, {
                             default: (0, l.w5)((() => [(0, l._)("div", s, [(0, l.Wm)(b, {
                                 type: "image/png",
                                 tag: "svg",
                                 margin: 2,
                                 width: 200,
                                 "error-correction-level": "low",
                                 color: {
                                     dark: "#111111",
                                     light: "#EEEEEE"
                                 },
-                                value: g.getImageQrData()
+                                value: c.getImageQrData()
                             }, null, 8, ["value"])])])),
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 }, 8, ["onClick"])
             }
             i(9665);
-            var m = i(528),
-                g = i(499),
-                c = i(6694),
+            var g = i(528),
+                c = i(499),
+                m = i(6694),
                 u = i(3752);
             const h = {
                 props: {
                     indexSelected: {
                         type: Number,
                         required: !0
                     },
@@ -200,42 +200,41 @@
                     console.log(this.indexSelected), this.currentSlideIndex = this.indexSelected, this.currentSlideId = this.itemRepository[this.indexSelected].id
                 },
                 data() {
                     return {
                         intervalTimerId: null,
                         remainingSeconds: 0,
                         remainingSecondsNormalized: 0,
-                        displayLinearProgressBar: !0,
-                        availableFilter: ["original", "_1977", "aden", "brannan", "brooklyn", "clarendon", "earlybird", "gingham", "hudson", "inkwell", "kelvin", "lark", "lofi", "maven", "mayfair", "moon", "nashville", "perpetua", "reyes", "rise", "slumber", "stinson", "toaster", "valencia", "walden", "willow", "xpro2"]
+                        displayLinearProgressBar: !0
                     }
                 },
                 setup() {
-                    const e = (0, c.R)(),
-                        t = (0, g.iH)(!1);
+                    const e = (0, m.R)(),
+                        t = (0, c.iH)(!1);
                     return {
                         uiSettingsStore: e,
                         openURL: u.Z,
-                        fabRight: (0, g.iH)(!1),
-                        currentSlideId: (0, g.iH)(""),
-                        currentSlideIndex: (0, g.iH)(0),
-                        autoplay: (0, g.iH)(!1),
-                        showFilterDialog: (0, g.iH)(!1),
+                        fabRight: (0, c.iH)(!1),
+                        currentSlideId: (0, c.iH)(""),
+                        currentSlideIndex: (0, c.iH)(0),
+                        autoplay: (0, c.iH)(!1),
+                        showFilterDialog: (0, c.iH)(!1),
                         rightDrawerOpen: t,
                         toggleRightDrawer() {
                             t.value = !t.value
                         },
                         handleSwipeDown({
                             evt: e
                         }) {
                             console.log("TODO: add method to close dialog programmatically")
                         }
                     }
                 },
                 components: {
-                    VueQrcode: m.ZP
+                    VueQrcode: g.ZP
                 },
                 mounted() {
                     this.startTimer()
                 },
                 beforeUnmount() {
                     clearInterval(this.intervalTimerId)
                 },
@@ -282,95 +281,95 @@
                                 path: "/"
                             }))
                         }), 50)
                     }
                 }
             };
             var p = i(1639),
-                w = i(7605),
-                y = i(6602),
+                y = i(7605),
+                w = i(6602),
                 S = i(1663),
                 I = i(8879),
                 f = i(136),
                 v = i(2857),
                 b = i(8289),
-                k = i(906),
+                _ = i(906),
                 q = i(335),
-                _ = i(2133),
-                x = i(7052),
-                D = i(1694),
+                k = i(2133),
+                D = i(7052),
+                x = i(1694),
                 Z = i(627),
                 R = i(2146),
                 Q = i(4871),
                 T = i(9984),
                 C = i.n(T);
             const j = (0, p.Z)(h, [
                     ["render", d],
-                    ["__scopeId", "data-v-41e04494"]
+                    ["__scopeId", "data-v-3e1a07b8"]
                 ]),
                 W = j;
             C()(h, "components", {
-                QLayout: w.Z,
-                QHeader: y.Z,
+                QLayout: y.Z,
+                QHeader: w.Z,
                 QToolbar: S.Z,
                 QBtn: I.Z,
                 QSpace: f.Z,
                 QIcon: v.Z,
                 QLinearProgress: b.Z,
-                QDrawer: k.Z,
+                QDrawer: _.Z,
                 QImg: q.Z,
-                QPageContainer: _.Z,
-                QCarousel: x.Z,
-                QCarouselSlide: D.Z,
+                QPageContainer: k.Z,
+                QCarousel: D.Z,
+                QCarouselSlide: x.Z,
                 QPageSticky: Z.Z
             }), C()(h, "directives", {
                 ClosePopup: R.Z,
                 TouchSwipe: Q.Z
             })
         },
-        5031: (e, t, i) => {
+        3835: (e, t, i) => {
             i.r(t), i.d(t, {
                 default: () => v
             });
             var l = i(9835),
-                a = i(6970);
-            const r = {
+                r = i(6970);
+            const a = {
                     class: "row justify-center q-gutter-sm"
                 },
                 o = {
                     class: "absolute-bottom text-subtitle2"
                 };
 
             function n(e, t, i, n, s, d) {
-                const m = (0, l.up)("q-img"),
-                    g = (0, l.up)("q-card"),
-                    c = (0, l.up)("q-intersection"),
+                const g = (0, l.up)("q-img"),
+                    c = (0, l.up)("q-card"),
+                    m = (0, l.up)("q-intersection"),
                     u = (0, l.up)("gallery-image-detail"),
                     h = (0, l.up)("q-dialog"),
                     p = (0, l.up)("q-page");
                 return (0, l.wg)(), (0, l.j4)(p, {
                     padding: ""
                 }, {
-                    default: (0, l.w5)((() => [(0, l._)("div", r, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(this.store.gallery.images, ((e, t) => ((0, l.wg)(), (0, l.j4)(c, {
+                    default: (0, l.w5)((() => [(0, l._)("div", a, [((0, l.wg)(!0), (0, l.iD)(l.HY, null, (0, l.Ko)(this.store.gallery.images, ((e, t) => ((0, l.wg)(), (0, l.j4)(m, {
                         key: e.id,
                         once: "",
                         class: "preview-item"
                     }, {
-                        default: (0, l.w5)((() => [(0, l.Wm)(g, {
+                        default: (0, l.w5)((() => [(0, l.Wm)(c, {
                             class: "q-ma-sm",
                             onClick: e => d.openPic(t)
                         }, {
-                            default: (0, l.w5)((() => [(0, l.Wm)(m, {
+                            default: (0, l.w5)((() => [(0, l.Wm)(g, {
                                 src: d.getImageDetail(t),
                                 loading: "eager",
                                 "no-transition": "",
                                 "no-spinner": "",
                                 ratio: 1
                             }, {
-                                default: (0, l.w5)((() => [(0, l._)("div", o, (0, a.zw)(this.store.gallery.images[t].caption), 1)])),
+                                default: (0, l.w5)((() => [(0, l._)("div", o, (0, r.zw)(this.store.gallery.images[t].caption), 1)])),
                                 _: 2
                             }, 1032, ["src"])])),
                             _: 2
                         }, 1032, ["onClick"])])),
                         _: 2
                     }, 1024)))), 128))]), (0, l.Wm)(h, {
                         "transition-show": "jump-up",
@@ -387,24 +386,24 @@
                         _: 1
                     }, 8, ["modelValue"])])),
                     _: 1
                 })
             }
             var s = i(7575),
                 d = i(499),
-                m = i(666);
-            const g = {
+                g = i(9815);
+            const c = {
                 components: {
-                    GalleryImageDetail: m.Z
+                    GalleryImageDetail: g.Z
                 },
                 setup() {
                     const e = (0, s.h)();
                     return {
                         store: e,
-                        GalleryImageDetail: m.Z,
+                        GalleryImageDetail: g.Z,
                         indexSelected: (0, d.iH)(null),
                         showImageDetail: (0, d.iH)(!1)
                     }
                 },
                 computed: {
                     numberOfImages: {
                         get() {
@@ -424,34 +423,34 @@
                     })).catch((e => console.log(e)))
                 },
                 methods: {
                     getImageDetail(e, t = "thumbnail") {
                         return this.store.gallery.images[e][t]
                     },
                     openPic(e) {
-                        console.log(e), this.indexSelected = e, this.showImageDetail = !0
+                        this.indexSelected = e, this.showImageDetail = !0
                     }
                 }
             };
-            var c = i(1639),
+            var m = i(1639),
                 u = i(9885),
                 h = i(1517),
                 p = i(4458),
-                w = i(335),
-                y = i(2074),
+                y = i(335),
+                w = i(2074),
                 S = i(9984),
                 I = i.n(S);
-            const f = (0, c.Z)(g, [
+            const f = (0, m.Z)(c, [
                     ["render", n],
-                    ["__scopeId", "data-v-11f3b215"]
+                    ["__scopeId", "data-v-633c8198"]
                 ]),
                 v = f;
-            I()(g, "components", {
+            I()(c, "components", {
                 QPage: u.Z,
                 QIntersection: h.Z,
                 QCard: p.Z,
-                QImg: w.Z,
-                QDialog: y.Z
+                QImg: y.Z,
+                QDialog: w.Z
             })
         }
     }
 ]);
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/391.70a80bd8.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/391.70a80bd8.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/429.76096bfa.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/429.76096bfa.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/546.92b02def.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/546.92b02def.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/705.fc48b137.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/705.fc48b137.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/706.f32434a0.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/706.1c5cc1da.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,117 +1,117 @@
 "use strict";
 (globalThis["webpackChunkqPhotobooth"] = globalThis["webpackChunkqPhotobooth"] || []).push([
     [706], {
-        666: (e, i, t) => {
-            t.d(i, {
+        9815: (e, t, i) => {
+            i.d(t, {
                 Z: () => W
             });
-            var r = t(9835),
-                a = t(6970);
+            var r = i(9835),
+                a = i(6970);
             const l = {
                     class: "q-mr-sm"
                 },
                 n = {
                     class: "q-mr-sm"
                 },
                 o = {
                     class: "absolute-bottom-left text-subtitle2"
                 },
                 s = {
                     class: "q-gutter-sm"
                 };
 
-            function d(e, i, t, d, m, c) {
-                const u = (0, r.up)("q-btn"),
+            function d(e, t, i, d, m, u) {
+                const c = (0, r.up)("q-btn"),
                     g = (0, r.up)("q-space"),
                     h = (0, r.up)("q-icon"),
                     p = (0, r.up)("q-toolbar"),
                     S = (0, r.up)("q-linear-progress"),
                     w = (0, r.up)("q-header"),
                     y = (0, r.up)("q-img"),
-                    v = (0, r.up)("q-drawer"),
-                    I = (0, r.up)("q-carousel-slide"),
+                    I = (0, r.up)("q-drawer"),
+                    v = (0, r.up)("q-carousel-slide"),
                     f = (0, r.up)("q-carousel"),
                     b = (0, r.up)("vue-qrcode"),
-                    k = (0, r.up)("q-page-sticky"),
+                    _ = (0, r.up)("q-page-sticky"),
                     q = (0, r.up)("q-page-container"),
-                    _ = (0, r.up)("q-layout"),
+                    k = (0, r.up)("q-layout"),
                     T = (0, r.Q2)("close-popup"),
                     R = (0, r.Q2)("touch-swipe");
-                return (0, r.wg)(), (0, r.j4)(_, {
+                return (0, r.wg)(), (0, r.j4)(k, {
                     view: "hhh Lpr ffr",
-                    onClick: c.abortTimer
+                    onClick: u.abortTimer
                 }, {
                     default: (0, r.w5)((() => [(0, r.Wm)(w, {
                         elevated: "",
                         class: "bg-primary text-white"
                     }, {
                         default: (0, r.w5)((() => [(0, r.Wm)(p, null, {
-                            default: (0, r.w5)((() => [(0, r.wy)((0, r.Wm)(u, {
+                            default: (0, r.w5)((() => [(0, r.wy)((0, r.Wm)(c, {
                                 dense: "",
                                 flat: "",
                                 icon: "close"
                             }, null, 512), [
                                 [T]
-                            ]), (0, r.Wm)(g), d.uiSettingsStore.uiSettings.gallery_show_delete ? (0, r.wy)(((0, r.wg)(), (0, r.j4)(u, {
+                            ]), (0, r.Wm)(g), d.uiSettingsStore.uiSettings.gallery_show_delete ? (0, r.wy)(((0, r.wg)(), (0, r.j4)(c, {
                                 key: 0,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "delete",
                                 label: "Delete",
-                                onClick: i[0] || (i[0] = e => c.deleteImage(d.currentSlideId))
+                                onClick: t[0] || (t[0] = e => u.deleteImage(d.currentSlideId))
                             }, null, 512)), [
                                 [T]
-                            ]) : (0, r.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_download ? ((0, r.wg)(), (0, r.j4)(u, {
+                            ]) : (0, r.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_download ? ((0, r.wg)(), (0, r.j4)(c, {
                                 key: 1,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "download",
                                 label: "Download",
-                                onClick: i[1] || (i[1] = e => {
-                                    d.openURL(t.itemRepository[d.currentSlideIndex]["full"])
+                                onClick: t[1] || (t[1] = e => {
+                                    d.openURL(i.itemRepository[d.currentSlideIndex]["full"])
                                 })
-                            })) : (0, r.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_print ? ((0, r.wg)(), (0, r.j4)(u, {
+                            })) : (0, r.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_print ? ((0, r.wg)(), (0, r.j4)(c, {
                                 key: 2,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "print",
                                 label: "Print"
-                            })) : (0, r.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_filter ? ((0, r.wg)(), (0, r.j4)(u, {
+                            })) : (0, r.kq)("", !0), d.uiSettingsStore.uiSettings.gallery_show_filter && d.uiSettingsStore.uiSettings.gallery_filter_userselectable.length > 0 ? ((0, r.wg)(), (0, r.j4)(c, {
                                 key: 3,
                                 flat: "",
                                 class: "q-mr-sm",
                                 icon: "filter",
                                 label: "Filter",
                                 onClick: d.toggleRightDrawer
                             }, null, 8, ["onClick"])) : (0, r.kq)("", !0), (0, r.Wm)(g), (0, r._)("div", l, [(0, r.Wm)(h, {
                                 name: "tag"
-                            }), (0, r._)("span", null, (0, a.zw)(d.currentSlideIndex + 1) + " of " + (0, a.zw)(t.itemRepository.length) + " total", 1)]), (0, r.Wm)(g), (0, r._)("div", n, [(0, r.Wm)(h, {
+                            }), (0, r._)("span", null, (0, a.zw)(d.currentSlideIndex + 1) + " of " + (0, a.zw)(i.itemRepository.length) + " total", 1)]), (0, r.Wm)(g), (0, r._)("div", n, [(0, r.Wm)(h, {
                                 name: "image"
-                            }), (0, r.Uk)(" " + (0, a.zw)(t.itemRepository[d.currentSlideIndex]["caption"]), 1)])])),
+                            }), (0, r.Uk)(" " + (0, a.zw)(i.itemRepository[d.currentSlideIndex]["caption"]), 1)])])),
                             _: 1
                         }), m.displayLinearProgressBar && m.remainingSeconds > 0 ? ((0, r.wg)(), (0, r.j4)(S, {
                             key: 0,
                             value: m.remainingSecondsNormalized,
                             "animation-speed": "200",
                             color: "grey"
                         }, null, 8, ["value"])) : (0, r.kq)("", !0)])),
                         _: 1
-                    }), d.uiSettingsStore.uiSettings.gallery_show_filter ? ((0, r.wg)(), (0, r.j4)(v, {
+                    }), d.uiSettingsStore.uiSettings.gallery_show_filter ? ((0, r.wg)(), (0, r.j4)(I, {
                         key: 0,
                         modelValue: d.rightDrawerOpen,
-                        "onUpdate:modelValue": i[2] || (i[2] = e => d.rightDrawerOpen = e),
+                        "onUpdate:modelValue": t[2] || (t[2] = e => d.rightDrawerOpen = e),
                         side: "right",
                         elevated: "",
                         overlay: ""
                     }, {
-                        default: (0, r.w5)((() => [((0, r.wg)(!0), (0, r.iD)(r.HY, null, (0, r.Ko)(m.availableFilter, (e => ((0, r.wg)(), (0, r.j4)(y, {
+                        default: (0, r.w5)((() => [((0, r.wg)(!0), (0, r.iD)(r.HY, null, (0, r.Ko)(d.uiSettingsStore.uiSettings.gallery_filter_userselectable, (e => ((0, r.wg)(), (0, r.j4)(y, {
                             src: `/mediaprocessing/preview/${d.currentSlideId}/${e}`,
                             key: e,
-                            onClick: i => c.applyFilter(d.currentSlideId, e)
+                            onClick: t => u.applyFilter(d.currentSlideId, e)
                         }, {
                             default: (0, r.w5)((() => [(0, r._)("div", o, (0, a.zw)(e), 1)])),
                             _: 2
                         }, 1032, ["src", "onClick"])))), 128))])),
                         _: 1
                     }, 8, ["modelValue"])) : (0, r.kq)("", !0), (0, r.Wm)(q, {
                         class: "q-pa-none galleryimagedetail full-height"
@@ -123,64 +123,64 @@
                                 height: "100%"
                             },
                             "control-type": "flat",
                             "control-color": "primary",
                             swipeable: "",
                             animated: "",
                             modelValue: d.currentSlideId,
-                            "onUpdate:modelValue": i[3] || (i[3] = e => d.currentSlideId = e),
+                            "onUpdate:modelValue": t[3] || (t[3] = e => d.currentSlideId = e),
                             thumbnails: "",
                             autoplay: d.autoplay,
                             draggable: "false",
                             arrows: "",
                             "transition-prev": "slide-right",
                             "transition-next": "slide-left",
-                            onTransition: i[4] || (i[4] = (e, i) => {
-                                d.currentSlideIndex = t.itemRepository.findIndex((i => i.id === e)), c.abortTimer()
+                            onTransition: t[4] || (t[4] = (e, t) => {
+                                d.currentSlideIndex = i.itemRepository.findIndex((t => t.id === e)), u.abortTimer()
                             })
                         }, {
-                            default: (0, r.w5)((() => [((0, r.wg)(!0), (0, r.iD)(r.HY, null, (0, r.Ko)(c.slicedImages, (e => ((0, r.wg)(), (0, r.j4)(I, {
+                            default: (0, r.w5)((() => [((0, r.wg)(!0), (0, r.iD)(r.HY, null, (0, r.Ko)(u.slicedImages, (e => ((0, r.wg)(), (0, r.j4)(v, {
                                 "img-src": e.preview,
                                 key: e.id,
                                 name: e.id
                             }, null, 8, ["img-src", "name"])))), 128))])),
                             _: 1
                         }, 8, ["modelValue", "autoplay"])), [
                             [R, d.handleSwipeDown, void 0, {
                                 mouse: !0,
                                 down: !0
                             }]
-                        ]), (0, r.Wm)(k, {
+                        ]), (0, r.Wm)(_, {
                             position: "top-right",
                             offset: [30, 30]
                         }, {
                             default: (0, r.w5)((() => [(0, r._)("div", s, [(0, r.Wm)(b, {
                                 type: "image/png",
                                 tag: "svg",
                                 margin: 2,
                                 width: 200,
                                 "error-correction-level": "low",
                                 color: {
                                     dark: "#111111",
                                     light: "#EEEEEE"
                                 },
-                                value: c.getImageQrData()
+                                value: u.getImageQrData()
                             }, null, 8, ["value"])])])),
                             _: 1
                         })])),
                         _: 1
                     })])),
                     _: 1
                 }, 8, ["onClick"])
             }
-            t(9665);
-            var m = t(528),
-                c = t(499),
-                u = t(6694),
-                g = t(3752);
+            i(9665);
+            var m = i(528),
+                u = i(499),
+                c = i(6694),
+                g = i(3752);
             const h = {
                 props: {
                     indexSelected: {
                         type: Number,
                         required: !0
                     },
                     itemRepository: {
@@ -188,44 +188,43 @@
                         required: !0
                     }
                 },
                 computed: {
                     slicedImages() {
                         this.itemRepository.length;
                         var e = Math.max(0, this.currentSlideIndex - 2),
-                            i = Math.max(0, this.currentSlideIndex + 3);
-                        return this.itemRepository.slice(e, i)
+                            t = Math.max(0, this.currentSlideIndex + 3);
+                        return this.itemRepository.slice(e, t)
                     }
                 },
                 beforeCreate() {
                     console.log(this.indexSelected), this.currentSlideIndex = this.indexSelected, this.currentSlideId = this.itemRepository[this.indexSelected].id
                 },
                 data() {
                     return {
                         intervalTimerId: null,
                         remainingSeconds: 0,
                         remainingSecondsNormalized: 0,
-                        displayLinearProgressBar: !0,
-                        availableFilter: ["original", "_1977", "aden", "brannan", "brooklyn", "clarendon", "earlybird", "gingham", "hudson", "inkwell", "kelvin", "lark", "lofi", "maven", "mayfair", "moon", "nashville", "perpetua", "reyes", "rise", "slumber", "stinson", "toaster", "valencia", "walden", "willow", "xpro2"]
+                        displayLinearProgressBar: !0
                     }
                 },
                 setup() {
-                    const e = (0, u.R)(),
-                        i = (0, c.iH)(!1);
+                    const e = (0, c.R)(),
+                        t = (0, u.iH)(!1);
                     return {
                         uiSettingsStore: e,
                         openURL: g.Z,
-                        fabRight: (0, c.iH)(!1),
-                        currentSlideId: (0, c.iH)(""),
-                        currentSlideIndex: (0, c.iH)(0),
-                        autoplay: (0, c.iH)(!1),
-                        showFilterDialog: (0, c.iH)(!1),
-                        rightDrawerOpen: i,
+                        fabRight: (0, u.iH)(!1),
+                        currentSlideId: (0, u.iH)(""),
+                        currentSlideIndex: (0, u.iH)(0),
+                        autoplay: (0, u.iH)(!1),
+                        showFilterDialog: (0, u.iH)(!1),
+                        rightDrawerOpen: t,
                         toggleRightDrawer() {
-                            i.value = !i.value
+                            t.value = !t.value
                         },
                         handleSwipeDown({
                             evt: e
                         }) {
                             console.log("TODO: add method to close dialog programmatically")
                         }
                     }
@@ -241,36 +240,36 @@
                 },
                 methods: {
                     async reloadImg(e) {
                         await fetch(e, {
                             cache: "reload",
                             mode: "no-cors"
                         });
-                        const i = (new Date).getTime();
-                        document.body.querySelectorAll(`img[src*='${e}']`).forEach((t => {
-                            t.src = e + "?" + i
-                        })), document.body.querySelectorAll(`div[style*="background-image"][style*="${e}"]`).forEach((t => t.style.backgroundImage = `url(${e}?${i})`))
+                        const t = (new Date).getTime();
+                        document.body.querySelectorAll(`img[src*='${e}']`).forEach((i => {
+                            i.src = e + "?" + t
+                        })), document.body.querySelectorAll(`div[style*="background-image"][style*="${e}"]`).forEach((i => i.style.backgroundImage = `url(${e}?${t})`))
                     },
-                    applyFilter(e, i) {
-                        this.$api.get(`/mediaprocessing/applyfilter/${e}/${i}`).then((i => {
-                            const t = this.itemRepository.findIndex((i => i.id === e));
-                            this.reloadImg(this.itemRepository[t].full), this.reloadImg(this.itemRepository[t].preview), this.reloadImg(this.itemRepository[t].thumbnail)
+                    applyFilter(e, t) {
+                        this.$api.get(`/mediaprocessing/applyfilter/${e}/${t}`).then((t => {
+                            const i = this.itemRepository.findIndex((t => t.id === e));
+                            this.reloadImg(this.itemRepository[i].full), this.reloadImg(this.itemRepository[i].preview), this.reloadImg(this.itemRepository[i].thumbnail)
                         })).catch((e => console.log(e)))
                     },
                     deleteImage(e) {
                         this.$api.get("/mediacollection/delete", {
                             params: {
                                 image_id: e
                             }
                         }).then((e => {
                             console.log(e), this.itemRepository.splice(this.currentSlideIndex, 1)
                         })).catch((e => console.log(e)))
                     },
-                    getImageDetail(e, i = "thumbnail") {
-                        return this.itemRepository[e][i]
+                    getImageDetail(e, t = "thumbnail") {
+                        return this.itemRepository[e][t]
                     },
                     getImageQrData() {
                         const e = String(this.uiSettingsStore.uiSettings.EXT_DOWNLOAD_URL).replace("{filename}", this.itemRepository[this.currentSlideIndex]["filename"]);
                         return e
                     },
                     abortTimer() {
                         clearInterval(this.intervalTimerId), this.remainingSeconds = 0, this.remainingSecondsNormalized = 0
@@ -281,63 +280,63 @@
                             this.remainingSecondsNormalized = this.remainingSeconds / e, this.remainingSeconds -= .05, this.remainingSeconds <= 0 && (clearInterval(this.intervalTimerId), this.$router.push({
                                 path: "/"
                             }))
                         }), 50)
                     }
                 }
             };
-            var p = t(1639),
-                S = t(7605),
-                w = t(6602),
-                y = t(1663),
-                v = t(8879),
-                I = t(136),
-                f = t(2857),
-                b = t(8289),
-                k = t(906),
-                q = t(335),
-                _ = t(2133),
-                T = t(7052),
-                R = t(1694),
-                D = t(627),
-                Z = t(2146),
-                x = t(4871),
-                Q = t(9984),
-                C = t.n(Q);
+            var p = i(1639),
+                S = i(7605),
+                w = i(6602),
+                y = i(1663),
+                I = i(8879),
+                v = i(136),
+                f = i(2857),
+                b = i(8289),
+                _ = i(906),
+                q = i(335),
+                k = i(2133),
+                T = i(7052),
+                R = i(1694),
+                D = i(627),
+                Z = i(2146),
+                x = i(4871),
+                Q = i(9984),
+                C = i.n(Q);
             const E = (0, p.Z)(h, [
                     ["render", d],
-                    ["__scopeId", "data-v-41e04494"]
+                    ["__scopeId", "data-v-3e1a07b8"]
                 ]),
                 W = E;
             C()(h, "components", {
                 QLayout: S.Z,
                 QHeader: w.Z,
                 QToolbar: y.Z,
-                QBtn: v.Z,
-                QSpace: I.Z,
+                QBtn: I.Z,
+                QSpace: v.Z,
                 QIcon: f.Z,
                 QLinearProgress: b.Z,
-                QDrawer: k.Z,
+                QDrawer: _.Z,
                 QImg: q.Z,
-                QPageContainer: _.Z,
+                QPageContainer: k.Z,
                 QCarousel: T.Z,
                 QCarouselSlide: R.Z,
                 QPageSticky: D.Z
             }), C()(h, "directives", {
                 ClosePopup: Z.Z,
                 TouchSwipe: x.Z
             })
         },
-        4706: (e, i, t) => {
-            t.r(i), t.d(i, {
+        4706: (e, t, i) => {
+            i.r(t), i.d(t, {
                 default: () => S
             });
-            var r = t(9835);
+            var r = i(9835);
 
-            function a(e, i, t, a, l, n) {
+            function a(e, t, i, a, l, n) {
                 const o = (0, r.up)("q-linear-progress"),
                     s = (0, r.up)("gallery-image-detail"),
                     d = (0, r.up)("q-dialog"),
                     m = (0, r.up)("q-page");
                 return (0, r.wg)(), (0, r.j4)(m, {
                     class: "q-pa-none fullscreen",
                     onClick: n.abortTimer
@@ -346,31 +345,31 @@
                         key: 0,
                         value: l.remainingSecondsNormalized,
                         "animation-speed": "200"
                     }, null, 8, ["value"])) : (0, r.kq)("", !0), (0, r.Wm)(d, {
                         "transition-show": "jump-up",
                         "transition-hide": "jump-down",
                         modelValue: l.showImageDetail,
-                        "onUpdate:modelValue": i[0] || (i[0] = e => l.showImageDetail = e),
+                        "onUpdate:modelValue": t[0] || (t[0] = e => l.showImageDetail = e),
                         maximized: ""
                     }, {
                         default: (0, r.w5)((() => [(0, r.Wm)(s, {
                             itemRepository: [this.store.gallery.newArrivalItem],
                             indexSelected: 0,
                             class: "full-height"
                         }, null, 8, ["itemRepository"])])),
                         _: 1
                     }, 8, ["modelValue"])])),
                     _: 1
                 }, 8, ["onClick"])
             }
-            t(9665);
-            var l = t(7575),
-                n = t(6694),
-                o = t(666);
+            i(9665);
+            var l = i(7575),
+                n = i(6694),
+                o = i(9815);
             const s = {
                 components: {
                     GalleryImageDetail: o.Z
                 },
                 data() {
                     return {
                         intervalTimerId: null,
@@ -378,18 +377,18 @@
                         remainingSecondsNormalized: 0,
                         displayLinearProgressBar: !0,
                         showImageDetail: !0
                     }
                 },
                 setup() {
                     const e = (0, l.h)(),
-                        i = (0, n.R)();
+                        t = (0, n.R)();
                     return {
                         store: e,
-                        uiSettingsStore: i,
+                        uiSettingsStore: t,
                         GalleryImageDetail: o.Z
                     }
                 },
                 mounted() {
                     this.startTimer()
                 },
                 beforeUnmount() {
@@ -405,25 +404,25 @@
                             this.remainingSecondsNormalized = this.remainingSeconds / e, this.remainingSeconds -= .05, this.remainingSeconds <= 0 && (clearInterval(this.intervalTimerId), this.$router.push({
                                 path: "/"
                             }))
                         }), 50)
                     }
                 }
             };
-            var d = t(1639),
-                m = t(9885),
-                c = t(8289),
-                u = t(2074),
-                g = t(9984),
-                h = t.n(g);
+            var d = i(1639),
+                m = i(9885),
+                u = i(8289),
+                c = i(2074),
+                g = i(9984),
+                h = i.n(g);
             const p = (0, d.Z)(s, [
                     ["render", a]
                 ]),
                 S = p;
             h()(s, "components", {
                 QPage: m.Z,
-                QLinearProgress: c.Z,
-                QDialog: u.Z
+                QLinearProgress: u.Z,
+                QDialog: c.Z
             })
         }
     }
 ]);
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/71.3aaf5d7d.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/272.a73245eb.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkqPhotobooth"] = globalThis["webpackChunkqPhotobooth"] || []).push([
-    [71], {
-        7071: (e, o, l) => {
+    [272], {
+        7272: (e, o, l) => {
             l.r(o), l.d(o, {
                 default: () => z
             });
             var t = l(9835),
                 r = l(6970);
             const n = {
                     class: "q-mt-md row justify-center"
@@ -20,34 +20,34 @@
                     class: "col-12 col-md-8 q-mb-xl"
                 },
                 c = {
                     class: "q-gutter-sm"
                 };
 
             function m(e, o, l, m, u, g) {
-                const d = (0, t.up)("q-tab"),
-                    p = (0, t.up)("q-tabs"),
+                const p = (0, t.up)("q-tab"),
+                    d = (0, t.up)("q-tabs"),
                     f = (0, t.up)("q-separator"),
                     b = (0, t.up)("BlitzForm"),
                     v = (0, t.up)("q-btn"),
                     h = (0, t.up)("q-page-sticky"),
                     y = (0, t.up)("q-page");
                 return (0, t.wg)(), (0, t.j4)(y, {
                     padding: ""
                 }, {
-                    default: (0, t.w5)((() => [(0, t.Wm)(p, {
+                    default: (0, t.w5)((() => [(0, t.Wm)(d, {
                         modelValue: m.selected_group,
                         "onUpdate:modelValue": o[0] || (o[0] = e => m.selected_group = e),
                         class: "text-grey",
                         "active-color": "secondary",
                         "indicator-color": "secondary",
                         "mobile-arrows": "",
                         align: "justify"
                     }, {
-                        default: (0, t.w5)((() => [((0, t.wg)(!0), (0, t.iD)(t.HY, null, (0, t.Ko)(m.main_groups, (e => ((0, t.wg)(), (0, t.j4)(d, {
+                        default: (0, t.w5)((() => [((0, t.wg)(!0), (0, t.iD)(t.HY, null, (0, t.Ko)(m.main_groups, (e => ((0, t.wg)(), (0, t.j4)(p, {
                             key: e,
                             label: e,
                             name: e
                         }, null, 8, ["label", "name"])))), 128))])),
                         _: 1
                     }, 8, ["modelValue"]), (0, t.Wm)(f), (0, t._)("div", n, [(0, t._)("div", a, [(0, t._)("div", s, (0, r.zw)(m.group_title), 1), (0, t._)("p", null, (0, r.zw)(m.group_description), 1)]), (0, t._)("div", i, [m.renderBlitzForm ? ((0, t.wg)(), (0, t.j4)(b, {
                         modelValue: m.serverConfig[m.selected_group],
@@ -76,30 +76,30 @@
                     })])),
                     _: 1
                 })
             }
             l(9665);
             var u = l(499),
                 g = l(1569),
-                d = l(9302),
-                p = l(6694),
+                p = l(9302),
+                d = l(6694),
                 f = l(6380);
             const b = {
                 components: {
                     BlitzForm: f.lU,
                     BlitzListForm: f.$C
                 },
                 setup() {
-                    const e = (0, d.Z)(),
+                    const e = (0, p.Z)(),
                         o = (0, u.iH)({});
                     let l = {};
                     const r = (0, u.iH)([]),
                         n = (0, u.iH)(!1),
                         a = (0, u.iH)(""),
-                        s = (0, p.R)(),
+                        s = (0, d.R)(),
                         i = (0, t.Fl)((() => "" != a.value ? l[a.value]["allOf"][0]["title"] : "-")),
                         c = (0, t.Fl)((() => "" != a.value ? l[a.value]["allOf"][0]["description"] : "-")),
                         m = (0, t.Fl)((() => "" != a.value ? f(l[a.value]) : [])),
                         f = e => {
                             const o = e => e.replace(/[&<>'"]/g, (e => ({
                                     "&": "&amp;",
                                     "<": "&lt;",
@@ -117,18 +117,18 @@
                                     return "boolean" == l["type"] && (t["component"] = "QToggle"), "integer" != l["type"] && "float" != l["type"] || (t["component"] = "QInput", l["ui_component"] && (t["component"] = l["ui_component"]), t["type"] = "number", t["labelAlways"] = !0, l["exclusiveMinimum"] && (t["min"] = l["exclusiveMinimum"]), l["exclusiveMaximum"] && (t["max"] = l["exclusiveMaximum"]), l["minimum"] && (t["min"] = l["minimum"]), l["maximum"] && (t["max"] = l["maximum"])), l["allOf"] && Object.keys(l["allOf"][0]).includes("enum") && (t["component"] = "QSelect", t["options"] = l["allOf"][0]["enum"]), t["subLabel"] = `${l["description"]||""} (default=${o(("default"in l?l["default"]:"undefined").toString())})`, t
                                 };
                             console.log("creating blitzar schema"), console.log(e);
                             let t = [];
                             return "allOf" in e ? Object.entries(e["allOf"][0]["properties"]).forEach((e => {
                                 const [o, r] = e;
                                 let n = l(o, r);
-                                "array" == r["type"] && r["items"] && "object" == r["items"]["type"] && (n["component"] = "BlitzListForm", n["schema"] = [], Object.entries(r["items"]["properties"]).forEach((e => {
+                                "array" == r["type"] && r["items"] && "object" == r["items"]["type"] ? (n["component"] = "BlitzListForm", n["schema"] = [], Object.entries(r["items"]["properties"]).forEach((e => {
                                     const [o, t] = e;
                                     n["schema"].push(l(o, t))
-                                }))), t.push(n)
+                                }))) : "array" == r["type"] && r["items"] && r["items"]["enum"] && "string" == r["items"]["type"] && (n["component"] = "QSelect", n["multiple"] = !0, n["use-chips"] = !0, n["stack-label"] = !0, n["options"] = r["items"]["enum"]), t.push(n)
                             })) : console.log("error, wrong format!, no direct props on main level"), console.log(t), t
                         },
                         b = () => {
                             g.api.get("/config/schema?schema_type=dereferenced").then((async e => {
                                 console.log(e.data), l = e.data.properties, r.value = Object.keys(l), a.value = r.value[0]
                             })).catch((o => {
                                 console.log(o), console.log("error"), e.notify({
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/862.525f2f13.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/862.525f2f13.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/863.e0c5ac02.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/863.e0c5ac02.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/954.7419ae78.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/954.7419ae78.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/app.3153eea4.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/app.64608eed.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -178,18 +178,18 @@
                         path: "/",
                         component: () => Promise.all([o.e(736), o.e(546)]).then(o.bind(o, 1546)),
                         children: [{
                             path: "",
                             component: () => Promise.all([o.e(736), o.e(705)]).then(o.bind(o, 4705))
                         }, {
                             path: "gallery",
-                            component: () => Promise.all([o.e(736), o.e(31)]).then(o.bind(o, 5031))
+                            component: () => Promise.all([o.e(736), o.e(835)]).then(o.bind(o, 3835))
                         }, {
                             path: "gallery/:id",
-                            component: () => Promise.all([o.e(736), o.e(31)]).then(o.bind(o, 5031))
+                            component: () => Promise.all([o.e(736), o.e(835)]).then(o.bind(o, 3835))
                         }, {
                             path: "newItemArrived",
                             component: () => Promise.all([o.e(736), o.e(706)]).then(o.bind(o, 4706))
                         }]
                     }, {
                         path: "/admin",
                         meta: {
@@ -198,27 +198,27 @@
                         },
                         component: () => Promise.all([o.e(736), o.e(247)]).then(o.bind(o, 2247)),
                         children: [{
                             path: "",
                             component: () => Promise.all([o.e(736), o.e(954)]).then(o.bind(o, 5954))
                         }, {
                             path: "gallery",
-                            component: () => Promise.all([o.e(736), o.e(31)]).then(o.bind(o, 5031))
+                            component: () => Promise.all([o.e(736), o.e(835)]).then(o.bind(o, 3835))
                         }, {
                             path: "status",
                             component: () => Promise.all([o.e(736), o.e(391)]).then(o.bind(o, 6391))
                         }, {
                             path: "help",
                             component: () => Promise.all([o.e(736), o.e(429)]).then(o.bind(o, 6429))
                         }, {
                             path: "playground",
                             component: () => Promise.all([o.e(736), o.e(863)]).then(o.bind(o, 2863))
                         }, {
                             path: "config",
-                            component: () => Promise.all([o.e(736), o.e(71)]).then(o.bind(o, 7071))
+                            component: () => Promise.all([o.e(736), o.e(272)]).then(o.bind(o, 7272))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => o.e(862).then(o.bind(o, 1862))
                     }],
                     Z = k,
                     R = (0, T.BC)((function() {
@@ -447,14 +447,15 @@
                                 GALLERY_EMPTY_MSG: null,
                                 TAKEPIC_MSG: null,
                                 TAKEPIC_MSG_TIME: null,
                                 AUTOCLOSE_NEW_ITEM_ARRIVED: null,
                                 SHOW_ADMIN_LINK_ON_FRONTPAGE: null,
                                 EXT_DOWNLOAD_URL: null,
                                 gallery_show_filter: null,
+                                gallery_filter_userselectable: null,
                                 gallery_show_download: null,
                                 gallery_show_delete: null,
                                 gallery_show_print: null
                             },
                             storeState: l.INIT
                         }),
                         actions: {
@@ -520,31 +521,31 @@
                 get: t[n]
             })
         }
     })(), (() => {
         o.f = {}, o.e = e => Promise.all(Object.keys(o.f).reduce(((t, n) => (o.f[n](e, t), t)), []))
     })(), (() => {
         o.u = e => "js/" + e + "." + {
-            31: "51d7e662",
-            71: "3aaf5d7d",
             247: "74c0e45d",
+            272: "a73245eb",
             391: "70a80bd8",
             429: "76096bfa",
             546: "92b02def",
             705: "fc48b137",
-            706: "f32434a0",
+            706: "1c5cc1da",
+            835: "70f6a199",
             862: "525f2f13",
             863: "e0c5ac02",
             954: "7419ae78"
         } [e] + ".js"
     })(), (() => {
         o.miniCssF = e => "css/" + e + "." + {
-            31: "363e41a9",
-            71: "0be6c807",
-            706: "42cb67d0"
+            272: "0be6c807",
+            706: "28b224d0",
+            835: "eb55e979"
         } [e] + ".css"
     })(), (() => {
         o.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
             } catch (e) {
@@ -626,17 +627,17 @@
                     e(n, i, null, r, l)
                 })),
                 r = {
                     143: 0
                 };
             o.f.miniCss = (e, t) => {
                 var o = {
-                    31: 1,
-                    71: 1,
-                    706: 1
+                    272: 1,
+                    706: 1,
+                    835: 1
                 };
                 r[e] ? t.push(r[e]) : 0 !== r[e] && o[e] && t.push(r[e] = n(e).then((() => {
                     r[e] = 0
                 }), (t => {
                     throw delete r[e], t
                 })))
             }
```

### Comparing `photobooth_app-0.1.0rc4/photobooth/web_spa/js/vendor.c9e02ba9.js` & `photobooth_app-0.1.0rc5/photobooth/web_spa/js/vendor.c9e02ba9.js`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/LICENSE.md` & `photobooth_app-0.1.0rc5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/README.md` & `photobooth_app-0.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `photobooth_app-0.1.0rc4/pyproject.toml` & `photobooth_app-0.1.0rc5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b70 726f 6a65 6374 5d0d 0a6e 616d 6520  [project]..name 
 00000010: 3d20 2270 686f 746f 626f 6f74 682d 6170  = "photobooth-ap
 00000020: 7022 0d0a 7265 7175 6972 6573 2d70 7974  p"..requires-pyt
 00000030: 686f 6e20 3d20 223e 3d33 2e39 2c3c 332e  hon = ">=3.9,<3.
 00000040: 3132 220d 0a76 6572 7369 6f6e 203d 2022  12"..version = "
-00000050: 302e 312e 3072 6334 220d 0a64 6573 6372  0.1.0rc4"..descr
+00000050: 302e 312e 3072 6335 220d 0a64 6573 6372  0.1.0rc5"..descr
 00000060: 6970 7469 6f6e 203d 2022 5068 6f74 6f62  iption = "Photob
 00000070: 6f6f 7468 2061 7070 2077 7269 7474 656e  ooth app written
 00000080: 2069 6e20 5079 7468 6f6e 2073 7570 706f   in Python suppo
 00000090: 7274 696e 6720 4453 4c52 2c20 7069 6361  rting DSLR, pica
 000000a0: 6d65 7261 322c 2077 6562 6361 6d65 7261  mera2, webcamera
 000000b0: 7322 0d0a 6175 7468 6f72 7320 3d20 5b7b  s"..authors = [{
 000000c0: 206e 616d 6520 3d20 224d 6963 6861 656c   name = "Michael
@@ -103,106 +103,107 @@
 00000660: 0a20 2022 7275 6666 7e3d 302e 302e 3237  .  "ruff~=0.0.27
 00000670: 3022 2c0d 0a20 2022 6874 7470 782d 7373  0",..  "httpx-ss
 00000680: 657e 3d30 2e33 2e31 222c 0d0a 2020 2268  e~=0.3.1",..  "h
 00000690: 7474 7078 7e3d 302e 3234 2e31 222c 0d0a  ttpx~=0.24.1",..
 000006a0: 2020 2273 696d 706c 656a 7065 677e 3d31    "simplejpeg~=1
 000006b0: 2e36 2e36 222c 0d0a 2020 2263 6f76 6572  .6.6",..  "cover
 000006c0: 6167 655b 746f 6d6c 5d7e 3d37 2e32 2e37  age[toml]~=7.2.7
-000006d0: 220d 0a5d 0d0a 2320 6c69 6263 616d 6572  "..]..# libcamer
-000006e0: 612f 7069 6361 6d65 7261 3220 6172 6520  a/picamera2 are 
-000006f0: 6176 6169 6c20 666f 7220 6e6f 7720 6f6e  avail for now on
-00000700: 6c79 2061 7320 7379 7374 656d 2070 7974  ly as system pyt
-00000710: 686f 6e20 7061 636b 6167 6520 2d20 6973  hon package - is
-00000720: 6f6c 6174 6564 2065 6e76 2063 616e 6e6f  olated env canno
-00000730: 7420 7573 6520 7468 656d 2077 6974 686f  t use them witho
-00000740: 7574 2067 6c6f 6261 6c20 6163 6365 7373  ut global access
-00000750: 0d0a 7379 7374 656d 2d70 6163 6b61 6765  ..system-package
-00000760: 7320 3d20 7472 7565 0d0a 0d0a 5b74 6f6f  s = true....[too
-00000770: 6c2e 6861 7463 682e 656e 7673 2e74 6573  l.hatch.envs.tes
-00000780: 742e 7363 7269 7074 735d 0d0a 7465 7374  t.scripts]..test
-00000790: 203d 2022 7079 7465 7374 202d 7620 2d2d   = "pytest -v --
-000007a0: 636f 762d 7265 706f 7274 3d74 6572 6d20  cov-report=term 
-000007b0: 2d2d 636f 762d 7265 706f 7274 3d78 6d6c  --cov-report=xml
-000007c0: 3a63 6f76 6572 6167 652e 786d 6c20 2d2d  :coverage.xml --
-000007d0: 636f 7620 2e2f 220d 0a0d 0a0d 0a0d 0a5b  cov ./"........[
-000007e0: 7072 6f6a 6563 742e 7572 6c73 5d0d 0a68  project.urls]..h
-000007f0: 6f6d 6570 6167 6520 3d20 2268 7474 7073  omepage = "https
-00000800: 3a2f 2f67 6974 6875 622e 636f 6d2f 6d67  ://github.com/mg
-00000810: 726c 2f70 686f 746f 626f 6f74 682d 6170  rl/photobooth-ap
-00000820: 7022 0d0a 7265 706f 7369 746f 7279 203d  p"..repository =
-00000830: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-00000840: 2e63 6f6d 2f6d 6772 6c2f 7068 6f74 6f62  .com/mgrl/photob
-00000850: 6f6f 7468 2d61 7070 220d 0a64 6f63 756d  ooth-app"..docum
-00000860: 656e 7461 7469 6f6e 203d 2022 6874 7470  entation = "http
-00000870: 733a 2f2f 6d67 726c 2e67 6974 6875 622e  s://mgrl.github.
-00000880: 696f 2f70 686f 746f 626f 6f74 682d 646f  io/photobooth-do
-00000890: 6373 220d 0a0d 0a5b 7072 6f6a 6563 742e  cs"....[project.
-000008a0: 7363 7269 7074 735d 0d0a 7068 6f74 6f62  scripts]..photob
-000008b0: 6f6f 7468 203d 2022 7068 6f74 6f62 6f6f  ooth = "photoboo
-000008c0: 7468 2e5f 5f6d 6169 6e5f 5f3a 6d61 696e  th.__main__:main
-000008d0: 220d 0a0d 0a5b 746f 6f6c 2e68 6174 6368  "....[tool.hatch
-000008e0: 2e62 7569 6c64 5d0d 0a69 6e63 6c75 6465  .build]..include
-000008f0: 203d 205b 0d0a 2020 222f 7068 6f74 6f62   = [..  "/photob
-00000900: 6f6f 7468 222c 0d0a 5d0d 0a0d 0a5b 6275  ooth",..]....[bu
-00000910: 696c 642d 7379 7374 656d 5d0d 0a72 6571  ild-system]..req
-00000920: 7569 7265 7320 3d20 5b22 6861 7463 686c  uires = ["hatchl
-00000930: 696e 6722 5d0d 0a62 7569 6c64 2d62 6163  ing"]..build-bac
-00000940: 6b65 6e64 203d 2022 6861 7463 686c 696e  kend = "hatchlin
-00000950: 672e 6275 696c 6422 0d0a 0d0a 5b74 6f6f  g.build"....[too
-00000960: 6c2e 7079 7465 7374 2e69 6e69 5f6f 7074  l.pytest.ini_opt
-00000970: 696f 6e73 5d0d 0a6c 6f67 5f63 6c69 203d  ions]..log_cli =
-00000980: 2074 7275 650d 0a6c 6f67 5f63 6c69 5f6c   true..log_cli_l
-00000990: 6576 656c 203d 2022 4445 4255 4722 0d0a  evel = "DEBUG"..
-000009a0: 6c6f 675f 636c 695f 666f 726d 6174 203d  log_cli_format =
-000009b0: 2022 2528 6173 6374 696d 6529 7320 5b25   "%(asctime)s [%
-000009c0: 286c 6576 656c 6e61 6d65 2938 735d 2025  (levelname)8s] %
-000009d0: 286d 6573 7361 6765 2973 2028 2528 6669  (message)s (%(fi
-000009e0: 6c65 6e61 6d65 2973 3a25 286c 696e 656e  lename)s:%(linen
-000009f0: 6f29 7329 220d 0a6c 6f67 5f63 6c69 5f64  o)s)"..log_cli_d
-00000a00: 6174 655f 666f 726d 6174 203d 2022 2559  ate_format = "%Y
-00000a10: 2d25 6d2d 2564 2025 483a 254d 3a25 5322  -%m-%d %H:%M:%S"
-00000a20: 0d0a 0d0a 5b74 6f6f 6c2e 636f 7665 7261  ....[tool.covera
-00000a30: 6765 2e72 756e 5d0d 0a23 2064 6973 6162  ge.run]..# disab
-00000a40: 6c65 2063 6f75 6c64 6e74 2d70 6172 7365  le couldnt-parse
-00000a50: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
-00000a60: 2e63 6f6d 2f6e 6564 6261 742f 636f 7665  .com/nedbat/cove
-00000a70: 7261 6765 7079 2f69 7373 7565 732f 3133  ragepy/issues/13
-00000a80: 3932 0d0a 6469 7361 626c 655f 7761 726e  92..disable_warn
-00000a90: 696e 6773 203d 205b 2263 6f75 6c64 6e74  ings = ["couldnt
-00000aa0: 2d70 6172 7365 225d 0d0a 6f6d 6974 203d  -parse"]..omit =
-00000ab0: 205b 0d0a 2020 2020 2274 6573 745f 2a2e   [..    "test_*.
-00000ac0: 7079 222c 0d0a 2020 2020 222e 2f74 6573  py",..    "./tes
-00000ad0: 7473 2f2a 222c 0d0a 2020 2020 222e 2f70  ts/*",..    "./p
-00000ae0: 686f 746f 626f 6f74 682f 7665 6e64 6f72  hotobooth/vendor
-00000af0: 2f2a 220d 0a20 2020 205d 0d0a 7061 7261  /*"..    ]..para
-00000b00: 6c6c 656c 203d 2074 7275 650d 0a63 6f6e  llel = true..con
-00000b10: 6375 7272 656e 6379 203d 205b 2274 6872  currency = ["thr
-00000b20: 6561 6422 2c22 6d75 6c74 6970 726f 6365  ead","multiproce
-00000b30: 7373 696e 6722 5d0d 0a0d 0a5b 746f 6f6c  ssing"]....[tool
-00000b40: 2e62 6c61 636b 5d0d 0a6c 696e 652d 6c65  .black]..line-le
-00000b50: 6e67 7468 203d 2031 3230 0d0a 0d0a 5b74  ngth = 120....[t
-00000b60: 6f6f 6c2e 7275 6666 5d0d 0a6c 696e 652d  ool.ruff]..line-
-00000b70: 6c65 6e67 7468 203d 2031 3230 0d0a 7365  length = 120..se
-00000b80: 6c65 6374 203d 205b 0d0a 2020 2245 222c  lect = [..  "E",
-00000b90: 2020 2023 2070 7963 6f64 6573 7479 6c65     # pycodestyle
-00000ba0: 0d0a 2020 2257 222c 2020 2023 2070 7963  ..  "W",   # pyc
-00000bb0: 6f64 6573 7479 6c65 0d0a 2020 2246 222c  odestyle..  "F",
-00000bc0: 2020 2023 2070 7966 6c61 6b65 730d 0a20     # pyflakes.. 
-00000bd0: 2022 4222 2c20 2020 2320 6275 6762 6561   "B",   # bugbea
-00000be0: 720d 0a20 2022 5550 222c 2020 2320 7079  r..  "UP",  # py
-00000bf0: 7570 6772 6164 650d 0a20 2022 4922 2c20  upgrade..  "I", 
-00000c00: 2020 2320 6973 6f72 740d 0a20 2023 2244    # isort..  #"D
-00000c10: 222c 2020 2023 2070 7964 6f63 7374 796c  ",   # pydocstyl
-00000c20: 6520 2020 2320 6164 6420 6c61 7465 720d  e   # add later.
-00000c30: 0a5d 0d0a 6967 6e6f 7265 203d 205b 0d0a  .]..ignore = [..
-00000c40: 2020 2242 3030 3822 2023 7573 6564 2066    "B008" #used f
-00000c50: 6f72 2044 4920 696e 6a65 6374 696f 6e0d  or DI injection.
-00000c60: 0a20 205d 0d0a 6578 7465 6e64 2d65 7863  .  ]..extend-exc
-00000c70: 6c75 6465 203d 205b 2276 656e 646f 7222  lude = ["vendor"
-00000c80: 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566 662e  ]....[tool.ruff.
-00000c90: 7065 722d 6669 6c65 2d69 676e 6f72 6573  per-file-ignores
-00000ca0: 5d0d 0a22 7068 6f74 6f62 6f6f 7468 2f61  ].."photobooth/a
-00000cb0: 7070 636f 6e66 6967 2e70 7922 203d 205b  ppconfig.py" = [
-00000cc0: 2245 3530 3122 5d0d 0a0d 0a5b 746f 6f6c  "E501"]....[tool
-00000cd0: 2e72 7566 662e 7079 646f 6373 7479 6c65  .ruff.pydocstyle
-00000ce0: 5d0d 0a63 6f6e 7665 6e74 696f 6e20 3d20  ]..convention = 
-00000cf0: 2267 6f6f 676c 6522                      "google"
+000006d0: 222c 0d0a 2020 2262 6c61 636b 220d 0a5d  ",..  "black"..]
+000006e0: 0d0a 2320 6c69 6263 616d 6572 612f 7069  ..# libcamera/pi
+000006f0: 6361 6d65 7261 3220 6172 6520 6176 6169  camera2 are avai
+00000700: 6c20 666f 7220 6e6f 7720 6f6e 6c79 2061  l for now only a
+00000710: 7320 7379 7374 656d 2070 7974 686f 6e20  s system python 
+00000720: 7061 636b 6167 6520 2d20 6973 6f6c 6174  package - isolat
+00000730: 6564 2065 6e76 2063 616e 6e6f 7420 7573  ed env cannot us
+00000740: 6520 7468 656d 2077 6974 686f 7574 2067  e them without g
+00000750: 6c6f 6261 6c20 6163 6365 7373 0d0a 7379  lobal access..sy
+00000760: 7374 656d 2d70 6163 6b61 6765 7320 3d20  stem-packages = 
+00000770: 7472 7565 0d0a 0d0a 5b74 6f6f 6c2e 6861  true....[tool.ha
+00000780: 7463 682e 656e 7673 2e74 6573 742e 7363  tch.envs.test.sc
+00000790: 7269 7074 735d 0d0a 7465 7374 203d 2022  ripts]..test = "
+000007a0: 7079 7465 7374 202d 7620 2d2d 636f 762d  pytest -v --cov-
+000007b0: 7265 706f 7274 3d74 6572 6d20 2d2d 636f  report=term --co
+000007c0: 762d 7265 706f 7274 3d78 6d6c 3a63 6f76  v-report=xml:cov
+000007d0: 6572 6167 652e 786d 6c20 2d2d 636f 7620  erage.xml --cov 
+000007e0: 2e2f 220d 0a0d 0a0d 0a0d 0a5b 7072 6f6a  ./"........[proj
+000007f0: 6563 742e 7572 6c73 5d0d 0a68 6f6d 6570  ect.urls]..homep
+00000800: 6167 6520 3d20 2268 7474 7073 3a2f 2f67  age = "https://g
+00000810: 6974 6875 622e 636f 6d2f 6d67 726c 2f70  ithub.com/mgrl/p
+00000820: 686f 746f 626f 6f74 682d 6170 7022 0d0a  hotobooth-app"..
+00000830: 7265 706f 7369 746f 7279 203d 2022 6874  repository = "ht
+00000840: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000850: 2f6d 6772 6c2f 7068 6f74 6f62 6f6f 7468  /mgrl/photobooth
+00000860: 2d61 7070 220d 0a64 6f63 756d 656e 7461  -app"..documenta
+00000870: 7469 6f6e 203d 2022 6874 7470 733a 2f2f  tion = "https://
+00000880: 6d67 726c 2e67 6974 6875 622e 696f 2f70  mgrl.github.io/p
+00000890: 686f 746f 626f 6f74 682d 646f 6373 220d  hotobooth-docs".
+000008a0: 0a0d 0a5b 7072 6f6a 6563 742e 7363 7269  ...[project.scri
+000008b0: 7074 735d 0d0a 7068 6f74 6f62 6f6f 7468  pts]..photobooth
+000008c0: 203d 2022 7068 6f74 6f62 6f6f 7468 2e5f   = "photobooth._
+000008d0: 5f6d 6169 6e5f 5f3a 6d61 696e 220d 0a0d  _main__:main"...
+000008e0: 0a5b 746f 6f6c 2e68 6174 6368 2e62 7569  .[tool.hatch.bui
+000008f0: 6c64 5d0d 0a69 6e63 6c75 6465 203d 205b  ld]..include = [
+00000900: 0d0a 2020 222f 7068 6f74 6f62 6f6f 7468  ..  "/photobooth
+00000910: 222c 0d0a 5d0d 0a0d 0a5b 6275 696c 642d  ",..]....[build-
+00000920: 7379 7374 656d 5d0d 0a72 6571 7569 7265  system]..require
+00000930: 7320 3d20 5b22 6861 7463 686c 696e 6722  s = ["hatchling"
+00000940: 5d0d 0a62 7569 6c64 2d62 6163 6b65 6e64  ]..build-backend
+00000950: 203d 2022 6861 7463 686c 696e 672e 6275   = "hatchling.bu
+00000960: 696c 6422 0d0a 0d0a 5b74 6f6f 6c2e 7079  ild"....[tool.py
+00000970: 7465 7374 2e69 6e69 5f6f 7074 696f 6e73  test.ini_options
+00000980: 5d0d 0a6c 6f67 5f63 6c69 203d 2074 7275  ]..log_cli = tru
+00000990: 650d 0a6c 6f67 5f63 6c69 5f6c 6576 656c  e..log_cli_level
+000009a0: 203d 2022 4445 4255 4722 0d0a 6c6f 675f   = "DEBUG"..log_
+000009b0: 636c 695f 666f 726d 6174 203d 2022 2528  cli_format = "%(
+000009c0: 6173 6374 696d 6529 7320 5b25 286c 6576  asctime)s [%(lev
+000009d0: 656c 6e61 6d65 2938 735d 2025 286d 6573  elname)8s] %(mes
+000009e0: 7361 6765 2973 2028 2528 6669 6c65 6e61  sage)s (%(filena
+000009f0: 6d65 2973 3a25 286c 696e 656e 6f29 7329  me)s:%(lineno)s)
+00000a00: 220d 0a6c 6f67 5f63 6c69 5f64 6174 655f  "..log_cli_date_
+00000a10: 666f 726d 6174 203d 2022 2559 2d25 6d2d  format = "%Y-%m-
+00000a20: 2564 2025 483a 254d 3a25 5322 0d0a 0d0a  %d %H:%M:%S"....
+00000a30: 5b74 6f6f 6c2e 636f 7665 7261 6765 2e72  [tool.coverage.r
+00000a40: 756e 5d0d 0a23 2064 6973 6162 6c65 2063  un]..# disable c
+00000a50: 6f75 6c64 6e74 2d70 6172 7365 3a20 6874  ouldnt-parse: ht
+00000a60: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000a70: 2f6e 6564 6261 742f 636f 7665 7261 6765  /nedbat/coverage
+00000a80: 7079 2f69 7373 7565 732f 3133 3932 0d0a  py/issues/1392..
+00000a90: 6469 7361 626c 655f 7761 726e 696e 6773  disable_warnings
+00000aa0: 203d 205b 2263 6f75 6c64 6e74 2d70 6172   = ["couldnt-par
+00000ab0: 7365 225d 0d0a 6f6d 6974 203d 205b 0d0a  se"]..omit = [..
+00000ac0: 2020 2020 2274 6573 745f 2a2e 7079 222c      "test_*.py",
+00000ad0: 0d0a 2020 2020 222e 2f74 6573 7473 2f2a  ..    "./tests/*
+00000ae0: 222c 0d0a 2020 2020 222e 2f70 686f 746f  ",..    "./photo
+00000af0: 626f 6f74 682f 7665 6e64 6f72 2f2a 220d  booth/vendor/*".
+00000b00: 0a20 2020 205d 0d0a 7061 7261 6c6c 656c  .    ]..parallel
+00000b10: 203d 2074 7275 650d 0a63 6f6e 6375 7272   = true..concurr
+00000b20: 656e 6379 203d 205b 2274 6872 6561 6422  ency = ["thread"
+00000b30: 2c22 6d75 6c74 6970 726f 6365 7373 696e  ,"multiprocessin
+00000b40: 6722 5d0d 0a0d 0a5b 746f 6f6c 2e62 6c61  g"]....[tool.bla
+00000b50: 636b 5d0d 0a6c 696e 652d 6c65 6e67 7468  ck]..line-length
+00000b60: 203d 2031 3230 0d0a 0d0a 5b74 6f6f 6c2e   = 120....[tool.
+00000b70: 7275 6666 5d0d 0a6c 696e 652d 6c65 6e67  ruff]..line-leng
+00000b80: 7468 203d 2031 3230 0d0a 7365 6c65 6374  th = 120..select
+00000b90: 203d 205b 0d0a 2020 2245 222c 2020 2023   = [..  "E",   #
+00000ba0: 2070 7963 6f64 6573 7479 6c65 0d0a 2020   pycodestyle..  
+00000bb0: 2257 222c 2020 2023 2070 7963 6f64 6573  "W",   # pycodes
+00000bc0: 7479 6c65 0d0a 2020 2246 222c 2020 2023  tyle..  "F",   #
+00000bd0: 2070 7966 6c61 6b65 730d 0a20 2022 4222   pyflakes..  "B"
+00000be0: 2c20 2020 2320 6275 6762 6561 720d 0a20  ,   # bugbear.. 
+00000bf0: 2022 5550 222c 2020 2320 7079 7570 6772   "UP",  # pyupgr
+00000c00: 6164 650d 0a20 2022 4922 2c20 2020 2320  ade..  "I",   # 
+00000c10: 6973 6f72 740d 0a20 2023 2244 222c 2020  isort..  #"D",  
+00000c20: 2023 2070 7964 6f63 7374 796c 6520 2020   # pydocstyle   
+00000c30: 2320 6164 6420 6c61 7465 720d 0a5d 0d0a  # add later..]..
+00000c40: 6967 6e6f 7265 203d 205b 0d0a 2020 2242  ignore = [..  "B
+00000c50: 3030 3822 2023 7573 6564 2066 6f72 2044  008" #used for D
+00000c60: 4920 696e 6a65 6374 696f 6e0d 0a20 205d  I injection..  ]
+00000c70: 0d0a 6578 7465 6e64 2d65 7863 6c75 6465  ..extend-exclude
+00000c80: 203d 205b 2276 656e 646f 7222 5d0d 0a0d   = ["vendor"]...
+00000c90: 0a5b 746f 6f6c 2e72 7566 662e 7065 722d  .[tool.ruff.per-
+00000ca0: 6669 6c65 2d69 676e 6f72 6573 5d0d 0a22  file-ignores].."
+00000cb0: 7068 6f74 6f62 6f6f 7468 2f61 7070 636f  photobooth/appco
+00000cc0: 6e66 6967 2e70 7922 203d 205b 2245 3530  nfig.py" = ["E50
+00000cd0: 3122 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566  1"]....[tool.ruf
+00000ce0: 662e 7079 646f 6373 7479 6c65 5d0d 0a63  f.pydocstyle]..c
+00000cf0: 6f6e 7665 6e74 696f 6e20 3d20 2267 6f6f  onvention = "goo
+00000d00: 676c 6522                                gle"
```

### Comparing `photobooth_app-0.1.0rc4/PKG-INFO` & `photobooth_app-0.1.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: photobooth-app
-Version: 0.1.0rc4
+Version: 0.1.0rc5
 Summary: Photobooth app written in Python supporting DSLR, picamera2, webcameras
 Project-URL: homepage, https://github.com/mgrl/photobooth-app
 Project-URL: repository, https://github.com/mgrl/photobooth-app
 Project-URL: documentation, https://mgrl.github.io/photobooth-docs
 Author-email: Michael G <me@mgrl.de>
 Maintainer-email: Michael G <me@mgrl.de>
 License-File: LICENSE.md
```

