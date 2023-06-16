# Comparing `tmp/pynecone-0.1.33a4.tar.gz` & `tmp/pynecone-0.1.34a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.33a4.tar", max compression
+gzip compressed data, was "pynecone-0.1.34a0.tar", max compression
```

## Comparing `pynecone-0.1.33a4.tar` & `pynecone-0.1.34a0.tar`

### file list

```diff
@@ -1,171 +1,172 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.33a4/LICENSE
--rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.33a4/README.md
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747147 pynecone-0.1.33a4/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-06-07 06:32:06.269060 pynecone-0.1.33a4/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-04-27 02:06:35.747631 pynecone-0.1.33a4/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1036 2023-04-27 02:06:35.747905 pynecone-0.1.33a4/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.33a4/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-05-15 02:04:07.604358 pynecone-0.1.33a4/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-05-15 02:04:07.604515 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-05-18 18:33:16.414872 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-05-15 02:04:07.604642 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-06-09 19:48:33.040538 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-05-22 21:40:04.765805 pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0       38 2023-05-15 02:04:07.604905 pynecone-0.1.33a4/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.33a4/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   257247 2023-05-26 18:45:47.401731 pynecone-0.1.33a4/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-05-26 18:45:47.402096 pynecone-0.1.33a4/pynecone/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.33a4/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0      995 2023-06-01 03:15:26.563786 pynecone-0.1.33a4/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.33a4/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.33a4/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.33a4/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     8450 2023-06-09 19:48:33.040820 pynecone-0.1.33a4/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1490 2023-06-07 06:05:03.874348 pynecone-0.1.33a4/pynecone/__init__.py
--rw-r--r--   0        0        0      320 2023-06-07 06:05:03.874470 pynecone-0.1.33a4/pynecone/admin.py
--rw-r--r--   0        0        0    21426 2023-06-09 19:48:39.955078 pynecone-0.1.33a4/pynecone/app.py
--rw-r--r--   0        0        0     2548 2023-06-07 19:04:43.443201 pynecone-0.1.33a4/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.33a4/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     6689 2023-06-09 19:48:33.041803 pynecone-0.1.33a4/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2642 2023-06-09 19:48:33.042227 pynecone-0.1.33a4/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7767 2023-06-09 19:48:39.955794 pynecone-0.1.33a4/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     7346 2023-06-07 06:05:03.875765 pynecone-0.1.33a4/pynecone/components/__init__.py
--rw-r--r--   0        0        0      229 2023-06-09 19:48:39.957002 pynecone-0.1.33a4/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-05-15 02:04:07.607680 pynecone-0.1.33a4/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.33a4/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.33a4/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-05-15 02:04:07.607851 pynecone-0.1.33a4/pynecone/components/base/head.py
--rw-r--r--   0        0        0      933 2023-06-09 19:48:39.957851 pynecone-0.1.33a4/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1412 2023-06-07 19:04:43.443671 pynecone-0.1.33a4/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    24243 2023-06-01 00:32:59.072142 pynecone-0.1.33a4/pynecone/components/component.py
--rw-r--r--   0        0        0      496 2023-05-26 18:45:47.404646 pynecone-0.1.33a4/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-05-15 02:04:07.608726 pynecone-0.1.33a4/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-05-15 02:04:07.608840 pynecone-0.1.33a4/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-05-15 02:04:07.608953 pynecone-0.1.33a4/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-05-15 02:04:07.609045 pynecone-0.1.33a4/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.33a4/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-05-15 02:04:07.609140 pynecone-0.1.33a4/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-05-15 02:04:07.609232 pynecone-0.1.33a4/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5793 2023-05-26 18:45:47.405454 pynecone-0.1.33a4/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0     2188 2023-05-26 18:45:47.406072 pynecone-0.1.33a4/pynecone/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-05-26 18:45:47.406587 pynecone-0.1.33a4/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3517 2023-06-09 19:48:39.958158 pynecone-0.1.33a4/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-05-15 02:04:07.609534 pynecone-0.1.33a4/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1741 2023-05-26 18:45:47.406922 pynecone-0.1.33a4/pynecone/components/disclosure/transition.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.33a4/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.33a4/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-05-15 02:04:07.609649 pynecone-0.1.33a4/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-05-15 02:04:07.609745 pynecone-0.1.33a4/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-05-15 02:04:07.609838 pynecone-0.1.33a4/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-05-15 02:04:07.609925 pynecone-0.1.33a4/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-05-15 02:04:07.610013 pynecone-0.1.33a4/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1308 2023-06-07 06:05:03.876023 pynecone-0.1.33a4/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-05-15 17:32:17.392510 pynecone-0.1.33a4/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-05-18 00:14:14.760429 pynecone-0.1.33a4/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      578 2023-05-18 00:14:14.760629 pynecone-0.1.33a4/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      243 2023-06-07 06:05:03.876332 pynecone-0.1.33a4/pynecone/components/forms/date_picker.py
--rw-r--r--   0        0        0      277 2023-06-07 06:05:03.876514 pynecone-0.1.33a4/pynecone/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.760816 pynecone-0.1.33a4/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0      243 2023-06-01 00:48:48.431001 pynecone-0.1.33a4/pynecone/components/forms/email.py
--rw-r--r--   0        0        0     2996 2023-05-26 18:45:47.407573 pynecone-0.1.33a4/pynecone/components/forms/form.py
--rw-r--r--   0        0        0      802 2023-05-15 02:04:07.610729 pynecone-0.1.33a4/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-06-09 18:42:18.512736 pynecone-0.1.33a4/pynecone/components/forms/input.py
--rw-r--r--   0        0        0    12667 2023-06-07 06:05:03.876768 pynecone-0.1.33a4/pynecone/components/forms/multiselect.py
--rw-r--r--   0        0        0     3897 2023-05-18 00:14:14.761460 pynecone-0.1.33a4/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-05-15 02:04:07.611101 pynecone-0.1.33a4/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-05-18 00:14:14.761619 pynecone-0.1.33a4/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-05-18 00:14:14.761823 pynecone-0.1.33a4/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-05-18 00:14:14.761962 pynecone-0.1.33a4/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3522 2023-06-07 06:05:03.877157 pynecone-0.1.33a4/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-05-18 00:14:14.762261 pynecone-0.1.33a4/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1573 2023-06-09 19:48:39.959122 pynecone-0.1.33a4/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1532 2023-06-09 19:48:39.959281 pynecone-0.1.33a4/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-05-18 00:14:14.762683 pynecone-0.1.33a4/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.33a4/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-05-15 02:04:07.613685 pynecone-0.1.33a4/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-05-15 02:04:07.613960 pynecone-0.1.33a4/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-05-22 21:39:53.010163 pynecone-0.1.33a4/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-05-15 02:04:07.614167 pynecone-0.1.33a4/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      766 2023-06-09 19:48:39.959611 pynecone-0.1.33a4/pynecone/components/layout/box.py
--rw-r--r--   0        0        0     2859 2023-05-22 21:39:53.010378 pynecone-0.1.33a4/pynecone/components/layout/card.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.33a4/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-05-18 00:14:14.762938 pynecone-0.1.33a4/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-05-15 02:04:07.614634 pynecone-0.1.33a4/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-05-15 02:04:07.614740 pynecone-0.1.33a4/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     3167 2023-05-26 18:45:47.408238 pynecone-0.1.33a4/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.33a4/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2418 2023-05-15 02:04:07.614987 pynecone-0.1.33a4/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-05-30 04:03:19.236282 pynecone-0.1.33a4/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.33a4/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.33a4/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-05-15 02:04:07.615111 pynecone-0.1.33a4/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-05-15 02:04:07.615242 pynecone-0.1.33a4/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.33a4/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.33a4/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0     1391 2023-06-01 03:15:26.564372 pynecone-0.1.33a4/pynecone/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-01 03:15:26.564561 pynecone-0.1.33a4/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564687 pynecone-0.1.33a4/pynecone/components/media/audio.py
--rw-r--r--   0        0        0     1524 2023-05-18 00:14:14.763360 pynecone-0.1.33a4/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.33a4/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1774 2023-06-01 03:15:26.564867 pynecone-0.1.33a4/pynecone/components/media/image.py
--rw-r--r--   0        0        0      197 2023-06-01 03:15:26.564984 pynecone-0.1.33a4/pynecone/components/media/video.py
--rw-r--r--   0        0        0      450 2023-06-07 06:05:03.877519 pynecone-0.1.33a4/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-05-15 02:04:07.615856 pynecone-0.1.33a4/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1616 2023-06-10 01:56:25.822303 pynecone-0.1.33a4/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-05-15 02:04:07.616129 pynecone-0.1.33a4/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-05-15 02:04:07.616229 pynecone-0.1.33a4/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2842 2023-06-07 06:05:03.878280 pynecone-0.1.33a4/pynecone/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-06-07 06:05:03.878625 pynecone-0.1.33a4/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-05-18 00:14:14.763711 pynecone-0.1.33a4/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1016 2023-06-07 06:05:03.878806 pynecone-0.1.33a4/pynecone/components/overlay/banner.py
--rw-r--r--   0        0        0     4681 2023-05-18 00:14:14.763867 pynecone-0.1.33a4/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-05-18 00:14:14.764021 pynecone-0.1.33a4/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-05-18 00:14:14.764177 pynecone-0.1.33a4/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-06-07 04:31:19.747990 pynecone-0.1.33a4/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-05-18 00:14:14.764530 pynecone-0.1.33a4/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.33a4/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-05-15 02:04:07.617454 pynecone-0.1.33a4/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-05-15 02:04:07.617560 pynecone-0.1.33a4/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-06-09 19:48:33.042551 pynecone-0.1.33a4/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.33a4/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      304 2023-06-01 00:32:59.073257 pynecone-0.1.33a4/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-05-15 02:04:07.617958 pynecone-0.1.33a4/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      682 2023-06-01 00:32:59.073664 pynecone-0.1.33a4/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3460 2023-06-07 06:05:03.879093 pynecone-0.1.33a4/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-05-15 02:04:07.618372 pynecone-0.1.33a4/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-05-15 02:04:07.618520 pynecone-0.1.33a4/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     6960 2023-06-09 19:48:39.960810 pynecone-0.1.33a4/pynecone/config.py
--rw-r--r--   0        0        0    10219 2023-06-09 19:48:33.049660 pynecone-0.1.33a4/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-27 02:06:35.757531 pynecone-0.1.33a4/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-27 02:06:35.757829 pynecone-0.1.33a4/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-27 02:06:35.758045 pynecone-0.1.33a4/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-27 02:06:35.758325 pynecone-0.1.33a4/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-27 02:06:35.758673 pynecone-0.1.33a4/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1320 2023-06-07 06:05:03.879903 pynecone-0.1.33a4/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-05-15 02:04:07.619552 pynecone-0.1.33a4/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-05-15 02:04:07.619858 pynecone-0.1.33a4/pynecone/el/precompile.py
--rw-r--r--   0        0        0    10977 2023-06-07 06:05:03.880324 pynecone-0.1.33a4/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-05-15 02:04:07.620772 pynecone-0.1.33a4/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-05-15 02:04:07.621034 pynecone-0.1.33a4/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-05-15 02:04:07.621188 pynecone-0.1.33a4/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2388 2023-06-09 19:48:39.961091 pynecone-0.1.33a4/pynecone/model.py
--rw-r--r--   0        0        0     8575 2023-06-07 19:04:43.444311 pynecone-0.1.33a4/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.33a4/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.33a4/pynecone/route.py
--rw-r--r--   0        0        0    30945 2023-06-09 19:48:33.050053 pynecone-0.1.33a4/pynecone/state.py
--rw-r--r--   0        0        0     1060 2023-05-15 02:04:07.621889 pynecone-0.1.33a4/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-05-15 02:04:07.622076 pynecone-0.1.33a4/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     7394 2023-06-09 19:48:33.050640 pynecone-0.1.33a4/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-05-15 02:04:07.622587 pynecone-0.1.33a4/pynecone/utils/console.py
--rw-r--r--   0        0        0     5317 2023-06-07 19:04:43.444774 pynecone-0.1.33a4/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11859 2023-06-09 19:48:33.051324 pynecone-0.1.33a4/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-05-15 02:04:07.623144 pynecone-0.1.33a4/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.33a4/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10873 2023-06-09 19:48:39.961277 pynecone-0.1.33a4/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.33a4/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-06-09 19:48:33.052076 pynecone-0.1.33a4/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4806 2023-06-01 03:15:26.565774 pynecone-0.1.33a4/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-05-15 02:04:07.623722 pynecone-0.1.33a4/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30928 2023-06-09 19:48:33.052425 pynecone-0.1.33a4/pynecone/vars.py
--rw-r--r--   0        0        0     1874 2023-06-10 01:56:28.309131 pynecone-0.1.33a4/pyproject.toml
--rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 pynecone-0.1.33a4/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.34a0/LICENSE
+-rw-r--r--   0        0        0     7876 2023-05-18 00:14:14.758659 pynecone-0.1.34a0/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 05:09:35.273793 pynecone-0.1.34a0/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-16 05:09:35.273930 pynecone-0.1.34a0/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-06-16 05:09:35.274029 pynecone-0.1.34a0/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-16 05:09:35.274187 pynecone-0.1.34a0/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-06-16 05:09:35.274347 pynecone-0.1.34a0/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-06-16 05:09:35.274660 pynecone-0.1.34a0/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-06-16 05:09:35.274990 pynecone-0.1.34a0/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-06-16 05:09:35.275137 pynecone-0.1.34a0/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-06-16 05:09:35.275226 pynecone-0.1.34a0/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-06-16 05:09:35.275478 pynecone-0.1.34a0/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-06-16 05:09:35.275791 pynecone-0.1.34a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0       38 2023-06-16 05:09:35.275938 pynecone-0.1.34a0/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-06-16 05:09:35.276075 pynecone-0.1.34a0/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   257247 2023-06-16 05:09:35.277131 pynecone-0.1.34a0/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-06-16 05:09:35.277373 pynecone-0.1.34a0/pynecone/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2023-06-16 05:09:35.277600 pynecone-0.1.34a0/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1029 2023-06-16 20:43:13.128932 pynecone-0.1.34a0/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-06-16 05:09:35.277911 pynecone-0.1.34a0/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-06-16 05:09:35.277968 pynecone-0.1.34a0/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0    29404 2023-06-16 05:09:35.278186 pynecone-0.1.34a0/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     8838 2023-06-16 20:43:13.129170 pynecone-0.1.34a0/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1636 2023-06-16 20:43:13.129363 pynecone-0.1.34a0/pynecone/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-16 05:09:35.278638 pynecone-0.1.34a0/pynecone/admin.py
+-rw-r--r--   0        0        0    21693 2023-06-16 20:43:13.129581 pynecone-0.1.34a0/pynecone/app.py
+-rw-r--r--   0        0        0     2548 2023-06-16 05:09:35.278940 pynecone-0.1.34a0/pynecone/base.py
+-rw-r--r--   0        0        0       29 2023-06-16 05:09:35.279040 pynecone-0.1.34a0/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     6689 2023-06-16 05:09:35.279155 pynecone-0.1.34a0/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2642 2023-06-16 05:09:35.279261 pynecone-0.1.34a0/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7767 2023-06-16 05:09:35.279374 pynecone-0.1.34a0/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     7471 2023-06-16 05:09:35.279688 pynecone-0.1.34a0/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-16 05:09:35.279922 pynecone-0.1.34a0/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-16 05:09:35.279996 pynecone-0.1.34a0/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-06-16 05:09:35.280073 pynecone-0.1.34a0/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-06-16 05:09:35.280133 pynecone-0.1.34a0/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-06-16 05:09:35.280191 pynecone-0.1.34a0/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      933 2023-06-16 05:09:35.280288 pynecone-0.1.34a0/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1412 2023-06-16 05:09:35.280378 pynecone-0.1.34a0/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    24243 2023-06-16 05:09:35.280545 pynecone-0.1.34a0/pynecone/components/component.py
+-rw-r--r--   0        0        0      496 2023-06-16 05:09:35.280902 pynecone-0.1.34a0/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-16 05:09:35.280992 pynecone-0.1.34a0/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-06-16 05:09:35.281074 pynecone-0.1.34a0/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-06-16 05:09:35.281150 pynecone-0.1.34a0/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-06-16 05:09:35.281254 pynecone-0.1.34a0/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-06-16 05:09:35.281333 pynecone-0.1.34a0/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-06-16 05:09:35.281415 pynecone-0.1.34a0/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-06-16 05:09:35.281495 pynecone-0.1.34a0/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5793 2023-06-16 05:09:35.281620 pynecone-0.1.34a0/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2188 2023-06-16 05:09:35.281738 pynecone-0.1.34a0/pynecone/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-06-16 05:09:35.281995 pynecone-0.1.34a0/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3517 2023-06-16 05:09:35.282101 pynecone-0.1.34a0/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-06-16 05:09:35.282180 pynecone-0.1.34a0/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1741 2023-06-16 05:09:35.282287 pynecone-0.1.34a0/pynecone/components/disclosure/transition.py
+-rw-r--r--   0        0        0      285 2023-06-16 05:09:35.282356 pynecone-0.1.34a0/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-06-16 05:09:35.282647 pynecone-0.1.34a0/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-06-16 05:09:35.282727 pynecone-0.1.34a0/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-06-16 05:09:35.282811 pynecone-0.1.34a0/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-06-16 05:09:35.282890 pynecone-0.1.34a0/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-06-16 05:09:35.282969 pynecone-0.1.34a0/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-06-16 05:09:35.283039 pynecone-0.1.34a0/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1471 2023-06-16 05:09:35.283322 pynecone-0.1.34a0/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-06-16 05:09:35.283424 pynecone-0.1.34a0/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-06-16 05:09:35.283533 pynecone-0.1.34a0/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3147 2023-06-16 05:09:35.283651 pynecone-0.1.34a0/pynecone/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      578 2023-06-16 05:09:35.283755 pynecone-0.1.34a0/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      243 2023-06-16 05:09:35.283847 pynecone-0.1.34a0/pynecone/components/forms/date_picker.py
+-rw-r--r--   0        0        0      277 2023-06-16 05:09:35.283931 pynecone-0.1.34a0/pynecone/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1949 2023-06-16 05:09:35.284031 pynecone-0.1.34a0/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0      243 2023-06-16 05:09:35.284144 pynecone-0.1.34a0/pynecone/components/forms/email.py
+-rw-r--r--   0        0        0     2996 2023-06-16 05:09:35.284270 pynecone-0.1.34a0/pynecone/components/forms/form.py
+-rw-r--r--   0        0        0      802 2023-06-16 05:09:35.284358 pynecone-0.1.34a0/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-06-16 05:09:35.284448 pynecone-0.1.34a0/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0    12667 2023-06-16 05:09:35.284573 pynecone-0.1.34a0/pynecone/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3897 2023-06-16 05:09:35.284676 pynecone-0.1.34a0/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-06-16 05:09:35.284744 pynecone-0.1.34a0/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-06-16 05:09:35.284841 pynecone-0.1.34a0/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-06-16 05:09:35.284950 pynecone-0.1.34a0/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-06-16 05:09:35.285054 pynecone-0.1.34a0/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3522 2023-06-16 05:09:35.285154 pynecone-0.1.34a0/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-06-16 05:09:35.285251 pynecone-0.1.34a0/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1573 2023-06-16 05:09:35.285337 pynecone-0.1.34a0/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1532 2023-06-16 05:09:35.285439 pynecone-0.1.34a0/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-06-16 05:09:35.285534 pynecone-0.1.34a0/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-06-16 05:09:35.285660 pynecone-0.1.34a0/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-16 05:09:35.285742 pynecone-0.1.34a0/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-06-16 05:09:35.285861 pynecone-0.1.34a0/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-06-16 05:09:35.286157 pynecone-0.1.34a0/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-06-16 05:09:35.286231 pynecone-0.1.34a0/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      766 2023-06-16 05:09:35.286317 pynecone-0.1.34a0/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0     2859 2023-06-16 05:09:35.286413 pynecone-0.1.34a0/pynecone/components/layout/card.py
+-rw-r--r--   0        0        0      396 2023-06-16 05:09:35.286474 pynecone-0.1.34a0/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-06-16 05:09:35.286583 pynecone-0.1.34a0/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-06-16 05:09:35.286649 pynecone-0.1.34a0/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-06-16 05:09:35.286714 pynecone-0.1.34a0/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     3167 2023-06-16 05:09:35.286852 pynecone-0.1.34a0/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2023-06-16 05:09:35.286940 pynecone-0.1.34a0/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2418 2023-06-16 05:09:35.287011 pynecone-0.1.34a0/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-06-16 05:09:35.287093 pynecone-0.1.34a0/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-06-16 05:09:35.287165 pynecone-0.1.34a0/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2023-06-16 05:09:35.287232 pynecone-0.1.34a0/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-06-16 05:09:35.287294 pynecone-0.1.34a0/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-06-16 05:09:35.287357 pynecone-0.1.34a0/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-06-16 05:09:35.287445 pynecone-0.1.34a0/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2023-06-16 05:09:35.287500 pynecone-0.1.34a0/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0     1391 2023-06-16 05:09:35.287587 pynecone-0.1.34a0/pynecone/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-16 05:09:35.287825 pynecone-0.1.34a0/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-16 05:09:35.287927 pynecone-0.1.34a0/pynecone/components/media/audio.py
+-rw-r--r--   0        0        0     1524 2023-06-16 05:09:35.288014 pynecone-0.1.34a0/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-06-16 05:09:35.288088 pynecone-0.1.34a0/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     2065 2023-06-16 20:30:09.574575 pynecone-0.1.34a0/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      197 2023-06-16 05:09:35.288271 pynecone-0.1.34a0/pynecone/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-06-16 05:09:35.288589 pynecone-0.1.34a0/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-06-16 05:09:35.288672 pynecone-0.1.34a0/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1616 2023-06-16 05:09:35.288784 pynecone-0.1.34a0/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-06-16 05:09:35.288849 pynecone-0.1.34a0/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-06-16 05:09:35.288915 pynecone-0.1.34a0/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2842 2023-06-16 05:09:35.289003 pynecone-0.1.34a0/pynecone/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-06-16 05:09:35.289274 pynecone-0.1.34a0/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-06-16 05:09:35.289387 pynecone-0.1.34a0/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1016 2023-06-16 05:09:35.289499 pynecone-0.1.34a0/pynecone/components/overlay/banner.py
+-rw-r--r--   0        0        0     4681 2023-06-16 05:09:35.289600 pynecone-0.1.34a0/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-06-16 05:09:35.289712 pynecone-0.1.34a0/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-06-16 05:09:35.289815 pynecone-0.1.34a0/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-06-16 05:09:35.289921 pynecone-0.1.34a0/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-06-16 05:09:35.290030 pynecone-0.1.34a0/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-06-16 05:09:35.290272 pynecone-0.1.34a0/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-16 05:09:35.290353 pynecone-0.1.34a0/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-06-16 05:09:35.290435 pynecone-0.1.34a0/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-06-16 05:09:35.290544 pynecone-0.1.34a0/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-06-16 05:09:35.290617 pynecone-0.1.34a0/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      304 2023-06-16 05:09:35.290747 pynecone-0.1.34a0/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-16 05:09:35.290812 pynecone-0.1.34a0/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      682 2023-06-16 05:09:35.290901 pynecone-0.1.34a0/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3460 2023-06-16 05:09:35.290998 pynecone-0.1.34a0/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-06-16 05:09:35.291063 pynecone-0.1.34a0/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-06-16 05:09:35.291128 pynecone-0.1.34a0/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     7051 2023-06-16 05:09:35.291265 pynecone-0.1.34a0/pynecone/config.py
+-rw-r--r--   0        0        0    10252 2023-06-16 05:09:35.291415 pynecone-0.1.34a0/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-06-16 05:09:35.291528 pynecone-0.1.34a0/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-16 05:09:35.291627 pynecone-0.1.34a0/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-06-16 05:09:35.291727 pynecone-0.1.34a0/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-06-16 05:09:35.291801 pynecone-0.1.34a0/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-06-16 05:09:35.291904 pynecone-0.1.34a0/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1320 2023-06-16 05:09:35.292004 pynecone-0.1.34a0/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-06-16 05:09:35.292266 pynecone-0.1.34a0/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-06-16 05:09:35.292389 pynecone-0.1.34a0/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    11876 2023-06-16 20:43:13.129852 pynecone-0.1.34a0/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-06-16 05:09:35.292653 pynecone-0.1.34a0/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-16 05:09:35.292762 pynecone-0.1.34a0/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-06-16 05:09:35.292844 pynecone-0.1.34a0/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2388 2023-06-16 05:09:35.292946 pynecone-0.1.34a0/pynecone/model.py
+-rw-r--r--   0        0        0     8575 2023-06-16 06:58:15.564372 pynecone-0.1.34a0/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-06-16 05:09:35.293110 pynecone-0.1.34a0/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-06-16 05:09:35.293208 pynecone-0.1.34a0/pynecone/route.py
+-rw-r--r--   0        0        0    30945 2023-06-16 05:09:35.293398 pynecone-0.1.34a0/pynecone/state.py
+-rw-r--r--   0        0        0     1121 2023-06-16 05:09:35.293539 pynecone-0.1.34a0/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-06-16 05:09:35.293673 pynecone-0.1.34a0/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     7394 2023-06-16 05:09:35.293800 pynecone-0.1.34a0/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-06-16 05:09:35.294005 pynecone-0.1.34a0/pynecone/utils/console.py
+-rw-r--r--   0        0        0     5317 2023-06-16 05:09:35.294115 pynecone-0.1.34a0/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11859 2023-06-16 05:09:35.294243 pynecone-0.1.34a0/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-06-16 05:09:35.294316 pynecone-0.1.34a0/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-06-16 05:09:35.294391 pynecone-0.1.34a0/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10905 2023-06-16 05:09:35.294530 pynecone-0.1.34a0/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-06-16 05:09:35.294639 pynecone-0.1.34a0/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-06-16 05:09:35.294743 pynecone-0.1.34a0/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4806 2023-06-16 05:09:35.294850 pynecone-0.1.34a0/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-06-16 05:09:35.294923 pynecone-0.1.34a0/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30928 2023-06-16 05:09:35.295168 pynecone-0.1.34a0/pynecone/vars.py
+-rw-r--r--   0        0        0     1874 2023-06-16 20:46:03.468826 pynecone-0.1.34a0/pyproject.toml
+-rw-r--r--   0        0        0     9511 1970-01-01 00:00:00.000000 pynecone-0.1.34a0/PKG-INFO
```

### Comparing `pynecone-0.1.33a4/LICENSE` & `pynecone-0.1.34a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/README.md` & `pynecone-0.1.34a0/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.34a0/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.34a0/pynecone/.templates/apps/default/default.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,32 +10,36 @@
 class State(pc.State):
     """The app state."""
 
     pass
 
 
 def index() -> pc.Component:
-    return pc.center(
+    return pc.fragment(
+        pc.color_mode_button(pc.color_mode_icon(), float="right"),
         pc.vstack(
             pc.heading("Welcome to Pynecone!", font_size="2em"),
             pc.box("Get started by editing ", pc.code(filename, font_size="1em")),
             pc.link(
                 "Check out our docs!",
                 href=docs_url,
                 border="0.1em solid",
                 padding="0.5em",
                 border_radius="0.5em",
                 _hover={
-                    "color": "rgb(107,99,246)",
+                    "color": pc.color_mode_cond(
+                        light="rgb(107,99,246)",
+                        dark="rgb(179, 175, 255)",
+                    )
                 },
             ),
             spacing="1.5em",
             font_size="2em",
+            padding_top="10%",
         ),
-        padding_top="10%",
     )
 
 
 # Add state and page to the app.
 app = pc.App(state=State)
 app.add_page(index)
 app.compile()
```

### Comparing `pynecone-0.1.33a4/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.34a0/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.34a0/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.34a0/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.34a0/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/.templates/web/package.json` & `pynecone-0.1.34a0/pynecone/.templates/web/package.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9940476190476191%*

 * *Differences: {"'dependencies'": "{'universal-cookie': '^4.0.4'}"}*

```diff
@@ -22,14 +22,15 @@
         "react-plotly.js": "^2.6.0",
         "react-syntax-highlighter": "^15.5.0",
         "rehype-katex": "^6.0.3",
         "rehype-raw": "^6.1.1",
         "remark-gfm": "^3.0.1",
         "remark-math": "^5.1.1",
         "socket.io-client": "^4.6.1",
+        "universal-cookie": "^4.0.4",
         "victory": "^36.6.8"
     },
     "name": "pynecone",
     "scripts": {
         "dev": "next dev",
         "export": "next build && next export -o _static",
         "prod": "next start"
```

### Comparing `pynecone-0.1.33a4/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.34a0/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.34a0/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.34a0/pynecone/.templates/web/utils/state.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,14 @@
 // State management for Pynecone web apps.
 import axios from "axios";
 import io from "socket.io-client";
 import JSON5 from "json5";
 import env from "env.json";
+import Cookies from "universal-cookie";
+
 
 // Endpoint URLs.
 const PINGURL = env.pingUrl
 const EVENTURL = env.eventUrl
 const UPLOADURL = env.uploadUrl
 
 // Global variable to hold the token.
@@ -90,14 +92,26 @@
     }
 
     if (event.name == "_console") {
         console.log(event.payload.message);
         return false;
     }
 
+    if (event.name == "_set_cookie") {
+        const cookies = new Cookies();
+        cookies.set(event.payload.key, event.payload.value);
+        localStorage.setItem(event.payload.key, event.payload.value);
+        return false;
+    }
+
+    if (event.name == "_set_local_storage") {
+        localStorage.setItem(event.payload.key, event.payload.value);
+        return false;
+    }
+
     if (event.name == "_alert") {
         alert(event.payload.message);
         return false;
     }
 
     if (event.name == "_set_focus") {
         const ref =
@@ -171,20 +185,20 @@
     // Set processing to true to block other events from being processed.
     setResult({
         ...result,
         processing: true
     });
 
     // Apply the next event in the queue.
-    const event = state.events[0];
+    const event = state.events.shift();
 
     // Set new events to avoid reprocessing the same event.
     setState(state => ({
         ...state,
-        events: state.events.slice(1)
+        events: state.events
     }));
 
     // Process events with handlers via REST and all others via websockets.
     let eventSent = false;
     if (event.handler) {
         eventSent = await applyRestEvent(event, state, setResult);
     } else {
```

### Comparing `pynecone-0.1.33a4/pynecone/__init__.py` & `pynecone-0.1.34a0/pynecone/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,19 +19,22 @@
 from .constants import Env as Env
 from .constants import Transports as Transports
 from .event import EVENT_ARG as EVENT_ARG
 from .event import EventChain as EventChain
 from .event import FileUpload as upload_files
 from .event import console_log as console_log
 from .event import redirect as redirect
+from .event import set_cookie as set_cookie
 from .event import set_focus as set_focus
+from .event import set_local_storage as set_local_storage
 from .event import set_value as set_value
 from .event import window_alert as window_alert
 from .middleware import Middleware as Middleware
 from .model import Model as Model
 from .model import session as session
 from .route import route as route
 from .state import ComputedVar as var
 from .state import State as State
+from .style import color_mode as color_mode
 from .style import toggle_color_mode as toggle_color_mode
 from .vars import Var as Var
 from .vars import cached_var as cached_var
```

### Comparing `pynecone-0.1.33a4/pynecone/app.py` & `pynecone-0.1.34a0/pynecone/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The main Pynecone app."""
 
 import asyncio
 import inspect
+from multiprocessing.pool import ThreadPool
 from typing import (
     Any,
     AsyncIterator,
     Callable,
     Coroutine,
     Dict,
     List,
@@ -450,25 +451,30 @@
         compiler.compile_document_root(self.stylesheets)
 
         # Compile the theme.
         compiler.compile_theme(self.style)
 
         # Compile the pages.
         custom_components = set()
+        thread_pool = ThreadPool()
         for route, component in self.pages.items():
             component.add_style(self.style)
-            compiler.compile_page(
-                route,
-                component,
-                self.state,
-                self.connect_error_component,
+            thread_pool.apply_async(
+                compiler.compile_page,
+                args=(
+                    route,
+                    component,
+                    self.state,
+                    self.connect_error_component,
+                ),
             )
-
             # Add the custom components from the page to the set.
             custom_components |= component.get_custom_components()
+        thread_pool.close()
+        thread_pool.join()
 
         # Compile the custom components.
         compiler.compile_components(custom_components)
 
 
 async def process(
     app: App, event: Event, sid: str, headers: Dict, client_ip: str
@@ -658,15 +664,17 @@
 
         # Get the client IP
         client_ip = environ["REMOTE_ADDR"]
 
         # Process the events.
         async for update in process(self.app, event, sid, headers, client_ip):
             # Emit the event.
-            await self.emit(str(constants.SocketEvent.EVENT), update.json(), to=sid)  # type: ignore
+            await asyncio.create_task(
+                self.emit(str(constants.SocketEvent.EVENT), update.json(), to=sid)
+            )
 
     async def on_ping(self, sid):
         """Event for testing the API endpoint.
 
         Args:
             sid: The Socket.IO session id.
         """
```

### Comparing `pynecone-0.1.33a4/pynecone/base.py` & `pynecone-0.1.34a0/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/compiler/compiler.py` & `pynecone-0.1.34a0/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/compiler/templates.py` & `pynecone-0.1.34a0/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/compiler/utils.py` & `pynecone-0.1.34a0/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/__init__.py` & `pynecone-0.1.34a0/pynecone/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,7 +234,10 @@
 highlight = Highlight.create
 markdown = Markdown.create
 span = Span.create
 text = Text.create
 script = ScriptTag.create
 aspect_ratio = AspectRatio.create
 kbd = KeyboardKey.create
+color_mode_button = ColorModeButton.create
+color_mode_icon = ColorModeIcon.create
+color_mode_switch = ColorModeSwitch.create
```

### Comparing `pynecone-0.1.33a4/pynecone/components/base/bare.py` & `pynecone-0.1.34a0/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/base/document.py` & `pynecone-0.1.34a0/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/base/link.py` & `pynecone-0.1.34a0/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/base/meta.py` & `pynecone-0.1.34a0/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/component.py` & `pynecone-0.1.34a0/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/datadisplay/code.py` & `pynecone-0.1.34a0/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.34a0/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.34a0/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/datadisplay/list.py` & `pynecone-0.1.34a0/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.34a0/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/datadisplay/table.py` & `pynecone-0.1.34a0/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/datadisplay/tag.py` & `pynecone-0.1.34a0/pynecone/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.34a0/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.34a0/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/disclosure/transition.py` & `pynecone-0.1.34a0/pynecone/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/feedback/alert.py` & `pynecone-0.1.34a0/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.34a0/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/feedback/progress.py` & `pynecone-0.1.34a0/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.34a0/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/feedback/spinner.py` & `pynecone-0.1.34a0/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/button.py` & `pynecone-0.1.34a0/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/checkbox.py` & `pynecone-0.1.34a0/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.34a0/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/editable.py` & `pynecone-0.1.34a0/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/form.py` & `pynecone-0.1.34a0/pynecone/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.34a0/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/input.py` & `pynecone-0.1.34a0/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/multiselect.py` & `pynecone-0.1.34a0/pynecone/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/numberinput.py` & `pynecone-0.1.34a0/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/pininput.py` & `pynecone-0.1.34a0/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/radio.py` & `pynecone-0.1.34a0/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.34a0/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/select.py` & `pynecone-0.1.34a0/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/slider.py` & `pynecone-0.1.34a0/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/switch.py` & `pynecone-0.1.34a0/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/textarea.py` & `pynecone-0.1.34a0/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/forms/upload.py` & `pynecone-0.1.34a0/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/graphing/plotly.py` & `pynecone-0.1.34a0/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/graphing/victory.py` & `pynecone-0.1.34a0/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/__init__.py` & `pynecone-0.1.34a0/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/box.py` & `pynecone-0.1.34a0/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/card.py` & `pynecone-0.1.34a0/pynecone/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/cond.py` & `pynecone-0.1.34a0/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/flex.py` & `pynecone-0.1.34a0/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/foreach.py` & `pynecone-0.1.34a0/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/grid.py` & `pynecone-0.1.34a0/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/html.py` & `pynecone-0.1.34a0/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/responsive.py` & `pynecone-0.1.34a0/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/stack.py` & `pynecone-0.1.34a0/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/layout/wrap.py` & `pynecone-0.1.34a0/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/libs/react_player.py` & `pynecone-0.1.34a0/pynecone/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/media/avatar.py` & `pynecone-0.1.34a0/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/media/icon.py` & `pynecone-0.1.34a0/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/media/image.py` & `pynecone-0.1.34a0/pynecone/components/media/image.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,18 +35,21 @@
 
     # If true, opt out of the fallbackSrc logic and use as img.
     ignore_fallback: Var[bool]
 
     # "eager" | "lazy"
     loading: Var[str]
 
-    # The image src attribute.
+    # The path/url to the image or PIL image object.
     src: Var[Any]
 
-    # The image srcset attribute.
+    # Provide multiple sources for an image, allowing the browser
+    # to select the most appropriate source based on factors like
+    # screen resolution and device capabilities.
+    # Learn more _[here](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)_
     src_set: Var[str]
 
     def get_triggers(self) -> Set[str]:
         """Get the event triggers for the component.
 
         Returns:
             The event triggers.
```

### Comparing `pynecone-0.1.33a4/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.34a0/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/navigation/link.py` & `pynecone-0.1.34a0/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.34a0/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/navigation/stepper.py` & `pynecone-0.1.34a0/pynecone/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/overlay/__init__.py` & `pynecone-0.1.34a0/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.34a0/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/overlay/banner.py` & `pynecone-0.1.34a0/pynecone/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/overlay/drawer.py` & `pynecone-0.1.34a0/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/overlay/menu.py` & `pynecone-0.1.34a0/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/overlay/modal.py` & `pynecone-0.1.34a0/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/overlay/popover.py` & `pynecone-0.1.34a0/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.34a0/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.34a0/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/tags/tag.py` & `pynecone-0.1.34a0/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/tags/tagless.py` & `pynecone-0.1.34a0/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/typography/highlight.py` & `pynecone-0.1.34a0/pynecone/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/components/typography/markdown.py` & `pynecone-0.1.34a0/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/config.py` & `pynecone-0.1.34a0/pynecone/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
 
     # Disable bun.
     disable_bun: bool = False
 
     # Additional frontend packages to install.
     frontend_packages: List[str] = []
 
-    # The Admin Dash
+    # The Admin Dash.
     admin_dash: Optional[AdminDash] = None
 
     # Backend transport methods.
     backend_transports: Optional[
         constants.Transports
     ] = constants.Transports.WEBSOCKET_POLLING
 
@@ -187,20 +187,23 @@
 
     # Whether credentials (cookies, authentication) are allowed in requests to the backend API.
     cors_credentials: Optional[bool] = True
 
     # The maximum size of a message when using the polling backend transport.
     polling_max_http_buffer_size: Optional[int] = constants.POLLING_MAX_HTTP_BUFFER_SIZE
 
-    # Dotenv file path
+    # Dotenv file path.
     env_path: Optional[str] = constants.DOT_ENV_FILE
 
-    # Whether to override OS environment variables
+    # Whether to override OS environment variables.
     override_os_envs: Optional[bool] = True
 
+    # Timeout when launching the gunicorn server.
+    timeout: int = constants.TIMEOUT
+
     def __init__(self, *args, **kwargs):
         """Initialize the config values.
 
         If db_url is not provided gets it from db_config.
 
         Args:
             *args: The args to pass to the Pydantic init method.
```

### Comparing `pynecone-0.1.33a4/pynecone/constants.py` & `pynecone-0.1.34a0/pynecone/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 # The default path where bun is installed.
 BUN_PATH = get_value("BUN_PATH", f"{BUN_ROOT_PATH}/bin/bun")
 # Command to install bun.
 INSTALL_BUN = f"curl -fsSL https://bun.sh/install | bash -s -- bun-v{MAX_BUN_VERSION}"
 # Default host in dev mode.
 BACKEND_HOST = get_value("BACKEND_HOST", "0.0.0.0")
 # The default timeout when launching the gunicorn server.
-TIMEOUT = 120
+TIMEOUT = get_value("TIMEOUT", 120, type_=int)
 # The command to run the backend in production mode.
 RUN_BACKEND_PROD = f"gunicorn --worker-class uvicorn.workers.UvicornH11Worker --preload --timeout {TIMEOUT} --log-level critical".split()
 RUN_BACKEND_PROD_WINDOWS = f"uvicorn --timeout-keep-alive {TIMEOUT}".split()
 # Socket.IO web server
 PING_INTERVAL = 25
 PING_TIMEOUT = 120
```

### Comparing `pynecone-0.1.33a4/pynecone/el/constants/html.py` & `pynecone-0.1.34a0/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/el/constants/pynecone.py` & `pynecone-0.1.34a0/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/el/constants/react.py` & `pynecone-0.1.34a0/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/el/element.py` & `pynecone-0.1.34a0/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/el/elements/__init__.py` & `pynecone-0.1.34a0/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/el/precompile.py` & `pynecone-0.1.34a0/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/event.py` & `pynecone-0.1.34a0/pynecone/event.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,14 +232,50 @@
         "_set_value",
         get_fn_signature(set_value),
         ref=Var.create_safe(format.format_ref(ref)),
         value=value,
     )
 
 
+def set_cookie(key: str, value: str) -> EventSpec:
+    """Set a cookie on the frontend.
+
+    Args:
+        key (str): The key identifying the cookie.
+        value (str): The value contained in the cookie.
+
+    Returns:
+        EventSpec: An event to set a cookie.
+    """
+    return server_side(
+        "_set_cookie",
+        get_fn_signature(set_cookie),
+        key=key,
+        value=value,
+    )
+
+
+def set_local_storage(key: str, value: str) -> EventSpec:
+    """Set a value in the local storage on the frontend.
+
+    Args:
+        key (str): The key identifying the variable in the local storage.
+        value (str): The value contained in the local storage.
+
+    Returns:
+        EventSpec: An event to set a key-value in local storage.
+    """
+    return server_side(
+        "_set_local_storage",
+        get_fn_signature(set_local_storage),
+        key=key,
+        value=value,
+    )
+
+
 def get_event(state, event):
     """Get the event from the given state.
 
     Args:
         state: The state.
         event: The event.
```

### Comparing `pynecone-0.1.33a4/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.34a0/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/middleware/middleware.py` & `pynecone-0.1.34a0/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/model.py` & `pynecone-0.1.34a0/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/pc.py` & `pynecone-0.1.34a0/pynecone/pc.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/route.py` & `pynecone-0.1.34a0/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/state.py` & `pynecone-0.1.34a0/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/style.py` & `pynecone-0.1.34a0/pynecone/style.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional
 
 from pynecone import constants
 from pynecone.event import EventChain
 from pynecone.utils import format
 from pynecone.vars import BaseVar, Var
 
+color_mode = BaseVar(name=constants.COLOR_MODE, type_="str")
 toggle_color_mode = BaseVar(name=constants.TOGGLE_COLOR_MODE, type_=EventChain)
 
 
 def convert(style_dict):
     """Format a style dictionary.
 
     Args:
```

### Comparing `pynecone-0.1.33a4/pynecone/utils/build.py` & `pynecone-0.1.34a0/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/console.py` & `pynecone-0.1.34a0/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/exec.py` & `pynecone-0.1.34a0/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/format.py` & `pynecone-0.1.34a0/pynecone/utils/format.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/imports.py` & `pynecone-0.1.34a0/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/path_ops.py` & `pynecone-0.1.34a0/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/prerequisites.py` & `pynecone-0.1.34a0/pynecone/utils/prerequisites.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,19 +176,19 @@
     """Initialize the template .gitignore file."""
     # The files to add to the .gitignore file.
     files = constants.DEFAULT_GITIGNORE
 
     # Subtract current ignored files.
     if os.path.exists(constants.GITIGNORE_FILE):
         with open(constants.GITIGNORE_FILE, "r") as f:
-            files -= set(f.read().splitlines())
+            files -= set(f.read().replace(" ", "").strip().splitlines())
 
     # Add the new files to the .gitignore file.
     with open(constants.GITIGNORE_FILE, "a") as f:
-        f.write(path_ops.join(files))
+        f.write(f"\n{path_ops.join(files)}")
 
 
 def initialize_app_directory(app_name: str, template: constants.Template):
     """Initialize the app directory on pc init.
 
     Args:
         app_name: The name of the app.
```

### Comparing `pynecone-0.1.33a4/pynecone/utils/processes.py` & `pynecone-0.1.34a0/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/telemetry.py` & `pynecone-0.1.34a0/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/types.py` & `pynecone-0.1.34a0/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/utils/watch.py` & `pynecone-0.1.34a0/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pynecone/vars.py` & `pynecone-0.1.34a0/pynecone/vars.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.33a4/pyproject.toml` & `pynecone-0.1.34a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.33a4"
+version = "0.1.34a0"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
@@ -61,15 +61,15 @@
 asynctest = "^0.13.0"
 pre-commit = {version = "^3.2.1", python = ">=3.8,<4.0"}
 
 [tool.poetry.scripts]
 pc = "pynecone.pc:main"
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.5.1"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pyright]
 
 [tool.ruff]
 
 select = ["B", "D", "E", "F", "I", "SIM", "W"]
```

### Comparing `pynecone-0.1.33a4/PKG-INFO` & `pynecone-0.1.34a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.33a4
+Version: 0.1.34a0
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

