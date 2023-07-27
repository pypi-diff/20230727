# Comparing `tmp/reflex-0.2.3a6.tar.gz` & `tmp/reflex-0.2.3a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.3a6.tar", max compression
+gzip compressed data, was "reflex-0.2.3a7.tar", max compression
```

## Comparing `reflex-0.2.3a6.tar` & `reflex-0.2.3a7.tar`

### file list

```diff
@@ -1,178 +1,178 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a6/LICENSE
--rw-r--r--   0        0        0     7905 2023-07-25 18:50:56.099599 reflex-0.2.3a6/README.md
--rw-r--r--   0        0        0     2002 2023-07-27 00:27:18.820268 reflex-0.2.3a6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a6/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1337 2023-07-26 04:50:13.391602 reflex-0.2.3a6/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a6/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.3a6/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a6/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a6/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a6/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a6/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a6/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a6/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a6/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a6/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a6/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a6/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a6/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a6/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a6/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.3a6/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a6/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a6/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a6/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a6/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a6/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0    10127 2023-07-26 23:51:58.835310 reflex-0.2.3a6/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.3a6/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a6/reflex/admin.py
--rw-r--r--   0        0        0    24459 2023-07-26 22:57:11.741737 reflex-0.2.3a6/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a6/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a6/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a6/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.3a6/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a6/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a6/reflex/components/__init__.py
--rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a6/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a6/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a6/reflex/components/base/body.py
--rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a6/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a6/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a6/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a6/reflex/components/base/meta.py
--rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a6/reflex/components/base/script.py
--rw-r--r--   0        0        0    24321 2023-07-25 18:39:55.676277 reflex-0.2.3a6/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a6/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a6/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.3a6/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a6/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a6/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a6/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a6/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a6/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a6/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a6/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a6/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a6/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a6/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a6/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a6/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a6/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a6/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a6/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a6/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a6/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a6/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a6/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a6/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a6/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a6/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a6/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a6/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a6/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a6/reflex/components/forms/debounce.py
--rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a6/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a6/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a6/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a6/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3246 2023-07-21 23:52:40.428089 reflex-0.2.3a6/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a6/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a6/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a6/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a6/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a6/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a6/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a6/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a6/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a6/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a6/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a6/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a6/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a6/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a6/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a6/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a6/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a6/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a6/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a6/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a6/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a6/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a6/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a6/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a6/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a6/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a6/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a6/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a6/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a6/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a6/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a6/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a6/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a6/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a6/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a6/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a6/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a6/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a6/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a6/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a6/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.3a6/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a6/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a6/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a6/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a6/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a6/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a6/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a6/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a6/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a6/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a6/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a6/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a6/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a6/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a6/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.3a6/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5008 2023-07-26 23:51:58.836068 reflex-0.2.3a6/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a6/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a6/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      278 2023-07-26 23:51:58.836239 reflex-0.2.3a6/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a6/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     3593 2023-07-26 23:51:58.836350 reflex-0.2.3a6/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a6/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a6/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7564 2023-07-26 23:56:51.622625 reflex-0.2.3a6/reflex/config.py
--rw-r--r--   0        0        0    12034 2023-07-27 00:18:01.968850 reflex-0.2.3a6/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a6/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a6/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a6/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a6/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a6/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a6/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a6/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a6/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a6/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a6/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a6/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a6/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     9604 2023-07-19 23:09:19.472388 reflex-0.2.3a6/reflex/model.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a6/reflex/py.typed
--rw-r--r--   0        0        0    10559 2023-07-26 23:56:51.624045 reflex-0.2.3a6/reflex/reflex.py
--rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.3a6/reflex/route.py
--rw-r--r--   0        0        0    32118 2023-07-26 23:51:58.837266 reflex-0.2.3a6/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a6/reflex/style.py
--rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.3a6/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a6/reflex/utils/__init__.py
--rw-r--r--   0        0        0     7732 2023-07-26 23:56:51.625397 reflex-0.2.3a6/reflex/utils/build.py
--rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.3a6/reflex/utils/console.py
--rw-r--r--   0        0        0     4045 2023-07-26 23:56:51.625698 reflex-0.2.3a6/reflex/utils/exec.py
--rw-r--r--   0        0        0    11845 2023-07-21 23:46:28.128377 reflex-0.2.3a6/reflex/utils/format.py
--rw-r--r--   0        0        0      585 2023-07-26 22:57:11.745697 reflex-0.2.3a6/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a6/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    14193 2023-07-26 23:56:51.626847 reflex-0.2.3a6/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     4200 2023-07-26 23:56:51.627344 reflex-0.2.3a6/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a6/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a6/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a6/reflex/utils/watch.py
--rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a6/reflex/vars.py
--rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 reflex-0.2.3a6/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a7/LICENSE
+-rw-r--r--   0        0        0     7905 2023-07-25 18:50:56.099599 reflex-0.2.3a7/README.md
+-rw-r--r--   0        0        0     2002 2023-07-27 02:12:09.661733 reflex-0.2.3a7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a7/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1337 2023-07-26 04:50:13.391602 reflex-0.2.3a7/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a7/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1225 2023-07-14 23:13:37.769942 reflex-0.2.3a7/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a7/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a7/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a7/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a7/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a7/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a7/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a7/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a7/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a7/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.3a7/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a7/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a7/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a7/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a7/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a7/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0    10127 2023-07-27 02:10:59.437571 reflex-0.2.3a7/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1965 2023-07-19 01:58:26.538410 reflex-0.2.3a7/reflex/__init__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a7/reflex/admin.py
+-rw-r--r--   0        0        0    24459 2023-07-26 22:57:11.741737 reflex-0.2.3a7/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a7/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a7/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a7/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.3a7/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a7/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a7/reflex/components/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a7/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a7/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a7/reflex/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a7/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a7/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a7/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a7/reflex/components/base/meta.py
+-rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a7/reflex/components/base/script.py
+-rw-r--r--   0        0        0    24321 2023-07-25 18:39:55.676277 reflex-0.2.3a7/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a7/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a7/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.3a7/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a7/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a7/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a7/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a7/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a7/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a7/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a7/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a7/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a7/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a7/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a7/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a7/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a7/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a7/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a7/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a7/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a7/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a7/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a7/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a7/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a7/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a7/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a7/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a7/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a7/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a7/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a7/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a7/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a7/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a7/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3246 2023-07-21 23:52:40.428089 reflex-0.2.3a7/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a7/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a7/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a7/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a7/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a7/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a7/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a7/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a7/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a7/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a7/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a7/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a7/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a7/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a7/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a7/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a7/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a7/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a7/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a7/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a7/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a7/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a7/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a7/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a7/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a7/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a7/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a7/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a7/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a7/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a7/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a7/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a7/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a7/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a7/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a7/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a7/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a7/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a7/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a7/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a7/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-07-14 23:13:37.778119 reflex-0.2.3a7/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a7/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a7/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a7/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a7/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a7/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a7/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a7/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a7/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a7/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a7/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a7/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a7/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a7/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a7/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.3a7/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-07-27 02:10:59.437877 reflex-0.2.3a7/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a7/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a7/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-07-27 02:10:59.438075 reflex-0.2.3a7/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a7/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3593 2023-07-27 02:10:59.438276 reflex-0.2.3a7/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a7/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a7/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7692 2023-07-27 01:47:00.564666 reflex-0.2.3a7/reflex/config.py
+-rw-r--r--   0        0        0    11209 2023-07-27 02:11:07.178831 reflex-0.2.3a7/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a7/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a7/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a7/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a7/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a7/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a7/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a7/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a7/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a7/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a7/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a7/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a7/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     9604 2023-07-19 23:09:19.472388 reflex-0.2.3a7/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a7/reflex/py.typed
+-rw-r--r--   0        0        0    11041 2023-07-27 02:11:07.179265 reflex-0.2.3a7/reflex/reflex.py
+-rw-r--r--   0        0        0     4104 2023-07-14 23:13:37.781214 reflex-0.2.3a7/reflex/route.py
+-rw-r--r--   0        0        0    32314 2023-07-27 02:11:44.068790 reflex-0.2.3a7/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a7/reflex/style.py
+-rw-r--r--   0        0        0    15063 2023-07-14 23:13:37.781613 reflex-0.2.3a7/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a7/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     7971 2023-07-27 01:47:00.567138 reflex-0.2.3a7/reflex/utils/build.py
+-rw-r--r--   0        0        0     1692 2023-07-19 01:58:26.541439 reflex-0.2.3a7/reflex/utils/console.py
+-rw-r--r--   0        0        0     4225 2023-07-27 01:47:00.567438 reflex-0.2.3a7/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-07-21 23:46:28.128377 reflex-0.2.3a7/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-07-26 22:57:11.745697 reflex-0.2.3a7/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a7/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    14208 2023-07-27 02:11:07.179634 reflex-0.2.3a7/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     4105 2023-07-27 01:47:00.568031 reflex-0.2.3a7/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a7/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a7/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a7/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a7/reflex/vars.py
+-rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 reflex-0.2.3a7/PKG-INFO
```

### Comparing `reflex-0.2.3a6/LICENSE` & `reflex-0.2.3a7/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/README.md` & `reflex-0.2.3a7/README.md`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/pyproject.toml` & `reflex-0.2.3a7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.3a6"
+version = "0.2.3a7"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `reflex-0.2.3a6/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.3a7/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/apps/default/default.py` & `reflex-0.2.3a7/reflex/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/assets/favicon.ico` & `reflex-0.2.3a7/reflex/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.3a7/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.3a7/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/web/bun.lockb` & `reflex-0.2.3a7/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/web/package.json` & `reflex-0.2.3a7/reflex/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/web/pages/_app.js` & `reflex-0.2.3a7/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.3a7/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/.templates/web/utils/state.js` & `reflex-0.2.3a7/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/__init__.py` & `reflex-0.2.3a7/reflex/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/app.py` & `reflex-0.2.3a7/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/base.py` & `reflex-0.2.3a7/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/compiler/compiler.py` & `reflex-0.2.3a7/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/compiler/templates.py` & `reflex-0.2.3a7/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/compiler/utils.py` & `reflex-0.2.3a7/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/__init__.py` & `reflex-0.2.3a7/reflex/components/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/base/bare.py` & `reflex-0.2.3a7/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/base/document.py` & `reflex-0.2.3a7/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/base/link.py` & `reflex-0.2.3a7/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/base/meta.py` & `reflex-0.2.3a7/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/base/script.py` & `reflex-0.2.3a7/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/component.py` & `reflex-0.2.3a7/reflex/components/component.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/datadisplay/code.py` & `reflex-0.2.3a7/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/datadisplay/datatable.py` & `reflex-0.2.3a7/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/datadisplay/divider.py` & `reflex-0.2.3a7/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/datadisplay/list.py` & `reflex-0.2.3a7/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/datadisplay/stat.py` & `reflex-0.2.3a7/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/datadisplay/table.py` & `reflex-0.2.3a7/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/datadisplay/tag.py` & `reflex-0.2.3a7/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/disclosure/accordion.py` & `reflex-0.2.3a7/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/disclosure/tabs.py` & `reflex-0.2.3a7/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/disclosure/transition.py` & `reflex-0.2.3a7/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/feedback/alert.py` & `reflex-0.2.3a7/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/feedback/circularprogress.py` & `reflex-0.2.3a7/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/feedback/progress.py` & `reflex-0.2.3a7/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/feedback/skeleton.py` & `reflex-0.2.3a7/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/feedback/spinner.py` & `reflex-0.2.3a7/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/__init__.py` & `reflex-0.2.3a7/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/button.py` & `reflex-0.2.3a7/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/checkbox.py` & `reflex-0.2.3a7/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.3a7/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.3a7/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/debounce.py` & `reflex-0.2.3a7/reflex/components/forms/debounce.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/editable.py` & `reflex-0.2.3a7/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/form.py` & `reflex-0.2.3a7/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/iconbutton.py` & `reflex-0.2.3a7/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/input.py` & `reflex-0.2.3a7/reflex/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/multiselect.py` & `reflex-0.2.3a7/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/numberinput.py` & `reflex-0.2.3a7/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/pininput.py` & `reflex-0.2.3a7/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/radio.py` & `reflex-0.2.3a7/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/rangeslider.py` & `reflex-0.2.3a7/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/select.py` & `reflex-0.2.3a7/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/slider.py` & `reflex-0.2.3a7/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/switch.py` & `reflex-0.2.3a7/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/textarea.py` & `reflex-0.2.3a7/reflex/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/forms/upload.py` & `reflex-0.2.3a7/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/graphing/plotly.py` & `reflex-0.2.3a7/reflex/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/graphing/victory.py` & `reflex-0.2.3a7/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/__init__.py` & `reflex-0.2.3a7/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/box.py` & `reflex-0.2.3a7/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/card.py` & `reflex-0.2.3a7/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/cond.py` & `reflex-0.2.3a7/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/flex.py` & `reflex-0.2.3a7/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/foreach.py` & `reflex-0.2.3a7/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/grid.py` & `reflex-0.2.3a7/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/html.py` & `reflex-0.2.3a7/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/responsive.py` & `reflex-0.2.3a7/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/stack.py` & `reflex-0.2.3a7/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/layout/wrap.py` & `reflex-0.2.3a7/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/libs/react_player.py` & `reflex-0.2.3a7/reflex/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/media/avatar.py` & `reflex-0.2.3a7/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/media/icon.py` & `reflex-0.2.3a7/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/media/image.py` & `reflex-0.2.3a7/reflex/components/media/image.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.3a7/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/navigation/link.py` & `reflex-0.2.3a7/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.3a7/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/navigation/stepper.py` & `reflex-0.2.3a7/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/overlay/__init__.py` & `reflex-0.2.3a7/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/overlay/alertdialog.py` & `reflex-0.2.3a7/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/overlay/banner.py` & `reflex-0.2.3a7/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/overlay/drawer.py` & `reflex-0.2.3a7/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/overlay/menu.py` & `reflex-0.2.3a7/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/overlay/modal.py` & `reflex-0.2.3a7/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/overlay/popover.py` & `reflex-0.2.3a7/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/overlay/tooltip.py` & `reflex-0.2.3a7/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/tags/iter_tag.py` & `reflex-0.2.3a7/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/tags/tag.py` & `reflex-0.2.3a7/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/tags/tagless.py` & `reflex-0.2.3a7/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/typography/highlight.py` & `reflex-0.2.3a7/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/components/typography/markdown.py` & `reflex-0.2.3a7/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/config.py` & `reflex-0.2.3a7/reflex/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,20 @@
 
     # The rxdeploy url.
     rxdeploy_url: Optional[str] = None
 
     # The environment mode.
     env: constants.Env = constants.Env.DEV
 
+    # The path to the bun executable.
+    bun_path: str = constants.BUN_PATH
+
+    # Disable bun.
+    disable_bun: bool = False
+
     # Additional frontend packages to install.
     frontend_packages: List[str] = []
 
     # The Admin Dash.
     admin_dash: Optional[AdminDash] = None
 
     # Backend transport methods.
```

### Comparing `reflex-0.2.3a6/reflex/constants.py` & `reflex-0.2.3a7/reflex/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Constants used throughout the package."""
 
 import os
-import platform
 import re
 from enum import Enum
 from types import SimpleNamespace
 from typing import Any, Type
 
 # importlib is only available for Python 3.8+ so we need the backport for Python 3.7
 try:
@@ -40,47 +39,20 @@
 
 
 # App names and versions.
 # The name of the Reflex package.
 MODULE_NAME = "reflex"
 # The current version of Reflex.
 VERSION = metadata.version(MODULE_NAME)
+# Minimum version of Node.js required to run Reflex.
+MIN_NODE_VERSION = "16.8.0"
 
-# Project dependencies.
-# The directory to store reflex dependencies.
-REFLEX_DIR = os.path.expandvars("$HOME/.reflex")
-
-# Bun config.
-# The Bun version.
-BUN_VERSION = "0.7.0"
-# The directory to store the bun.
-BUN_ROOT_PATH = f"{REFLEX_DIR}/.bun"
-# The bun path.
-BUN_PATH = f"{BUN_ROOT_PATH}/bin/bun"
-# Command to install bun.
-INSTALL_BUN = f"curl -fsSL https://bun.sh/install | env BUN_INSTALL={BUN_ROOT_PATH} bash -s -- bun-v{BUN_VERSION}"
-
-# NVM / Node config.
-# The Node version.
-NODE_VERSION = "18.17.0"
-# The directory to store nvm.
-NVM_ROOT_PATH = f"{REFLEX_DIR}/.nvm"
-# The nvm path.
-NVM_PATH = f"{NVM_ROOT_PATH}/nvm.sh"
-# The node bin path.
-NODE_BIN_PATH = f"{NVM_ROOT_PATH}/versions/node/v{NODE_VERSION}/bin"
-# The default path where node is installed.
-NODE_PATH = "node" if platform.system() == "Windows" else f"{NODE_BIN_PATH}/node"
-# The default path where npm is installed.
-NPM_PATH = "npm" if platform.system() == "Windows" else f"{NODE_BIN_PATH}/npm"
-# Command to install nvm.
-INSTALL_NVM = f"curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | env NVM_DIR={NVM_ROOT_PATH} bash"
-# Command to install node.
-INSTALL_NODE = f"bash -c \". {NVM_ROOT_PATH}/nvm.sh && nvm install {NODE_VERSION}\""
-
+# Valid bun versions.
+MIN_BUN_VERSION = "0.5.9"
+MAX_BUN_VERSION = "0.6.9"
 
 # Files and directories used to init a new project.
 # The root directory of the reflex library.
 ROOT_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 # The name of the assets directory.
 APP_ASSETS_DIR = "assets"
 # The template directory used during reflex init.
@@ -134,14 +106,20 @@
 FRONTEND_PORT = get_value("FRONTEND_PORT", "3000")
 # The backend default port.
 BACKEND_PORT = get_value("BACKEND_PORT", "8000")
 # The backend api url.
 API_URL = get_value("API_URL", "http://localhost:8000")
 # The deploy url
 DEPLOY_URL = get_value("DEPLOY_URL")
+# bun root location
+BUN_ROOT_PATH = "$HOME/.bun"
+# The default path where bun is installed.
+BUN_PATH = get_value("BUN_PATH", f"{BUN_ROOT_PATH}/bin/bun")
+# Command to install bun.
+INSTALL_BUN = f"curl -fsSL https://bun.sh/install | bash -s -- bun-v{MAX_BUN_VERSION}"
 # Default host in dev mode.
 BACKEND_HOST = get_value("BACKEND_HOST", "0.0.0.0")
 # The default timeout when launching the gunicorn server.
 TIMEOUT = get_value("TIMEOUT", 120, type_=int)
 # The command to run the backend in production mode.
 RUN_BACKEND_PROD = f"gunicorn --worker-class uvicorn.workers.UvicornH11Worker --preload --timeout {TIMEOUT} --log-level critical".split()
 RUN_BACKEND_PROD_WINDOWS = f"uvicorn --timeout-keep-alive {TIMEOUT}".split()
```

### Comparing `reflex-0.2.3a6/reflex/el/constants/html.py` & `reflex-0.2.3a7/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/el/constants/react.py` & `reflex-0.2.3a7/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/el/constants/reflex.py` & `reflex-0.2.3a7/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/el/element.py` & `reflex-0.2.3a7/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/el/elements/__init__.py` & `reflex-0.2.3a7/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/el/precompile.py` & `reflex-0.2.3a7/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/event.py` & `reflex-0.2.3a7/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.3a7/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/middleware/middleware.py` & `reflex-0.2.3a7/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/model.py` & `reflex-0.2.3a7/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/reflex.py` & `reflex-0.2.3a7/reflex/reflex.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,36 +28,43 @@
 def init(
     name: str = typer.Option(None, help="Name of the app to be initialized."),
     template: constants.Template = typer.Option(
         constants.Template.DEFAULT, help="Template to use for the app."
     ),
 ):
     """Initialize a new Reflex app in the current directory."""
-    # Get the app name.
     app_name = prerequisites.get_default_app_name() if name is None else name
-    console.rule(f"[bold]Initializing {app_name}")
 
-    # Set up the web project.
-    prerequisites.initialize_frontend_dependencies()
+    # Make sure they don't name the app "reflex".
+    if app_name == constants.MODULE_NAME:
+        console.print(
+            f"[red]The app directory cannot be named [bold]{constants.MODULE_NAME}."
+        )
+        raise typer.Exit()
+
+    console.rule(f"[bold]Initializing {app_name}")
+    # Set up the web directory.
+    prerequisites.validate_and_install_bun()
+    prerequisites.initialize_web_directory()
 
     # Migrate Pynecone projects to Reflex.
     prerequisites.migrate_to_reflex()
 
     # Set up the app directory, only if the config doesn't exist.
     if not os.path.exists(constants.CONFIG_FILE):
         prerequisites.create_config(app_name)
         prerequisites.initialize_app_directory(app_name, template)
         build.set_reflex_project_hash()
         telemetry.send("init", get_config().telemetry_enabled)
     else:
+        build.set_reflex_project_hash()
         telemetry.send("reinit", get_config().telemetry_enabled)
 
     # Initialize the .gitignore.
     prerequisites.initialize_gitignore()
-
     # Finish initializing the app.
     console.log(f"[bold green]Finished Initializing: {app_name}")
 
 
 @cli.command()
 def run(
     env: constants.Env = typer.Option(
@@ -73,15 +80,15 @@
     frontend_port: str = typer.Option(None, help="Specify a different frontend port."),
     backend_port: str = typer.Option(None, help="Specify a different backend port."),
     backend_host: str = typer.Option(None, help="Specify the backend host."),
 ):
     """Run the app in the current directory."""
     if platform.system() == "Windows":
         console.print(
-            "[yellow][WARNING] We strongly advise using Windows Subsystem for Linux (WSL) for optimal performance with reflex."
+            "[yellow][WARNING] We strongly advise you to use Windows Subsystem for Linux (WSL) for optimal performance when using Reflex. Due to compatibility issues with one of our dependencies, Bun, you may experience slower performance on Windows. By using WSL, you can expect to see a significant speed increase."
         )
     # Set ports as os env variables to take precedence over config and
     # .env variables(if override_os_envs flag in config is set to False).
     build.set_os_env(
         frontend_port=frontend_port,
         backend_port=backend_port,
         backend_host=backend_host,
```

### Comparing `reflex-0.2.3a6/reflex/route.py` & `reflex-0.2.3a7/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/state.py` & `reflex-0.2.3a7/reflex/state.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,14 +591,18 @@
 
         if types.is_backend_variable(name) and name != "_backend_vars":
             self._backend_vars.__setitem__(name, value)
             self.dirty_vars.add(name)
             self.mark_dirty()
             return
 
+        # Make sure lists and dicts are converted to ReflexList and ReflexDict.
+        if name in self.vars and types._isinstance(value, Union[List, Dict]):
+            value = _convert_mutable_datatypes(value, self._reassign_field, name)
+
         # Set the attribute.
         super().__setattr__(name, value)
 
         # Add the var to the dirty list.
         if name in self.vars or name in self.computed_var_dependencies:
             self.dirty_vars.add(name)
             self.mark_dirty()
@@ -986,25 +990,26 @@
             The function to reassign the field in the parent state.
         field_name: the name of the field in the parent state
 
     Returns:
         The converted field_value
     """
     if isinstance(field_value, list):
-        for index in range(len(field_value)):
-            field_value[index] = _convert_mutable_datatypes(
-                field_value[index], reassign_field, field_name
-            )
+        field_value = [
+            _convert_mutable_datatypes(value, reassign_field, field_name)
+            for value in field_value
+        ]
 
         field_value = ReflexList(
             field_value, reassign_field=reassign_field, field_name=field_name
         )
 
     if isinstance(field_value, dict):
-        for key, value in field_value.items():
-            field_value[key] = _convert_mutable_datatypes(
-                value, reassign_field, field_name
-            )
+        field_value = {
+            key: _convert_mutable_datatypes(value, reassign_field, field_name)
+            for key, value in field_value.items()
+        }
         field_value = ReflexDict(
             field_value, reassign_field=reassign_field, field_name=field_name
         )
+
     return field_value
```

### Comparing `reflex-0.2.3a6/reflex/style.py` & `reflex-0.2.3a7/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/testing.py` & `reflex-0.2.3a7/reflex/testing.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/utils/build.py` & `reflex-0.2.3a7/reflex/utils/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
     # Add a single task to the progress object
     task = progress.add_task("Creating Production Build: ", total=len(checkpoints))
 
     # Start the subprocess with the progress bar.
     try:
         with progress, new_process(
-            [constants.NPM_PATH, "run", command],
+            [prerequisites.get_package_manager(), "run", command],
             cwd=constants.WEB_DIR,
         ) as export_process:
             assert export_process.stdout is not None, "No stdout for export process."
             for line in export_process.stdout:
                 if loglevel == constants.LogLevel.DEBUG:
                     print(line, end="")
 
@@ -202,38 +202,44 @@
 
 
 def setup_frontend(
     root: Path,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
     disable_telemetry: bool = True,
 ):
-    """Set up the frontend to run the app.
+    """Set up the frontend.
 
     Args:
         root: The root path of the project.
         loglevel: The log level to use.
         disable_telemetry: Whether to disable the Next telemetry.
     """
+    # Validate bun version.
+    prerequisites.validate_and_install_bun(initialize=False)
+
+    # Initialize the web directory if it doesn't exist.
+    web_dir = prerequisites.create_web_directory(root)
+
     # Install frontend packages.
-    prerequisites.install_frontend_packages()
+    prerequisites.install_frontend_packages(web_dir)
 
     # Copy asset files to public folder.
     path_ops.cp(
         src=str(root / constants.APP_ASSETS_DIR),
         dest=str(root / constants.WEB_ASSETS_DIR),
     )
 
-    # Set the environment variables in client (env.json).
+    # set the environment variables in client(env.json)
     set_environment_variables()
 
     # Disable the Next telemetry.
     if disable_telemetry:
         new_process(
             [
-                "npm",
+                prerequisites.get_package_manager(),
                 "run",
                 "next",
                 "telemetry",
                 "disable",
             ],
             cwd=constants.WEB_DIR,
             stdout=subprocess.DEVNULL,
```

### Comparing `reflex-0.2.3a6/reflex/utils/console.py` & `reflex-0.2.3a7/reflex/utils/console.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/utils/exec.py` & `reflex-0.2.3a7/reflex/utils/exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import subprocess
 from pathlib import Path
 
 from rich import print
 
 from reflex import constants
 from reflex.config import get_config
-from reflex.utils import console, processes
+from reflex.utils import console, prerequisites, processes
 from reflex.utils.processes import new_process
 from reflex.utils.watch import AssetFolderWatch
 
 
 def start_watching_assets_folder(root):
     """Start watching assets folder.
 
@@ -64,15 +64,17 @@
     """
     # Start watching asset folder.
     start_watching_assets_folder(root)
 
     # Run the frontend in development mode.
     console.rule("[bold green]App Running")
     os.environ["PORT"] = get_config().frontend_port if port is None else port
-    run_process_and_launch_url([constants.NPM_PATH, "run", "dev"], loglevel)
+    run_process_and_launch_url(
+        [prerequisites.get_package_manager(), "run", "dev"], loglevel
+    )
 
 
 def run_frontend_prod(
     root: Path,
     port: str,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
@@ -84,15 +86,17 @@
         loglevel: The log level to use.
     """
     # Set the port.
     os.environ["PORT"] = get_config().frontend_port if port is None else port
 
     # Run the frontend in production mode.
     console.rule("[bold green]App Running")
-    run_process_and_launch_url([constants.NPM_PATH, "run", "prod"], loglevel)
+    run_process_and_launch_url(
+        [prerequisites.get_package_manager(), "run", "prod"], loglevel
+    )
 
 
 def run_backend(
     app_name: str,
     host: str,
     port: int,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
@@ -114,15 +118,20 @@
         str(port),
         "--log-level",
         loglevel,
         "--reload",
         "--reload-dir",
         app_name.split(".")[0],
     ]
-    subprocess.run(cmd)
+    process = subprocess.Popen(cmd)
+
+    try:
+        process.wait()
+    except KeyboardInterrupt:
+        process.terminate()
 
 
 def run_backend_prod(
     app_name: str,
     host: str,
     port: int,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
```

### Comparing `reflex-0.2.3a6/reflex/utils/format.py` & `reflex-0.2.3a7/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/utils/imports.py` & `reflex-0.2.3a7/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/utils/path_ops.py` & `reflex-0.2.3a7/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/utils/prerequisites.py` & `reflex-0.2.3a7/reflex/utils/prerequisites.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,45 +21,46 @@
 from redis import Redis
 
 from reflex import constants, model
 from reflex.config import get_config
 from reflex.utils import console, path_ops
 
 
-def check_node_version():
+def check_node_version(min_version=constants.MIN_NODE_VERSION):
     """Check the version of Node.js.
 
+    Args:
+        min_version: The minimum version of Node.js required.
+
     Returns:
-        Whether the version of Node.js is valid.
+        Whether the version of Node.js is high enough.
     """
     try:
         # Run the node -v command and capture the output
         result = subprocess.run(
-            [constants.NODE_PATH, "-v"],
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
+            ["node", "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
         # The output will be in the form "vX.Y.Z", but version.parse() can handle it
         current_version = version.parse(result.stdout.decode())
         # Compare the version numbers
-        return current_version == version.parse(constants.NODE_VERSION)
+        return current_version >= version.parse(min_version)
     except Exception:
         return False
 
 
 def get_bun_version() -> Optional[version.Version]:
     """Get the version of bun.
 
     Returns:
         The version of bun.
     """
     try:
         # Run the bun -v command and capture the output
         result = subprocess.run(
-            [constants.BUN_PATH, "-v"],
+            [os.path.expandvars(get_config().bun_path), "-v"],
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         return version.parse(result.stdout.decode().strip())
     except Exception:
         return None
 
@@ -68,26 +69,35 @@
     """Get the package manager executable.
 
     Returns:
         The path to the package manager.
 
     Raises:
         FileNotFoundError: If bun or npm is not installed.
+        Exit: If the app directory is invalid.
+
     """
-    get_config()
+    config = get_config()
+
+    # Check that the node version is valid.
+    if not check_node_version():
+        console.print(
+            f"[red]Node.js version {constants.MIN_NODE_VERSION} or higher is required to run Reflex."
+        )
+        raise typer.Exit()
 
     # On Windows, we use npm instead of bun.
-    if platform.system() == "Windows":
+    if platform.system() == "Windows" or config.disable_bun:
         npm_path = path_ops.which("npm")
         if npm_path is None:
             raise FileNotFoundError("Reflex requires npm to be installed on Windows.")
         return npm_path
 
     # On other platforms, we use bun.
-    return constants.BUN_PATH
+    return os.path.expandvars(get_config().bun_path)
 
 
 def get_app() -> ModuleType:
     """Get the app module based on the default config.
 
     Returns:
         The app based on the default config.
@@ -129,24 +139,15 @@
     """Get the default app name.
 
     The default app name is the name of the current directory.
 
     Returns:
         The default app name.
     """
-    app_name = os.getcwd().split(os.path.sep)[-1].replace("-", "_")
-
-    # Make sure the app is not named "reflex".
-    if app_name == constants.MODULE_NAME:
-        console.print(
-            f"[red]The app directory cannot be named [bold]{constants.MODULE_NAME}."
-        )
-        raise typer.Exit()
-
-    return app_name
+    return os.getcwd().split(os.path.sep)[-1].replace("-", "_")
 
 
 def create_config(app_name: str):
     """Create a new rxconfig file.
 
     Args:
         app_name: The name of the app.
@@ -155,14 +156,29 @@
     from reflex.compiler import templates
 
     config_name = f"{re.sub(r'[^a-zA-Z]', '', app_name).capitalize()}Config"
     with open(constants.CONFIG_FILE, "w") as f:
         f.write(templates.RXCONFIG.render(app_name=app_name, config_name=config_name))
 
 
+def create_web_directory(root: Path) -> str:
+    """Creates a web directory in the given root directory
+    and returns the path to the directory.
+
+    Args:
+        root (Path): The root directory of the project.
+
+    Returns:
+        The path to the web directory.
+    """
+    web_dir = str(root / constants.WEB_DIR)
+    path_ops.cp(constants.WEB_TEMPLATE_DIR, web_dir, overwrite=False)
+    return web_dir
+
+
 def initialize_gitignore():
     """Initialize the template .gitignore file."""
     # The files to add to the .gitignore file.
     files = constants.DEFAULT_GITIGNORE
 
     # Subtract current ignored files.
     if os.path.exists(constants.GITIGNORE_FILE):
@@ -212,77 +228,56 @@
 
     # Write the current version of distributed reflex package to a REFLEX_JSON."""
     with open(constants.REFLEX_JSON, "w") as f:
         reflex_json = {"version": constants.VERSION}
         json.dump(reflex_json, f, ensure_ascii=False)
 
 
-def initialize_bun():
-    """Check that bun requirements are met, and install if not.
+def validate_and_install_bun(initialize=True):
+    """Check that bun version requirements are met. If they are not,
+    ask user whether to install required version.
+
+    Args:
+        initialize: whether this function is called on `reflex init` or `reflex run`.
 
     Raises:
         Exit: If the bun version is not supported.
 
     """
-    if platform.system == "Windows":
-        # Bun is not supported on Windows.
-        return
-
-    # Check the bun version.
-    if get_bun_version() != version.parse(constants.BUN_VERSION):
-        remove_existing_bun_installation()
-        install_bun()
-
-
-def remove_existing_bun_installation():
-    """Remove existing bun installation."""
-    if os.path.exists(constants.BUN_PATH):
-        path_ops.rm(constants.BUN_ROOT_PATH)
-
-
-def initialize_node():
-    """Validate nodejs have install or not."""
-    if not check_node_version():
-        install_node()
-
-
-def install_node():
-    """Install nvm and nodejs onto the user's system.
-
-
-    Raises:
-        FileNotFoundError: if unzip or curl packages are not found.
-        Exit: if installation failed
-    """
-    if platform.system() == "Windows":
+    bun_version = get_bun_version()
+    if bun_version is not None and (
+        bun_version < version.parse(constants.MIN_BUN_VERSION)
+        or bun_version > version.parse(constants.MAX_BUN_VERSION)
+    ):
         console.print(
-            f"[red]Node.js version {constants.NODE_VERSION} or higher is required to run Reflex."
+            f"""[red]Bun version {bun_version} is not supported by Reflex. Please change your to bun version to be between {constants.MIN_BUN_VERSION} and {constants.MAX_BUN_VERSION}."""
+        )
+        action = console.ask(
+            "Enter 'yes' to install the latest supported bun version or 'no' to exit.",
+            choices=["yes", "no"],
+            default="no",
         )
-        raise typer.Exit()
-
-    # Only install if bun is not already installed.
-    console.log("Installing nvm...")
-
-    # Check if curl is installed
-    curl_path = path_ops.which("curl")
-    if curl_path is None:
-        raise FileNotFoundError("Reflex requires curl to be installed.")
 
-    # Create the nvm directory and install.
-    path_ops.mkdir(constants.NVM_ROOT_PATH)
-    result = subprocess.run(constants.INSTALL_NVM, shell=True)
+        if action == "yes":
+            remove_existing_bun_installation()
+            install_bun()
+            return
+        else:
+            raise typer.Exit()
 
-    if result.returncode != 0:
-        raise typer.Exit(code=result.returncode)
+    if initialize:
+        install_bun()
 
-    console.log("Installing node...")
-    result = subprocess.run(constants.INSTALL_NODE, shell=True)
 
-    if result.returncode != 0:
-        raise typer.Exit(code=result.returncode)
+def remove_existing_bun_installation():
+    """Remove existing bun installation."""
+    package_manager = get_package_manager()
+    if os.path.exists(package_manager):
+        console.log("Removing bun...")
+        path_ops.rm(os.path.expandvars(constants.BUN_ROOT_PATH))
 
 
 def install_bun():
     """Install bun onto the user's system.
 
     Raises:
         FileNotFoundError: if unzip or curl packages are not found.
@@ -290,15 +285,15 @@
     """
     # Bun is not supported on Windows.
     if platform.system() == "Windows":
         console.log("Skipping bun installation on Windows.")
         return
 
     # Only install if bun is not already installed.
-    if not os.path.exists(constants.BUN_PATH):
+    if not os.path.exists(get_package_manager()):
         console.log("Installing bun...")
 
         # Check if curl is installed
         curl_path = path_ops.which("curl")
         if curl_path is None:
             raise FileNotFoundError("Reflex requires curl to be installed.")
 
@@ -309,32 +304,37 @@
 
         result = subprocess.run(constants.INSTALL_BUN, shell=True)
 
         if result.returncode != 0:
             raise typer.Exit(code=result.returncode)
 
 
-def install_frontend_packages():
-    """Installs the base and custom frontend packages."""
+def install_frontend_packages(web_dir: str):
+    """Installs the base and custom frontend packages
+    into the given web directory.
+
+    Args:
+        web_dir: The directory where the frontend code is located.
+    """
     # Install the frontend packages.
     console.rule("[bold]Installing frontend packages")
 
     # Install the base packages.
     subprocess.run(
         [get_package_manager(), "install"],
-        cwd=constants.WEB_DIR,
+        cwd=web_dir,
         stdout=subprocess.PIPE,
     )
 
     # Install the app packages.
     packages = get_config().frontend_packages
     if len(packages) > 0:
         subprocess.run(
             [get_package_manager(), "add", *packages],
-            cwd=constants.WEB_DIR,
+            cwd=web_dir,
             stdout=subprocess.PIPE,
         )
 
 
 def is_initialized() -> bool:
     """Check whether the app is initialized.
 
@@ -353,27 +353,14 @@
     if not os.path.exists(constants.REFLEX_JSON):
         return False
     with open(constants.REFLEX_JSON) as f:  # type: ignore
         app_version = json.load(f)["version"]
     return app_version == constants.VERSION
 
 
-def initialize_frontend_dependencies():
-    """Initialize all the frontend dependencies."""
-    # Create the reflex directory.
-    path_ops.mkdir(constants.REFLEX_DIR)
-
-    # Install the frontend dependencies.
-    initialize_bun()
-    initialize_node()
-
-    # Set up the web directory.
-    initialize_web_directory()
-
-
 def check_admin_settings():
     """Check if admin settings are set and valid for logging in cli app."""
     admin_dash = get_config().admin_dash
     current_time = datetime.now()
     if admin_dash:
         if not admin_dash.models:
             console.print(
```

### Comparing `reflex-0.2.3a6/reflex/utils/processes.py` & `reflex-0.2.3a7/reflex/utils/processes.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,18 +130,16 @@
     Args:
         args: A string, or a sequence of program arguments.
         **kwargs: Kwargs to override default wrap values to pass to subprocess.Popen as arguments.
 
     Returns:
         Execute a child program in a new process.
     """
-    env = os.environ.copy()
-    env["PATH"] = os.pathsep.join([constants.NODE_BIN_PATH, env["PATH"]])
     kwargs = {
-        "env": env,
+        "env": os.environ,
         "stderr": subprocess.STDOUT,
         "stdout": subprocess.PIPE,  # Redirect stdout to a pipe
         "universal_newlines": True,  # Set universal_newlines to True for text mode
         "encoding": "UTF-8",
         **kwargs,
     }
     return subprocess.Popen(
```

### Comparing `reflex-0.2.3a6/reflex/utils/telemetry.py` & `reflex-0.2.3a7/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/utils/types.py` & `reflex-0.2.3a7/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/utils/watch.py` & `reflex-0.2.3a7/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/reflex/vars.py` & `reflex-0.2.3a7/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a6/PKG-INFO` & `reflex-0.2.3a7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.3a6
+Version: 0.2.3a7
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

