# Comparing `tmp/feffery_utils_components-0.2.0a7.tar.gz` & `tmp/feffery_utils_components-0.2.0a8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feffery_utils_components-0.2.0a7.tar", last modified: Fri Jul 21 02:39:01 2023, max compression
+gzip compressed data, was "feffery_utils_components-0.2.0a8.tar", last modified: Tue Aug  8 01:23:04 2023, max compression
```

## Comparing `feffery_utils_components-0.2.0a7.tar` & `feffery_utils_components-0.2.0a8.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 02:39:01.691739 feffery_utils_components-0.2.0a7/
--rw-rw-rw-   0        0        0     1087 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a7/LICENSE
--rw-rw-rw-   0        0        0      484 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a7/MANIFEST.in
--rw-rw-rw-   0        0        0      342 2023-07-21 02:39:01.690740 feffery_utils_components-0.2.0a7/PKG-INFO
--rw-rw-rw-   0        0        0     1432 2023-05-28 10:44:03.000000 feffery_utils_components-0.2.0a7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-21 02:39:01.677209 feffery_utils_components-0.2.0a7/feffery_utils_components/
--rw-rw-rw-   0        0        0     1877 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyAutoAnimate.py
--rw-rw-rw-   0        0        0     2015 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyBlockColorPicker.py
--rw-rw-rw-   0        0        0     2093 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCaptcha.py
--rw-rw-rw-   0        0        0     2207 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCircleColorPicker.py
--rw-rw-rw-   0        0        0     2784 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCompareSlider.py
--rw-rw-rw-   0        0        0     2049 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCookie.py
--rw-rw-rw-   0        0        0     1616 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCountDown.py
--rw-rw-rw-   0        0        0     2508 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCountUp.py
--rw-rw-rw-   0        0        0     1431 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCssVar.py
--rw-rw-rw-   0        0        0     2078 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyDeviceDetect.py
--rw-rw-rw-   0        0        0     4313 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyDiv.py
--rw-rw-rw-   0        0        0     1556 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyDocumentVisibility.py
--rw-rw-rw-   0        0        0     1449 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyExecuteJs.py
--rw-rw-rw-   0        0        0     1610 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyExternalCss.py
--rw-rw-rw-   0        0        0     1602 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyExternalJs.py
--rw-rw-rw-   0        0        0     2390 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyExtraSpinner.py
--rw-rw-rw-   0        0        0     1526 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyEyeDropper.py
--rw-rw-rw-   0        0        0     2687 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyFancyButton.py
--rw-rw-rw-   0        0        0     2816 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyFancyMessage.py
--rw-rw-rw-   0        0        0     3737 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyFancyNotification.py
--rw-rw-rw-   0        0        0     1733 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyFullscreen.py
--rw-rw-rw-   0        0        0     1483 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGeolocation.py
--rw-rw-rw-   0        0        0     2037 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGithubColorPicker.py
--rw-rw-rw-   0        0        0     5043 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGrid.py
--rw-rw-rw-   0        0        0     1749 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGridItem.py
--rw-rw-rw-   0        0        0     3888 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGuide.py
--rw-rw-rw-   0        0        0     1727 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyHexColorPicker.py
--rw-rw-rw-   0        0        0     2498 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyHighlightWords.py
--rw-rw-rw-   0        0        0     1529 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyIdle.py
--rw-rw-rw-   0        0        0     1728 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyImagePaste.py
--rw-rw-rw-   0        0        0     1713 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyInViewport.py
--rw-rw-rw-   0        0        0     3879 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyJsonViewer.py
--rw-rw-rw-   0        0        0     1704 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyKeyPress.py
--rw-rw-rw-   0        0        0     2109 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLazyLoad.py
--rw-rw-rw-   0        0        0     1809 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyListenPaste.py
--rw-rw-rw-   0        0        0     1538 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyListenScroll.py
--rw-rw-rw-   0        0        0     1462 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyListenUnload.py
--rw-rw-rw-   0        0        0     1768 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLocalLargeStorage.py
--rw-rw-rw-   0        0        0     1748 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLocalStorage.py
--rw-rw-rw-   0        0        0     2108 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLocation.py
--rw-rw-rw-   0        0        0     1627 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLongPress.py
--rw-rw-rw-   0        0        0     3312 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyMotion.py
--rw-rw-rw-   0        0        0     1463 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyMousePosition.py
--rw-rw-rw-   0        0        0     1577 2023-07-08 13:15:23.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyPopout.py
--rw-rw-rw-   0        0        0     2479 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyQRCode.py
--rw-rw-rw-   0        0        0     1449 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyRawHTML.py
--rw-rw-rw-   0        0        0     1505 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyReload.py
--rw-rw-rw-   0        0        0     3724 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyResizable.py
--rw-rw-rw-   0        0        0     1459 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyResponsive.py
--rw-rw-rw-   0        0        0     1737 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyRgbColorPicker.py
--rw-rw-rw-   0        0        0     2653 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyScroll.py
--rw-rw-rw-   0        0        0     2531 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyScrollbars.py
--rw-rw-rw-   0        0        0     1756 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySessionStorage.py
--rw-rw-rw-   0        0        0     1433 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySetTitle.py
--rw-rw-rw-   0        0        0     1753 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyShadowDom.py
--rw-rw-rw-   0        0        0     3498 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyShortcutPanel.py
--rw-rw-rw-   0        0        0     1358 2023-06-15 10:22:23.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySortable.py
--rw-rw-rw-   0        0        0     1945 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySortableContainer.py
--rw-rw-rw-   0        0        0     1698 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySortableItem.py
--rw-rw-rw-   0        0        0     3103 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySortableList.py
--rw-rw-rw-   0        0        0     2472 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySplit.py
--rw-rw-rw-   0        0        0     1686 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySplitPane.py
--rw-rw-rw-   0        0        0     1874 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySticky.py
--rw-rw-rw-   0        0        0     1433 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyStyle.py
--rw-rw-rw-   0        0        0     1820 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyTextSelection.py
--rw-rw-rw-   0        0        0     1533 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyTimeout.py
--rw-rw-rw-   0        0        0     2845 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyTopProgress.py
--rw-rw-rw-   0        0        0     2057 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyTwitterColorPicker.py
--rw-rw-rw-   0        0        0     1606 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyUnmount.py
--rw-rw-rw-   0        0        0     2050 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyVirtualList.py
--rw-rw-rw-   0        0        0     2311 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyWebSocket.py
--rw-rw-rw-   0        0        0     1629 2023-07-21 02:38:59.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyWheelColorPicker.py
--rw-rw-rw-   0        0        0     1528 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyWindowSize.py
--rw-rw-rw-   0        0        0     2610 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/__init__.py
--rw-rw-rw-   0        0        0     5225 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/_imports_.py
--rw-rw-rw-   0        0        0  1421084 2023-07-21 02:38:55.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/feffery_utils_components.min.js
--rw-rw-rw-   0        0        0   215113 2023-07-21 02:39:00.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/metadata.json
--rw-rw-rw-   0        0        0     4096 2023-07-21 02:38:57.000000 feffery_utils_components-0.2.0a7/feffery_utils_components/package-info.json
-drwxrwxrwx   0        0        0        0 2023-07-21 02:39:01.688737 feffery_utils_components-0.2.0a7/feffery_utils_components.egg-info/
--rw-rw-rw-   0        0        0      342 2023-07-21 02:39:01.000000 feffery_utils_components-0.2.0a7/feffery_utils_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3876 2023-07-21 02:39:01.000000 feffery_utils_components-0.2.0a7/feffery_utils_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 02:39:01.000000 feffery_utils_components-0.2.0a7/feffery_utils_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-07-21 02:39:01.000000 feffery_utils_components-0.2.0a7/feffery_utils_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-21 02:39:01.000000 feffery_utils_components-0.2.0a7/feffery_utils_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4096 2023-07-21 02:37:49.000000 feffery_utils_components-0.2.0a7/package.json
--rw-rw-rw-   0        0        0       42 2023-07-21 02:39:01.692737 feffery_utils_components-0.2.0a7/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-06-16 02:41:22.000000 feffery_utils_components-0.2.0a7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 01:23:04.448094 feffery_utils_components-0.2.0a8/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a8/LICENSE
+-rw-rw-rw-   0        0        0      484 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a8/MANIFEST.in
+-rw-rw-rw-   0        0        0      342 2023-08-08 01:23:04.447588 feffery_utils_components-0.2.0a8/PKG-INFO
+-rw-rw-rw-   0        0        0     1432 2023-05-28 10:44:03.000000 feffery_utils_components-0.2.0a8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 01:23:04.438609 feffery_utils_components-0.2.0a8/feffery_utils_components/
+-rw-rw-rw-   0        0        0     1877 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyAutoAnimate.py
+-rw-rw-rw-   0        0        0     2015 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyBlockColorPicker.py
+-rw-rw-rw-   0        0        0     2093 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCaptcha.py
+-rw-rw-rw-   0        0        0     2207 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCircleColorPicker.py
+-rw-rw-rw-   0        0        0     2784 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCompareSlider.py
+-rw-rw-rw-   0        0        0     2049 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCookie.py
+-rw-rw-rw-   0        0        0     1616 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCountDown.py
+-rw-rw-rw-   0        0        0     2508 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCountUp.py
+-rw-rw-rw-   0        0        0     1431 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCssVar.py
+-rw-rw-rw-   0        0        0     2078 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyDeviceDetect.py
+-rw-rw-rw-   0        0        0     4313 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyDiv.py
+-rw-rw-rw-   0        0        0     1556 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyDocumentVisibility.py
+-rw-rw-rw-   0        0        0     1449 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyExecuteJs.py
+-rw-rw-rw-   0        0        0     1610 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyExternalCss.py
+-rw-rw-rw-   0        0        0     1602 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyExternalJs.py
+-rw-rw-rw-   0        0        0     2390 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyExtraSpinner.py
+-rw-rw-rw-   0        0        0     1526 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyEyeDropper.py
+-rw-rw-rw-   0        0        0     2687 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyFancyButton.py
+-rw-rw-rw-   0        0        0     2816 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyFancyMessage.py
+-rw-rw-rw-   0        0        0     3737 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyFancyNotification.py
+-rw-rw-rw-   0        0        0     1733 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyFullscreen.py
+-rw-rw-rw-   0        0        0     1483 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGeolocation.py
+-rw-rw-rw-   0        0        0     2037 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGithubColorPicker.py
+-rw-rw-rw-   0        0        0     5043 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGrid.py
+-rw-rw-rw-   0        0        0     1749 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGridItem.py
+-rw-rw-rw-   0        0        0     3888 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGuide.py
+-rw-rw-rw-   0        0        0     1727 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyHexColorPicker.py
+-rw-rw-rw-   0        0        0     2498 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyHighlightWords.py
+-rw-rw-rw-   0        0        0     1529 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyIdle.py
+-rw-rw-rw-   0        0        0     1728 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyImagePaste.py
+-rw-rw-rw-   0        0        0     1713 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyInViewport.py
+-rw-rw-rw-   0        0        0     3879 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyJsonViewer.py
+-rw-rw-rw-   0        0        0     1704 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyKeyPress.py
+-rw-rw-rw-   0        0        0     2109 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLazyLoad.py
+-rw-rw-rw-   0        0        0     1809 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyListenPaste.py
+-rw-rw-rw-   0        0        0     1538 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyListenScroll.py
+-rw-rw-rw-   0        0        0     1462 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyListenUnload.py
+-rw-rw-rw-   0        0        0     1768 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLocalLargeStorage.py
+-rw-rw-rw-   0        0        0     1748 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLocalStorage.py
+-rw-rw-rw-   0        0        0     2108 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLocation.py
+-rw-rw-rw-   0        0        0     1627 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLongPress.py
+-rw-rw-rw-   0        0        0     3312 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyMotion.py
+-rw-rw-rw-   0        0        0     1463 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyMousePosition.py
+-rw-rw-rw-   0        0        0     1577 2023-07-08 13:15:23.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyPopout.py
+-rw-rw-rw-   0        0        0     2479 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyQRCode.py
+-rw-rw-rw-   0        0        0     1449 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyRawHTML.py
+-rw-rw-rw-   0        0        0     1505 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyReload.py
+-rw-rw-rw-   0        0        0     3724 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyResizable.py
+-rw-rw-rw-   0        0        0     1459 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyResponsive.py
+-rw-rw-rw-   0        0        0     1737 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyRgbColorPicker.py
+-rw-rw-rw-   0        0        0     2653 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyScroll.py
+-rw-rw-rw-   0        0        0     2531 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyScrollbars.py
+-rw-rw-rw-   0        0        0     1756 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySessionStorage.py
+-rw-rw-rw-   0        0        0     1433 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySetTitle.py
+-rw-rw-rw-   0        0        0     1753 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyShadowDom.py
+-rw-rw-rw-   0        0        0     3498 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyShortcutPanel.py
+-rw-rw-rw-   0        0        0     1358 2023-06-15 10:22:23.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySortable.py
+-rw-rw-rw-   0        0        0     1945 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySortableContainer.py
+-rw-rw-rw-   0        0        0     1698 2023-06-13 03:49:15.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySortableItem.py
+-rw-rw-rw-   0        0        0     3103 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySortableList.py
+-rw-rw-rw-   0        0        0     2472 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySplit.py
+-rw-rw-rw-   0        0        0     1686 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySplitPane.py
+-rw-rw-rw-   0        0        0     1874 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySticky.py
+-rw-rw-rw-   0        0        0     1433 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyStyle.py
+-rw-rw-rw-   0        0        0     1820 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyTextSelection.py
+-rw-rw-rw-   0        0        0     1533 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyTimeout.py
+-rw-rw-rw-   0        0        0     2845 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyTopProgress.py
+-rw-rw-rw-   0        0        0     2057 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyTwitterColorPicker.py
+-rw-rw-rw-   0        0        0     1606 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyUnmount.py
+-rw-rw-rw-   0        0        0     2050 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyVirtualList.py
+-rw-rw-rw-   0        0        0     2311 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyWebSocket.py
+-rw-rw-rw-   0        0        0     1629 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyWheelColorPicker.py
+-rw-rw-rw-   0        0        0     1528 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyWindowSize.py
+-rw-rw-rw-   0        0        0     2610 2023-04-03 01:54:13.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/__init__.py
+-rw-rw-rw-   0        0        0     5225 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/_imports_.py
+-rw-rw-rw-   0        0        0     5717 2023-08-08 01:21:41.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/alias.py
+-rw-rw-rw-   0        0        0  1421084 2023-08-08 01:23:00.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/feffery_utils_components.min.js
+-rw-rw-rw-   0        0        0   215113 2023-08-08 01:23:03.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/metadata.json
+-rw-rw-rw-   0        0        0     4096 2023-08-08 01:23:01.000000 feffery_utils_components-0.2.0a8/feffery_utils_components/package-info.json
+drwxrwxrwx   0        0        0        0 2023-08-08 01:23:04.445328 feffery_utils_components-0.2.0a8/feffery_utils_components.egg-info/
+-rw-rw-rw-   0        0        0      342 2023-08-08 01:23:04.000000 feffery_utils_components-0.2.0a8/feffery_utils_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3910 2023-08-08 01:23:04.000000 feffery_utils_components-0.2.0a8/feffery_utils_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 01:23:04.000000 feffery_utils_components-0.2.0a8/feffery_utils_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-08 01:23:04.000000 feffery_utils_components-0.2.0a8/feffery_utils_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-08-08 01:23:04.000000 feffery_utils_components-0.2.0a8/feffery_utils_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4096 2023-08-08 01:15:18.000000 feffery_utils_components-0.2.0a8/package.json
+-rw-rw-rw-   0        0        0       42 2023-08-08 01:23:04.448094 feffery_utils_components-0.2.0a8/setup.cfg
+-rw-rw-rw-   0        0        0      729 2023-06-16 02:41:22.000000 feffery_utils_components-0.2.0a8/setup.py
```

### Comparing `feffery_utils_components-0.2.0a7/LICENSE` & `feffery_utils_components-0.2.0a8/LICENSE`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/README.md` & `feffery_utils_components-0.2.0a8/README.md`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyAutoAnimate.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyAutoAnimate.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyBlockColorPicker.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyBlockColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCaptcha.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCaptcha.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCircleColorPicker.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCircleColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCompareSlider.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCompareSlider.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCookie.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCookie.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCountDown.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCountDown.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCountUp.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCountUp.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyCssVar.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyCssVar.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyDeviceDetect.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyDeviceDetect.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyDiv.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyDiv.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyDocumentVisibility.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyDocumentVisibility.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyExecuteJs.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyExecuteJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyExternalCss.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyExternalCss.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyExternalJs.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyExternalJs.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyExtraSpinner.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyExtraSpinner.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyEyeDropper.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyEyeDropper.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyFancyButton.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyFancyButton.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyFancyMessage.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyFancyMessage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyFancyNotification.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyFancyNotification.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyFullscreen.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyFullscreen.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGeolocation.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGeolocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGithubColorPicker.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGithubColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGrid.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGrid.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGridItem.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGridItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyGuide.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyGuide.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyHexColorPicker.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyHexColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyHighlightWords.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyHighlightWords.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyIdle.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyIdle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyImagePaste.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyImagePaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyInViewport.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyInViewport.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyJsonViewer.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyJsonViewer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyKeyPress.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyKeyPress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLazyLoad.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLazyLoad.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyListenPaste.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyListenPaste.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyListenScroll.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyListenScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyListenUnload.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyListenUnload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLocalLargeStorage.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLocalLargeStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLocalStorage.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLocalStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLocation.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLocation.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyLongPress.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyLongPress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyMotion.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyMotion.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyMousePosition.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyMousePosition.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyPopout.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyPopout.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyQRCode.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyQRCode.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyRawHTML.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyRawHTML.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyReload.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyReload.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyResizable.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyResizable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyResponsive.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyResponsive.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyRgbColorPicker.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyRgbColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyScroll.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyScroll.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyScrollbars.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyScrollbars.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySessionStorage.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySessionStorage.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySetTitle.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySetTitle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyShadowDom.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyShadowDom.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyShortcutPanel.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyShortcutPanel.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySortable.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySortable.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySortableContainer.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySortableContainer.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySortableItem.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySortableItem.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySortableList.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySortableList.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySplit.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySplit.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySplitPane.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySplitPane.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferySticky.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferySticky.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyStyle.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyStyle.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyTextSelection.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyTextSelection.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyTimeout.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyTimeout.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyTopProgress.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyTopProgress.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyTwitterColorPicker.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyTwitterColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyUnmount.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyUnmount.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyVirtualList.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyVirtualList.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyWebSocket.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyWebSocket.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyWheelColorPicker.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyWheelColorPicker.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/FefferyWindowSize.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/FefferyWindowSize.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/__init__.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/__init__.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/_imports_.py` & `feffery_utils_components-0.2.0a8/feffery_utils_components/_imports_.py`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/feffery_utils_components.min.js` & `feffery_utils_components-0.2.0a8/feffery_utils_components/feffery_utils_components.min.js`

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
-            return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-a7m1689907101"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
+            return n ? ((t = (n = e.split("/")).slice(-1)[0].split(".")).splice(1, 0, "v0_2_0-a8m1691457757"), n.splice(-1, 1, t.join(".")), n.join("/")) : e
         }), o(o.s = 494)
     }([function(e, t) {
                 e.exports = window.PropTypes
             }, function(e, t) {
                 e.exports = window.React
             }, function(e, t, n) {
                 "use strict";
```

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/metadata.json` & `feffery_utils_components-0.2.0a8/feffery_utils_components/metadata.json`

 * *Files identical despite different names*

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components/package-info.json` & `feffery_utils_components-0.2.0a8/feffery_utils_components/package-info.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.0-a8'"}*

```diff
@@ -114,9 +114,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-a7"
+    "version": "0.2.0-a8"
 }
```

### Comparing `feffery_utils_components-0.2.0a7/feffery_utils_components.egg-info/SOURCES.txt` & `feffery_utils_components-0.2.0a8/feffery_utils_components.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 feffery_utils_components/FefferyUnmount.py
 feffery_utils_components/FefferyVirtualList.py
 feffery_utils_components/FefferyWebSocket.py
 feffery_utils_components/FefferyWheelColorPicker.py
 feffery_utils_components/FefferyWindowSize.py
 feffery_utils_components/__init__.py
 feffery_utils_components/_imports_.py
+feffery_utils_components/alias.py
 feffery_utils_components/feffery_utils_components.min.js
 feffery_utils_components/metadata.json
 feffery_utils_components/package-info.json
 feffery_utils_components.egg-info/PKG-INFO
 feffery_utils_components.egg-info/SOURCES.txt
 feffery_utils_components.egg-info/dependency_links.txt
 feffery_utils_components.egg-info/requires.txt
```

### Comparing `feffery_utils_components-0.2.0a7/package.json` & `feffery_utils_components-0.2.0a8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9666666666666667%*

 * *Differences: {"'version'": "'0.2.0-a8'"}*

```diff
@@ -114,9 +114,9 @@
         "build": "npm run build:js && npm run build:backends",
         "build:activated": "npm run build:js && npm run build:backends-activated",
         "build:backends": "dash-generate-components ./src/lib/components feffery_utils_components -p package-info.json --r-prefix '' --jl-prefix ''",
         "build:backends-activated": "(. venv/bin/activate || venv\\scripts\\activate && npm run build:py_and_r)",
         "build:js": "webpack --mode production",
         "start": "webpack-serve --config ./webpack.serve.config.js --open"
     },
-    "version": "0.2.0-a7"
+    "version": "0.2.0-a8"
 }
```

### Comparing `feffery_utils_components-0.2.0a7/setup.py` & `feffery_utils_components-0.2.0a8/setup.py`

 * *Files identical despite different names*

