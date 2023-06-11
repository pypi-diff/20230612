# Comparing `tmp/kk-0.9.0.tar.gz` & `tmp/kk-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kk-0.9.0.tar", last modified: Wed Feb 15 13:24:43 2023, max compression
+gzip compressed data, was "kk-0.9.1.tar", last modified: Sun Jun 11 23:11:06 2023, max compression
```

## Comparing `kk-0.9.0.tar` & `kk-0.9.1.tar`

### file list

```diff
@@ -1,137 +1,137 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.849274 kk-0.9.0/
--rw-r--r--   0 root         (0) root         (0)      589 2023-02-15 13:24:43.849274 kk-0.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3203 2022-07-14 13:13:22.000000 kk-0.9.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.821275 kk-0.9.0/kk/
--rw-r--r--   0 root         (0) root         (0)      129 2023-02-15 13:24:37.000000 kk-0.9.0/kk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36919 2023-01-23 04:04:42.000000 kk-0.9.0/kk/handler.py
--rwxr-xr-x   0 root         (0) root         (0)     4035 2022-07-14 13:13:22.000000 kk-0.9.0/kk/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.825275 kk-0.9.0/kk/static/
--rw-r--r--   0 root         (0) root         (0)     4286 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.829275 kk-0.9.0/kk/static/img/
--rw-r--r--   0 root         (0) root         (0)     5153 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/apk.png
--rw-r--r--   0 root         (0) root         (0)    17071 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/audio.png
--rw-r--r--   0 root         (0) root         (0)     7434 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/bash.png
--rw-r--r--   0 root         (0) root         (0)     6382 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/c.png
--rw-r--r--   0 root         (0) root         (0)     6673 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/cpp.png
--rw-r--r--   0 root         (0) root         (0)     9366 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/csharp.png
--rw-r--r--   0 root         (0) root         (0)     5635 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/css.png
--rw-r--r--   0 root         (0) root         (0)    16755 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/database.png
--rw-r--r--   0 root         (0) root         (0)     8139 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/excel.png
--rw-r--r--   0 root         (0) root         (0)     2245 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/exe.png
--rw-r--r--   0 root         (0) root         (0)     2822 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/file.png
--rw-r--r--   0 root         (0) root         (0)     3688 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/folder.png
--rw-r--r--   0 root         (0) root         (0)    12494 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/go.png
--rw-r--r--   0 root         (0) root         (0)     8140 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/html.png
--rw-r--r--   0 root         (0) root         (0)     7301 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/image.png
--rw-r--r--   0 root         (0) root         (0)     8962 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/ini.png
--rw-r--r--   0 root         (0) root         (0)     7287 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/iso.png
--rw-r--r--   0 root         (0) root         (0)    15616 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/java.png
--rw-r--r--   0 root         (0) root         (0)    10518 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/javascript.png
--rw-r--r--   0 root         (0) root         (0)     3847 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/json.png
--rw-r--r--   0 root         (0) root         (0)     2997 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/kindle.png
--rw-r--r--   0 root         (0) root         (0)     9954 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/lua.png
--rw-r--r--   0 root         (0) root         (0)     4006 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/mac.png
--rw-r--r--   0 root         (0) root         (0)     2901 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/markdown.png
--rw-r--r--   0 root         (0) root         (0)    12717 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/pdf.png
--rw-r--r--   0 root         (0) root         (0)    12577 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/php.png
--rw-r--r--   0 root         (0) root         (0)     3574 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/ppt.png
--rw-r--r--   0 root         (0) root         (0)     9024 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/python.png
--rw-r--r--   0 root         (0) root         (0)     2901 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/txt.png
--rw-r--r--   0 root         (0) root         (0)    15897 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/video.png
--rw-r--r--   0 root         (0) root         (0)    13413 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/vue.png
--rw-r--r--   0 root         (0) root         (0)     7904 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/word.png
--rw-r--r--   0 root         (0) root         (0)    11355 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/yaml.png
--rw-r--r--   0 root         (0) root         (0)     3509 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/img/zip.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.821275 kk-0.9.0/kk/static/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.833275 kk-0.9.0/kk/static/src/css/
--rw-r--r--   0 root         (0) root         (0)    45250 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/DPlayer.min.css
--rw-r--r--   0 root         (0) root         (0)     5254 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/iconfont.css
--rw-r--r--   0 root         (0) root         (0)     5572 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/iconfont.eot
--rw-r--r--   0 root         (0) root         (0)    15798 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/iconfont.svg
--rw-r--r--   0 root         (0) root         (0)     5404 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/iconfont.ttf
--rw-r--r--   0 root         (0) root         (0)     3536 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/iconfont.woff
--rw-r--r--   0 root         (0) root         (0)     2904 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/iconfont.woff2
--rw-r--r--   0 root         (0) root         (0)     3584 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/markdown.css
--rw-r--r--   0 root         (0) root         (0)     2477 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/monokai_sublime.css
--rw-r--r--   0 root         (0) root         (0)     9673 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/css/style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.837275 kk-0.9.0/kk/static/src/js/
--rw-r--r--   0 root         (0) root         (0)   116781 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/DPlayer.min.js
--rw-r--r--   0 root         (0) root         (0)    10453 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/clipboard.min.js
--rw-r--r--   0 root         (0) root         (0)   173418 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/flv.min.js
--rw-r--r--   0 root         (0) root         (0)    80655 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/highcharts-more.js
--rw-r--r--   0 root         (0) root         (0)   254576 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/highcharts.js
--rw-r--r--   0 root         (0) root         (0)   749330 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/highlight.pack.min.js
--rw-r--r--   0 root         (0) root         (0)   231552 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/hls.min.js
--rw-r--r--   0 root         (0) root         (0)     5595 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/imagesloaded.pkgd.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    24104 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/masonry.pkgd.min.js
--rw-r--r--   0 root         (0) root         (0)    19989 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/page.js
--rw-r--r--   0 root         (0) root         (0)     2221 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/utils.js
--rw-r--r--   0 root         (0) root         (0)    70754 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/js/webuploader.nolog.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.841275 kk-0.9.0/kk/static/src/layui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.841275 kk-0.9.0/kk/static/src/layui/css/
--rw-r--r--   0 root         (0) root         (0)    74304 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/layui.css
--rw-r--r--   0 root         (0) root         (0)     9886 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/layui.mobile.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.841275 kk-0.9.0/kk/static/src/layui/css/modules/
--rw-r--r--   0 root         (0) root         (0)     1064 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/modules/code.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.821275 kk-0.9.0/kk/static/src/layui/css/modules/laydate/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.841275 kk-0.9.0/kk/static/src/layui/css/modules/laydate/default/
--rw-r--r--   0 root         (0) root         (0)     7538 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/modules/laydate/default/laydate.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.821275 kk-0.9.0/kk/static/src/layui/css/modules/layer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.841275 kk-0.9.0/kk/static/src/layui/css/modules/layer/default/
--rw-r--r--   0 root         (0) root         (0)     5911 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/modules/layer/default/icon-ext.png
--rw-r--r--   0 root         (0) root         (0)    11493 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/modules/layer/default/icon.png
--rw-r--r--   0 root         (0) root         (0)    14426 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/modules/layer/default/layer.css
--rw-r--r--   0 root         (0) root         (0)     5793 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/modules/layer/default/loading-0.gif
--rw-r--r--   0 root         (0) root         (0)      701 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/modules/layer/default/loading-1.gif
--rw-r--r--   0 root         (0) root         (0)     1787 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/css/modules/layer/default/loading-2.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.845275 kk-0.9.0/kk/static/src/layui/font/
--rw-r--r--   0 root         (0) root         (0)    46684 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/font/iconfont.eot
--rw-r--r--   0 root         (0) root         (0)   305858 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/font/iconfont.svg
--rw-r--r--   0 root         (0) root         (0)    46508 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/font/iconfont.ttf
--rw-r--r--   0 root         (0) root         (0)    30628 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/font/iconfont.woff
--rw-r--r--   0 root         (0) root         (0)    25964 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/font/iconfont.woff2
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.821275 kk-0.9.0/kk/static/src/layui/lay/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.849274 kk-0.9.0/kk/static/src/layui/lay/modules/
--rw-r--r--   0 root         (0) root         (0)     3863 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/carousel.js
--rw-r--r--   0 root         (0) root         (0)     1178 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/code.js
--rw-r--r--   0 root         (0) root         (0)    11740 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/colorpicker.js
--rw-r--r--   0 root         (0) root         (0)     7265 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/element.js
--rw-r--r--   0 root         (0) root         (0)     2027 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/flow.js
--rw-r--r--   0 root         (0) root         (0)     9464 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/form.js
--rw-r--r--   0 root         (0) root         (0)    97649 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/jquery.js
--rw-r--r--   0 root         (0) root         (0)    27378 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/laydate.js
--rw-r--r--   0 root         (0) root         (0)    12636 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/layedit.js
--rw-r--r--   0 root         (0) root         (0)    22042 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/layer.js
--rw-r--r--   0 root         (0) root         (0)     4473 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/laypage.js
--rw-r--r--   0 root         (0) root         (0)     1837 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/laytpl.js
--rw-r--r--   0 root         (0) root         (0)    53632 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/mobile.js
--rw-r--r--   0 root         (0) root         (0)     2754 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/rate.js
--rw-r--r--   0 root         (0) root         (0)     7050 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/slider.js
--rw-r--r--   0 root         (0) root         (0)    31564 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/table.js
--rw-r--r--   0 root         (0) root         (0)     6325 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/transfer.js
--rw-r--r--   0 root         (0) root         (0)    11545 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/tree.js
--rw-r--r--   0 root         (0) root         (0)     7467 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/upload.js
--rw-r--r--   0 root         (0) root         (0)     3837 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/lay/modules/util.js
--rw-r--r--   0 root         (0) root         (0)   278423 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/layui.all.js
--rw-r--r--   0 root         (0) root         (0)     7348 2022-07-14 13:13:22.000000 kk-0.9.0/kk/static/src/layui/layui.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.849274 kk-0.9.0/kk/templates/
--rw-r--r--   0 root         (0) root         (0)     3760 2022-07-14 13:13:22.000000 kk-0.9.0/kk/templates/admin.html
--rw-r--r--   0 root         (0) root         (0)     4262 2023-02-15 13:22:41.000000 kk-0.9.0/kk/templates/base.html
--rw-r--r--   0 root         (0) root         (0)     4032 2022-07-14 13:13:22.000000 kk-0.9.0/kk/templates/chart.html
--rw-r--r--   0 root         (0) root         (0)    13650 2023-01-23 03:57:25.000000 kk-0.9.0/kk/templates/index.html
--rw-r--r--   0 root         (0) root         (0)     1772 2022-07-14 13:13:22.000000 kk-0.9.0/kk/templates/manage.html
--rw-r--r--   0 root         (0) root         (0)     1461 2022-07-14 13:13:22.000000 kk-0.9.0/kk/templates/reset.html
--rw-r--r--   0 root         (0) root         (0)     2995 2022-07-14 13:13:22.000000 kk-0.9.0/kk/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     1052 2022-07-14 13:13:22.000000 kk-0.9.0/kk/templates/signin.html
--rw-r--r--   0 root         (0) root         (0)     1849 2022-07-14 13:13:22.000000 kk-0.9.0/kk/templates/signup.html
--rw-r--r--   0 root         (0) root         (0)     5965 2022-07-14 13:13:22.000000 kk-0.9.0/kk/templates/table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-15 13:24:43.825275 kk-0.9.0/kk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      589 2023-02-15 13:24:43.000000 kk-0.9.0/kk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3642 2023-02-15 13:24:43.000000 kk-0.9.0/kk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-15 13:24:43.000000 kk-0.9.0/kk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-02-15 13:24:43.000000 kk-0.9.0/kk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-02-15 13:24:43.000000 kk-0.9.0/kk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        3 2023-02-15 13:24:43.000000 kk-0.9.0/kk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-15 13:24:43.849274 kk-0.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1319 2023-01-10 04:30:46.000000 kk-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.289095 kk-0.9.1/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-06-11 23:11:06.289095 kk-0.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3203 2022-07-14 13:13:22.000000 kk-0.9.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.269092 kk-0.9.1/kk/
+-rw-r--r--   0 root         (0) root         (0)      129 2023-06-11 23:11:01.000000 kk-0.9.1/kk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36919 2023-01-23 04:04:42.000000 kk-0.9.1/kk/handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     4035 2022-07-14 13:13:22.000000 kk-0.9.1/kk/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.269092 kk-0.9.1/kk/static/
+-rw-r--r--   0 root         (0) root         (0)     4286 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.273093 kk-0.9.1/kk/static/img/
+-rw-r--r--   0 root         (0) root         (0)     5153 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/apk.png
+-rw-r--r--   0 root         (0) root         (0)    17071 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/audio.png
+-rw-r--r--   0 root         (0) root         (0)     7434 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/bash.png
+-rw-r--r--   0 root         (0) root         (0)     6382 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/c.png
+-rw-r--r--   0 root         (0) root         (0)     6673 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/cpp.png
+-rw-r--r--   0 root         (0) root         (0)     9366 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/csharp.png
+-rw-r--r--   0 root         (0) root         (0)     5635 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/css.png
+-rw-r--r--   0 root         (0) root         (0)    16755 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/database.png
+-rw-r--r--   0 root         (0) root         (0)     8139 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/excel.png
+-rw-r--r--   0 root         (0) root         (0)     2245 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/exe.png
+-rw-r--r--   0 root         (0) root         (0)     2822 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/file.png
+-rw-r--r--   0 root         (0) root         (0)     3688 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/folder.png
+-rw-r--r--   0 root         (0) root         (0)    12494 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/go.png
+-rw-r--r--   0 root         (0) root         (0)     8140 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/html.png
+-rw-r--r--   0 root         (0) root         (0)     7301 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/image.png
+-rw-r--r--   0 root         (0) root         (0)     8962 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/ini.png
+-rw-r--r--   0 root         (0) root         (0)     7287 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/iso.png
+-rw-r--r--   0 root         (0) root         (0)    15616 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/java.png
+-rw-r--r--   0 root         (0) root         (0)    10518 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/javascript.png
+-rw-r--r--   0 root         (0) root         (0)     3847 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/json.png
+-rw-r--r--   0 root         (0) root         (0)     2997 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/kindle.png
+-rw-r--r--   0 root         (0) root         (0)     9954 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/lua.png
+-rw-r--r--   0 root         (0) root         (0)     4006 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/mac.png
+-rw-r--r--   0 root         (0) root         (0)     2901 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/markdown.png
+-rw-r--r--   0 root         (0) root         (0)    12717 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/pdf.png
+-rw-r--r--   0 root         (0) root         (0)    12577 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/php.png
+-rw-r--r--   0 root         (0) root         (0)     3574 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/ppt.png
+-rw-r--r--   0 root         (0) root         (0)     9024 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/python.png
+-rw-r--r--   0 root         (0) root         (0)     2901 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/txt.png
+-rw-r--r--   0 root         (0) root         (0)    15897 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/video.png
+-rw-r--r--   0 root         (0) root         (0)    13413 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/vue.png
+-rw-r--r--   0 root         (0) root         (0)     7904 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/word.png
+-rw-r--r--   0 root         (0) root         (0)    11355 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/yaml.png
+-rw-r--r--   0 root         (0) root         (0)     3509 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/img/zip.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.269092 kk-0.9.1/kk/static/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.277094 kk-0.9.1/kk/static/src/css/
+-rw-r--r--   0 root         (0) root         (0)    45250 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/DPlayer.min.css
+-rw-r--r--   0 root         (0) root         (0)     5254 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/iconfont.css
+-rw-r--r--   0 root         (0) root         (0)     5572 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/iconfont.eot
+-rw-r--r--   0 root         (0) root         (0)    15798 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/iconfont.svg
+-rw-r--r--   0 root         (0) root         (0)     5404 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/iconfont.ttf
+-rw-r--r--   0 root         (0) root         (0)     3536 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/iconfont.woff
+-rw-r--r--   0 root         (0) root         (0)     2904 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/iconfont.woff2
+-rw-r--r--   0 root         (0) root         (0)     3584 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/markdown.css
+-rw-r--r--   0 root         (0) root         (0)     2477 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/monokai_sublime.css
+-rw-r--r--   0 root         (0) root         (0)     9673 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/css/style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.277094 kk-0.9.1/kk/static/src/js/
+-rw-r--r--   0 root         (0) root         (0)   116781 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/DPlayer.min.js
+-rw-r--r--   0 root         (0) root         (0)    10453 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/clipboard.min.js
+-rw-r--r--   0 root         (0) root         (0)   173418 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/flv.min.js
+-rw-r--r--   0 root         (0) root         (0)    80655 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/highcharts-more.js
+-rw-r--r--   0 root         (0) root         (0)   254576 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/highcharts.js
+-rw-r--r--   0 root         (0) root         (0)   749330 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/highlight.pack.min.js
+-rw-r--r--   0 root         (0) root         (0)   231552 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/hls.min.js
+-rw-r--r--   0 root         (0) root         (0)     5595 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/imagesloaded.pkgd.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    24104 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/masonry.pkgd.min.js
+-rw-r--r--   0 root         (0) root         (0)    19990 2023-06-11 23:06:09.000000 kk-0.9.1/kk/static/src/js/page.js
+-rw-r--r--   0 root         (0) root         (0)     2221 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/utils.js
+-rw-r--r--   0 root         (0) root         (0)    70754 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/js/webuploader.nolog.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.281094 kk-0.9.1/kk/static/src/layui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.281094 kk-0.9.1/kk/static/src/layui/css/
+-rw-r--r--   0 root         (0) root         (0)    74304 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/layui.css
+-rw-r--r--   0 root         (0) root         (0)     9886 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/layui.mobile.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.281094 kk-0.9.1/kk/static/src/layui/css/modules/
+-rw-r--r--   0 root         (0) root         (0)     1064 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/modules/code.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.269092 kk-0.9.1/kk/static/src/layui/css/modules/laydate/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.281094 kk-0.9.1/kk/static/src/layui/css/modules/laydate/default/
+-rw-r--r--   0 root         (0) root         (0)     7538 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/modules/laydate/default/laydate.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.269092 kk-0.9.1/kk/static/src/layui/css/modules/layer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.281094 kk-0.9.1/kk/static/src/layui/css/modules/layer/default/
+-rw-r--r--   0 root         (0) root         (0)     5911 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/modules/layer/default/icon-ext.png
+-rw-r--r--   0 root         (0) root         (0)    11493 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/modules/layer/default/icon.png
+-rw-r--r--   0 root         (0) root         (0)    14426 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/modules/layer/default/layer.css
+-rw-r--r--   0 root         (0) root         (0)     5793 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/modules/layer/default/loading-0.gif
+-rw-r--r--   0 root         (0) root         (0)      701 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/modules/layer/default/loading-1.gif
+-rw-r--r--   0 root         (0) root         (0)     1787 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/css/modules/layer/default/loading-2.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.285094 kk-0.9.1/kk/static/src/layui/font/
+-rw-r--r--   0 root         (0) root         (0)    46684 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/font/iconfont.eot
+-rw-r--r--   0 root         (0) root         (0)   305858 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/font/iconfont.svg
+-rw-r--r--   0 root         (0) root         (0)    46508 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/font/iconfont.ttf
+-rw-r--r--   0 root         (0) root         (0)    30628 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/font/iconfont.woff
+-rw-r--r--   0 root         (0) root         (0)    25964 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/font/iconfont.woff2
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.269092 kk-0.9.1/kk/static/src/layui/lay/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.285094 kk-0.9.1/kk/static/src/layui/lay/modules/
+-rw-r--r--   0 root         (0) root         (0)     3863 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/carousel.js
+-rw-r--r--   0 root         (0) root         (0)     1178 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/code.js
+-rw-r--r--   0 root         (0) root         (0)    11740 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/colorpicker.js
+-rw-r--r--   0 root         (0) root         (0)     7265 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/element.js
+-rw-r--r--   0 root         (0) root         (0)     2027 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/flow.js
+-rw-r--r--   0 root         (0) root         (0)     9464 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/form.js
+-rw-r--r--   0 root         (0) root         (0)    97649 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/jquery.js
+-rw-r--r--   0 root         (0) root         (0)    27378 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/laydate.js
+-rw-r--r--   0 root         (0) root         (0)    12636 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/layedit.js
+-rw-r--r--   0 root         (0) root         (0)    22042 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/layer.js
+-rw-r--r--   0 root         (0) root         (0)     4473 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/laypage.js
+-rw-r--r--   0 root         (0) root         (0)     1837 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/laytpl.js
+-rw-r--r--   0 root         (0) root         (0)    53632 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/mobile.js
+-rw-r--r--   0 root         (0) root         (0)     2754 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/rate.js
+-rw-r--r--   0 root         (0) root         (0)     7050 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/slider.js
+-rw-r--r--   0 root         (0) root         (0)    31564 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/table.js
+-rw-r--r--   0 root         (0) root         (0)     6325 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/transfer.js
+-rw-r--r--   0 root         (0) root         (0)    11545 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/tree.js
+-rw-r--r--   0 root         (0) root         (0)     7467 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/upload.js
+-rw-r--r--   0 root         (0) root         (0)     3837 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/lay/modules/util.js
+-rw-r--r--   0 root         (0) root         (0)   278423 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/layui.all.js
+-rw-r--r--   0 root         (0) root         (0)     7348 2022-07-14 13:13:22.000000 kk-0.9.1/kk/static/src/layui/layui.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.289095 kk-0.9.1/kk/templates/
+-rw-r--r--   0 root         (0) root         (0)     3760 2022-07-14 13:13:22.000000 kk-0.9.1/kk/templates/admin.html
+-rw-r--r--   0 root         (0) root         (0)     4262 2023-02-19 15:22:17.000000 kk-0.9.1/kk/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     4032 2022-07-14 13:13:22.000000 kk-0.9.1/kk/templates/chart.html
+-rw-r--r--   0 root         (0) root         (0)    13678 2023-06-11 23:07:52.000000 kk-0.9.1/kk/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)     1772 2022-07-14 13:13:22.000000 kk-0.9.1/kk/templates/manage.html
+-rw-r--r--   0 root         (0) root         (0)     1461 2022-07-14 13:13:22.000000 kk-0.9.1/kk/templates/reset.html
+-rw-r--r--   0 root         (0) root         (0)     2995 2022-07-14 13:13:22.000000 kk-0.9.1/kk/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     1052 2022-07-14 13:13:22.000000 kk-0.9.1/kk/templates/signin.html
+-rw-r--r--   0 root         (0) root         (0)     1849 2022-07-14 13:13:22.000000 kk-0.9.1/kk/templates/signup.html
+-rw-r--r--   0 root         (0) root         (0)     5965 2022-07-14 13:13:22.000000 kk-0.9.1/kk/templates/table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-11 23:11:06.269092 kk-0.9.1/kk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      589 2023-06-11 23:11:06.000000 kk-0.9.1/kk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3642 2023-06-11 23:11:06.000000 kk-0.9.1/kk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-11 23:11:06.000000 kk-0.9.1/kk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-11 23:11:06.000000 kk-0.9.1/kk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-11 23:11:06.000000 kk-0.9.1/kk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        3 2023-06-11 23:11:06.000000 kk-0.9.1/kk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-11 23:11:06.289095 kk-0.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1319 2023-01-10 04:30:46.000000 kk-0.9.1/setup.py
```

### Comparing `kk-0.9.0/PKG-INFO` & `kk-0.9.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk
-Version: 0.9.0
+Version: 0.9.1
 Summary: a simple file server
 Home-page: https://github.com/zkdfbb/kk
 Author: digua
 Author-email: zkdfbb@qq.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kk-0.9.0/README.md` & `kk-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/handler.py` & `kk-0.9.1/kk/handler.py`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/index.py` & `kk-0.9.1/kk/index.py`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/favicon.ico` & `kk-0.9.1/kk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/apk.png` & `kk-0.9.1/kk/static/img/apk.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/audio.png` & `kk-0.9.1/kk/static/img/audio.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/bash.png` & `kk-0.9.1/kk/static/img/bash.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/c.png` & `kk-0.9.1/kk/static/img/c.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/cpp.png` & `kk-0.9.1/kk/static/img/cpp.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/csharp.png` & `kk-0.9.1/kk/static/img/csharp.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/css.png` & `kk-0.9.1/kk/static/img/css.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/database.png` & `kk-0.9.1/kk/static/img/database.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/excel.png` & `kk-0.9.1/kk/static/img/excel.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/exe.png` & `kk-0.9.1/kk/static/img/exe.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/file.png` & `kk-0.9.1/kk/static/img/file.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/folder.png` & `kk-0.9.1/kk/static/img/folder.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/go.png` & `kk-0.9.1/kk/static/img/go.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/html.png` & `kk-0.9.1/kk/static/img/html.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/image.png` & `kk-0.9.1/kk/static/img/image.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/ini.png` & `kk-0.9.1/kk/static/img/ini.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/iso.png` & `kk-0.9.1/kk/static/img/iso.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/java.png` & `kk-0.9.1/kk/static/img/java.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/javascript.png` & `kk-0.9.1/kk/static/img/javascript.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/json.png` & `kk-0.9.1/kk/static/img/json.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/kindle.png` & `kk-0.9.1/kk/static/img/kindle.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/lua.png` & `kk-0.9.1/kk/static/img/lua.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/mac.png` & `kk-0.9.1/kk/static/img/mac.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/markdown.png` & `kk-0.9.1/kk/static/img/markdown.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/pdf.png` & `kk-0.9.1/kk/static/img/pdf.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/php.png` & `kk-0.9.1/kk/static/img/php.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/ppt.png` & `kk-0.9.1/kk/static/img/ppt.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/python.png` & `kk-0.9.1/kk/static/img/python.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/txt.png` & `kk-0.9.1/kk/static/img/txt.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/video.png` & `kk-0.9.1/kk/static/img/video.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/vue.png` & `kk-0.9.1/kk/static/img/vue.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/word.png` & `kk-0.9.1/kk/static/img/word.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/yaml.png` & `kk-0.9.1/kk/static/img/yaml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/img/zip.png` & `kk-0.9.1/kk/static/img/zip.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/DPlayer.min.css` & `kk-0.9.1/kk/static/src/css/DPlayer.min.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/iconfont.css` & `kk-0.9.1/kk/static/src/css/iconfont.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/iconfont.eot` & `kk-0.9.1/kk/static/src/css/iconfont.eot`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/iconfont.svg` & `kk-0.9.1/kk/static/src/css/iconfont.svg`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/iconfont.ttf` & `kk-0.9.1/kk/static/src/css/iconfont.ttf`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/iconfont.woff` & `kk-0.9.1/kk/static/src/css/iconfont.woff`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/iconfont.woff2` & `kk-0.9.1/kk/static/src/css/iconfont.woff2`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/markdown.css` & `kk-0.9.1/kk/static/src/css/markdown.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/monokai_sublime.css` & `kk-0.9.1/kk/static/src/css/monokai_sublime.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/css/style.css` & `kk-0.9.1/kk/static/src/css/style.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/DPlayer.min.js` & `kk-0.9.1/kk/static/src/js/DPlayer.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/clipboard.min.js` & `kk-0.9.1/kk/static/src/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/flv.min.js` & `kk-0.9.1/kk/static/src/js/flv.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/highcharts-more.js` & `kk-0.9.1/kk/static/src/js/highcharts-more.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/highcharts.js` & `kk-0.9.1/kk/static/src/js/highcharts.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/highlight.pack.min.js` & `kk-0.9.1/kk/static/src/js/highlight.pack.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/hls.min.js` & `kk-0.9.1/kk/static/src/js/hls.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/imagesloaded.pkgd.min.js` & `kk-0.9.1/kk/static/src/js/imagesloaded.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/jquery.min.js` & `kk-0.9.1/kk/static/src/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/masonry.pkgd.min.js` & `kk-0.9.1/kk/static/src/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/page.js` & `kk-0.9.1/kk/static/src/js/page.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -332,15 +332,15 @@
             }
         })
 
         $(document).on("click", ".batch-preview", function() {
             if (getCookie("preview")) {
                 removeCookie("preview")
             } else {
-                setCookie("preview", "on")
+                setCookie("preview", "off")
             }
             location.reload()
         })
 
         $(document).on('click', '.batch-display', function() {
             if (getCookie("table")) {
                 removeCookie("table")
```

### Comparing `kk-0.9.0/kk/static/src/js/utils.js` & `kk-0.9.1/kk/static/src/js/utils.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/js/webuploader.nolog.min.js` & `kk-0.9.1/kk/static/src/js/webuploader.nolog.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/layui.css` & `kk-0.9.1/kk/static/src/layui/css/layui.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/layui.mobile.css` & `kk-0.9.1/kk/static/src/layui/css/layui.mobile.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/modules/code.css` & `kk-0.9.1/kk/static/src/layui/css/modules/code.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/modules/laydate/default/laydate.css` & `kk-0.9.1/kk/static/src/layui/css/modules/laydate/default/laydate.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/modules/layer/default/icon-ext.png` & `kk-0.9.1/kk/static/src/layui/css/modules/layer/default/icon-ext.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/modules/layer/default/icon.png` & `kk-0.9.1/kk/static/src/layui/css/modules/layer/default/icon.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/modules/layer/default/layer.css` & `kk-0.9.1/kk/static/src/layui/css/modules/layer/default/layer.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/modules/layer/default/loading-0.gif` & `kk-0.9.1/kk/static/src/layui/css/modules/layer/default/loading-0.gif`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/modules/layer/default/loading-1.gif` & `kk-0.9.1/kk/static/src/layui/css/modules/layer/default/loading-1.gif`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/css/modules/layer/default/loading-2.gif` & `kk-0.9.1/kk/static/src/layui/css/modules/layer/default/loading-2.gif`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/font/iconfont.eot` & `kk-0.9.1/kk/static/src/layui/font/iconfont.eot`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/font/iconfont.svg` & `kk-0.9.1/kk/static/src/layui/font/iconfont.svg`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/font/iconfont.ttf` & `kk-0.9.1/kk/static/src/layui/font/iconfont.ttf`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/font/iconfont.woff` & `kk-0.9.1/kk/static/src/layui/font/iconfont.woff`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/font/iconfont.woff2` & `kk-0.9.1/kk/static/src/layui/font/iconfont.woff2`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/carousel.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/carousel.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/code.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/code.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/colorpicker.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/colorpicker.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/element.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/element.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/flow.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/flow.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/form.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/form.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/jquery.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/jquery.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/laydate.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/laydate.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/layedit.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/layedit.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/layer.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/layer.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/laypage.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/laypage.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/laytpl.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/laytpl.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/mobile.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/mobile.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/rate.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/rate.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/slider.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/slider.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/table.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/table.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/transfer.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/transfer.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/tree.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/tree.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/upload.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/upload.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/lay/modules/util.js` & `kk-0.9.1/kk/static/src/layui/lay/modules/util.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/layui.all.js` & `kk-0.9.1/kk/static/src/layui/layui.all.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/static/src/layui/layui.js` & `kk-0.9.1/kk/static/src/layui/layui.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/admin.html` & `kk-0.9.1/kk/templates/admin.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/base.html` & `kk-0.9.1/kk/templates/base.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/chart.html` & `kk-0.9.1/kk/templates/chart.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/index.html` & `kk-0.9.1/kk/templates/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     <i class="layui-icon layui-icon-share layui-tips" tips="批量分享/取消分享" style="font-size:16px"></i>
   </a>
   {% end %}
   <a class="batch-tools" href="javascript:;">
     <i class="icon iconfont icon-shezhi layui-tips" tips="显示/隐藏工具栏"></i>
   </a>
   <a class="batch-preview" href="javascript:;">
-    <i class="icon iconfont {{ 'icon-biyan' if handler.get_cookie('preview') else 'icon-zhengyan' }} layui-tips" tips="切换预览模式" style="font-size:16px"></i>
+    <i class="icon iconfont {{ 'icon-biyan' if not handler.get_cookie('preview') else 'icon-zhengyan' }} layui-tips" tips="切换预览模式" style="font-size:16px"></i>
   </a>
   <a class="batch-display" href="javascript:;">
     <i class="icon iconfont {{ 'icon-liebiao' if handler.get_cookie('table') else 'icon-suolvetu' }} layui-tips" tips="切换布局模式"></i>
   </a>
 </div>
 
 {% set paths = handler.request.path.rstrip('/').split('/') %}
@@ -67,24 +67,24 @@
 <div class="layui-row">
   <div class="layui-col-md2" style="min-height:0.1px;">
     <ul id="tree" {% if not handler.get_cookie('tree') %}class="layui-hide"{% end %}></ul>
   </div>
   <div class="tree-table layui-col-md{{ 10 if handler.get_cookie('tree') else 12 }}">
     {% if handler.get_cookie('table') %}
     <div id="masonry" class="layui-row layui-col-space15">
-			{% set col = 3 if handler.get_cookie('preview') and any([doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] for doc in entries]) else 2 %}
+			{% set col = 3 if not handler.get_cookie('preview') and any([doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] for doc in entries]) else 2 %}
       {% for doc in entries %}
       <div class="grid-item layui-col-md{{ col }}">
         <div class="layui-card">
           <div class="layui-card-body">
             {% set icon = 'folder.png' if doc.is_dir else handler.icon.get(doc.path.suffix.lower(), 'file.png') %}
             <a class="file-link" href="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}">
-              {% if handler.get_cookie('preview') and doc.path.suffix.lower() in ['.jpg', '.jpeg', '.png', '.bmp', '.gif', '.webp'] %}
+              {% if not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.jpg', '.jpeg', '.png', '.bmp', '.gif', '.webp'] %}
               <img style="display:block" src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}" {% if handler.args.w %}width="{{ int(handler.args.w) }}"{% end %} {% if handler.args.h %}height="{{ int(handler.args.h) }}"{% end %}>
-              {% elif handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] %}
+              {% elif not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] %}
               <audio style="display:block" controls="controls"><source src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}"></audio>
               {% else %}
               {% set icon = 'folder.png' if doc.is_dir else handler.icon.get(doc.path.suffix.lower(), 'file.png') %}
               <img width=80 height=80 style="margin-bottom:3px" src="{{ static_url(f'img/{icon}') }}">
               {% end %}
               <span class="table-name">{{ doc.path.name }}</span>
             </a>
@@ -123,19 +123,19 @@
           <th class="pc" style="width:70px"><a href="{{ handler.add_args(sort='size', order=((0 - handler.args.order) if handler.args.sort == 'size' and handler.args.order else -1)) }}"><span>文件大小</span>{% if handler.args.sort == 'size' and handler.args.order == 1 %}<span class="arrow-down arrow-up"></span>{% elif handler.args.sort == 'size' and handler.args.order == - 1 %}<span class="arrow-down"></span>{% end %}</a></th>
         </tr>
       </thead>
       <tbody>
         {% for doc in entries %}
         <tr>
           <td class="btn-select" style="text-align:left !important">
-            {% if handler.get_cookie('preview') and doc.path.suffix.lower() in ['.jpg', '.jpeg', '.png', '.bmp', '.gif', '.webp'] %}
+            {% if not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.jpg', '.jpeg', '.png', '.bmp', '.gif', '.webp'] %}
             <img style="display:block" src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}" {% if handler.args.w %}width="{{ int(handler.args.w) }}"{% end %} {% if handler.args.h %}height="{{ int(handler.args.h) }}"{% end %}>
-            {% elif handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] %}
+            {% elif not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] %}
             <audio style="display:block" controls="controls" ><source src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}"></audio>
-            {% elif handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp4', 'mkv'] %}
+            {% elif not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp4', 'mkv'] %}
             <video style="display:block" controls="controls"><source src="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}"></video>
             {% else %}
             {% set icon = 'folder.png' if doc.is_dir else handler.icon.get(doc.path.suffix.lower(), 'file.png') %}
             <img class="icon" src="{{ static_url(f'img/{icon}') }}" {% if icon in ['folder.png'] %}style="width:22px;height:22px"{% elif icon in ['pdf.png', 'audio.png', 'excel.png'] %}style="width:18px;height:18px"{% end %}>
             {% end %}
             <a class="file-link list-name" href="/disk/{{ doc.path }}{% if doc.key or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}">{% if absolute %}{{ doc.path }}{% else %}{{ doc.path.name }}{% end %}</a>
           </td>
```

#### html2text {}

```diff
@@ -12,41 +12,41 @@
 else 1) %}
 {%_if_(i_==_2_and_handler.app.options.auth)_or_i_==_1_%}{%_else_%}{
 {_urllib.parse.unquote(path)_}}{%_end_%}
  {% end %} {% end %}
 {% end %}
 % if not handler.get_cookie('tree') %}class="layui-hide"{% end %}>
 {% if handler.get_cookie('table') %}
-{% set col = 3 if handler.get_cookie('preview') and any([doc.path.suffix.lower
-() in ['.mp3', '.amr', '.ogg', '.wav'] for doc in entries]) else 2 %} {% for
-doc in entries %}
+{% set col = 3 if not handler.get_cookie('preview') and any(
+[doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] for doc in
+entries]) else 2 %} {% for doc in entries %}
 {% set icon = 'folder.png' if doc.is_dir else handler.icon.get
-(doc.path.suffix.lower(), 'file.png') %} {%_if_handler.get_cookie('preview')
-and_doc.path.suffix.lower()_in_['.jpg',_'.jpeg',_'.png',_'.bmp',_'.gif',
-'.webp']_%}_%_if_handler.args.w_%}width="{{_int(handler.args.w)_}}"{%_end_%}_{%
-if_handler.args.h_%}height="{{_int(handler.args.h)_}}"{%_end_%}>_{%_elif
-handler.get_cookie('preview')_and_doc.path.suffix.lower()_in_['.mp3',_'.amr',
-'.ogg',_'.wav']_%}__{%_else_%}_{%_set_icon_=_'folder.png'_if_doc.is_dir_else
-handler.icon.get(doc.path.suffix.lower(),_'file.png')_%}_[{{_static_url(f'img/
-{icon}')_}}]_{%_end_%}_{{_doc.path.name_}}
+(doc.path.suffix.lower(), 'file.png') %} {%_if_not_handler.get_cookie
+('preview')_and_doc.path.suffix.lower()_in_['.jpg',_'.jpeg',_'.png',_'.bmp',
+'.gif',_'.webp']_%}_%_if_handler.args.w_%}width="{{_int(handler.args.w)_}}"{%
+end_%}_{%_if_handler.args.h_%}height="{{_int(handler.args.h)_}}"{%_end_%}>_{%
+elif_not_handler.get_cookie('preview')_and_doc.path.suffix.lower()_in_['.mp3',
+'.amr',_'.ogg',_'.wav']_%}__{%_else_%}_{%_set_icon_=_'folder.png'_if_doc.is_dir
+else_handler.icon.get(doc.path.suffix.lower(),_'file.png')_%}_[{{_static_url
+(f'img/{icon}')_}}]_{%_end_%}_{{_doc.path.name_}}
        {% if handler.app.options.delete and not
 (handler.request.path.startswith("/disk/public") and not current_user.admin)%}
 {% end %}
 {% end %}
 {% else %}
 æä»¶å{%_if_handler.args.sort_in_[None,_'name']_and_handler.args.order_in_[è¿ææ�æä»¶æä½         ä¿®æ¹æ¶é´{%_if_handler.args.sort_==_'time'_and_handler.args.order_==_1_%}{æä»¶å¤§å°{%_if_handler.args.sort_==_'size'_and_handler.args.order_==_1_%}{%_elif
 %}{%_elif_handler.args.sort_==_'name'_and_handler.args.order_==_-_1_%}{%_end_%}                                                        handler.args.sort_==_'time'_and_handler.args.order_==_-_1_%}{%_end_%}                    handler.args.sort_==_'size'_and_handler.args.order_==_-_1_%}{%_end_%}
                                                                                                              {% if
-{% if handler.get_cookie('preview') and doc.path.suffix.lower() in ['.jpg', '.jpeg',                  handler.app.options.delete and
-'.png', '.bmp', '.gif', '.webp'] %}                                                                   not
+{% if not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.jpg',                       handler.app.options.delete and
+'.jpeg', '.png', '.bmp', '.gif', '.webp'] %}                                                          not
 % if handler.args.w %}width="{{ int(handler.args.w) }}"{% end %} {% if handler.args.h                 (handler.request.path.startswith
-%}height="{{ int(handler.args.h) }}"{% end %}> {% elif handler.get_cookie('preview')   {              ('/disk/public') and not
-and doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] %}  {% elif            {              current_user.admin)%}    {% end
-handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp4', 'mkv'] %}  {%    doc.expired_at %} {% if                         {{ handler.convert_time(doc.mtime) }}                                                    {{ handler.convert_size(doc.size) }}
-else %} {% set icon = 'folder.png' if doc.is_dir else handler.icon.get                 or '' }}       (handler.app.options.auth and
+%}height="{{ int(handler.args.h) }}"{% end %}> {% elif not handler.get_cookie          {              ('/disk/public') and not
+('preview') and doc.path.suffix.lower() in ['.mp3', '.amr', '.ogg', '.wav'] %}  {%     {              current_user.admin)%}    {% end
+elif not handler.get_cookie('preview') and doc.path.suffix.lower() in ['.mp4', 'mkv']  doc.expired_at %} {% if                         {{ handler.convert_time(doc.mtime) }}                                                    {{ handler.convert_size(doc.size) }}
+%}  {% else %} {% set icon = 'folder.png' if doc.is_dir else handler.icon.get          or '' }}       (handler.app.options.auth and
 (doc.path.suffix.lower(), 'file.png') %}                                                              handler.request.path.startswith
 % if icon in ['folder.png'] %}style="width:22px;height:22px"{% elif icon in                           ('/disk/public') and not
 ['pdf.png', 'audio.png', 'excel.png'] %}style="width:18px;height:18px"{% end %}> {%                   current_user.admin) %}    {%
 end %} {%_if_absolute_%}{{_doc.path_}}{%_else_%}{{_doc.path.name_}}{%_end_%}                          elif handler.app.options.auth %}
                                                                                                       {% end %}
 {% end %}
 {% end %}
```

### Comparing `kk-0.9.0/kk/templates/manage.html` & `kk-0.9.1/kk/templates/manage.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/reset.html` & `kk-0.9.1/kk/templates/reset.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/search.html` & `kk-0.9.1/kk/templates/search.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/signin.html` & `kk-0.9.1/kk/templates/signin.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/signup.html` & `kk-0.9.1/kk/templates/signup.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk/templates/table.html` & `kk-0.9.1/kk/templates/table.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/kk.egg-info/PKG-INFO` & `kk-0.9.1/kk.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk
-Version: 0.9.0
+Version: 0.9.1
 Summary: a simple file server
 Home-page: https://github.com/zkdfbb/kk
 Author: digua
 Author-email: zkdfbb@qq.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kk-0.9.0/kk.egg-info/SOURCES.txt` & `kk-0.9.1/kk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kk-0.9.0/setup.py` & `kk-0.9.1/setup.py`

 * *Files identical despite different names*

