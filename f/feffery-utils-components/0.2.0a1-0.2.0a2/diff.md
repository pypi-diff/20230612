# Comparing `tmp/feffery_utils_components-0.2.0a1.tar.gz` & `tmp/feffery_utils_components-0.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_utils_components-0.2.0a1.tar", last modified: Mon May 29 05:42:41 2023, max compression
+gzip compressed data, was "feffery_utils_components-0.2.0a2.tar", last modified: Mon Jun 12 07:42:59 2023, max compression
```

## Comparing `feffery_utils_components-0.2.0a1.tar` & `feffery_utils_components-0.2.0a2.tar`

### file list

```diff
@@ -1,85 +1,86 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 05:42:41.231263 feffery_utils_components-0.2.0a1/
--rw-rw-rw-   0        0        0     1087 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a1/LICENSE
--rw-rw-rw-   0        0        0      484 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a1/MANIFEST.in
--rw-rw-rw-   0        0        0      342 2023-05-29 05:42:41.230255 feffery_utils_components-0.2.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-05-28 10:44:03.000000 feffery_utils_components-0.2.0a1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 05:42:41.223075 feffery_utils_components-0.2.0a1/feffery_utils_components/
--rw-rw-rw-   0        0        0     1877 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyAutoAnimate.py
--rw-rw-rw-   0        0        0     2015 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyBlockColorPicker.py
--rw-rw-rw-   0        0        0     2093 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCaptcha.py
--rw-rw-rw-   0        0        0     2207 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCircleColorPicker.py
--rw-rw-rw-   0        0        0     2049 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCookie.py
--rw-rw-rw-   0        0        0     1616 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCountDown.py
--rw-rw-rw-   0        0        0     2508 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCountUp.py
--rw-rw-rw-   0        0        0     1431 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCssVar.py
--rw-rw-rw-   0        0        0     2078 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyDeviceDetect.py
--rw-rw-rw-   0        0        0     4313 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyDiv.py
--rw-rw-rw-   0        0        0     1556 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyDocumentVisibility.py
--rw-rw-rw-   0        0        0     1449 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyExecuteJs.py
--rw-rw-rw-   0        0        0     1610 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyExternalCss.py
--rw-rw-rw-   0        0        0     1602 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyExternalJs.py
--rw-rw-rw-   0        0        0     2390 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyExtraSpinner.py
--rw-rw-rw-   0        0        0     1526 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyEyeDropper.py
--rw-rw-rw-   0        0        0     2687 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyFancyButton.py
--rw-rw-rw-   0        0        0     2816 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyFancyMessage.py
--rw-rw-rw-   0        0        0     3737 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyFancyNotification.py
--rw-rw-rw-   0        0        0     1733 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyFullscreen.py
--rw-rw-rw-   0        0        0     1483 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGeolocation.py
--rw-rw-rw-   0        0        0     2037 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGithubColorPicker.py
--rw-rw-rw-   0        0        0     5043 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGrid.py
--rw-rw-rw-   0        0        0     1749 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGridItem.py
--rw-rw-rw-   0        0        0     3888 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGuide.py
--rw-rw-rw-   0        0        0     1727 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyHexColorPicker.py
--rw-rw-rw-   0        0        0     2498 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyHighlightWords.py
--rw-rw-rw-   0        0        0     1529 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyIdle.py
--rw-rw-rw-   0        0        0     1728 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyImagePaste.py
--rw-rw-rw-   0        0        0     1713 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyInViewport.py
--rw-rw-rw-   0        0        0     3879 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyJsonViewer.py
--rw-rw-rw-   0        0        0     1704 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyKeyPress.py
--rw-rw-rw-   0        0        0     2109 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyLazyLoad.py
--rw-rw-rw-   0        0        0     1809 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyListenPaste.py
--rw-rw-rw-   0        0        0     1538 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyListenScroll.py
--rw-rw-rw-   0        0        0     1462 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyListenUnload.py
--rw-rw-rw-   0        0        0     2108 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyLocation.py
--rw-rw-rw-   0        0        0     3312 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyMotion.py
--rw-rw-rw-   0        0        0     1463 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyMousePosition.py
--rw-rw-rw-   0        0        0     2479 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyQRCode.py
--rw-rw-rw-   0        0        0     1449 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyRawHTML.py
--rw-rw-rw-   0        0        0     1505 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyReload.py
--rw-rw-rw-   0        0        0     3724 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyResizable.py
--rw-rw-rw-   0        0        0     1459 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyResponsive.py
--rw-rw-rw-   0        0        0     1737 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyRgbColorPicker.py
--rw-rw-rw-   0        0        0     2653 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyScroll.py
--rw-rw-rw-   0        0        0     2531 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyScrollbars.py
--rw-rw-rw-   0        0        0     1651 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySessionStorage.py
--rw-rw-rw-   0        0        0     1433 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySetTitle.py
--rw-rw-rw-   0        0        0     1753 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyShadowDom.py
--rw-rw-rw-   0        0        0     3498 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyShortcutPanel.py
--rw-rw-rw-   0        0        0     1945 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySortableContainer.py
--rw-rw-rw-   0        0        0     1698 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySortableItem.py
--rw-rw-rw-   0        0        0     2472 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySplit.py
--rw-rw-rw-   0        0        0     1686 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySplitPane.py
--rw-rw-rw-   0        0        0     1874 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySticky.py
--rw-rw-rw-   0        0        0     1433 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyStyle.py
--rw-rw-rw-   0        0        0     1533 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyTimeout.py
--rw-rw-rw-   0        0        0     2845 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyTopProgress.py
--rw-rw-rw-   0        0        0     2057 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyTwitterColorPicker.py
--rw-rw-rw-   0        0        0     1606 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyUnmount.py
--rw-rw-rw-   0        0        0     2050 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyVirtualList.py
--rw-rw-rw-   0        0        0     2311 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyWebSocket.py
--rw-rw-rw-   0        0        0     1629 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyWheelColorPicker.py
--rw-rw-rw-   0        0        0     1528 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyWindowSize.py
--rw-rw-rw-   0        0        0     2610 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/__init__.py
--rw-rw-rw-   0        0        0     4900 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/_imports_.py
--rw-rw-rw-   0        0        0  1333851 2023-05-29 05:42:37.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/feffery_utils_components.min.js
--rw-rw-rw-   0        0        0   201566 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/metadata.json
--rw-rw-rw-   0        0        0     3997 2023-05-29 05:42:38.000000 feffery_utils_components-0.2.0a1/feffery_utils_components/package-info.json
-drwxrwxrwx   0        0        0        0 2023-05-29 05:42:41.229249 feffery_utils_components-0.2.0a1/feffery_utils_components.egg-info/
--rw-rw-rw-   0        0        0      342 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3498 2023-05-29 05:42:41.000000 feffery_utils_components-0.2.0a1/feffery_utils_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-29 05:42:40.000000 feffery_utils_components-0.2.0a1/feffery_utils_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3997 2023-05-29 05:41:29.000000 feffery_utils_components-0.2.0a1/package.json
--rw-rw-rw-   0        0        0       42 2023-05-29 05:42:41.231263 feffery_utils_components-0.2.0a1/setup.cfg
--rw-rw-rw-   0        0        0      728 2023-05-06 01:25:35.000000 feffery_utils_components-0.2.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 07:42:59.525867 feffery_utils_components-0.2.0a2/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a2/LICENSE
+-rw-rw-rw-   0        0        0      484 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a2/MANIFEST.in
+-rw-rw-rw-   0        0        0      342 2023-06-12 07:42:59.524859 feffery_utils_components-0.2.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-05-28 10:44:03.000000 feffery_utils_components-0.2.0a2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 07:42:59.517733 feffery_utils_components-0.2.0a2/feffery_utils_components/
+-rw-rw-rw-   0        0        0     1877 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyAutoAnimate.py
+-rw-rw-rw-   0        0        0     2015 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyBlockColorPicker.py
+-rw-rw-rw-   0        0        0     2093 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCaptcha.py
+-rw-rw-rw-   0        0        0     2207 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCircleColorPicker.py
+-rw-rw-rw-   0        0        0     2780 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCompareSlider.py
+-rw-rw-rw-   0        0        0     2049 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCookie.py
+-rw-rw-rw-   0        0        0     1616 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCountDown.py
+-rw-rw-rw-   0        0        0     2508 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCountUp.py
+-rw-rw-rw-   0        0        0     1431 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCssVar.py
+-rw-rw-rw-   0        0        0     2078 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyDeviceDetect.py
+-rw-rw-rw-   0        0        0     4313 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyDiv.py
+-rw-rw-rw-   0        0        0     1556 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyDocumentVisibility.py
+-rw-rw-rw-   0        0        0     1449 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyExecuteJs.py
+-rw-rw-rw-   0        0        0     1610 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyExternalCss.py
+-rw-rw-rw-   0        0        0     1602 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyExternalJs.py
+-rw-rw-rw-   0        0        0     2390 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyExtraSpinner.py
+-rw-rw-rw-   0        0        0     1526 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyEyeDropper.py
+-rw-rw-rw-   0        0        0     2687 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyFancyButton.py
+-rw-rw-rw-   0        0        0     2816 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyFancyMessage.py
+-rw-rw-rw-   0        0        0     3737 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyFancyNotification.py
+-rw-rw-rw-   0        0        0     1733 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyFullscreen.py
+-rw-rw-rw-   0        0        0     1483 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGeolocation.py
+-rw-rw-rw-   0        0        0     2037 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGithubColorPicker.py
+-rw-rw-rw-   0        0        0     5043 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGrid.py
+-rw-rw-rw-   0        0        0     1749 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGridItem.py
+-rw-rw-rw-   0        0        0     3888 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGuide.py
+-rw-rw-rw-   0        0        0     1727 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyHexColorPicker.py
+-rw-rw-rw-   0        0        0     2498 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyHighlightWords.py
+-rw-rw-rw-   0        0        0     1529 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyIdle.py
+-rw-rw-rw-   0        0        0     1728 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyImagePaste.py
+-rw-rw-rw-   0        0        0     1713 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyInViewport.py
+-rw-rw-rw-   0        0        0     3879 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyJsonViewer.py
+-rw-rw-rw-   0        0        0     1704 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyKeyPress.py
+-rw-rw-rw-   0        0        0     2109 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyLazyLoad.py
+-rw-rw-rw-   0        0        0     1809 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyListenPaste.py
+-rw-rw-rw-   0        0        0     1538 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyListenScroll.py
+-rw-rw-rw-   0        0        0     1462 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyListenUnload.py
+-rw-rw-rw-   0        0        0     2108 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyLocation.py
+-rw-rw-rw-   0        0        0     3312 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyMotion.py
+-rw-rw-rw-   0        0        0     1463 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyMousePosition.py
+-rw-rw-rw-   0        0        0     2479 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyQRCode.py
+-rw-rw-rw-   0        0        0     1449 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyRawHTML.py
+-rw-rw-rw-   0        0        0     1505 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyReload.py
+-rw-rw-rw-   0        0        0     3724 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyResizable.py
+-rw-rw-rw-   0        0        0     1459 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyResponsive.py
+-rw-rw-rw-   0        0        0     1737 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyRgbColorPicker.py
+-rw-rw-rw-   0        0        0     2653 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyScroll.py
+-rw-rw-rw-   0        0        0     2531 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyScrollbars.py
+-rw-rw-rw-   0        0        0     1651 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySessionStorage.py
+-rw-rw-rw-   0        0        0     1433 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySetTitle.py
+-rw-rw-rw-   0        0        0     1753 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyShadowDom.py
+-rw-rw-rw-   0        0        0     3498 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyShortcutPanel.py
+-rw-rw-rw-   0        0        0     1945 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySortableContainer.py
+-rw-rw-rw-   0        0        0     1698 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySortableItem.py
+-rw-rw-rw-   0        0        0     2472 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySplit.py
+-rw-rw-rw-   0        0        0     1686 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySplitPane.py
+-rw-rw-rw-   0        0        0     1874 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySticky.py
+-rw-rw-rw-   0        0        0     1433 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyStyle.py
+-rw-rw-rw-   0        0        0     1533 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyTimeout.py
+-rw-rw-rw-   0        0        0     2845 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyTopProgress.py
+-rw-rw-rw-   0        0        0     2057 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyTwitterColorPicker.py
+-rw-rw-rw-   0        0        0     1606 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyUnmount.py
+-rw-rw-rw-   0        0        0     2050 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyVirtualList.py
+-rw-rw-rw-   0        0        0     2311 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyWebSocket.py
+-rw-rw-rw-   0        0        0     1629 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyWheelColorPicker.py
+-rw-rw-rw-   0        0        0     1528 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyWindowSize.py
+-rw-rw-rw-   0        0        0     2610 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/__init__.py
+-rw-rw-rw-   0        0        0     4985 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/_imports_.py
+-rw-rw-rw-   0        0        0  1340713 2023-06-12 07:42:56.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/feffery_utils_components.min.js
+-rw-rw-rw-   0        0        0   205372 2023-06-12 07:42:58.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/metadata.json
+-rw-rw-rw-   0        0        0     4036 2023-06-12 07:42:57.000000 feffery_utils_components-0.2.0a2/feffery_utils_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-06-12 07:42:59.523602 feffery_utils_components-0.2.0a2/feffery_utils_components.egg-info/
+-rw-rw-rw-   0        0        0      342 2023-06-12 07:42:59.000000 feffery_utils_components-0.2.0a2/feffery_utils_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3547 2023-06-12 07:42:59.000000 feffery_utils_components-0.2.0a2/feffery_utils_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 07:42:59.000000 feffery_utils_components-0.2.0a2/feffery_utils_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-12 07:42:59.000000 feffery_utils_components-0.2.0a2/feffery_utils_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-06-12 07:42:59.000000 feffery_utils_components-0.2.0a2/feffery_utils_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4036 2023-06-12 06:36:34.000000 feffery_utils_components-0.2.0a2/package.json
+-rw-rw-rw-   0        0        0       42 2023-06-12 07:42:59.525867 feffery_utils_components-0.2.0a2/setup.cfg
+-rw-rw-rw-   0        0        0      728 2023-05-06 01:25:35.000000 feffery_utils_components-0.2.0a2/setup.py
```

### Comparing `feffery_utils_components-0.2.0a1/LICENSE` & `feffery_utils_components-0.2.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/README.md` & `feffery_utils_components-0.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyAutoAnimate.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyAutoAnimate.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyBlockColorPicker.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyBlockColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCaptcha.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCaptcha.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCircleColorPicker.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCircleColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCookie.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCookie.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCountDown.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCountDown.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCountUp.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCountUp.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyCssVar.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyCssVar.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyDeviceDetect.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyDeviceDetect.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyDiv.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyDiv.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyDocumentVisibility.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyDocumentVisibility.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyExecuteJs.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyExecuteJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyExternalCss.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyExternalCss.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyExternalJs.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyExternalJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyExtraSpinner.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyExtraSpinner.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyEyeDropper.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyEyeDropper.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyFancyButton.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyFancyButton.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyFancyMessage.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyFancyMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyFancyNotification.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyFancyNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyFullscreen.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyFullscreen.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGeolocation.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGeolocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGithubColorPicker.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGithubColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGrid.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGridItem.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGridItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyGuide.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyGuide.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyHexColorPicker.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyHexColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyHighlightWords.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyHighlightWords.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyIdle.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyIdle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyImagePaste.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyImagePaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyInViewport.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyInViewport.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyJsonViewer.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyJsonViewer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyKeyPress.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyKeyPress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyLazyLoad.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyLazyLoad.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyListenPaste.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyListenPaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyListenScroll.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyListenScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyListenUnload.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyListenUnload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyLocation.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyLocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyMotion.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyMotion.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyMousePosition.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyMousePosition.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyQRCode.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyQRCode.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyRawHTML.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyRawHTML.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyReload.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyReload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyResizable.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyResizable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyResponsive.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyResponsive.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyRgbColorPicker.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyRgbColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyScroll.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyScrollbars.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyScrollbars.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySessionStorage.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySessionStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySetTitle.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySetTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyShadowDom.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyShadowDom.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyShortcutPanel.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyShortcutPanel.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySortableContainer.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySortableContainer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySortableItem.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySortableItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySplit.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySplit.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySplitPane.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySplitPane.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferySticky.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferySticky.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyStyle.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyStyle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyTimeout.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyTimeout.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyTopProgress.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyTopProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyTwitterColorPicker.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyTwitterColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyUnmount.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyUnmount.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyVirtualList.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyVirtualList.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyWebSocket.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyWebSocket.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyWheelColorPicker.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyWheelColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/FefferyWindowSize.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/FefferyWindowSize.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/__init__.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/_imports_.py` & `feffery_utils_components-0.2.0a2/feffery_utils_components/_imports_.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from .FefferyHexColorPicker import FefferyHexColorPicker
 from .FefferyRgbColorPicker import FefferyRgbColorPicker
 from .FefferyTwitterColorPicker import FefferyTwitterColorPicker
 from .FefferyWheelColorPicker import FefferyWheelColorPicker
 from .FefferyGrid import FefferyGrid
 from .FefferyGridItem import FefferyGridItem
 from .FefferyCaptcha import FefferyCaptcha
+from .FefferyCompareSlider import FefferyCompareSlider
 from .FefferyCountDown import FefferyCountDown
 from .FefferyCountUp import FefferyCountUp
 from .FefferyCssVar import FefferyCssVar
 from .FefferyDiv import FefferyDiv
 from .FefferyExecuteJs import FefferyExecuteJs
 from .FefferyExternalCss import FefferyExternalCss
 from .FefferyExternalJs import FefferyExternalJs
@@ -73,14 +74,15 @@
     "FefferyHexColorPicker",
     "FefferyRgbColorPicker",
     "FefferyTwitterColorPicker",
     "FefferyWheelColorPicker",
     "FefferyGrid",
     "FefferyGridItem",
     "FefferyCaptcha",
+    "FefferyCompareSlider",
     "FefferyCountDown",
     "FefferyCountUp",
     "FefferyCssVar",
     "FefferyDiv",
     "FefferyExecuteJs",
     "FefferyExternalCss",
     "FefferyExternalJs",
```

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/feffery_utils_components.min.js` & `feffery_utils_components-0.2.0a2/feffery_utils_components/feffery_utils_components.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -57,15 +57,15 @@
         return Object.defineProperty(o, "p", {
             get: (e = i().src.split("/").slice(0, -1).join("/") + "/", function() {
                 return e
             })
         }), "undefined" != typeof jsonpScriptSrc && (a = jsonpScriptSrc, jsonpScriptSrc = function(e) {
             var t, n = /\/_dash-component-suites\//.test(i().src),
                 e = a(e);
-            return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-a1m1685338940"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
+            return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-a2m1686555752"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
         }), o(o.s = 494)
     }([function(e, t) {
                 e.exports = window.PropTypes
             }, function(e, t) {
                 e.exports = window.React
             }, function(e, t, n) {
                 "use strict";
@@ -51788,16 +51788,353 @@
                 }, m1.defaultProps = {
                     direction: ["top", "right", "bottom", "left", "topRight", "bottomRight", "bottomLeft", "topLeft"],
                     minWidth: 10,
                     minHeight: 10,
                     grid: [1, 1],
                     bounds: "window"
                 };
-                var b1 = m1,
-                    v1 = (o.d(e, "FefferyCaptcha", function() {
+                var b1 = m1;
+                const v1 = Object(ze.forwardRef)((e, t) => D.a.createElement("div", Object.assign({}, e, {
+                        style: {
+                            position: "absolute",
+                            top: 0,
+                            left: 0,
+                            width: "100%",
+                            height: "100%",
+                            willChange: "clip",
+                            userSelect: "none",
+                            KhtmlUserSelect: "none",
+                            MozUserSelect: "none",
+                            WebkitUserSelect: "none"
+                        },
+                        "data-rcs": "clip-item",
+                        ref: t
+                    }))),
+                    y1 = (v1.displayName = "ContainerClip", Object(ze.forwardRef)(({
+                        children: e,
+                        portrait: t
+                    }, n) => {
+                        return D.a.createElement("div", {
+                            style: {
+                                position: "absolute",
+                                top: 0,
+                                width: "100%",
+                                height: "100%",
+                                pointerEvents: "none"
+                            },
+                            "data-rcs": "handle-container",
+                            ref: n
+                        }, D.a.createElement("div", {
+                            style: {
+                                position: "absolute",
+                                width: t ? "100%" : void 0,
+                                height: t ? void 0 : "100%",
+                                transform: t ? "translateY(-50%)" : "translateX(-50%)",
+                                pointerEvents: "all"
+                            }
+                        }, e))
+                    })),
+                    w1 = (y1.displayName = "ThisHandleContainer", ({
+                        flip: e
+                    }) => {
+                        return D.a.createElement("div", {
+                            style: {
+                                width: 0,
+                                height: 0,
+                                borderTop: "8px solid transparent",
+                                borderRight: "10px solid",
+                                borderBottom: "8px solid transparent",
+                                transform: e ? "rotate(180deg)" : void 0
+                            }
+                        })
+                    }),
+                    _1 = ({
+                        portrait: e,
+                        buttonStyle: t,
+                        linesStyle: n,
+                        style: r,
+                        ...o
+                    }) => {
+                        r = {
+                            display: "flex",
+                            flexDirection: e ? "row" : "column",
+                            placeItems: "center",
+                            height: "100%",
+                            cursor: e ? "ns-resize" : "ew-resize",
+                            pointerEvents: "none",
+                            color: "#fff",
+                            ...r
+                        }, n = {
+                            flexGrow: 1,
+                            height: e ? 2 : "100%",
+                            width: e ? "100%" : 2,
+                            backgroundColor: "currentColor",
+                            pointerEvents: "auto",
+                            boxShadow: "0 0 7px rgba(0,0,0,.35)",
+                            ...n
+                        }, e = {
+                            display: "grid",
+                            gridAutoFlow: "column",
+                            gap: 8,
+                            placeContent: "center",
+                            flexShrink: 0,
+                            width: 56,
+                            height: 56,
+                            borderRadius: "50%",
+                            borderStyle: "solid",
+                            borderWidth: 2,
+                            pointerEvents: "auto",
+                            backdropFilter: "blur(7px)",
+                            WebkitBackdropFilter: "blur(7px)",
+                            boxShadow: "0 0 7px rgba(0,0,0,.35)",
+                            transform: e ? "rotate(90deg)" : void 0,
+                            ...t
+                        };
+                        return D.a.createElement("div", Object.assign({
+                            className: "__rcs-handle-root"
+                        }, o, {
+                            style: r
+                        }), D.a.createElement("div", {
+                            className: "__rcs-handle-line",
+                            style: n
+                        }), D.a.createElement("div", {
+                            className: "__rcs-handle-button",
+                            style: e
+                        }, D.a.createElement(w1, null), D.a.createElement(w1, {
+                            flip: !0
+                        })), D.a.createElement("div", {
+                            className: "__rcs-handle-line",
+                            style: n
+                        }))
+                    },
+                    x1 = (t, e, n, r) => {
+                        const o = Object(ze.useRef)();
+                        Object(ze.useEffect)(() => {
+                            o.current = e
+                        }, [e]), Object(ze.useEffect)(() => {
+                            if (n && n.addEventListener) {
+                                const e = e => o.current && o.current(e);
+                                return n.addEventListener(t, e, r), () => {
+                                    n.removeEventListener(t, e, r)
+                                }
+                            }
+                        }, [t, n, r])
+                    },
+                    O1 = "undefined" != typeof window && window.document && window.document.createElement ? ze.useLayoutEffect : ze.useEffect,
+                    E1 = {
+                        passive: !0
+                    },
+                    S1 = {
+                        capture: !0,
+                        passive: !1
+                    },
+                    j1 = ({
+                        handle: e,
+                        itemOne: t,
+                        itemTwo: n,
+                        onlyHandleDraggable: r = !1,
+                        onPositionChange: c,
+                        portrait: o = !1,
+                        position: i = 50,
+                        boundsPadding: a = 0,
+                        changePositionOnHover: s = !1,
+                        style: l,
+                        ...u
+                    }) => {
+                        const f = Object(ze.useRef)(null),
+                            d = Object(ze.useRef)(null),
+                            p = Object(ze.useRef)(null),
+                            h = Object(ze.useRef)(i),
+                            g = (e => {
+                                const t = Object(ze.useRef)(e);
+                                return Object(ze.useEffect)(() => {
+                                    t.current = e
+                                }), t.current
+                            })(i),
+                            [m, b] = Object(ze.useState)(!1),
+                            v = Object(ze.useRef)(!1),
+                            [y, w] = Object(ze.useState)(),
+                            [_, x] = Object(ze.useState)(!1),
+                            O = (Object(ze.useEffect)(() => {
+                                w((r ? p : f).current)
+                            }, [r]), Object(ze.useCallback)(function({
+                                x: e,
+                                y: t,
+                                isOffset: n,
+                                portrait: r,
+                                boundsPadding: o
+                            }) {
+                                var {
+                                    top: i,
+                                    left: a,
+                                    width: s,
+                                    height: l
+                                } = f.current.getBoundingClientRect();
+                                0 === s || 0 === l || (t = Math.min(Math.max(r ? n ? t - i - window.pageYOffset : t : n ? e - a - window.pageXOffset : e, 0), r ? l : s) / (i = r ? l / (f.current.offsetHeight || 1) : s / (f.current.offsetWidth || 1)), n = s / i, a = l / i, e = r ? 0 == t || t == a : 0 == t || t == n, l = (s = t / (r ? a : n) * 100) === h.current && (0 === h.current || 100 === h.current), _ && l && e) || (x(!0), h.current = s, i = Math.min(Math.max(t, 0 + o), (r ? a : n) - o), d.current.style.clip = r ? `rect(auto,auto,${i}px,auto)` : `rect(auto,${i}px,auto,auto)`, p.current.style.transform = r ? `translate3d(0,${i}px,0)` : `translate3d(${i}px,0,0)`, c && c(h.current))
+                            }, [_, c])),
+                            E = (Object(ze.useEffect)(() => {
+                                var {
+                                    width: e,
+                                    height: t
+                                } = f.current.getBoundingClientRect(), n = i === g ? h.current : i;
+                                O({
+                                    portrait: o,
+                                    boundsPadding: a,
+                                    x: e / 100 * n,
+                                    y: t / 100 * n
+                                })
+                            }, [o, i, g, a, O]), Object(ze.useCallback)(e => {
+                                e.preventDefault(), O({
+                                    portrait: o,
+                                    boundsPadding: a,
+                                    isOffset: !0,
+                                    x: (e instanceof MouseEvent ? e : e.touches[0]).pageX,
+                                    y: (e instanceof MouseEvent ? e : e.touches[0]).pageY
+                                }), b(!0)
+                            }, [o, a, O])),
+                            S = Object(ze.useCallback)(function(e) {
+                                O({
+                                    portrait: o,
+                                    boundsPadding: a,
+                                    isOffset: !0,
+                                    x: (e instanceof MouseEvent ? e : e.touches[0]).pageX,
+                                    y: (e instanceof MouseEvent ? e : e.touches[0]).pageY
+                                })
+                            }, [o, a, O]),
+                            j = Object(ze.useCallback)(() => {
+                                b(!1)
+                            }, []),
+                            k = Object(ze.useCallback)(({
+                                width: e,
+                                height: t
+                            }) => {
+                                var {
+                                    width: n,
+                                    height: r
+                                } = f.current.getBoundingClientRect();
+                                O({
+                                    portrait: o,
+                                    boundsPadding: a,
+                                    x: e / 100 * h.current * n / e,
+                                    y: t / 100 * h.current * r / t
+                                })
+                            }, [o, a, O]);
+                        Object(ze.useEffect)(() => (m && !v.current && (window.addEventListener("mousemove", S, E1), window.addEventListener("mouseup", j, E1), window.addEventListener("touchmove", S, E1), window.addEventListener("touchend", j, E1), v.current = !0), () => {
+                            v.current && (window.removeEventListener("mousemove", S), window.removeEventListener("mouseup", j), window.removeEventListener("touchmove", S), window.removeEventListener("touchend", j), v.current = !1)
+                        }), [S, j, m]); {
+                            var C = f,
+                                z = k;
+                            const P = Object(ze.useRef)(),
+                                T = Object(ze.useCallback)(() => {
+                                    C.current && P.current && P.current.observe(C.current)
+                                }, [C]);
+                            O1(() => (P.current = new ResizeObserver(([e]) => z(e.contentRect)), T(), () => {
+                                P.current && P.current.disconnect()
+                            }), [z, T])
+                        }
+                        Object(ze.useEffect)(() => {
+                            const e = f.current,
+                                t = () => {
+                                    m || j()
+                                };
+                            return s && (e.addEventListener("mousemove", S, E1), e.addEventListener("mouseleave", t, E1)), () => {
+                                e.removeEventListener("mousemove", S), e.removeEventListener("mouseleave", t)
+                            }
+                        }, [s, S, j, m]), x1("mousedown", E, y, S1), x1("touchstart", E, y, S1);
+                        e = e || D.a.createElement(_1, {
+                            portrait: o
+                        }), l = {
+                            position: "relative",
+                            overflow: "hidden",
+                            cursor: m ? o ? "ns-resize" : "ew-resize" : void 0,
+                            userSelect: "none",
+                            KhtmlUserSelect: "none",
+                            msUserSelect: "none",
+                            MozUserSelect: "none",
+                            WebkitUserSelect: "none",
+                            ...l
+                        };
+                        return D.a.createElement("div", Object.assign({}, u, {
+                            ref: f,
+                            style: l,
+                            "data-rcs": "root"
+                        }), n, D.a.createElement(v1, {
+                            ref: d
+                        }, t), D.a.createElement(y1, {
+                            portrait: o,
+                            ref: p
+                        }, e))
+                    };
+
+                function k1(e) {
+                    var t = e.id,
+                        n = e.style,
+                        r = e.className,
+                        o = e.firstItem,
+                        i = e.secondItem,
+                        a = e.position,
+                        s = e.onlyHandleDraggable,
+                        l = e.boundsPadding,
+                        c = e.direction,
+                        u = e.buttonStyle,
+                        f = e.lineStyle,
+                        d = e.rootStyle,
+                        p = e.setProps,
+                        e = e.loading_state;
+                    return React.createElement(j1, {
+                        id: t,
+                        style: n,
+                        className: r,
+                        itemOne: o,
+                        itemTwo: i,
+                        position: a,
+                        onlyHandleDraggable: s,
+                        boundsPadding: l,
+                        portrait: "vertical" === c,
+                        onPositionChange: function(e) {
+                            return p({
+                                position: e
+                            })
+                        },
+                        handle: React.createElement(_1, {
+                            buttonStyle: u,
+                            lineStyle: f,
+                            style: d,
+                            portrait: "vertical" === c
+                        }),
+                        "data-dash-is-loading": e && e.is_loading || void 0
+                    })
+                }
+                k1.propTypes = {
+                    id: t.a.string,
+                    style: t.a.object,
+                    className: t.a.string,
+                    firstItem: t.a.node,
+                    secondItem: t.a.node,
+                    position: t.a.number,
+                    onlyHandleDraggable: t.a.bool,
+                    boundsPadding: t.a.number,
+                    direction: t.a.oneOf(["horizontal", "vertical"]),
+                    buttonStyle: t.a.object,
+                    lineStyle: t.a.object,
+                    rootStyle: t.a.object,
+                    loading_state: t.a.shape({
+                        is_loading: t.a.bool,
+                        prop_name: t.a.string,
+                        component_name: t.a.string
+                    }),
+                    setProps: t.a.func
+                }, k1.defaultProps = {
+                    position: 50,
+                    onlyHandleDraggable: !0,
+                    boundsPadding: 0,
+                    direction: "horizontal"
+                };
+                var C1 = k1,
+                    z1 = (o.d(e, "FefferyCaptcha", function() {
                         return M
                     }), o.d(e, "FefferyTopProgress", function() {
                         return J
                     }), o.d(e, "FefferyShortcutPanel", function() {
                         return Q.a
                     }), o.d(e, "FefferyGuide", function() {
                         return ee.a
@@ -51917,17 +52254,19 @@
                         return Uy
                     }), o.d(e, "FefferyLocation", function() {
                         return Fy
                     }), o.d(e, "FefferyCookie", function() {
                         return r1
                     }), o.d(e, "FefferyResizable", function() {
                         return b1
+                    }), o.d(e, "FefferyCompareSlider", function() {
+                        return C1
                     }), sessionStorage.setItem);
                 sessionStorage.setItem = function(e, t) {
-                    v1.apply(this, [e, t]);
+                    z1.apply(this, [e, t]);
                     var n = new Event("sessionStorageSetItem");
                     n.triggerKey = e, n[e] = t, window.dispatchEvent(n)
                 }
             }, function(I, L, e) {
                 "use strict";
                 const o = window,
                     N = o.ShadowRoot && (void 0 === o.ShadyCSS || o.ShadyCSS.nativeShadow) && "adoptedStyleSheets" in Document.prototype && "replace" in CSSStyleSheet.prototype,
```

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/metadata.json` & `feffery_utils_components-0.2.0a2/feffery_utils_components/metadata.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9846153846153847%*

 * *Differences: {"'src/lib/components/FefferyCompareSlider.react.js'": "OrderedDict([('description', ''), "*

 * *                                                       "('displayName', 'FefferyCompareSlider'), "*

 * *                                                       "('methods', []), ('props', "*

 * *                                                       "OrderedDict([('id', OrderedDict([('type', "*

 * *                                                       "OrderedDict([('name', 'string')])), "*

 * *                                           […]*

```diff
@@ -107,14 +107,162 @@
                 "required": false,
                 "type": {
                     "name": "number"
                 }
             }
         }
     },
+    "src/lib/components/FefferyCompareSlider.react.js": {
+        "description": "",
+        "displayName": "FefferyCompareSlider",
+        "methods": [],
+        "props": {
+            "boundsPadding": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "0"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "buttonStyle": {
+                "description": "\u8bbe\u7f6e\u62d6\u62fd\u63a7\u4ef6\u6309\u94ae\u90e8\u5206\u7684css\u6837\u5f0f",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "className": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "direction": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "'horizontal'"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "enum",
+                    "value": [
+                        {
+                            "computed": false,
+                            "value": "'horizontal'"
+                        },
+                        {
+                            "computed": false,
+                            "value": "'vertical'"
+                        }
+                    ]
+                }
+            },
+            "firstItem": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "node"
+                }
+            },
+            "id": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "string"
+                }
+            },
+            "lineStyle": {
+                "description": "\u8bbe\u7f6e\u62d6\u62fd\u63a7\u4ef6\u7ebf\u6761\u90e8\u5206\u7684css\u6837\u5f0f",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "loading_state": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "shape",
+                    "value": {
+                        "component_name": {
+                            "description": "Holds the name of the component that is loading",
+                            "name": "string",
+                            "required": false
+                        },
+                        "is_loading": {
+                            "description": "Determines if the component is loading or not",
+                            "name": "bool",
+                            "required": false
+                        },
+                        "prop_name": {
+                            "description": "Holds which property is loading",
+                            "name": "string",
+                            "required": false
+                        }
+                    }
+                }
+            },
+            "onlyHandleDraggable": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "true"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "bool"
+                }
+            },
+            "position": {
+                "defaultValue": {
+                    "computed": false,
+                    "value": "50"
+                },
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "number"
+                }
+            },
+            "rootStyle": {
+                "description": "\u8bbe\u7f6e\u62d6\u62fd\u63a7\u4ef6\u6839\u5143\u7d20\u90e8\u5206\u7684css\u6837\u5f0f",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            },
+            "secondItem": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "node"
+                }
+            },
+            "setProps": {
+                "description": "Dash-assigned callback that should be called to report property changes\r\nto Dash, to make them available for callbacks.",
+                "required": false,
+                "type": {
+                    "name": "func"
+                }
+            },
+            "style": {
+                "description": "",
+                "required": false,
+                "type": {
+                    "name": "object"
+                }
+            }
+        }
+    },
     "src/lib/components/FefferyCountDown.react.js": {
         "description": "",
         "displayName": "FefferyCountDown",
         "methods": [],
         "props": {
             "countdown": {
                 "description": "",
```

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components/package-info.json` & `feffery_utils_components-0.2.0a2/feffery_utils_components/package-info.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659090909090909%*

 * *Differences: {"'dependencies'": "{'react-compare-slider': '^2.2.0'}", "'version'": "'0.2.0-a2'"}*

```diff
@@ -31,14 +31,15 @@
         "ramda": "^0.26.1",
         "rc-virtual-list": "^3.4.8",
         "re-resizable": "^6.9.9",
         "react-awesome-button": "^7.0.5",
         "react-captcha-code": "^1.0.7",
         "react-color": "^2.19.3",
         "react-colorful": "^5.6.1",
+        "react-compare-slider": "^2.2.0",
         "react-copy-to-clipboard": "^5.0.4",
         "react-countup": "^6.4.2",
         "react-device-detect": "^2.2.2",
         "react-flip-numbers": "^3.0.7",
         "react-grid-layout": "^1.3.4",
         "react-highlight-words": "^0.18.0",
         "react-hot-toast": "^2.4.0",
@@ -111,9 +112,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-a1"
+    "version": "0.2.0-a2"
 }
```

### Comparing `feffery_utils_components-0.2.0a1/feffery_utils_components.egg-info/SOURCES.txt` & `feffery_utils_components-0.2.0a2/feffery_utils_components.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 README.md
 package.json
 setup.py
 feffery_utils_components/FefferyAutoAnimate.py
 feffery_utils_components/FefferyBlockColorPicker.py
 feffery_utils_components/FefferyCaptcha.py
 feffery_utils_components/FefferyCircleColorPicker.py
+feffery_utils_components/FefferyCompareSlider.py
 feffery_utils_components/FefferyCookie.py
 feffery_utils_components/FefferyCountDown.py
 feffery_utils_components/FefferyCountUp.py
 feffery_utils_components/FefferyCssVar.py
 feffery_utils_components/FefferyDeviceDetect.py
 feffery_utils_components/FefferyDiv.py
 feffery_utils_components/FefferyDocumentVisibility.py
```

### Comparing `feffery_utils_components-0.2.0a1/package.json` & `feffery_utils_components-0.2.0a2/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9659090909090909%*

 * *Differences: {"'dependencies'": "{'react-compare-slider': '^2.2.0'}", "'version'": "'0.2.0-a2'"}*

```diff
@@ -31,14 +31,15 @@
         "ramda": "^0.26.1",
         "rc-virtual-list": "^3.4.8",
         "re-resizable": "^6.9.9",
         "react-awesome-button": "^7.0.5",
         "react-captcha-code": "^1.0.7",
         "react-color": "^2.19.3",
         "react-colorful": "^5.6.1",
+        "react-compare-slider": "^2.2.0",
         "react-copy-to-clipboard": "^5.0.4",
         "react-countup": "^6.4.2",
         "react-device-detect": "^2.2.2",
         "react-flip-numbers": "^3.0.7",
         "react-grid-layout": "^1.3.4",
         "react-highlight-words": "^0.18.0",
         "react-hot-toast": "^2.4.0",
@@ -111,9 +112,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-a1"
+    "version": "0.2.0-a2"
 }
```

### Comparing `feffery_utils_components-0.2.0a1/setup.py` & `feffery_utils_components-0.2.0a2/setup.py`

 * *Files identical despite different names*

