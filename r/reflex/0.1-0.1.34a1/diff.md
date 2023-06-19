# Comparing `tmp/reflex-0.1.tar.gz` & `tmp/reflex-0.1.34a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.1.tar", last modified: Mon Dec 26 00:43:52 2005, max compression, from Unix
+gzip compressed data, was "reflex-0.1.34a1.tar", max compression
```

## Comparing `reflex-0.1.tar` & `reflex-0.1.34a1.tar`

### file list

```diff
@@ -1,9 +1,175 @@
-drwxr-xr-x   0 talin      (501) staff       (20)        0 2005-12-26 00:43:52.000000 reflex-0.1/
--rw-r--r--   0 talin      (501) staff       (20)     4680 2005-12-26 00:43:52.000000 reflex-0.1/PKG-INFO
--r--------   0 talin      (501) wheel        (0)       82 2005-12-26 00:20:53.000000 reflex-0.1/._reflex.py
--rw-r--r--   0 talin      (501) staff       (20)     9723 2005-12-26 00:20:53.000000 reflex-0.1/reflex.py
--r--------   0 talin      (501) wheel        (0)       82 2005-12-26 00:41:29.000000 reflex-0.1/._setup.py
--rw-r--r--   0 talin      (501) staff       (20)     1153 2005-12-26 00:41:29.000000 reflex-0.1/setup.py
-drwxr-xr-x   0 talin      (501) staff       (20)        0 2005-12-26 00:43:52.000000 reflex-0.1/test/
--r--------   0 talin      (501) wheel        (0)       82 2005-12-26 00:07:11.000000 reflex-0.1/test/._test_reflex.py
--rw-r--r--   0 talin      (501) staff       (20)     2455 2005-12-26 00:07:11.000000 reflex-0.1/test/test_reflex.py
+-rw-r--r--   0        0        0    11354 2023-06-19 22:34:24.681273 reflex-0.1.34a1/LICENSE
+-rw-r--r--   0        0        0     7932 2023-06-19 22:36:51.179169 reflex-0.1.34a1/README.md
+-rw-r--r--   0        0        0     1859 2023-06-19 22:47:24.392655 reflex-0.1.34a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-19 22:33:46.770141 reflex-0.1.34a1/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1336 2023-06-19 22:35:59.095973 reflex-0.1.34a1/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:33:46.770260 reflex-0.1.34a1/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1225 2023-06-19 22:35:59.096017 reflex-0.1.34a1/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-06-19 22:33:46.770420 reflex-0.1.34a1/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      181 2023-06-19 22:35:59.096045 reflex-0.1.34a1/reflex/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-06-19 22:33:46.770667 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-06-19 22:33:46.770722 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-06-19 22:33:46.770774 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-06-19 22:33:46.770836 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-06-19 22:33:46.770901 reflex-0.1.34a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-06-19 22:33:46.770962 reflex-0.1.34a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-06-19 22:33:46.771043 reflex-0.1.34a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-06-19 22:33:46.771125 reflex-0.1.34a1/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-06-19 22:33:46.771903 reflex-0.1.34a1/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-06-19 22:33:46.771990 reflex-0.1.34a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2023-06-19 22:33:46.772046 reflex-0.1.34a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1141 2023-06-19 22:35:59.096002 reflex-0.1.34a1/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-06-19 22:33:46.772194 reflex-0.1.34a1/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-06-19 22:33:46.772250 reflex-0.1.34a1/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-06-19 22:33:46.772306 reflex-0.1.34a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-06-19 22:33:46.772513 reflex-0.1.34a1/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-06-19 22:33:46.772579 reflex-0.1.34a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     8836 2023-06-19 22:34:24.888565 reflex-0.1.34a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1634 2023-06-19 22:34:24.831036 reflex-0.1.34a1/reflex/__init__.py
+-rw-r--r--   0        0        0      318 2023-06-19 22:34:24.699927 reflex-0.1.34a1/reflex/admin.py
+-rw-r--r--   0        0        0    21877 2023-06-19 22:35:59.095850 reflex-0.1.34a1/reflex/app.py
+-rw-r--r--   0        0        0     2544 2023-06-19 22:34:24.719267 reflex-0.1.34a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-06-19 22:34:24.870104 reflex-0.1.34a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     7317 2023-06-19 22:35:59.095958 reflex-0.1.34a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-06-19 22:35:59.095943 reflex-0.1.34a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     7751 2023-06-19 22:35:59.095988 reflex-0.1.34a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7471 2023-06-19 22:33:46.773466 reflex-0.1.34a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-19 22:33:46.773564 reflex-0.1.34a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-06-19 22:35:59.096413 reflex-0.1.34a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-06-19 22:35:59.096444 reflex-0.1.34a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0      721 2023-06-19 22:35:59.096461 reflex-0.1.34a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-06-19 22:35:59.096397 reflex-0.1.34a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-06-19 22:35:59.096774 reflex-0.1.34a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-06-19 22:35:59.096367 reflex-0.1.34a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0    24223 2023-06-19 22:35:59.096035 reflex-0.1.34a1/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-06-19 22:33:46.775571 reflex-0.1.34a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-06-19 22:35:59.096735 reflex-0.1.34a1/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2503 2023-06-19 22:35:59.096726 reflex-0.1.34a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4025 2023-06-19 22:35:59.096802 reflex-0.1.34a1/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-06-19 22:35:59.096963 reflex-0.1.34a1/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-06-19 22:35:59.097170 reflex-0.1.34a1/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-06-19 22:35:59.096789 reflex-0.1.34a1/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-06-19 22:35:59.096813 reflex-0.1.34a1/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5785 2023-06-19 22:35:59.096689 reflex-0.1.34a1/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-06-19 22:35:59.096714 reflex-0.1.34a1/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-06-19 22:33:46.776227 reflex-0.1.34a1/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-06-19 22:35:59.097561 reflex-0.1.34a1/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-06-19 22:35:59.097606 reflex-0.1.34a1/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-06-19 22:35:59.097594 reflex-0.1.34a1/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-06-19 22:35:59.097898 reflex-0.1.34a1/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-06-19 22:33:46.776580 reflex-0.1.34a1/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1565 2023-06-19 22:35:59.096900 reflex-0.1.34a1/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-06-19 22:35:59.096909 reflex-0.1.34a1/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-06-19 22:35:59.096826 reflex-0.1.34a1/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-06-19 22:35:59.096882 reflex-0.1.34a1/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-06-19 22:35:59.096860 reflex-0.1.34a1/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1471 2023-06-19 22:33:46.776951 reflex-0.1.34a1/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-06-19 22:35:59.097156 reflex-0.1.34a1/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-06-19 22:35:59.096923 reflex-0.1.34a1/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-06-19 22:35:59.097250 reflex-0.1.34a1/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-06-19 22:35:59.097214 reflex-0.1.34a1/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-06-19 22:35:59.097099 reflex-0.1.34a1/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-06-19 22:35:59.097488 reflex-0.1.34a1/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1943 2023-06-19 22:35:59.097191 reflex-0.1.34a1/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-06-19 22:35:59.097108 reflex-0.1.34a1/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-06-19 22:35:59.097052 reflex-0.1.34a1/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-06-19 22:35:59.097201 reflex-0.1.34a1/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2872 2023-06-19 22:35:59.097131 reflex-0.1.34a1/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-06-19 22:35:59.097088 reflex-0.1.34a1/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-06-19 22:35:59.097001 reflex-0.1.34a1/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-06-19 22:35:59.097391 reflex-0.1.34a1/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-06-19 22:35:59.097118 reflex-0.1.34a1/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-06-19 22:35:59.097238 reflex-0.1.34a1/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-06-19 22:35:59.097071 reflex-0.1.34a1/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-06-19 22:35:59.097295 reflex-0.1.34a1/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-06-19 22:35:59.097039 reflex-0.1.34a1/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-06-19 22:35:59.097182 reflex-0.1.34a1/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     1526 2023-06-19 22:35:59.097226 reflex-0.1.34a1/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-06-19 22:35:59.097145 reflex-0.1.34a1/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-06-19 22:33:46.778441 reflex-0.1.34a1/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1351 2023-06-19 22:35:59.096527 reflex-0.1.34a1/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-06-19 22:35:59.097946 reflex-0.1.34a1/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-06-19 22:33:46.778696 reflex-0.1.34a1/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-19 22:35:59.097415 reflex-0.1.34a1/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-06-19 22:35:59.097509 reflex-0.1.34a1/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-06-19 22:35:59.097305 reflex-0.1.34a1/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-06-19 22:35:59.097347 reflex-0.1.34a1/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-06-19 22:35:59.097704 reflex-0.1.34a1/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-06-19 22:35:59.097321 reflex-0.1.34a1/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-06-19 22:35:59.097277 reflex-0.1.34a1/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-06-19 22:35:59.097333 reflex-0.1.34a1/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-06-19 22:35:59.097526 reflex-0.1.34a1/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-06-19 22:35:59.097545 reflex-0.1.34a1/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-06-19 22:35:59.097451 reflex-0.1.34a1/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-06-19 22:35:59.097261 reflex-0.1.34a1/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-06-19 22:35:59.097576 reflex-0.1.34a1/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-06-19 22:35:59.097437 reflex-0.1.34a1/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-06-19 22:35:59.097268 reflex-0.1.34a1/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-06-19 22:33:46.779636 reflex-0.1.34a1/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-06-19 22:35:59.096477 reflex-0.1.34a1/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1385 2023-06-19 22:35:59.096490 reflex-0.1.34a1/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-19 22:33:46.779841 reflex-0.1.34a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-06-19 22:35:59.096067 reflex-0.1.34a1/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-06-19 22:35:59.096077 reflex-0.1.34a1/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-06-19 22:35:59.096429 reflex-0.1.34a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2053 2023-06-19 22:35:59.096054 reflex-0.1.34a1/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-06-19 22:35:59.096061 reflex-0.1.34a1/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-06-19 22:33:46.780197 reflex-0.1.34a1/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2017 2023-06-19 22:35:59.096547 reflex-0.1.34a1/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1606 2023-06-19 22:35:59.096600 reflex-0.1.34a1/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-06-19 22:35:59.096566 reflex-0.1.34a1/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-06-19 22:35:59.096616 reflex-0.1.34a1/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-06-19 22:35:59.096580 reflex-0.1.34a1/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-06-19 22:33:46.780630 reflex-0.1.34a1/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-06-19 22:35:59.096337 reflex-0.1.34a1/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-06-19 22:35:59.096326 reflex-0.1.34a1/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-06-19 22:35:59.096353 reflex-0.1.34a1/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-06-19 22:35:59.096282 reflex-0.1.34a1/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-06-19 22:35:59.096302 reflex-0.1.34a1/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-06-19 22:35:59.096382 reflex-0.1.34a1/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-06-19 22:35:59.096313 reflex-0.1.34a1/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-06-19 22:33:46.781218 reflex-0.1.34a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-06-19 22:35:59.096675 reflex-0.1.34a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2294 2023-06-19 22:35:59.096659 reflex-0.1.34a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5008 2023-06-19 22:35:59.096643 reflex-0.1.34a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-06-19 22:35:59.096705 reflex-0.1.34a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-06-19 22:35:59.096266 reflex-0.1.34a1/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-19 22:35:59.096084 reflex-0.1.34a1/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-06-19 22:35:59.096228 reflex-0.1.34a1/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     3454 2023-06-19 22:35:59.096099 reflex-0.1.34a1/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-06-19 22:35:59.096238 reflex-0.1.34a1/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-06-19 22:35:59.096249 reflex-0.1.34a1/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7120 2023-06-19 22:35:59.095927 reflex-0.1.34a1/reflex/config.py
+-rw-r--r--   0        0        0    10382 2023-06-19 22:36:51.202098 reflex-0.1.34a1/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-06-19 22:33:46.782066 reflex-0.1.34a1/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-06-19 22:35:59.097790 reflex-0.1.34a1/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-06-19 22:33:46.782213 reflex-0.1.34a1/reflex/el/constants/html.py
+-rw-r--r--   0        0        0     1701 2023-06-19 22:35:59.097774 reflex-0.1.34a1/reflex/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-06-19 22:33:46.782376 reflex-0.1.34a1/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1318 2023-06-19 22:35:59.097806 reflex-0.1.34a1/reflex/el/element.py
+-rw-r--r--   0        0        0   108514 2023-06-19 22:35:59.097834 reflex-0.1.34a1/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2657 2023-06-19 22:35:59.097738 reflex-0.1.34a1/reflex/el/precompile.py
+-rw-r--r--   0        0        0    11866 2023-06-19 22:35:59.095898 reflex-0.1.34a1/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-06-19 22:34:24.888652 reflex-0.1.34a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-06-19 22:35:59.097851 reflex-0.1.34a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-06-19 22:35:59.097863 reflex-0.1.34a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     2382 2023-06-19 22:35:59.095833 reflex-0.1.34a1/reflex/model.py
+-rw-r--r--   0        0        0        0 2023-06-19 22:33:46.783154 reflex-0.1.34a1/reflex/py.typed
+-rw-r--r--   0        0        0     4104 2023-06-19 22:35:59.095862 reflex-0.1.34a1/reflex/route.py
+-rw-r--r--   0        0        0     8549 2023-06-19 22:36:51.179201 reflex-0.1.34a1/reflex/rx.py
+-rw-r--r--   0        0        0    30933 2023-06-19 22:35:59.095822 reflex-0.1.34a1/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-06-19 22:35:59.095871 reflex-0.1.34a1/reflex/style.py
+-rw-r--r--   0        0        0       24 2023-06-19 22:34:24.870062 reflex-0.1.34a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     7378 2023-06-19 22:35:59.097756 reflex-0.1.34a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-06-19 22:33:46.783773 reflex-0.1.34a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     5305 2023-06-19 22:35:59.098892 reflex-0.1.34a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0    11845 2023-06-19 22:35:59.097652 reflex-0.1.34a1/reflex/utils/format.py
+-rw-r--r--   0        0        0      585 2023-06-19 22:35:59.097721 reflex-0.1.34a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-06-19 22:33:46.784040 reflex-0.1.34a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    10881 2023-06-19 22:36:51.202382 reflex-0.1.34a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     3015 2023-06-19 22:35:59.097617 reflex-0.1.34a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2369 2023-06-19 22:35:59.097638 reflex-0.1.34a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-06-19 22:35:59.097667 reflex-0.1.34a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-06-19 22:35:59.097626 reflex-0.1.34a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    30916 2023-06-19 22:35:59.095790 reflex-0.1.34a1/reflex/vars.py
+-rw-r--r--   0        0        0     9559 1970-01-01 00:00:00.000000 reflex-0.1.34a1/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

