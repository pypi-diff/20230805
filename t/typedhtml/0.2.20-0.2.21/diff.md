# Comparing `tmp/typedhtml-0.2.20.tar.gz` & `tmp/typedhtml-0.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedhtml-0.2.20.tar", max compression
+gzip compressed data, was "typedhtml-0.2.21.tar", max compression
```

## Comparing `typedhtml-0.2.20.tar` & `typedhtml-0.2.21.tar`

### file list

```diff
@@ -1,163 +1,163 @@
--rw-r--r--   0        0        0        0 2023-07-21 23:03:24.783891 typedhtml-0.2.20/README.md
--rw-r--r--   0        0        0      445 2023-08-04 02:59:24.375951 typedhtml-0.2.20/pyproject.toml
--rw-r--r--   0        0        0      154 2023-07-23 17:35:32.083325 typedhtml-0.2.20/typedhtml/__init__.py
--rw-r--r--   0        0        0    17317 2023-07-30 04:02:53.837237 typedhtml-0.2.20/typedhtml/attributes.py
--rw-r--r--   0        0        0      928 2023-08-03 17:02:56.805763 typedhtml-0.2.20/typedhtml/document.py
--rw-r--r--   0        0        0     2969 2023-07-22 18:24:49.759970 typedhtml-0.2.20/typedhtml/events.py
--rw-r--r--   0        0        0     7350 2023-07-29 21:39:52.638892 typedhtml-0.2.20/typedhtml/globals.py
--rw-r--r--   0        0        0     2316 2023-07-28 18:24:47.790231 typedhtml-0.2.20/typedhtml/ionic/__init__.py
--rw-r--r--   0        0        0     1574 2023-07-28 01:13:49.254759 typedhtml-0.2.20/typedhtml/ionic/accordion.py
--rw-r--r--   0        0        0     1150 2023-07-28 01:25:16.419662 typedhtml-0.2.20/typedhtml/ionic/action_sheet.py
--rw-r--r--   0        0        0     1074 2023-07-28 01:23:40.404251 typedhtml-0.2.20/typedhtml/ionic/alert.py
--rw-r--r--   0        0        0      797 2023-07-28 02:46:55.995956 typedhtml-0.2.20/typedhtml/ionic/app.py
--rw-r--r--   0        0        0     1072 2023-07-28 01:31:11.627505 typedhtml-0.2.20/typedhtml/ionic/badge.py
--rw-r--r--   0        0        0      772 2023-07-28 01:43:04.458673 typedhtml-0.2.20/typedhtml/ionic/base.py
--rw-r--r--   0        0        0     1875 2023-07-28 01:49:55.994594 typedhtml-0.2.20/typedhtml/ionic/breadcrumbs.py
--rw-r--r--   0        0        0     1182 2023-07-28 02:02:43.508818 typedhtml-0.2.20/typedhtml/ionic/button.py
--rw-r--r--   0        0        0     2972 2023-07-28 02:28:21.855563 typedhtml-0.2.20/typedhtml/ionic/card.py
--rw-r--r--   0        0        0     1082 2023-07-28 02:38:02.024120 typedhtml-0.2.20/typedhtml/ionic/checkbox.py
--rw-r--r--   0        0        0      761 2023-07-28 02:42:33.210151 typedhtml-0.2.20/typedhtml/ionic/chip.py
--rw-r--r--   0        0        0      863 2023-07-28 02:52:43.694801 typedhtml-0.2.20/typedhtml/ionic/content.py
--rw-r--r--   0        0        0     2267 2023-07-28 03:15:46.536131 typedhtml-0.2.20/typedhtml/ionic/date_time.py
--rw-r--r--   0        0        0     2486 2023-07-28 03:52:28.913633 typedhtml-0.2.20/typedhtml/ionic/fab.py
--rw-r--r--   0        0        0     1933 2023-07-28 04:18:31.097247 typedhtml-0.2.20/typedhtml/ionic/grid.py
--rw-r--r--   0        0        0      848 2023-07-28 14:35:15.328885 typedhtml-0.2.20/typedhtml/ionic/icon.py
--rw-r--r--   0        0        0     3023 2023-07-28 18:24:09.684178 typedhtml-0.2.20/typedhtml/ionic/indicators.py
--rw-r--r--   0        0        0     1761 2023-07-28 04:29:59.985088 typedhtml-0.2.20/typedhtml/ionic/infinite_scroll.py
--rw-r--r--   0        0        0     3342 2023-07-28 15:25:04.708910 typedhtml-0.2.20/typedhtml/ionic/input_.py
--rw-r--r--   0        0        0     4792 2023-07-28 16:22:48.188256 typedhtml-0.2.20/typedhtml/ionic/item.py
--rw-r--r--   0        0        0     1399 2023-07-28 16:26:56.425276 typedhtml-0.2.20/typedhtml/ionic/list_.py
--rw-r--r--   0        0        0     1792 2023-07-28 16:39:58.286853 typedhtml-0.2.20/typedhtml/ionic/media.py
--rw-r--r--   0        0        0     2574 2023-07-28 16:52:38.424944 typedhtml-0.2.20/typedhtml/ionic/menu.py
--rw-r--r--   0        0        0     1732 2023-07-28 17:04:23.812131 typedhtml-0.2.20/typedhtml/ionic/modal.py
--rw-r--r--   0        0        0     1025 2023-07-28 17:13:19.102152 typedhtml-0.2.20/typedhtml/ionic/nav.py
--rw-r--r--   0        0        0      890 2023-07-28 03:28:56.915318 typedhtml-0.2.20/typedhtml/ionic/picker.py
--rw-r--r--   0        0        0      815 2023-07-28 18:10:52.273797 typedhtml-0.2.20/typedhtml/ionic/popover.py
--rw-r--r--   0        0        0      831 2023-07-28 02:09:19.236163 typedhtml-0.2.20/typedhtml/ionic/ripple_effect.py
--rw-r--r--   0        0        0     1934 2023-07-28 15:44:54.720947 typedhtml-0.2.20/typedhtml/ionic/textarea.py
--rw-r--r--   0        0        0        0 2023-07-25 19:54:45.714922 typedhtml-0.2.20/typedhtml/py.typed
--rw-r--r--   0        0        0     1211 2023-07-23 06:34:06.643229 typedhtml-0.2.20/typedhtml/svg.py
--rw-r--r--   0        0        0    31931 2023-07-27 20:43:26.614161 typedhtml-0.2.20/typedhtml/tags.py
--rw-r--r--   0        0        0     9335 2023-07-27 23:09:30.008200 typedhtml-0.2.20/typedhtml/ui5/__init__.py
--rw-r--r--   0        0        0     3264 2023-07-24 03:41:38.489987 typedhtml-0.2.20/typedhtml/ui5/avatar.py
--rw-r--r--   0        0        0      863 2023-07-24 03:38:24.465498 typedhtml-0.2.20/typedhtml/ui5/badge.py
--rw-r--r--   0        0        0      528 2023-07-27 21:07:09.900283 typedhtml-0.2.20/typedhtml/ui5/bar.py
--rw-r--r--   0        0        0      244 2023-07-25 12:45:43.227706 typedhtml-0.2.20/typedhtml/ui5/barcode_scanner_dialog.py
--rw-r--r--   0        0        0      692 2023-07-27 16:15:58.159590 typedhtml-0.2.20/typedhtml/ui5/base.py
--rw-r--r--   0        0        0     1354 2023-07-24 03:41:10.194619 typedhtml-0.2.20/typedhtml/ui5/breadcrumbs.py
--rw-r--r--   0        0        0      797 2023-07-24 03:42:17.102817 typedhtml-0.2.20/typedhtml/ui5/busy_indicator.py
--rw-r--r--   0        0        0     1091 2023-07-24 03:42:46.370478 typedhtml-0.2.20/typedhtml/ui5/button.py
--rw-r--r--   0        0        0     1214 2023-07-24 21:22:07.958588 typedhtml-0.2.20/typedhtml/ui5/calendar.py
--rw-r--r--   0        0        0     1424 2023-07-24 03:44:35.261001 typedhtml-0.2.20/typedhtml/ui5/card.py
--rw-r--r--   0        0        0     1356 2023-07-24 03:44:57.515274 typedhtml-0.2.20/typedhtml/ui5/carousel.py
--rw-r--r--   0        0        0     1405 2023-07-24 03:45:38.605099 typedhtml-0.2.20/typedhtml/ui5/checkbox.py
--rw-r--r--   0        0        0     1551 2023-07-24 03:48:24.851505 typedhtml-0.2.20/typedhtml/ui5/color_palette.py
--rw-r--r--   0        0        0      619 2023-07-24 03:48:50.205563 typedhtml-0.2.20/typedhtml/ui5/color_picker.py
--rw-r--r--   0        0        0     1018 2023-07-24 03:49:37.145966 typedhtml-0.2.20/typedhtml/ui5/combobox.py
--rw-r--r--   0        0        0     1062 2023-07-24 03:50:02.077503 typedhtml-0.2.20/typedhtml/ui5/datepicker.py
--rw-r--r--   0        0        0      797 2023-07-24 21:22:33.226998 typedhtml-0.2.20/typedhtml/ui5/daterange_picker.py
--rw-r--r--   0        0        0      634 2023-07-24 03:51:37.839555 typedhtml-0.2.20/typedhtml/ui5/datetime_picker.py
--rw-r--r--   0        0        0      724 2023-07-24 03:51:59.287201 typedhtml-0.2.20/typedhtml/ui5/dialog.py
--rw-r--r--   0        0        0      920 2023-07-25 12:52:50.880741 typedhtml-0.2.20/typedhtml/ui5/dynamic_side_content.py
--rw-r--r--   0        0        0     1018 2023-07-24 03:52:52.259960 typedhtml-0.2.20/typedhtml/ui5/file_uploader.py
--rw-r--r--   0        0        0     1066 2023-07-25 13:05:33.331084 typedhtml-0.2.20/typedhtml/ui5/flexible_column_layout.py
--rw-r--r--   0        0        0      989 2023-07-24 03:53:09.125464 typedhtml-0.2.20/typedhtml/ui5/icon.py
--rw-r--r--   0        0        0     3220 2023-07-25 15:00:10.774344 typedhtml-0.2.20/typedhtml/ui5/illustrated_message.py
--rw-r--r--   0        0        0     1104 2023-07-24 18:46:05.721707 typedhtml-0.2.20/typedhtml/ui5/input.py
--rw-r--r--   0        0        0      677 2023-07-24 03:35:27.924512 typedhtml-0.2.20/typedhtml/ui5/label.py
--rw-r--r--   0        0        0      848 2023-07-24 04:19:28.264763 typedhtml-0.2.20/typedhtml/ui5/link.py
--rw-r--r--   0        0        0     2336 2023-07-24 04:55:43.979158 typedhtml-0.2.20/typedhtml/ui5/list.py
--rw-r--r--   0        0        0     1113 2023-07-25 15:12:47.396435 typedhtml-0.2.20/typedhtml/ui5/media_gallery.py
--rw-r--r--   0        0        0     1292 2023-07-24 05:07:02.147480 typedhtml-0.2.20/typedhtml/ui5/menu.py
--rw-r--r--   0        0        0      934 2023-07-24 05:11:38.448763 typedhtml-0.2.20/typedhtml/ui5/message_strip.py
--rw-r--r--   0        0        0     2111 2023-07-24 05:32:56.437095 typedhtml-0.2.20/typedhtml/ui5/multi_combobox.py
--rw-r--r--   0        0        0     1217 2023-07-24 05:47:28.390516 typedhtml-0.2.20/typedhtml/ui5/multi_input.py
--rw-r--r--   0        0        0     1341 2023-07-25 15:35:21.371287 typedhtml-0.2.20/typedhtml/ui5/notification_list_group.py
--rw-r--r--   0        0        0      651 2023-07-25 19:36:15.108104 typedhtml-0.2.20/typedhtml/ui5/notification_list_item.py
--rw-r--r--   0        0        0      822 2023-07-25 16:29:47.448554 typedhtml-0.2.20/typedhtml/ui5/page.py
--rw-r--r--   0        0        0      786 2023-07-24 05:56:13.272720 typedhtml-0.2.20/typedhtml/ui5/panel.py
--rw-r--r--   0        0        0     1049 2023-07-24 16:47:51.776836 typedhtml-0.2.20/typedhtml/ui5/popover.py
--rw-r--r--   0        0        0      851 2023-07-25 16:47:28.910479 typedhtml-0.2.20/typedhtml/ui5/product_switch.py
--rw-r--r--   0        0        0      813 2023-07-24 16:53:02.111474 typedhtml-0.2.20/typedhtml/ui5/progress.py
--rw-r--r--   0        0        0     1147 2023-07-24 17:23:34.365913 typedhtml-0.2.20/typedhtml/ui5/radio.py
--rw-r--r--   0        0        0      739 2023-07-24 17:26:16.577498 typedhtml-0.2.20/typedhtml/ui5/range_slider.py
--rw-r--r--   0        0        0      846 2023-07-24 17:30:46.775794 typedhtml-0.2.20/typedhtml/ui5/rating_indicator.py
--rw-r--r--   0        0        0      460 2023-07-24 19:03:12.882005 typedhtml-0.2.20/typedhtml/ui5/responsive_popover.py
--rw-r--r--   0        0        0     1240 2023-07-24 17:45:46.706947 typedhtml-0.2.20/typedhtml/ui5/segmented_button.py
--rw-r--r--   0        0        0     1330 2023-07-24 17:52:58.144971 typedhtml-0.2.20/typedhtml/ui5/select.py
--rw-r--r--   0        0        0     1267 2023-07-25 19:13:16.274085 typedhtml-0.2.20/typedhtml/ui5/shell_bar.py
--rw-r--r--   0        0        0     1369 2023-07-25 17:45:11.869783 typedhtml-0.2.20/typedhtml/ui5/side_nav.py
--rw-r--r--   0        0        0      686 2023-07-24 18:07:42.261132 typedhtml-0.2.20/typedhtml/ui5/slider.py
--rw-r--r--   0        0        0      992 2023-07-24 18:15:29.579762 typedhtml-0.2.20/typedhtml/ui5/split_button.py
--rw-r--r--   0        0        0      925 2023-07-24 18:19:41.715572 typedhtml-0.2.20/typedhtml/ui5/step_input.py
--rw-r--r--   0        0        0      915 2023-07-24 18:23:43.502304 typedhtml-0.2.20/typedhtml/ui5/switch.py
--rw-r--r--   0        0        0     1983 2023-07-27 23:08:48.167999 typedhtml-0.2.20/typedhtml/ui5/tab_container.py
--rw-r--r--   0        0        0     2066 2023-07-24 19:41:17.961063 typedhtml-0.2.20/typedhtml/ui5/table.py
--rw-r--r--   0        0        0      904 2023-07-24 20:54:41.376476 typedhtml-0.2.20/typedhtml/ui5/textarea.py
--rw-r--r--   0        0        0      665 2023-07-24 20:57:46.970970 typedhtml-0.2.20/typedhtml/ui5/time_picker.py
--rw-r--r--   0        0        0      784 2023-07-25 17:58:03.447272 typedhtml-0.2.20/typedhtml/ui5/timeline.py
--rw-r--r--   0        0        0      566 2023-07-24 21:01:29.280885 typedhtml-0.2.20/typedhtml/ui5/title.py
--rw-r--r--   0        0        0      708 2023-07-24 21:04:14.974066 typedhtml-0.2.20/typedhtml/ui5/toast.py
--rw-r--r--   0        0        0      496 2023-07-24 22:06:21.633647 typedhtml-0.2.20/typedhtml/ui5/toggle_button.py
--rw-r--r--   0        0        0     1135 2023-07-24 22:10:33.706725 typedhtml-0.2.20/typedhtml/ui5/tree.py
--rw-r--r--   0        0        0     1470 2023-07-25 18:12:53.064206 typedhtml-0.2.20/typedhtml/ui5/upload_collection.py
--rw-r--r--   0        0        0     1685 2023-07-25 19:37:34.851255 typedhtml-0.2.20/typedhtml/ui5/view_settings_dialog.py
--rw-r--r--   0        0        0      871 2023-07-25 18:36:11.056458 typedhtml-0.2.20/typedhtml/ui5/wizard.py
--rw-r--r--   0        0        0    35582 2023-08-04 01:26:29.004526 typedhtml-0.2.20/typedhtml/uikit/__init__.py
--rw-r--r--   0        0        0     2039 2023-07-30 02:45:54.331788 typedhtml-0.2.20/typedhtml/uikit/accordion.py
--rw-r--r--   0        0        0     1002 2023-07-30 00:45:53.730093 typedhtml-0.2.20/typedhtml/uikit/alert.py
--rw-r--r--   0        0        0     1396 2023-07-30 03:44:36.419547 typedhtml-0.2.20/typedhtml/uikit/article.py
--rw-r--r--   0        0        0      580 2023-07-29 23:32:37.144903 typedhtml-0.2.20/typedhtml/uikit/badge.py
--rw-r--r--   0        0        0      634 2023-07-30 00:10:54.011077 typedhtml-0.2.20/typedhtml/uikit/breadcrumb.py
--rw-r--r--   0        0        0     1807 2023-08-01 21:11:55.823123 typedhtml-0.2.20/typedhtml/uikit/button.py
--rw-r--r--   0        0        0     1019 2023-07-30 04:28:19.810091 typedhtml-0.2.20/typedhtml/uikit/card.py
--rw-r--r--   0        0        0     2718 2023-07-30 05:01:12.937645 typedhtml-0.2.20/typedhtml/uikit/comment.py
--rw-r--r--   0        0        0      700 2023-07-30 05:30:15.427965 typedhtml-0.2.20/typedhtml/uikit/container.py
--rw-r--r--   0        0        0     1076 2023-07-30 05:37:29.859374 typedhtml-0.2.20/typedhtml/uikit/countdown.py
--rw-r--r--   0        0        0     1490 2023-07-30 05:48:07.238431 typedhtml-0.2.20/typedhtml/uikit/cover.py
--rw-r--r--   0        0        0      747 2023-07-30 13:38:43.189527 typedhtml-0.2.20/typedhtml/uikit/description_list.py
--rw-r--r--   0        0        0      818 2023-07-30 13:46:24.425132 typedhtml-0.2.20/typedhtml/uikit/divider.py
--rw-r--r--   0        0        0      713 2023-07-30 14:12:49.793691 typedhtml-0.2.20/typedhtml/uikit/dotnav.py
--rw-r--r--   0        0        0     6843 2023-08-03 22:43:41.355530 typedhtml-0.2.20/typedhtml/uikit/drop.py
--rw-r--r--   0        0        0     1175 2023-07-30 21:11:51.653854 typedhtml-0.2.20/typedhtml/uikit/flex.py
--rw-r--r--   0        0        0     3048 2023-07-31 03:53:13.506269 typedhtml-0.2.20/typedhtml/uikit/form.py
--rw-r--r--   0        0        0     1451 2023-08-01 15:04:11.204510 typedhtml-0.2.20/typedhtml/uikit/grid.py
--rw-r--r--   0        0        0     1454 2023-08-04 02:57:57.517875 typedhtml-0.2.20/typedhtml/uikit/heading.py
--rw-r--r--   0        0        0     1369 2023-08-01 16:39:16.100340 typedhtml-0.2.20/typedhtml/uikit/height.py
--rw-r--r--   0        0        0     3942 2023-08-04 01:52:51.454770 typedhtml-0.2.20/typedhtml/uikit/icon.py
--rw-r--r--   0        0        0      735 2023-08-01 17:45:34.681437 typedhtml-0.2.20/typedhtml/uikit/image.py
--rw-r--r--   0        0        0      664 2023-08-01 17:53:57.680786 typedhtml-0.2.20/typedhtml/uikit/label.py
--rw-r--r--   0        0        0      668 2023-08-01 18:19:58.914046 typedhtml-0.2.20/typedhtml/uikit/leader.py
--rw-r--r--   0        0        0     1188 2023-08-01 18:53:47.254569 typedhtml-0.2.20/typedhtml/uikit/lightbox.py
--rw-r--r--   0        0        0      653 2023-08-01 21:15:02.579834 typedhtml-0.2.20/typedhtml/uikit/link.py
--rw-r--r--   0        0        0      937 2023-08-01 19:34:43.081406 typedhtml-0.2.20/typedhtml/uikit/list_.py
--rw-r--r--   0        0        0      509 2023-08-01 20:13:09.975200 typedhtml-0.2.20/typedhtml/uikit/marker.py
--rw-r--r--   0        0        0     3682 2023-08-04 02:58:34.861796 typedhtml-0.2.20/typedhtml/uikit/modal.py
--rw-r--r--   0        0        0     4292 2023-08-03 14:21:26.452314 typedhtml-0.2.20/typedhtml/uikit/nav.py
--rw-r--r--   0        0        0     1117 2023-08-02 02:49:31.913647 typedhtml-0.2.20/typedhtml/uikit/offcanvas.py
--rw-r--r--   0        0        0     1052 2023-08-02 03:50:04.022224 typedhtml-0.2.20/typedhtml/uikit/overlay.py
--rw-r--r--   0        0        0      750 2023-08-02 15:08:11.203442 typedhtml-0.2.20/typedhtml/uikit/pagination.py
--rw-r--r--   0        0        0      615 2023-08-02 15:44:53.708761 typedhtml-0.2.20/typedhtml/uikit/placeholder.py
--rw-r--r--   0        0        0      601 2023-08-02 15:48:49.988648 typedhtml-0.2.20/typedhtml/uikit/progress.py
--rw-r--r--   0        0        0     1388 2023-08-02 17:47:13.555449 typedhtml-0.2.20/typedhtml/uikit/scroll.py
--rw-r--r--   0        0        0     1400 2023-08-03 22:04:55.250494 typedhtml-0.2.20/typedhtml/uikit/search.py
--rw-r--r--   0        0        0     1117 2023-08-02 18:19:29.740480 typedhtml-0.2.20/typedhtml/uikit/section.py
--rw-r--r--   0        0        0     1442 2023-08-02 18:40:24.644418 typedhtml-0.2.20/typedhtml/uikit/slidenav.py
--rw-r--r--   0        0        0      968 2023-08-02 19:25:42.258643 typedhtml-0.2.20/typedhtml/uikit/slider.py
--rw-r--r--   0        0        0      898 2023-08-02 19:47:37.065310 typedhtml-0.2.20/typedhtml/uikit/sortable.py
--rw-r--r--   0        0        0      647 2023-08-02 19:51:55.423247 typedhtml-0.2.20/typedhtml/uikit/spinner.py
--rw-r--r--   0        0        0     1446 2023-08-02 20:09:29.176838 typedhtml-0.2.20/typedhtml/uikit/sticky.py
--rw-r--r--   0        0        0      727 2023-08-02 20:15:24.483637 typedhtml-0.2.20/typedhtml/uikit/subnav.py
--rw-r--r--   0        0        0      682 2023-08-02 20:25:21.123875 typedhtml-0.2.20/typedhtml/uikit/svg.py
--rw-r--r--   0        0        0      917 2023-08-02 20:36:12.362830 typedhtml-0.2.20/typedhtml/uikit/tab.py
--rw-r--r--   0        0        0     1357 2023-08-02 22:41:13.049593 typedhtml-0.2.20/typedhtml/uikit/table.py
--rw-r--r--   0        0        0      553 2023-08-03 00:19:24.803338 typedhtml-0.2.20/typedhtml/uikit/thumbnav.py
--rw-r--r--   0        0        0      763 2023-08-03 00:28:06.088042 typedhtml-0.2.20/typedhtml/uikit/tile.py
--rw-r--r--   0        0        0     1334 2023-08-03 00:53:29.465992 typedhtml-0.2.20/typedhtml/uikit/toggle.py
--rw-r--r--   0        0        0     1011 2023-08-03 01:08:48.746954 typedhtml-0.2.20/typedhtml/uikit/tooltip.py
--rw-r--r--   0        0        0      425 2023-08-03 01:39:31.301159 typedhtml-0.2.20/typedhtml/uikit/totop.py
--rw-r--r--   0        0        0     7878 2023-08-03 00:27:09.531334 typedhtml-0.2.20/typedhtml/uikit/types.py
--rw-r--r--   0        0        0      909 2023-07-30 03:38:57.926387 typedhtml-0.2.20/typedhtml/uikit/util.py
--rw-r--r--   0        0        0      790 2023-08-03 02:00:08.807579 typedhtml-0.2.20/typedhtml/uikit/video.py
--rw-r--r--   0        0        0      536 2023-07-27 16:09:36.125132 typedhtml-0.2.20/typedhtml/util.py
--rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 typedhtml-0.2.20/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-21 23:03:24.783891 typedhtml-0.2.21/README.md
+-rw-r--r--   0        0        0      445 2023-08-04 14:57:04.767847 typedhtml-0.2.21/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-07-23 17:35:32.083325 typedhtml-0.2.21/typedhtml/__init__.py
+-rw-r--r--   0        0        0    17317 2023-07-30 04:02:53.837237 typedhtml-0.2.21/typedhtml/attributes.py
+-rw-r--r--   0        0        0      928 2023-08-03 17:02:56.805763 typedhtml-0.2.21/typedhtml/document.py
+-rw-r--r--   0        0        0     2969 2023-07-22 18:24:49.759970 typedhtml-0.2.21/typedhtml/events.py
+-rw-r--r--   0        0        0     7350 2023-07-29 21:39:52.638892 typedhtml-0.2.21/typedhtml/globals.py
+-rw-r--r--   0        0        0     2316 2023-07-28 18:24:47.790231 typedhtml-0.2.21/typedhtml/ionic/__init__.py
+-rw-r--r--   0        0        0     1574 2023-07-28 01:13:49.254759 typedhtml-0.2.21/typedhtml/ionic/accordion.py
+-rw-r--r--   0        0        0     1150 2023-07-28 01:25:16.419662 typedhtml-0.2.21/typedhtml/ionic/action_sheet.py
+-rw-r--r--   0        0        0     1074 2023-07-28 01:23:40.404251 typedhtml-0.2.21/typedhtml/ionic/alert.py
+-rw-r--r--   0        0        0      797 2023-07-28 02:46:55.995956 typedhtml-0.2.21/typedhtml/ionic/app.py
+-rw-r--r--   0        0        0     1072 2023-07-28 01:31:11.627505 typedhtml-0.2.21/typedhtml/ionic/badge.py
+-rw-r--r--   0        0        0      772 2023-07-28 01:43:04.458673 typedhtml-0.2.21/typedhtml/ionic/base.py
+-rw-r--r--   0        0        0     1875 2023-07-28 01:49:55.994594 typedhtml-0.2.21/typedhtml/ionic/breadcrumbs.py
+-rw-r--r--   0        0        0     1182 2023-07-28 02:02:43.508818 typedhtml-0.2.21/typedhtml/ionic/button.py
+-rw-r--r--   0        0        0     2972 2023-07-28 02:28:21.855563 typedhtml-0.2.21/typedhtml/ionic/card.py
+-rw-r--r--   0        0        0     1082 2023-07-28 02:38:02.024120 typedhtml-0.2.21/typedhtml/ionic/checkbox.py
+-rw-r--r--   0        0        0      761 2023-07-28 02:42:33.210151 typedhtml-0.2.21/typedhtml/ionic/chip.py
+-rw-r--r--   0        0        0      863 2023-07-28 02:52:43.694801 typedhtml-0.2.21/typedhtml/ionic/content.py
+-rw-r--r--   0        0        0     2267 2023-07-28 03:15:46.536131 typedhtml-0.2.21/typedhtml/ionic/date_time.py
+-rw-r--r--   0        0        0     2486 2023-07-28 03:52:28.913633 typedhtml-0.2.21/typedhtml/ionic/fab.py
+-rw-r--r--   0        0        0     1933 2023-07-28 04:18:31.097247 typedhtml-0.2.21/typedhtml/ionic/grid.py
+-rw-r--r--   0        0        0      848 2023-07-28 14:35:15.328885 typedhtml-0.2.21/typedhtml/ionic/icon.py
+-rw-r--r--   0        0        0     3023 2023-07-28 18:24:09.684178 typedhtml-0.2.21/typedhtml/ionic/indicators.py
+-rw-r--r--   0        0        0     1761 2023-07-28 04:29:59.985088 typedhtml-0.2.21/typedhtml/ionic/infinite_scroll.py
+-rw-r--r--   0        0        0     3342 2023-07-28 15:25:04.708910 typedhtml-0.2.21/typedhtml/ionic/input_.py
+-rw-r--r--   0        0        0     4792 2023-07-28 16:22:48.188256 typedhtml-0.2.21/typedhtml/ionic/item.py
+-rw-r--r--   0        0        0     1399 2023-07-28 16:26:56.425276 typedhtml-0.2.21/typedhtml/ionic/list_.py
+-rw-r--r--   0        0        0     1792 2023-07-28 16:39:58.286853 typedhtml-0.2.21/typedhtml/ionic/media.py
+-rw-r--r--   0        0        0     2574 2023-07-28 16:52:38.424944 typedhtml-0.2.21/typedhtml/ionic/menu.py
+-rw-r--r--   0        0        0     1732 2023-07-28 17:04:23.812131 typedhtml-0.2.21/typedhtml/ionic/modal.py
+-rw-r--r--   0        0        0     1025 2023-07-28 17:13:19.102152 typedhtml-0.2.21/typedhtml/ionic/nav.py
+-rw-r--r--   0        0        0      890 2023-07-28 03:28:56.915318 typedhtml-0.2.21/typedhtml/ionic/picker.py
+-rw-r--r--   0        0        0      815 2023-07-28 18:10:52.273797 typedhtml-0.2.21/typedhtml/ionic/popover.py
+-rw-r--r--   0        0        0      831 2023-07-28 02:09:19.236163 typedhtml-0.2.21/typedhtml/ionic/ripple_effect.py
+-rw-r--r--   0        0        0     1934 2023-07-28 15:44:54.720947 typedhtml-0.2.21/typedhtml/ionic/textarea.py
+-rw-r--r--   0        0        0        0 2023-07-25 19:54:45.714922 typedhtml-0.2.21/typedhtml/py.typed
+-rw-r--r--   0        0        0     1211 2023-07-23 06:34:06.643229 typedhtml-0.2.21/typedhtml/svg.py
+-rw-r--r--   0        0        0    31931 2023-07-27 20:43:26.614161 typedhtml-0.2.21/typedhtml/tags.py
+-rw-r--r--   0        0        0     9335 2023-07-27 23:09:30.008200 typedhtml-0.2.21/typedhtml/ui5/__init__.py
+-rw-r--r--   0        0        0     3264 2023-07-24 03:41:38.489987 typedhtml-0.2.21/typedhtml/ui5/avatar.py
+-rw-r--r--   0        0        0      863 2023-07-24 03:38:24.465498 typedhtml-0.2.21/typedhtml/ui5/badge.py
+-rw-r--r--   0        0        0      528 2023-07-27 21:07:09.900283 typedhtml-0.2.21/typedhtml/ui5/bar.py
+-rw-r--r--   0        0        0      244 2023-07-25 12:45:43.227706 typedhtml-0.2.21/typedhtml/ui5/barcode_scanner_dialog.py
+-rw-r--r--   0        0        0      692 2023-07-27 16:15:58.159590 typedhtml-0.2.21/typedhtml/ui5/base.py
+-rw-r--r--   0        0        0     1354 2023-07-24 03:41:10.194619 typedhtml-0.2.21/typedhtml/ui5/breadcrumbs.py
+-rw-r--r--   0        0        0      797 2023-07-24 03:42:17.102817 typedhtml-0.2.21/typedhtml/ui5/busy_indicator.py
+-rw-r--r--   0        0        0     1091 2023-07-24 03:42:46.370478 typedhtml-0.2.21/typedhtml/ui5/button.py
+-rw-r--r--   0        0        0     1214 2023-07-24 21:22:07.958588 typedhtml-0.2.21/typedhtml/ui5/calendar.py
+-rw-r--r--   0        0        0     1424 2023-07-24 03:44:35.261001 typedhtml-0.2.21/typedhtml/ui5/card.py
+-rw-r--r--   0        0        0     1356 2023-07-24 03:44:57.515274 typedhtml-0.2.21/typedhtml/ui5/carousel.py
+-rw-r--r--   0        0        0     1405 2023-07-24 03:45:38.605099 typedhtml-0.2.21/typedhtml/ui5/checkbox.py
+-rw-r--r--   0        0        0     1551 2023-07-24 03:48:24.851505 typedhtml-0.2.21/typedhtml/ui5/color_palette.py
+-rw-r--r--   0        0        0      619 2023-07-24 03:48:50.205563 typedhtml-0.2.21/typedhtml/ui5/color_picker.py
+-rw-r--r--   0        0        0     1018 2023-07-24 03:49:37.145966 typedhtml-0.2.21/typedhtml/ui5/combobox.py
+-rw-r--r--   0        0        0     1062 2023-07-24 03:50:02.077503 typedhtml-0.2.21/typedhtml/ui5/datepicker.py
+-rw-r--r--   0        0        0      797 2023-07-24 21:22:33.226998 typedhtml-0.2.21/typedhtml/ui5/daterange_picker.py
+-rw-r--r--   0        0        0      634 2023-07-24 03:51:37.839555 typedhtml-0.2.21/typedhtml/ui5/datetime_picker.py
+-rw-r--r--   0        0        0      724 2023-07-24 03:51:59.287201 typedhtml-0.2.21/typedhtml/ui5/dialog.py
+-rw-r--r--   0        0        0      920 2023-07-25 12:52:50.880741 typedhtml-0.2.21/typedhtml/ui5/dynamic_side_content.py
+-rw-r--r--   0        0        0     1018 2023-07-24 03:52:52.259960 typedhtml-0.2.21/typedhtml/ui5/file_uploader.py
+-rw-r--r--   0        0        0     1066 2023-07-25 13:05:33.331084 typedhtml-0.2.21/typedhtml/ui5/flexible_column_layout.py
+-rw-r--r--   0        0        0      989 2023-07-24 03:53:09.125464 typedhtml-0.2.21/typedhtml/ui5/icon.py
+-rw-r--r--   0        0        0     3220 2023-07-25 15:00:10.774344 typedhtml-0.2.21/typedhtml/ui5/illustrated_message.py
+-rw-r--r--   0        0        0     1104 2023-07-24 18:46:05.721707 typedhtml-0.2.21/typedhtml/ui5/input.py
+-rw-r--r--   0        0        0      677 2023-07-24 03:35:27.924512 typedhtml-0.2.21/typedhtml/ui5/label.py
+-rw-r--r--   0        0        0      848 2023-07-24 04:19:28.264763 typedhtml-0.2.21/typedhtml/ui5/link.py
+-rw-r--r--   0        0        0     2336 2023-07-24 04:55:43.979158 typedhtml-0.2.21/typedhtml/ui5/list.py
+-rw-r--r--   0        0        0     1113 2023-07-25 15:12:47.396435 typedhtml-0.2.21/typedhtml/ui5/media_gallery.py
+-rw-r--r--   0        0        0     1292 2023-07-24 05:07:02.147480 typedhtml-0.2.21/typedhtml/ui5/menu.py
+-rw-r--r--   0        0        0      934 2023-07-24 05:11:38.448763 typedhtml-0.2.21/typedhtml/ui5/message_strip.py
+-rw-r--r--   0        0        0     2111 2023-07-24 05:32:56.437095 typedhtml-0.2.21/typedhtml/ui5/multi_combobox.py
+-rw-r--r--   0        0        0     1217 2023-07-24 05:47:28.390516 typedhtml-0.2.21/typedhtml/ui5/multi_input.py
+-rw-r--r--   0        0        0     1341 2023-07-25 15:35:21.371287 typedhtml-0.2.21/typedhtml/ui5/notification_list_group.py
+-rw-r--r--   0        0        0      651 2023-07-25 19:36:15.108104 typedhtml-0.2.21/typedhtml/ui5/notification_list_item.py
+-rw-r--r--   0        0        0      822 2023-07-25 16:29:47.448554 typedhtml-0.2.21/typedhtml/ui5/page.py
+-rw-r--r--   0        0        0      786 2023-07-24 05:56:13.272720 typedhtml-0.2.21/typedhtml/ui5/panel.py
+-rw-r--r--   0        0        0     1049 2023-07-24 16:47:51.776836 typedhtml-0.2.21/typedhtml/ui5/popover.py
+-rw-r--r--   0        0        0      851 2023-07-25 16:47:28.910479 typedhtml-0.2.21/typedhtml/ui5/product_switch.py
+-rw-r--r--   0        0        0      813 2023-07-24 16:53:02.111474 typedhtml-0.2.21/typedhtml/ui5/progress.py
+-rw-r--r--   0        0        0     1147 2023-07-24 17:23:34.365913 typedhtml-0.2.21/typedhtml/ui5/radio.py
+-rw-r--r--   0        0        0      739 2023-07-24 17:26:16.577498 typedhtml-0.2.21/typedhtml/ui5/range_slider.py
+-rw-r--r--   0        0        0      846 2023-07-24 17:30:46.775794 typedhtml-0.2.21/typedhtml/ui5/rating_indicator.py
+-rw-r--r--   0        0        0      460 2023-07-24 19:03:12.882005 typedhtml-0.2.21/typedhtml/ui5/responsive_popover.py
+-rw-r--r--   0        0        0     1240 2023-07-24 17:45:46.706947 typedhtml-0.2.21/typedhtml/ui5/segmented_button.py
+-rw-r--r--   0        0        0     1330 2023-07-24 17:52:58.144971 typedhtml-0.2.21/typedhtml/ui5/select.py
+-rw-r--r--   0        0        0     1267 2023-07-25 19:13:16.274085 typedhtml-0.2.21/typedhtml/ui5/shell_bar.py
+-rw-r--r--   0        0        0     1369 2023-07-25 17:45:11.869783 typedhtml-0.2.21/typedhtml/ui5/side_nav.py
+-rw-r--r--   0        0        0      686 2023-07-24 18:07:42.261132 typedhtml-0.2.21/typedhtml/ui5/slider.py
+-rw-r--r--   0        0        0      992 2023-07-24 18:15:29.579762 typedhtml-0.2.21/typedhtml/ui5/split_button.py
+-rw-r--r--   0        0        0      925 2023-07-24 18:19:41.715572 typedhtml-0.2.21/typedhtml/ui5/step_input.py
+-rw-r--r--   0        0        0      915 2023-07-24 18:23:43.502304 typedhtml-0.2.21/typedhtml/ui5/switch.py
+-rw-r--r--   0        0        0     1983 2023-07-27 23:08:48.167999 typedhtml-0.2.21/typedhtml/ui5/tab_container.py
+-rw-r--r--   0        0        0     2066 2023-07-24 19:41:17.961063 typedhtml-0.2.21/typedhtml/ui5/table.py
+-rw-r--r--   0        0        0      904 2023-07-24 20:54:41.376476 typedhtml-0.2.21/typedhtml/ui5/textarea.py
+-rw-r--r--   0        0        0      665 2023-07-24 20:57:46.970970 typedhtml-0.2.21/typedhtml/ui5/time_picker.py
+-rw-r--r--   0        0        0      784 2023-07-25 17:58:03.447272 typedhtml-0.2.21/typedhtml/ui5/timeline.py
+-rw-r--r--   0        0        0      566 2023-07-24 21:01:29.280885 typedhtml-0.2.21/typedhtml/ui5/title.py
+-rw-r--r--   0        0        0      708 2023-07-24 21:04:14.974066 typedhtml-0.2.21/typedhtml/ui5/toast.py
+-rw-r--r--   0        0        0      496 2023-07-24 22:06:21.633647 typedhtml-0.2.21/typedhtml/ui5/toggle_button.py
+-rw-r--r--   0        0        0     1135 2023-07-24 22:10:33.706725 typedhtml-0.2.21/typedhtml/ui5/tree.py
+-rw-r--r--   0        0        0     1470 2023-07-25 18:12:53.064206 typedhtml-0.2.21/typedhtml/ui5/upload_collection.py
+-rw-r--r--   0        0        0     1685 2023-07-25 19:37:34.851255 typedhtml-0.2.21/typedhtml/ui5/view_settings_dialog.py
+-rw-r--r--   0        0        0      871 2023-07-25 18:36:11.056458 typedhtml-0.2.21/typedhtml/ui5/wizard.py
+-rw-r--r--   0        0        0    35582 2023-08-04 01:26:29.004526 typedhtml-0.2.21/typedhtml/uikit/__init__.py
+-rw-r--r--   0        0        0     2039 2023-07-30 02:45:54.331788 typedhtml-0.2.21/typedhtml/uikit/accordion.py
+-rw-r--r--   0        0        0     1002 2023-07-30 00:45:53.730093 typedhtml-0.2.21/typedhtml/uikit/alert.py
+-rw-r--r--   0        0        0     1396 2023-07-30 03:44:36.419547 typedhtml-0.2.21/typedhtml/uikit/article.py
+-rw-r--r--   0        0        0      580 2023-07-29 23:32:37.144903 typedhtml-0.2.21/typedhtml/uikit/badge.py
+-rw-r--r--   0        0        0      634 2023-07-30 00:10:54.011077 typedhtml-0.2.21/typedhtml/uikit/breadcrumb.py
+-rw-r--r--   0        0        0     1807 2023-08-01 21:11:55.823123 typedhtml-0.2.21/typedhtml/uikit/button.py
+-rw-r--r--   0        0        0     1019 2023-07-30 04:28:19.810091 typedhtml-0.2.21/typedhtml/uikit/card.py
+-rw-r--r--   0        0        0     2718 2023-07-30 05:01:12.937645 typedhtml-0.2.21/typedhtml/uikit/comment.py
+-rw-r--r--   0        0        0      728 2023-08-04 14:56:42.957976 typedhtml-0.2.21/typedhtml/uikit/container.py
+-rw-r--r--   0        0        0     1076 2023-07-30 05:37:29.859374 typedhtml-0.2.21/typedhtml/uikit/countdown.py
+-rw-r--r--   0        0        0     1490 2023-07-30 05:48:07.238431 typedhtml-0.2.21/typedhtml/uikit/cover.py
+-rw-r--r--   0        0        0      747 2023-07-30 13:38:43.189527 typedhtml-0.2.21/typedhtml/uikit/description_list.py
+-rw-r--r--   0        0        0      818 2023-07-30 13:46:24.425132 typedhtml-0.2.21/typedhtml/uikit/divider.py
+-rw-r--r--   0        0        0      713 2023-07-30 14:12:49.793691 typedhtml-0.2.21/typedhtml/uikit/dotnav.py
+-rw-r--r--   0        0        0     6843 2023-08-03 22:43:41.355530 typedhtml-0.2.21/typedhtml/uikit/drop.py
+-rw-r--r--   0        0        0     1175 2023-07-30 21:11:51.653854 typedhtml-0.2.21/typedhtml/uikit/flex.py
+-rw-r--r--   0        0        0     3048 2023-07-31 03:53:13.506269 typedhtml-0.2.21/typedhtml/uikit/form.py
+-rw-r--r--   0        0        0     1451 2023-08-01 15:04:11.204510 typedhtml-0.2.21/typedhtml/uikit/grid.py
+-rw-r--r--   0        0        0     1454 2023-08-04 02:57:57.517875 typedhtml-0.2.21/typedhtml/uikit/heading.py
+-rw-r--r--   0        0        0     1369 2023-08-01 16:39:16.100340 typedhtml-0.2.21/typedhtml/uikit/height.py
+-rw-r--r--   0        0        0     3942 2023-08-04 01:52:51.454770 typedhtml-0.2.21/typedhtml/uikit/icon.py
+-rw-r--r--   0        0        0      735 2023-08-01 17:45:34.681437 typedhtml-0.2.21/typedhtml/uikit/image.py
+-rw-r--r--   0        0        0      664 2023-08-01 17:53:57.680786 typedhtml-0.2.21/typedhtml/uikit/label.py
+-rw-r--r--   0        0        0      668 2023-08-01 18:19:58.914046 typedhtml-0.2.21/typedhtml/uikit/leader.py
+-rw-r--r--   0        0        0     1188 2023-08-01 18:53:47.254569 typedhtml-0.2.21/typedhtml/uikit/lightbox.py
+-rw-r--r--   0        0        0      653 2023-08-01 21:15:02.579834 typedhtml-0.2.21/typedhtml/uikit/link.py
+-rw-r--r--   0        0        0      937 2023-08-01 19:34:43.081406 typedhtml-0.2.21/typedhtml/uikit/list_.py
+-rw-r--r--   0        0        0      509 2023-08-01 20:13:09.975200 typedhtml-0.2.21/typedhtml/uikit/marker.py
+-rw-r--r--   0        0        0     3682 2023-08-04 02:58:34.861796 typedhtml-0.2.21/typedhtml/uikit/modal.py
+-rw-r--r--   0        0        0     4292 2023-08-03 14:21:26.452314 typedhtml-0.2.21/typedhtml/uikit/nav.py
+-rw-r--r--   0        0        0     1117 2023-08-02 02:49:31.913647 typedhtml-0.2.21/typedhtml/uikit/offcanvas.py
+-rw-r--r--   0        0        0     1052 2023-08-02 03:50:04.022224 typedhtml-0.2.21/typedhtml/uikit/overlay.py
+-rw-r--r--   0        0        0      750 2023-08-02 15:08:11.203442 typedhtml-0.2.21/typedhtml/uikit/pagination.py
+-rw-r--r--   0        0        0      615 2023-08-02 15:44:53.708761 typedhtml-0.2.21/typedhtml/uikit/placeholder.py
+-rw-r--r--   0        0        0      601 2023-08-02 15:48:49.988648 typedhtml-0.2.21/typedhtml/uikit/progress.py
+-rw-r--r--   0        0        0     1388 2023-08-02 17:47:13.555449 typedhtml-0.2.21/typedhtml/uikit/scroll.py
+-rw-r--r--   0        0        0     1400 2023-08-03 22:04:55.250494 typedhtml-0.2.21/typedhtml/uikit/search.py
+-rw-r--r--   0        0        0     1117 2023-08-02 18:19:29.740480 typedhtml-0.2.21/typedhtml/uikit/section.py
+-rw-r--r--   0        0        0     1442 2023-08-02 18:40:24.644418 typedhtml-0.2.21/typedhtml/uikit/slidenav.py
+-rw-r--r--   0        0        0      968 2023-08-02 19:25:42.258643 typedhtml-0.2.21/typedhtml/uikit/slider.py
+-rw-r--r--   0        0        0      898 2023-08-02 19:47:37.065310 typedhtml-0.2.21/typedhtml/uikit/sortable.py
+-rw-r--r--   0        0        0      647 2023-08-02 19:51:55.423247 typedhtml-0.2.21/typedhtml/uikit/spinner.py
+-rw-r--r--   0        0        0     1446 2023-08-02 20:09:29.176838 typedhtml-0.2.21/typedhtml/uikit/sticky.py
+-rw-r--r--   0        0        0      727 2023-08-02 20:15:24.483637 typedhtml-0.2.21/typedhtml/uikit/subnav.py
+-rw-r--r--   0        0        0      682 2023-08-02 20:25:21.123875 typedhtml-0.2.21/typedhtml/uikit/svg.py
+-rw-r--r--   0        0        0      917 2023-08-02 20:36:12.362830 typedhtml-0.2.21/typedhtml/uikit/tab.py
+-rw-r--r--   0        0        0     1357 2023-08-02 22:41:13.049593 typedhtml-0.2.21/typedhtml/uikit/table.py
+-rw-r--r--   0        0        0      553 2023-08-03 00:19:24.803338 typedhtml-0.2.21/typedhtml/uikit/thumbnav.py
+-rw-r--r--   0        0        0      763 2023-08-03 00:28:06.088042 typedhtml-0.2.21/typedhtml/uikit/tile.py
+-rw-r--r--   0        0        0     1334 2023-08-03 00:53:29.465992 typedhtml-0.2.21/typedhtml/uikit/toggle.py
+-rw-r--r--   0        0        0     1011 2023-08-03 01:08:48.746954 typedhtml-0.2.21/typedhtml/uikit/tooltip.py
+-rw-r--r--   0        0        0      425 2023-08-03 01:39:31.301159 typedhtml-0.2.21/typedhtml/uikit/totop.py
+-rw-r--r--   0        0        0     7878 2023-08-03 00:27:09.531334 typedhtml-0.2.21/typedhtml/uikit/types.py
+-rw-r--r--   0        0        0      909 2023-07-30 03:38:57.926387 typedhtml-0.2.21/typedhtml/uikit/util.py
+-rw-r--r--   0        0        0      790 2023-08-03 02:00:08.807579 typedhtml-0.2.21/typedhtml/uikit/video.py
+-rw-r--r--   0        0        0      536 2023-07-27 16:09:36.125132 typedhtml-0.2.21/typedhtml/util.py
+-rw-r--r--   0        0        0      428 1970-01-01 00:00:00.000000 typedhtml-0.2.21/PKG-INFO
```

### Comparing `typedhtml-0.2.20/typedhtml/attributes.py` & `typedhtml-0.2.21/typedhtml/attributes.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/document.py` & `typedhtml-0.2.21/typedhtml/document.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/events.py` & `typedhtml-0.2.21/typedhtml/events.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/globals.py` & `typedhtml-0.2.21/typedhtml/globals.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/__init__.py` & `typedhtml-0.2.21/typedhtml/ionic/__init__.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/accordion.py` & `typedhtml-0.2.21/typedhtml/ionic/accordion.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/action_sheet.py` & `typedhtml-0.2.21/typedhtml/ionic/action_sheet.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/alert.py` & `typedhtml-0.2.21/typedhtml/ionic/alert.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/app.py` & `typedhtml-0.2.21/typedhtml/ionic/app.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/badge.py` & `typedhtml-0.2.21/typedhtml/ionic/badge.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/base.py` & `typedhtml-0.2.21/typedhtml/ionic/base.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/breadcrumbs.py` & `typedhtml-0.2.21/typedhtml/ionic/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/button.py` & `typedhtml-0.2.21/typedhtml/ionic/button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/card.py` & `typedhtml-0.2.21/typedhtml/ionic/card.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/checkbox.py` & `typedhtml-0.2.21/typedhtml/ionic/checkbox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/chip.py` & `typedhtml-0.2.21/typedhtml/ionic/chip.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/content.py` & `typedhtml-0.2.21/typedhtml/ionic/content.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/date_time.py` & `typedhtml-0.2.21/typedhtml/ionic/date_time.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/fab.py` & `typedhtml-0.2.21/typedhtml/ionic/fab.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/grid.py` & `typedhtml-0.2.21/typedhtml/ionic/grid.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/icon.py` & `typedhtml-0.2.21/typedhtml/ionic/icon.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/indicators.py` & `typedhtml-0.2.21/typedhtml/ionic/indicators.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/infinite_scroll.py` & `typedhtml-0.2.21/typedhtml/ionic/infinite_scroll.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/input_.py` & `typedhtml-0.2.21/typedhtml/ionic/input_.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/item.py` & `typedhtml-0.2.21/typedhtml/ionic/item.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/list_.py` & `typedhtml-0.2.21/typedhtml/ionic/list_.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/media.py` & `typedhtml-0.2.21/typedhtml/ionic/media.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/menu.py` & `typedhtml-0.2.21/typedhtml/ionic/menu.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/modal.py` & `typedhtml-0.2.21/typedhtml/ionic/modal.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/nav.py` & `typedhtml-0.2.21/typedhtml/ionic/nav.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/picker.py` & `typedhtml-0.2.21/typedhtml/ionic/picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/popover.py` & `typedhtml-0.2.21/typedhtml/ionic/popover.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/ripple_effect.py` & `typedhtml-0.2.21/typedhtml/ionic/ripple_effect.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ionic/textarea.py` & `typedhtml-0.2.21/typedhtml/ionic/textarea.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/svg.py` & `typedhtml-0.2.21/typedhtml/svg.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/tags.py` & `typedhtml-0.2.21/typedhtml/tags.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/__init__.py` & `typedhtml-0.2.21/typedhtml/ui5/__init__.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/avatar.py` & `typedhtml-0.2.21/typedhtml/ui5/avatar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/badge.py` & `typedhtml-0.2.21/typedhtml/ui5/badge.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/bar.py` & `typedhtml-0.2.21/typedhtml/ui5/bar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/base.py` & `typedhtml-0.2.21/typedhtml/ui5/base.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/breadcrumbs.py` & `typedhtml-0.2.21/typedhtml/ui5/breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/busy_indicator.py` & `typedhtml-0.2.21/typedhtml/ui5/busy_indicator.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/button.py` & `typedhtml-0.2.21/typedhtml/ui5/button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/calendar.py` & `typedhtml-0.2.21/typedhtml/ui5/calendar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/card.py` & `typedhtml-0.2.21/typedhtml/ui5/card.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/carousel.py` & `typedhtml-0.2.21/typedhtml/ui5/carousel.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/checkbox.py` & `typedhtml-0.2.21/typedhtml/ui5/checkbox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/color_palette.py` & `typedhtml-0.2.21/typedhtml/ui5/color_palette.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/color_picker.py` & `typedhtml-0.2.21/typedhtml/ui5/color_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/combobox.py` & `typedhtml-0.2.21/typedhtml/ui5/combobox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/datepicker.py` & `typedhtml-0.2.21/typedhtml/ui5/datepicker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/daterange_picker.py` & `typedhtml-0.2.21/typedhtml/ui5/daterange_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/datetime_picker.py` & `typedhtml-0.2.21/typedhtml/ui5/datetime_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/dialog.py` & `typedhtml-0.2.21/typedhtml/ui5/dialog.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/dynamic_side_content.py` & `typedhtml-0.2.21/typedhtml/ui5/dynamic_side_content.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/file_uploader.py` & `typedhtml-0.2.21/typedhtml/ui5/file_uploader.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/flexible_column_layout.py` & `typedhtml-0.2.21/typedhtml/ui5/flexible_column_layout.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/icon.py` & `typedhtml-0.2.21/typedhtml/ui5/icon.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/illustrated_message.py` & `typedhtml-0.2.21/typedhtml/ui5/illustrated_message.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/input.py` & `typedhtml-0.2.21/typedhtml/ui5/input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/label.py` & `typedhtml-0.2.21/typedhtml/ui5/label.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/link.py` & `typedhtml-0.2.21/typedhtml/ui5/link.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/list.py` & `typedhtml-0.2.21/typedhtml/ui5/list.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/media_gallery.py` & `typedhtml-0.2.21/typedhtml/ui5/media_gallery.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/menu.py` & `typedhtml-0.2.21/typedhtml/ui5/menu.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/message_strip.py` & `typedhtml-0.2.21/typedhtml/ui5/message_strip.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/multi_combobox.py` & `typedhtml-0.2.21/typedhtml/ui5/multi_combobox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/multi_input.py` & `typedhtml-0.2.21/typedhtml/ui5/multi_input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/notification_list_group.py` & `typedhtml-0.2.21/typedhtml/ui5/notification_list_group.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/notification_list_item.py` & `typedhtml-0.2.21/typedhtml/ui5/notification_list_item.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/page.py` & `typedhtml-0.2.21/typedhtml/ui5/page.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/panel.py` & `typedhtml-0.2.21/typedhtml/ui5/panel.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/popover.py` & `typedhtml-0.2.21/typedhtml/ui5/popover.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/product_switch.py` & `typedhtml-0.2.21/typedhtml/ui5/product_switch.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/progress.py` & `typedhtml-0.2.21/typedhtml/ui5/progress.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/radio.py` & `typedhtml-0.2.21/typedhtml/ui5/radio.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/range_slider.py` & `typedhtml-0.2.21/typedhtml/ui5/range_slider.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/rating_indicator.py` & `typedhtml-0.2.21/typedhtml/ui5/rating_indicator.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/segmented_button.py` & `typedhtml-0.2.21/typedhtml/ui5/segmented_button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/select.py` & `typedhtml-0.2.21/typedhtml/ui5/select.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/shell_bar.py` & `typedhtml-0.2.21/typedhtml/ui5/shell_bar.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/side_nav.py` & `typedhtml-0.2.21/typedhtml/ui5/side_nav.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/slider.py` & `typedhtml-0.2.21/typedhtml/ui5/slider.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/split_button.py` & `typedhtml-0.2.21/typedhtml/ui5/split_button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/step_input.py` & `typedhtml-0.2.21/typedhtml/ui5/step_input.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/switch.py` & `typedhtml-0.2.21/typedhtml/ui5/switch.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/tab_container.py` & `typedhtml-0.2.21/typedhtml/ui5/tab_container.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/table.py` & `typedhtml-0.2.21/typedhtml/ui5/table.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/textarea.py` & `typedhtml-0.2.21/typedhtml/ui5/textarea.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/time_picker.py` & `typedhtml-0.2.21/typedhtml/ui5/time_picker.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/timeline.py` & `typedhtml-0.2.21/typedhtml/ui5/timeline.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/title.py` & `typedhtml-0.2.21/typedhtml/ui5/title.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/toast.py` & `typedhtml-0.2.21/typedhtml/ui5/toast.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/tree.py` & `typedhtml-0.2.21/typedhtml/ui5/tree.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/upload_collection.py` & `typedhtml-0.2.21/typedhtml/ui5/upload_collection.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/view_settings_dialog.py` & `typedhtml-0.2.21/typedhtml/ui5/view_settings_dialog.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/ui5/wizard.py` & `typedhtml-0.2.21/typedhtml/ui5/wizard.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/__init__.py` & `typedhtml-0.2.21/typedhtml/uikit/__init__.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/accordion.py` & `typedhtml-0.2.21/typedhtml/uikit/accordion.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/alert.py` & `typedhtml-0.2.21/typedhtml/uikit/alert.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/article.py` & `typedhtml-0.2.21/typedhtml/uikit/article.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/badge.py` & `typedhtml-0.2.21/typedhtml/uikit/badge.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/breadcrumb.py` & `typedhtml-0.2.21/typedhtml/uikit/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/button.py` & `typedhtml-0.2.21/typedhtml/uikit/button.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/card.py` & `typedhtml-0.2.21/typedhtml/uikit/card.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/comment.py` & `typedhtml-0.2.21/typedhtml/uikit/comment.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/container.py` & `typedhtml-0.2.21/typedhtml/uikit/container.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # Copyright 2023 Takin Profit. All rights reserved.
 # Use of this source code is governed by a BSD-style
 # license that can be found in the LICENSE file.
 
-from typing import Any, Optional, Unpack
+from typing import Any, Optional, Union, Unpack
 
 from typedhtml.globals import GLOBAL_ATTR
 from typedhtml.tags import div
 from typedhtml.uikit.types import Container
 from typedhtml.uikit.util import add_val
 
 
 def container(
-    *args: Any, size: Optional[Container] = None, **kwargs: Unpack[GLOBAL_ATTR]
+    *args: Any,
+    size: Optional[Union[Container, str]] = None,
+    **kwargs: Unpack[GLOBAL_ATTR],
 ) -> div:
     """The Container component is a simple wrapper for your site content.
 
     see: `https://getuikit.com/docs/container`_
     """
 
     add_val("cls", f"uk-container {size or ''}", kwargs)  # type: ignore
```

### Comparing `typedhtml-0.2.20/typedhtml/uikit/countdown.py` & `typedhtml-0.2.21/typedhtml/uikit/countdown.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/cover.py` & `typedhtml-0.2.21/typedhtml/uikit/cover.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/description_list.py` & `typedhtml-0.2.21/typedhtml/uikit/description_list.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/divider.py` & `typedhtml-0.2.21/typedhtml/uikit/divider.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/dotnav.py` & `typedhtml-0.2.21/typedhtml/uikit/dotnav.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/drop.py` & `typedhtml-0.2.21/typedhtml/uikit/drop.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/flex.py` & `typedhtml-0.2.21/typedhtml/uikit/flex.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/form.py` & `typedhtml-0.2.21/typedhtml/uikit/form.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/grid.py` & `typedhtml-0.2.21/typedhtml/uikit/grid.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/heading.py` & `typedhtml-0.2.21/typedhtml/uikit/heading.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/height.py` & `typedhtml-0.2.21/typedhtml/uikit/height.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/icon.py` & `typedhtml-0.2.21/typedhtml/uikit/icon.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/image.py` & `typedhtml-0.2.21/typedhtml/uikit/image.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/label.py` & `typedhtml-0.2.21/typedhtml/uikit/label.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/leader.py` & `typedhtml-0.2.21/typedhtml/uikit/leader.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/lightbox.py` & `typedhtml-0.2.21/typedhtml/uikit/lightbox.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/link.py` & `typedhtml-0.2.21/typedhtml/uikit/link.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/list_.py` & `typedhtml-0.2.21/typedhtml/uikit/list_.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/modal.py` & `typedhtml-0.2.21/typedhtml/uikit/modal.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/nav.py` & `typedhtml-0.2.21/typedhtml/uikit/nav.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/offcanvas.py` & `typedhtml-0.2.21/typedhtml/uikit/offcanvas.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/overlay.py` & `typedhtml-0.2.21/typedhtml/uikit/overlay.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/pagination.py` & `typedhtml-0.2.21/typedhtml/uikit/pagination.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/placeholder.py` & `typedhtml-0.2.21/typedhtml/uikit/placeholder.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/progress.py` & `typedhtml-0.2.21/typedhtml/uikit/progress.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/scroll.py` & `typedhtml-0.2.21/typedhtml/uikit/scroll.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/search.py` & `typedhtml-0.2.21/typedhtml/uikit/search.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/section.py` & `typedhtml-0.2.21/typedhtml/uikit/section.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/slidenav.py` & `typedhtml-0.2.21/typedhtml/uikit/slidenav.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/slider.py` & `typedhtml-0.2.21/typedhtml/uikit/slider.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/sortable.py` & `typedhtml-0.2.21/typedhtml/uikit/sortable.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/spinner.py` & `typedhtml-0.2.21/typedhtml/uikit/spinner.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/sticky.py` & `typedhtml-0.2.21/typedhtml/uikit/sticky.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/subnav.py` & `typedhtml-0.2.21/typedhtml/uikit/subnav.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/svg.py` & `typedhtml-0.2.21/typedhtml/uikit/svg.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/tab.py` & `typedhtml-0.2.21/typedhtml/uikit/tab.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/table.py` & `typedhtml-0.2.21/typedhtml/uikit/table.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/thumbnav.py` & `typedhtml-0.2.21/typedhtml/uikit/thumbnav.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/tile.py` & `typedhtml-0.2.21/typedhtml/uikit/tile.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/toggle.py` & `typedhtml-0.2.21/typedhtml/uikit/toggle.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/tooltip.py` & `typedhtml-0.2.21/typedhtml/uikit/tooltip.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/types.py` & `typedhtml-0.2.21/typedhtml/uikit/types.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/util.py` & `typedhtml-0.2.21/typedhtml/uikit/util.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/uikit/video.py` & `typedhtml-0.2.21/typedhtml/uikit/video.py`

 * *Files identical despite different names*

### Comparing `typedhtml-0.2.20/typedhtml/util.py` & `typedhtml-0.2.21/typedhtml/util.py`

 * *Files identical despite different names*

