# Comparing `tmp/matlab-proxy-0.5.9.tar.gz` & `tmp/matlab-proxy-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-proxy-0.5.9.tar", last modified: Wed Apr 26 05:20:09 2023, max compression
+gzip compressed data, was "matlab-proxy-0.6.0.tar", last modified: Mon Jun 12 11:21:26 2023, max compression
```

## Comparing `matlab-proxy-0.5.9.tar` & `matlab-proxy-0.6.0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8116 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/README.md
--rw-r--r--   0 runner    (1001) docker     (123)  1276762 2023-04-26 05:19:52.000000 matlab-proxy-0.5.9/gui/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/public/
--rw-r--r--   0 runner    (1001) docker     (123)   130876 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/actionCreators/
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/actionCreators/actionCreators.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/actionCreators/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/actions/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/components/App/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/components/App/3p/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.952679 matlab-proxy-0.5.9/gui/src/components/App/3p/css/
--rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   153678 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/css/site7.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.svg
--rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.woff
--rw-r--r--   0 runner    (1001) docker     (123)   289658 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
--rw-r--r--   0 runner    (1001) docker     (123)    70212 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    70288 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
--rw-r--r--   0 runner    (1001) docker     (123)   138707 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.svg
--rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    38732 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/components/App/3p/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/App/3p/images/bug_reports/
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/bug_reports/workaround.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/App.css
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/App.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)   220290 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/MATLAB-env-blur.png
--rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/App/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/Confirmation/
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Confirmation/Confirmation.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Confirmation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/Controls/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/Controls.css
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/Controls.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/feedback.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/help.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/restart.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/sign-out.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/start.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Controls/terminate.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/Error/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Error/Error.css
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Error/Error.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Error/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.956679 matlab-proxy-0.5.9/gui/src/components/Help/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Help/Help.css
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Help/Help.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Help/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/Information/
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Information/Information.css
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Information/Information.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Information/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/LicensingGatherer.css
--rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/MHLM.js
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/NLM.js
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/MatlabJsd/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/MatlabJsd/MatlabJsd.css
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/MatlabJsd/MatlabJsd.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/MatlabJsd/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/Overlay/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Overlay/Overlay.css
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Overlay/Overlay.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/Overlay/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/OverlayTrigger.css
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/gripper.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/index.js
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/trigger-error.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/trigger-ok.svg
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/index.js
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/jest.config.json
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/reducers/
--rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/reducers/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/reducers/reducers.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/selectors/
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/selectors/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/selectors/selectors.spec.js
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/serviceWorker.js
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/setupTests.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.948679 matlab-proxy-0.5.9/gui/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/gui/src/test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/gui/src/test/utils/react-test.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/matlab_proxy/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23827 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    44905 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/app_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/default_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/devel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/matlab_proxy/icons/
--rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/icons/matlab.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/matlab_proxy/matlab/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1532 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/matlab/startup.m
--rw-r--r--   0 runner    (1001) docker     (123)    12186 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/matlab_proxy/util/
--rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/list_servers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/matlab_proxy/util/mwi/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/custom_http_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/mwi/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/matlab_proxy/util/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 05:20:09.960679 matlab-proxy-0.5.9/matlab_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10416 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-26 05:19:30.000000 matlab-proxy-0.5.9/matlab_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-26 05:20:09.964679 matlab-proxy-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-04-26 05:18:51.000000 matlab-proxy-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.570898 matlab-proxy-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-12 11:21:26.570898 matlab-proxy-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8117 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.538898 matlab-proxy-0.6.0/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)  1276762 2023-06-12 11:21:04.000000 matlab-proxy-0.6.0/gui/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.542898 matlab-proxy-0.6.0/gui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)   130876 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.542898 matlab-proxy-0.6.0/gui/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.542898 matlab-proxy-0.6.0/gui/src/actionCreators/
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/actionCreators/actionCreators.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7920 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/actionCreators/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.542898 matlab-proxy-0.6.0/gui/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/actions/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.534898 matlab-proxy-0.6.0/gui/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.542898 matlab-proxy-0.6.0/gui/src/components/App/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.534898 matlab-proxy-0.6.0/gui/src/components/App/3p/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.542898 matlab-proxy-0.6.0/gui/src/components/App/3p/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   121200 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   153678 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/css/site7.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.546898 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    20127 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   108738 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45404 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23424 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    18028 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16377 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-eps.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     6448 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-eps.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     6528 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-eps.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   289658 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    70212 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    70288 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   138707 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    38656 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    38732 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.534898 matlab-proxy-0.6.0/gui/src/components/App/3p/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.546898 matlab-proxy-0.6.0/gui/src/components/App/3p/images/bug_reports/
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/images/bug_reports/workaround.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.534898 matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.550898 matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/App.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)   220290 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/MATLAB-env-blur.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6702 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/App/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.550898 matlab-proxy-0.6.0/gui/src/components/Confirmation/
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Confirmation/Confirmation.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Confirmation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.550898 matlab-proxy-0.6.0/gui/src/components/Controls/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/Controls.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/Controls.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/feedback.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/help.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/sign-out.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/start.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Controls/terminate.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.550898 matlab-proxy-0.6.0/gui/src/components/Error/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Error/Error.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Error/Error.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Error/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.554898 matlab-proxy-0.6.0/gui/src/components/Help/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Help/Help.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Help/Help.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Help/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.554898 matlab-proxy-0.6.0/gui/src/components/Information/
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Information/Information.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Information/Information.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Information/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.554898 matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/LicensingGatherer.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/MHLM.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/NLM.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.554898 matlab-proxy-0.6.0/gui/src/components/MatlabJsd/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/MatlabJsd/MatlabJsd.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/MatlabJsd/MatlabJsd.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/MatlabJsd/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.558898 matlab-proxy-0.6.0/gui/src/components/Overlay/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Overlay/Overlay.css
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Overlay/Overlay.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/Overlay/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.558898 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/OverlayTrigger.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/gripper.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/trigger-error.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/trigger-ok.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/jest.config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.558898 matlab-proxy-0.6.0/gui/src/reducers/
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/reducers/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14469 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/reducers/reducers.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.558898 matlab-proxy-0.6.0/gui/src/selectors/
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/selectors/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14263 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/selectors/selectors.spec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/serviceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/setupTests.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.534898 matlab-proxy-0.6.0/gui/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.558898 matlab-proxy-0.6.0/gui/src/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/gui/src/test/utils/react-test.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.562898 matlab-proxy-0.6.0/matlab_proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23991 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44905 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/app_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/default_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/devel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.562898 matlab-proxy-0.6.0/matlab_proxy/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/icons/matlab.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.562898 matlab-proxy-0.6.0/matlab_proxy/matlab/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1535 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/matlab/startup.m
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.566898 matlab-proxy-0.6.0/matlab_proxy/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/list_servers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10941 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.566898 matlab-proxy-0.6.0/matlab_proxy/util/mwi/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/custom_http_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.570898 matlab-proxy-0.6.0/matlab_proxy/util/mwi/embedded_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/embedded_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/embedded_connector/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/embedded_connector/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/mwi/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/matlab_proxy/util/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 11:21:26.562898 matlab-proxy-0.6.0/matlab_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-06-12 11:20:38.000000 matlab-proxy-0.6.0/matlab_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4870 2023-06-12 11:20:38.000000 matlab-proxy-0.6.0/matlab_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:20:38.000000 matlab-proxy-0.6.0/matlab_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-12 11:20:38.000000 matlab-proxy-0.6.0/matlab_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 11:20:38.000000 matlab-proxy-0.6.0/matlab_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-12 11:20:38.000000 matlab-proxy-0.6.0/matlab_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-12 11:20:38.000000 matlab-proxy-0.6.0/matlab_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-12 11:21:26.570898 matlab-proxy-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-06-12 11:19:52.000000 matlab-proxy-0.6.0/setup.py
```

### Comparing `matlab-proxy-0.5.9/LICENSE.md` & `matlab-proxy-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/PKG-INFO` & `matlab-proxy-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.5.9
+Version: 0.6.0
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
         
-        Copyright (c) 2020-2022 The MathWorks, Inc. All rights reserved.
+        Copyright (c) 2020-2023 The MathWorks, Inc. All rights reserved.
         
         ----
         
         `matlab-proxy` is a Python® package which enables you to launch MATLAB® and access it from a web browser.
         
         Installation of this package creates an executable `matlab-proxy-app`, which launches MATLAB and provides a URL to access it. 
          
@@ -51,15 +51,15 @@
           ```bash
           # On a RHEL based system:
           $ yum search Xvfb
           xorg-x11-server-Xvfb.x86_64 : A X Windows System virtual framebuffer X server.
         
           $ sudo yum install xorg-x11-server-Xvfb
           ```
-        * Python versions: **3.7** | **3.8** | **3.9**  | **3.10**
+        * Python versions: **3.8** | **3.9**  | **3.10** | **3.11**
         * [Browser Requirements](https://www.mathworks.com/support/requirements/browser-requirements.html)
         
         * Supported Operating Systems:
             * Linux®
             * Windows® Operating System ( starting v0.4.0 of matlab-proxy )
             * MacOS (starting v0.5.0 of matlab-proxy )    
         See [Platform Support](#platform-support) for more information 
@@ -187,14 +187,14 @@
         We encourage you to try this repository with your environment and provide feedback. 
         If you encounter a technical issue or have an enhancement request, create an issue [here](https://github.com/mathworks/matlab-proxy/issues)
 Keywords: Proxy,MATLAB Proxy,MATLAB,MATLAB Javascript Desktop,MATLAB Web Desktop,Remote MATLAB Web Access
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ~=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `matlab-proxy-0.5.9/README.md` & `matlab-proxy-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # MATLAB Proxy
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
 
-Copyright (c) 2020-2022 The MathWorks, Inc. All rights reserved.
+Copyright (c) 2020-2023 The MathWorks, Inc. All rights reserved.
 
 ----
 
 `matlab-proxy` is a Python® package which enables you to launch MATLAB® and access it from a web browser.
 
 Installation of this package creates an executable `matlab-proxy-app`, which launches MATLAB and provides a URL to access it. 
  
@@ -43,15 +43,15 @@
   ```bash
   # On a RHEL based system:
   $ yum search Xvfb
   xorg-x11-server-Xvfb.x86_64 : A X Windows System virtual framebuffer X server.
 
   $ sudo yum install xorg-x11-server-Xvfb
   ```
-* Python versions: **3.7** | **3.8** | **3.9**  | **3.10**
+* Python versions: **3.8** | **3.9**  | **3.10** | **3.11**
 * [Browser Requirements](https://www.mathworks.com/support/requirements/browser-requirements.html)
 
 * Supported Operating Systems:
     * Linux®
     * Windows® Operating System ( starting v0.4.0 of matlab-proxy )
     * MacOS (starting v0.5.0 of matlab-proxy )    
 See [Platform Support](#platform-support) for more information
```

### Comparing `matlab-proxy-0.5.9/gui/README.md` & `matlab-proxy-0.6.0/gui/README.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/package-lock.json` & `matlab-proxy-0.6.0/gui/package-lock.json`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/package.json` & `matlab-proxy-0.6.0/gui/package.json`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/public/favicon.ico` & `matlab-proxy-0.6.0/gui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/public/index.html` & `matlab-proxy-0.6.0/gui/public/index.html`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 <head>
   <meta charset="utf-8" />
   <link rel="icon" href="%PUBLIC_URL%/favicon.ico" />
   <meta name="viewport" content="width=device-width, initial-scale=1" />
   <meta name="theme-color" content="#000000" />
   <meta name="description" content="MATLAB" />
+  <meta name="internal_mw_identifier" content="MWI_MATLAB_PROXY_IDENTIFIER" />
   <link rel="manifest" href="%PUBLIC_URL%/manifest.json" />
   <title>MATLAB</title>
 </head>
 
 <body>
   <noscript>You need to enable JavaScript to run this app.</noscript>
   <div id="root"></div>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 
 
 
 
 
 
+
 You need to enable JavaScript to run this app.
```

### Comparing `matlab-proxy-0.5.9/gui/src/actionCreators/actionCreators.spec.js` & `matlab-proxy-0.6.0/gui/src/actionCreators/actionCreators.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/actionCreators/index.js` & `matlab-proxy-0.6.0/gui/src/actionCreators/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/actions/index.js` & `matlab-proxy-0.6.0/gui/src/actions/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/css/bootstrap.min.css` & `matlab-proxy-0.6.0/gui/src/components/App/3p/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/css/site7.min.css` & `matlab-proxy-0.6.0/gui/src/components/App/3p/css/site7.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.svg` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-eps.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.ttf` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-eps.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-eps.woff` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-eps.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.svg` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-pictograms.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks-pictograms.woff` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks-pictograms.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.svg` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.ttf` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/fonts/mathworks.woff` & `matlab-proxy-0.6.0/gui/src/components/App/3p/fonts/mathworks.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/images/bug_reports/workaround.gif` & `matlab-proxy-0.6.0/gui/src/components/App/3p/images/bug_reports/workaround.gif`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg` & `matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg` & `matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg` & `matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg` & `matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/3p/images/responsive/global/ico-sprite.png` & `matlab-proxy-0.6.0/gui/src/components/App/3p/images/responsive/global/ico-sprite.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/App.css` & `matlab-proxy-0.6.0/gui/src/components/App/App.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/App.spec.js` & `matlab-proxy-0.6.0/gui/src/components/App/App.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/MATLAB-env-blur.png` & `matlab-proxy-0.6.0/gui/src/components/App/MATLAB-env-blur.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/App/index.js` & `matlab-proxy-0.6.0/gui/src/components/App/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Confirmation/Confirmation.spec.js` & `matlab-proxy-0.6.0/gui/src/components/Confirmation/Confirmation.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Confirmation/index.js` & `matlab-proxy-0.6.0/gui/src/components/Confirmation/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/Controls.css` & `matlab-proxy-0.6.0/gui/src/components/Controls/Controls.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/Controls.spec.js` & `matlab-proxy-0.6.0/gui/src/components/Controls/Controls.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/feedback.svg` & `matlab-proxy-0.6.0/gui/src/components/Controls/feedback.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/help.svg` & `matlab-proxy-0.6.0/gui/src/components/Controls/help.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/index.js` & `matlab-proxy-0.6.0/gui/src/components/Controls/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/restart.svg` & `matlab-proxy-0.6.0/gui/src/components/Controls/restart.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/sign-out.svg` & `matlab-proxy-0.6.0/gui/src/components/Controls/sign-out.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/start.svg` & `matlab-proxy-0.6.0/gui/src/components/Controls/start.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/stop.svg` & `matlab-proxy-0.6.0/gui/src/components/Controls/stop.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Controls/terminate.svg` & `matlab-proxy-0.6.0/gui/src/components/Controls/terminate.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Error/Error.spec.js` & `matlab-proxy-0.6.0/gui/src/components/Error/Error.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Error/index.js` & `matlab-proxy-0.6.0/gui/src/components/Error/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Help/Help.spec.js` & `matlab-proxy-0.6.0/gui/src/components/Help/Help.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Help/index.js` & `matlab-proxy-0.6.0/gui/src/components/Help/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Information/Information.css` & `matlab-proxy-0.6.0/gui/src/components/Information/Information.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Information/Information.spec.js` & `matlab-proxy-0.6.0/gui/src/components/Information/Information.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Information/index.js` & `matlab-proxy-0.6.0/gui/src/components/Information/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js` & `matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/MHLM.js` & `matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/MHLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/NLM.js` & `matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/NLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/LicensingGatherer/index.js` & `matlab-proxy-0.6.0/gui/src/components/LicensingGatherer/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/MatlabJsd/MatlabJsd.spec.js` & `matlab-proxy-0.6.0/gui/src/components/MatlabJsd/MatlabJsd.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Overlay/Overlay.css` & `matlab-proxy-0.6.0/gui/src/components/Overlay/Overlay.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Overlay/Overlay.spec.js` & `matlab-proxy-0.6.0/gui/src/components/Overlay/Overlay.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/Overlay/index.js` & `matlab-proxy-0.6.0/gui/src/components/Overlay/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/OverlayTrigger.css` & `matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/OverlayTrigger.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js` & `matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js` & `matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/index.js` & `matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/trigger-error.svg` & `matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/trigger-error.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/components/OverlayTrigger/trigger-ok.svg` & `matlab-proxy-0.6.0/gui/src/components/OverlayTrigger/trigger-ok.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/index.js` & `matlab-proxy-0.6.0/gui/src/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/logo.svg` & `matlab-proxy-0.6.0/gui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/reducers/index.js` & `matlab-proxy-0.6.0/gui/src/reducers/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/reducers/reducers.spec.js` & `matlab-proxy-0.6.0/gui/src/reducers/reducers.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/selectors/index.js` & `matlab-proxy-0.6.0/gui/src/selectors/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/selectors/selectors.spec.js` & `matlab-proxy-0.6.0/gui/src/selectors/selectors.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/serviceWorker.js` & `matlab-proxy-0.6.0/gui/src/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/gui/src/test/utils/react-test.js` & `matlab-proxy-0.6.0/gui/src/test/utils/react-test.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/__init__.py` & `matlab-proxy-0.6.0/matlab_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/app.py` & `matlab-proxy-0.6.0/matlab_proxy/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 import matlab_proxy
 from matlab_proxy import settings, util
 from matlab_proxy.app_state import AppState
 from matlab_proxy.default_configuration import config
 from matlab_proxy.util import list_servers, mwi
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 from matlab_proxy.util.mwi import token_auth
-from matlab_proxy.util.mwi.exceptions import LicensingError, InvalidTokenError
+from matlab_proxy.util.mwi.exceptions import AppError, LicensingError, InvalidTokenError
 
 mimetypes.add_type("font/woff", ".woff")
 mimetypes.add_type("font/woff2", ".woff2")
 mimetypes.add_type("font/eot", ".eot")
 mimetypes.add_type("font/ttf", ".ttf")
 mimetypes.add_type("application/json", ".map")
 mimetypes.add_type("image/png", ".ico")
@@ -72,19 +72,22 @@
         error (Object): Instance of NetworkLicensingError or OnlineLicensingError or MatlabError
 
     Returns:
         Dict: Containing information about the error.
     """
     if error is None:
         return None
-    return {
-        "message": error.message,
-        "logs": error.logs,
-        "type": error.__class__.__name__,
-    }
+    if isinstance(error, AppError):
+        return {
+            "message": error.message,
+            "logs": error.logs,
+            "type": error.__class__.__name__,
+        }
+    else:
+        return {"message": error.__str__, "logs": "", "type": error.__class__.__name__}
 
 
 async def create_status_response(app, loadUrl=None):
     """Send a generic status response about the state of server,MATLAB and MATLAB Licensing
 
     Args:
         app (aiohttp.web.Application): Web Server
@@ -396,15 +399,15 @@
     """
     reqH = req.headers.copy()
 
     state = req.app["state"]
     matlab_port = state.matlab_port
     matlab_protocol = req.app["settings"]["matlab_protocol"]
     mwapikey = req.app["settings"]["mwapikey"]
-    matlab_base_url = f"{matlab_protocol}://localhost:{matlab_port}"
+    matlab_base_url = f"{matlab_protocol}://127.0.0.1:{matlab_port}"
 
     # WebSocket
     if (
         reqH.get("connection")
         and reqH.get("connection").lower() == "upgrade"
         and reqH.get("upgrade")
         and reqH.get("upgrade").lower() == "websocket"
```

### Comparing `matlab-proxy-0.5.9/matlab_proxy/app_state.py` & `matlab-proxy-0.6.0/matlab_proxy/app_state.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/default_configuration.py` & `matlab-proxy-0.6.0/matlab_proxy/default_configuration.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/devel.py` & `matlab-proxy-0.6.0/matlab_proxy/devel.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/icons/matlab.svg` & `matlab-proxy-0.6.0/matlab_proxy/icons/matlab.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/matlab/startup.m` & `matlab-proxy-0.6.0/matlab_proxy/matlab/startup.m`

 * *Files 1% similar despite different names*

```diff
@@ -30,7 +30,8 @@
 matlab_settings = settings;
 if ~matlab_settings.matlab.addons.explorer.hasSetting('isExplorerSupported')
     matlab_settings.matlab.addons.explorer.addSetting('isExplorerSupported');
 end
 matlab_settings.matlab.addons.explorer.isExplorerSupported.TemporaryValue = false;
 
 clear
+clc
```

### Comparing `matlab-proxy-0.5.9/matlab_proxy/settings.py` & `matlab-proxy-0.6.0/matlab_proxy/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import sys
 import tempfile
 import uuid
 import xml.etree.ElementTree as ET
 from pathlib import Path
 
 import matlab_proxy
-from matlab_proxy.util import mwi
+from matlab_proxy.util import mwi, system
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 from matlab_proxy.util.mwi import token_auth
 
 logger = mwi.logger.get()
 
 
 def get_matlab_path():
@@ -152,25 +152,30 @@
 
         # NLM Connection String provided by MLM_LICENSE_FILE environment variable
         nlm_conn_str = mwi.validators.validate_mlm_license_file(
             os.environ.get(mwi_env.get_env_name_network_license_manager())
         )
         matlab_lic_mode = ["-licmode", "file"] if nlm_conn_str else ""
 
+        # flag to hide MATLAB Window
+        flag_to_hide_desktop = (
+            "-noDisplayDesktop" if system.is_windows() else "-nodesktop"
+        )
+
         # All config related to matlab-proxy will be saved to user's home folder.
         # This will allow for other user's to launch the integration from the same system
         # and not have their config's overwritten.
         mwi_config_folder = get_mwi_config_folder()
         return {
             "matlab_path": matlab_path,
             "matlab_version": get_matlab_version(matlab_path),
             "matlab_cmd": [
                 "matlab",
                 "-nosplash",
-                "-nodesktop",
+                flag_to_hide_desktop,
                 "-softwareopengl",
                 *matlab_lic_mode,
                 "-r",
                 f"try; run('{matlab_startup_file}'); catch ME; disp(ME.message); end;",
             ],
             "create_xvfb_cmd": create_xvfb_cmd,
             "base_url": mwi.validators.validate_base_url(
```

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/__init__.py` & `matlab-proxy-0.6.0/matlab_proxy/util/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 import matlab_proxy
 from matlab_proxy.util import mwi, system
 from matlab_proxy.util.event_loop import *
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 
 logger = mwi.logger.get()
 
+# Global value to detect whether interrupt signal handler has been triggered or not.
+interrupt_signal_caught = False
+
 
 def parse_cli_args():
     """Parses CLI arguments passed to the main() function.
 
     Returns:
         dict: Containing the parsed arguments
     """
@@ -93,16 +96,26 @@
 
     def catch_interrupt_signal(*args):
         """Nested method which works as a interrupt signal handler.
 
         Raises:
             SystemExit: Raises SystemExit which will stop execution of loop.run_forever() in app.main()
         """
-        logger.debug("Interrupt Signal handler called with args:\n", *args)
-        raise SystemExit
+        logger.debug("Interrupt Signal handler called")
+
+        # Only raise SystemExit when the handler is invoked for the first time.
+        # Ignore subsequent handler invocations of interrupt signals. This is
+        # required so that asyncio event loop gracefully cancels pending tasks
+        # and exits.
+        global interrupt_signal_caught
+        if interrupt_signal_caught is False:
+            interrupt_signal_caught = True
+            raise SystemExit
+
+        logger.debug("Interrupt is already being serviced.")
 
     for interrupt_signal in system.get_supported_termination_signals():
         logger.debug(f"Registering handler for signal: {interrupt_signal} ")
 
         if system.is_posix():
             loop.add_signal_handler(interrupt_signal, catch_interrupt_signal)
         else:
```

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/event_loop.py` & `matlab-proxy-0.6.0/matlab_proxy/util/event_loop.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/list_servers.py` & `matlab-proxy-0.6.0/matlab_proxy/util/list_servers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mw.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mw.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mwi/custom_http_headers.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mwi/custom_http_headers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/helpers.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mwi/embedded_connector/helpers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mwi/embedded_connector/request.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mwi/embedded_connector/request.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mwi/environment_variables.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mwi/environment_variables.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mwi/exceptions.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mwi/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,11 +159,14 @@
     """Logs any error to stdout.
 
     Args:
         logger (logging): A instance of the logging.getLogger()
         err (Class): An instance of one of the  Error classes as defined above.
         Example: OnlineLicensingError, EntitlementError
     """
-    logs_str = ("\n" + "\n".join(err.logs)) if err.logs is not None else ""
-    logger.error(
-        err.message if err.message else "An Exception was raised:\n" + logs_str
-    )
+    if isinstance(err, AppError):
+        logs_str = ("\n" + "\n".join(err.logs)) if err.logs is not None else ""
+        logger.error(
+            err.message if err.message else "An Exception was raised:\n" + logs_str
+        )
+    else:
+        logger.error(err)
```

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mwi/logger.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mwi/logger.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mwi/token_auth.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mwi/token_auth.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/mwi/validators.py` & `matlab-proxy-0.6.0/matlab_proxy/util/mwi/validators.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/system.py` & `matlab-proxy-0.6.0/matlab_proxy/util/system.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/matlab_proxy/util/windows.py` & `matlab-proxy-0.6.0/matlab_proxy/util/windows.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2022 The MathWorks, Inc.
 import asyncio
 
 from matlab_proxy import util
 from matlab_proxy.util import mwi
 from matlab_proxy.util.mwi import environment_variables as mwi_env
 
+
 """ This file contains methods specific to non-posix / windows OS.
 """
 
 logger = mwi.logger.get()
 
 
 def get_event_loop():
@@ -39,31 +40,32 @@
 
     Raises:
         AssertionError: When assertions are not met.
 
     Returns:
         psutil.Process(): The MATLAB process object.
     """
+    import psutil
 
     intermediate_proc = await asyncio.create_subprocess_exec(
         *matlab_cmd,
         env=matlab_env,
         stderr=asyncio.subprocess.STDOUT,
     )
 
     # In testing mode, the devel.py file is run, which is the fake MATLAB server.
     # So, there is no need to check for an intermediate process when testing and can return
     # the same process as a psutil.Process() object.
     if mwi_env.is_testing_mode_enabled() or mwi_env.is_development_mode_enabled():
-        import psutil
-
         proc = psutil.Process(intermediate_proc.pid)
 
         return proc
 
+    matlab = None
+
     try:
         children = util.get_child_processes(intermediate_proc)
 
         # Ensure that only 1 child process has been created.
         assert (
             len(children) == 1
         ), "Multiple child processes were created. Was expecting only 1."
@@ -72,10 +74,27 @@
         matlab = children[0]
         assert (
             "MATLAB.exe" == matlab.name()
         ), "Expecting the child process name to be MATLAB.exe"
 
     except AssertionError as err:
         raise err
+    except psutil.NoSuchProcess:
+        # We reach here when the intermediate process launched by matlab-proxy died
+        # before we can query for its child processes. Hence, to find the actual MATLAB
+        # process, we check all the processes name and parent process id. Ideally, this
+        # approach should work in all cases unless MATLAB itself has exited / crashed.
+        logger.debug(
+            "Intermediate process not found. Querying all process to find MATLAB"
+        )
+        for process in psutil.process_iter():
+            if (
+                process.name() == "MATLAB.exe"
+                and process.ppid() == intermediate_proc.pid
+            ):
+                matlab = process
+                break
+
+    assert matlab != None, "MATLAB Process ID not found"
 
     # Return the actual MATLAB processes
-    return children[0]
+    return matlab
```

### Comparing `matlab-proxy-0.5.9/matlab_proxy.egg-info/PKG-INFO` & `matlab-proxy-0.6.0/matlab_proxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.5.9
+Version: 0.6.0
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
         
-        Copyright (c) 2020-2022 The MathWorks, Inc. All rights reserved.
+        Copyright (c) 2020-2023 The MathWorks, Inc. All rights reserved.
         
         ----
         
         `matlab-proxy` is a Python® package which enables you to launch MATLAB® and access it from a web browser.
         
         Installation of this package creates an executable `matlab-proxy-app`, which launches MATLAB and provides a URL to access it. 
          
@@ -51,15 +51,15 @@
           ```bash
           # On a RHEL based system:
           $ yum search Xvfb
           xorg-x11-server-Xvfb.x86_64 : A X Windows System virtual framebuffer X server.
         
           $ sudo yum install xorg-x11-server-Xvfb
           ```
-        * Python versions: **3.7** | **3.8** | **3.9**  | **3.10**
+        * Python versions: **3.8** | **3.9**  | **3.10** | **3.11**
         * [Browser Requirements](https://www.mathworks.com/support/requirements/browser-requirements.html)
         
         * Supported Operating Systems:
             * Linux®
             * Windows® Operating System ( starting v0.4.0 of matlab-proxy )
             * MacOS (starting v0.5.0 of matlab-proxy )    
         See [Platform Support](#platform-support) for more information 
@@ -187,14 +187,14 @@
         We encourage you to try this repository with your environment and provide feedback. 
         If you encounter a technical issue or have an enhancement request, create an issue [here](https://github.com/mathworks/matlab-proxy/issues)
 Keywords: Proxy,MATLAB Proxy,MATLAB,MATLAB Javascript Desktop,MATLAB Web Desktop,Remote MATLAB Web Access
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: ~=3.7
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `matlab-proxy-0.5.9/matlab_proxy.egg-info/SOURCES.txt` & `matlab-proxy-0.6.0/matlab_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.5.9/setup.py` & `matlab-proxy-0.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 INSTALL_REQUIRES = ["aiohttp>=3.7.4", "psutil", "aiohttp_session[secure]"]
 
 HERE = Path(__file__).parent.resolve()
 long_description = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="matlab-proxy",
-    version="0.5.9",
+    version="0.6.0",
     url=config["doc_url"],
     author="The MathWorks, Inc.",
     author_email="cloud@mathworks.com",
     license="MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE",
     description="Python® package enables you to launch MATLAB® and access it from a web browser.",
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -82,20 +82,20 @@
         "MATLAB Web Desktop",
         "Remote MATLAB Web Access",
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    python_requires="~=3.7",
+    python_requires="~=3.8",
     install_requires=INSTALL_REQUIRES,
     tests_require=TESTS_REQUIRES,
     extras_require={"dev": ["aiohttp-devtools", "black"] + TESTS_REQUIRES},
     # The entrypoint will be used by multiple packages that have this package as an installation
     # dependency. These packages can use the same API, get_entrypoint_name(), to make their configs discoverable
     entry_points={
         matlab_proxy.get_entrypoint_name(): [
```

