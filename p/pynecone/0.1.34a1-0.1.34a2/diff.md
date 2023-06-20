# Comparing `tmp/pynecone-0.1.34a1.tar.gz` & `tmp/pynecone-0.1.34a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.34a1.tar", max compression
+gzip compressed data, was "pynecone-0.1.34a2.tar", max compression
```

## Comparing `pynecone-0.1.34a1.tar` & `pynecone-0.1.34a2.tar`

### file list

```diff
@@ -1,175 +1,175 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.34a1/LICENSE
--rw-r--r--   0        0        0     7985 2023-06-19 21:09:12.736508 pynecone-0.1.34a1/README.md
--rw-r--r--   0        0        0        0 2023-06-16 05:09:35.273793 pynecone-0.1.34a1/pynecone/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1340 2023-06-16 05:09:35.273930 pynecone-0.1.34a1/pynecone/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-06-16 05:09:35.274029 pynecone-0.1.34a1/pynecone/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1232 2023-06-16 05:09:35.274187 pynecone-0.1.34a1/pynecone/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-06-16 05:09:35.274347 pynecone-0.1.34a1/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      183 2023-06-16 05:09:35.274660 pynecone-0.1.34a1/pynecone/.templates/jinja/app/pcconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-06-16 05:09:35.274990 pynecone-0.1.34a1/pynecone/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-06-16 05:09:35.275137 pynecone-0.1.34a1/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-06-16 05:09:35.275226 pynecone-0.1.34a1/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-06-16 05:09:35.275478 pynecone-0.1.34a1/pynecone/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-06-16 05:09:35.275791 pynecone-0.1.34a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-06-19 21:09:12.736858 pynecone-0.1.34a1/pynecone/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-06-16 05:09:35.275938 pynecone-0.1.34a1/pynecone/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-06-16 05:09:35.276075 pynecone-0.1.34a1/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-06-19 21:09:12.738040 pynecone-0.1.34a1/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-06-16 05:09:35.277373 pynecone-0.1.34a1/pynecone/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       47 2023-06-16 05:09:35.277600 pynecone-0.1.34a1/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0     1143 2023-06-19 21:09:12.738227 pynecone-0.1.34a1/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-06-16 05:09:35.277911 pynecone-0.1.34a1/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-06-19 21:09:12.738431 pynecone-0.1.34a1/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-06-19 21:09:12.738679 pynecone-0.1.34a1/pynecone/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-06-16 05:09:35.278186 pynecone-0.1.34a1/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-06-19 21:09:12.738771 pynecone-0.1.34a1/pynecone/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0     8838 2023-06-17 20:30:12.955812 pynecone-0.1.34a1/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1636 2023-06-17 20:30:12.956097 pynecone-0.1.34a1/pynecone/__init__.py
--rw-r--r--   0        0        0      320 2023-06-16 05:09:35.278638 pynecone-0.1.34a1/pynecone/admin.py
--rw-r--r--   0        0        0    21913 2023-06-19 21:09:12.739037 pynecone-0.1.34a1/pynecone/app.py
--rw-r--r--   0        0        0     2548 2023-06-16 05:09:35.278940 pynecone-0.1.34a1/pynecone/base.py
--rw-r--r--   0        0        0       29 2023-06-16 05:09:35.279040 pynecone-0.1.34a1/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     7335 2023-06-19 21:09:12.739412 pynecone-0.1.34a1/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     2739 2023-06-19 21:09:12.739600 pynecone-0.1.34a1/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     7767 2023-06-16 05:09:35.279374 pynecone-0.1.34a1/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     7471 2023-06-16 05:09:35.279688 pynecone-0.1.34a1/pynecone/components/__init__.py
--rw-r--r--   0        0        0      229 2023-06-16 05:09:35.279922 pynecone-0.1.34a1/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      727 2023-06-16 05:09:35.279996 pynecone-0.1.34a1/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-06-16 05:09:35.280073 pynecone-0.1.34a1/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-06-16 05:09:35.280133 pynecone-0.1.34a1/pynecone/components/base/document.py
--rw-r--r--   0        0        0      265 2023-06-16 05:09:35.280191 pynecone-0.1.34a1/pynecone/components/base/head.py
--rw-r--r--   0        0        0      933 2023-06-16 05:09:35.280288 pynecone-0.1.34a1/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1412 2023-06-16 05:09:35.280378 pynecone-0.1.34a1/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    24243 2023-06-16 05:09:35.280545 pynecone-0.1.34a1/pynecone/components/component.py
--rw-r--r--   0        0        0      496 2023-06-16 05:09:35.280902 pynecone-0.1.34a1/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      334 2023-06-16 05:09:35.280992 pynecone-0.1.34a1/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2513 2023-06-16 05:09:35.281074 pynecone-0.1.34a1/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4033 2023-06-16 05:09:35.281150 pynecone-0.1.34a1/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      537 2023-06-16 05:09:35.281254 pynecone-0.1.34a1/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-06-16 05:09:35.281333 pynecone-0.1.34a1/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1430 2023-06-16 05:09:35.281415 pynecone-0.1.34a1/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2157 2023-06-16 05:09:35.281495 pynecone-0.1.34a1/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5793 2023-06-16 05:09:35.281620 pynecone-0.1.34a1/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0     2188 2023-06-16 05:09:35.281738 pynecone-0.1.34a1/pynecone/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-06-16 05:09:35.281995 pynecone-0.1.34a1/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3517 2023-06-16 05:09:35.282101 pynecone-0.1.34a1/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2777 2023-06-16 05:09:35.282180 pynecone-0.1.34a1/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1741 2023-06-16 05:09:35.282287 pynecone-0.1.34a1/pynecone/components/disclosure/transition.py
--rw-r--r--   0        0        0      285 2023-06-16 05:09:35.282356 pynecone-0.1.34a1/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-06-16 05:09:35.282647 pynecone-0.1.34a1/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1571 2023-06-16 05:09:35.282727 pynecone-0.1.34a1/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1905 2023-06-16 05:09:35.282811 pynecone-0.1.34a1/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      879 2023-06-16 05:09:35.282890 pynecone-0.1.34a1/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1785 2023-06-16 05:09:35.282969 pynecone-0.1.34a1/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      678 2023-06-16 05:09:35.283039 pynecone-0.1.34a1/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1471 2023-06-16 05:09:35.283322 pynecone-0.1.34a1/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1765 2023-06-16 05:09:35.283424 pynecone-0.1.34a1/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2454 2023-06-16 05:09:35.283533 pynecone-0.1.34a1/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0     3147 2023-06-16 05:09:35.283651 pynecone-0.1.34a1/pynecone/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      578 2023-06-16 05:09:35.283755 pynecone-0.1.34a1/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      243 2023-06-16 05:09:35.283847 pynecone-0.1.34a1/pynecone/components/forms/date_picker.py
--rw-r--r--   0        0        0      277 2023-06-16 05:09:35.283931 pynecone-0.1.34a1/pynecone/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     1949 2023-06-16 05:09:35.284031 pynecone-0.1.34a1/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0      243 2023-06-16 05:09:35.284144 pynecone-0.1.34a1/pynecone/components/forms/email.py
--rw-r--r--   0        0        0     2996 2023-06-16 05:09:35.284270 pynecone-0.1.34a1/pynecone/components/forms/form.py
--rw-r--r--   0        0        0      802 2023-06-16 05:09:35.284358 pynecone-0.1.34a1/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2880 2023-06-16 05:09:35.284448 pynecone-0.1.34a1/pynecone/components/forms/input.py
--rw-r--r--   0        0        0    12667 2023-06-16 05:09:35.284573 pynecone-0.1.34a1/pynecone/components/forms/multiselect.py
--rw-r--r--   0        0        0     3897 2023-06-16 05:09:35.284676 pynecone-0.1.34a1/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      253 2023-06-16 05:09:35.284744 pynecone-0.1.34a1/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2670 2023-06-16 05:09:35.284841 pynecone-0.1.34a1/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3043 2023-06-16 05:09:35.284950 pynecone-0.1.34a1/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2853 2023-06-16 05:09:35.285054 pynecone-0.1.34a1/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3522 2023-06-16 05:09:35.285154 pynecone-0.1.34a1/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     3124 2023-06-16 05:09:35.285251 pynecone-0.1.34a1/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1573 2023-06-16 05:09:35.285337 pynecone-0.1.34a1/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1532 2023-06-16 05:09:35.285439 pynecone-0.1.34a1/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2915 2023-06-16 05:09:35.285534 pynecone-0.1.34a1/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-06-16 05:09:35.285660 pynecone-0.1.34a1/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1357 2023-06-16 05:09:35.285742 pynecone-0.1.34a1/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17360 2023-06-16 05:09:35.285861 pynecone-0.1.34a1/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-06-16 05:09:35.286157 pynecone-0.1.34a1/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      324 2023-06-16 05:09:35.286231 pynecone-0.1.34a1/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      766 2023-06-16 05:09:35.286317 pynecone-0.1.34a1/pynecone/components/layout/box.py
--rw-r--r--   0        0        0     2859 2023-06-16 05:09:35.286413 pynecone-0.1.34a1/pynecone/components/layout/card.py
--rw-r--r--   0        0        0      396 2023-06-16 05:09:35.286474 pynecone-0.1.34a1/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3844 2023-06-16 05:09:35.286583 pynecone-0.1.34a1/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      363 2023-06-16 05:09:35.286649 pynecone-0.1.34a1/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      656 2023-06-16 05:09:35.286714 pynecone-0.1.34a1/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     3167 2023-06-16 05:09:35.286852 pynecone-0.1.34a1/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2023-06-16 05:09:35.286940 pynecone-0.1.34a1/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     4327 2023-06-19 21:55:00.208072 pynecone-0.1.34a1/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-06-16 05:09:35.287093 pynecone-0.1.34a1/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-06-16 05:09:35.287165 pynecone-0.1.34a1/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2023-06-16 05:09:35.287232 pynecone-0.1.34a1/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      995 2023-06-16 05:09:35.287294 pynecone-0.1.34a1/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1471 2023-06-16 05:09:35.287357 pynecone-0.1.34a1/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-06-16 05:09:35.287445 pynecone-0.1.34a1/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2023-06-16 05:09:35.287500 pynecone-0.1.34a1/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0     1391 2023-06-16 05:09:35.287587 pynecone-0.1.34a1/pynecone/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-06-16 05:09:35.287825 pynecone-0.1.34a1/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0      197 2023-06-16 05:09:35.287927 pynecone-0.1.34a1/pynecone/components/media/audio.py
--rw-r--r--   0        0        0     1524 2023-06-16 05:09:35.288014 pynecone-0.1.34a1/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-06-16 05:09:35.288088 pynecone-0.1.34a1/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     2065 2023-06-17 20:30:12.957848 pynecone-0.1.34a1/pynecone/components/media/image.py
--rw-r--r--   0        0        0      197 2023-06-16 05:09:35.288271 pynecone-0.1.34a1/pynecone/components/media/video.py
--rw-r--r--   0        0        0      450 2023-06-16 05:09:35.288589 pynecone-0.1.34a1/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2023 2023-06-16 05:09:35.288672 pynecone-0.1.34a1/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1616 2023-06-16 05:09:35.288784 pynecone-0.1.34a1/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      530 2023-06-16 05:09:35.288849 pynecone-0.1.34a1/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      507 2023-06-16 05:09:35.288915 pynecone-0.1.34a1/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2842 2023-06-16 05:09:35.289003 pynecone-0.1.34a1/pynecone/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-06-16 05:09:35.289274 pynecone-0.1.34a1/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5027 2023-06-16 05:09:35.289387 pynecone-0.1.34a1/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1016 2023-06-16 05:09:35.289499 pynecone-0.1.34a1/pynecone/components/overlay/banner.py
--rw-r--r--   0        0        0     4681 2023-06-16 05:09:35.289600 pynecone-0.1.34a1/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5530 2023-06-16 05:09:35.289712 pynecone-0.1.34a1/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4917 2023-06-16 05:09:35.289815 pynecone-0.1.34a1/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5688 2023-06-16 05:09:35.289921 pynecone-0.1.34a1/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1949 2023-06-16 05:09:35.290030 pynecone-0.1.34a1/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-06-16 05:09:35.290272 pynecone-0.1.34a1/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      451 2023-06-16 05:09:35.290353 pynecone-0.1.34a1/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-06-16 05:09:35.290435 pynecone-0.1.34a1/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5018 2023-06-16 05:09:35.290544 pynecone-0.1.34a1/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-06-16 05:09:35.290617 pynecone-0.1.34a1/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      304 2023-06-16 05:09:35.290747 pynecone-0.1.34a1/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      282 2023-06-16 05:09:35.290812 pynecone-0.1.34a1/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      682 2023-06-16 05:09:35.290901 pynecone-0.1.34a1/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     3460 2023-06-16 05:09:35.290998 pynecone-0.1.34a1/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      337 2023-06-16 05:09:35.291063 pynecone-0.1.34a1/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      306 2023-06-16 05:09:35.291128 pynecone-0.1.34a1/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     7132 2023-06-19 21:09:12.739787 pynecone-0.1.34a1/pynecone/config.py
--rw-r--r--   0        0        0    10422 2023-06-19 21:55:00.208286 pynecone-0.1.34a1/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-06-16 05:09:35.291528 pynecone-0.1.34a1/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-06-16 05:09:35.291627 pynecone-0.1.34a1/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-06-16 05:09:35.291727 pynecone-0.1.34a1/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-06-16 05:09:35.291801 pynecone-0.1.34a1/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-06-16 05:09:35.291904 pynecone-0.1.34a1/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1320 2023-06-16 05:09:35.292004 pynecone-0.1.34a1/pynecone/el/element.py
--rw-r--r--   0        0        0   108518 2023-06-16 05:09:35.292266 pynecone-0.1.34a1/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2667 2023-06-16 05:09:35.292389 pynecone-0.1.34a1/pynecone/el/precompile.py
--rw-r--r--   0        0        0    11876 2023-06-17 20:30:12.959513 pynecone-0.1.34a1/pynecone/event.py
--rw-r--r--   0        0        0      113 2023-06-16 05:09:35.292653 pynecone-0.1.34a1/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     1738 2023-06-16 05:09:35.292762 pynecone-0.1.34a1/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1167 2023-06-16 05:09:35.292844 pynecone-0.1.34a1/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     2388 2023-06-16 05:09:35.292946 pynecone-0.1.34a1/pynecone/model.py
--rw-r--r--   0        0        0     8575 2023-06-16 06:58:15.564372 pynecone-0.1.34a1/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-06-16 05:09:35.293110 pynecone-0.1.34a1/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-06-16 05:09:35.293208 pynecone-0.1.34a1/pynecone/route.py
--rw-r--r--   0        0        0    30945 2023-06-16 05:09:35.293398 pynecone-0.1.34a1/pynecone/state.py
--rw-r--r--   0        0        0     1121 2023-06-16 05:09:35.293539 pynecone-0.1.34a1/pynecone/style.py
--rw-r--r--   0        0        0       26 2023-06-16 05:09:35.293673 pynecone-0.1.34a1/pynecone/utils/__init__.py
--rw-r--r--   0        0        0     7394 2023-06-16 05:09:35.293800 pynecone-0.1.34a1/pynecone/utils/build.py
--rw-r--r--   0        0        0     1759 2023-06-16 05:09:35.294005 pynecone-0.1.34a1/pynecone/utils/console.py
--rw-r--r--   0        0        0     5317 2023-06-16 05:09:35.294115 pynecone-0.1.34a1/pynecone/utils/exec.py
--rw-r--r--   0        0        0    11859 2023-06-16 05:09:35.294243 pynecone-0.1.34a1/pynecone/utils/format.py
--rw-r--r--   0        0        0      587 2023-06-16 05:09:35.294316 pynecone-0.1.34a1/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-06-16 05:09:35.294391 pynecone-0.1.34a1/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0    10905 2023-06-16 05:09:35.294530 pynecone-0.1.34a1/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-06-16 05:09:35.294639 pynecone-0.1.34a1/pynecone/utils/processes.py
--rw-r--r--   0        0        0     2397 2023-06-16 05:09:35.294743 pynecone-0.1.34a1/pynecone/utils/telemetry.py
--rw-r--r--   0        0        0     4806 2023-06-16 05:09:35.294850 pynecone-0.1.34a1/pynecone/utils/types.py
--rw-r--r--   0        0        0     2634 2023-06-16 05:09:35.294923 pynecone-0.1.34a1/pynecone/utils/watch.py
--rw-r--r--   0        0        0    30928 2023-06-16 05:09:35.295168 pynecone-0.1.34a1/pynecone/vars.py
--rw-r--r--   0        0        0     1874 2023-06-19 22:50:36.084624 pynecone-0.1.34a1/pyproject.toml
--rw-r--r--   0        0        0     9620 1970-01-01 00:00:00.000000 pynecone-0.1.34a1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.34a2/LICENSE
+-rw-r--r--   0        0        0     7985 2023-06-19 21:09:12.736508 pynecone-0.1.34a2/README.md
+-rw-r--r--   0        0        0        0 2023-06-16 05:09:35.273793 pynecone-0.1.34a2/pynecone/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1340 2023-06-16 05:09:35.273930 pynecone-0.1.34a2/pynecone/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-06-16 05:09:35.274029 pynecone-0.1.34a2/pynecone/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-16 05:09:35.274187 pynecone-0.1.34a2/pynecone/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15406 2023-06-16 05:09:35.274347 pynecone-0.1.34a2/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      183 2023-06-16 05:09:35.274660 pynecone-0.1.34a2/pynecone/.templates/jinja/app/pcconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-06-16 05:09:35.274990 pynecone-0.1.34a2/pynecone/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-06-16 05:09:35.275137 pynecone-0.1.34a2/pynecone/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-06-16 05:09:35.275226 pynecone-0.1.34a2/pynecone/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3312 2023-06-16 05:09:35.275478 pynecone-0.1.34a2/pynecone/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-06-16 05:09:35.275791 pynecone-0.1.34a2/pynecone/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-06-19 21:09:12.736858 pynecone-0.1.34a2/pynecone/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-06-16 05:09:35.275938 pynecone-0.1.34a2/pynecone/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-06-16 05:09:35.276075 pynecone-0.1.34a2/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-06-19 21:09:12.738040 pynecone-0.1.34a2/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-06-16 05:09:35.277373 pynecone-0.1.34a2/pynecone/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       47 2023-06-16 05:09:35.277600 pynecone-0.1.34a2/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1143 2023-06-19 21:09:12.738227 pynecone-0.1.34a2/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-06-16 05:09:35.277911 pynecone-0.1.34a2/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-06-19 21:09:12.738431 pynecone-0.1.34a2/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-06-19 21:09:12.738679 pynecone-0.1.34a2/pynecone/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-06-16 05:09:35.278186 pynecone-0.1.34a2/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-06-19 21:09:12.738771 pynecone-0.1.34a2/pynecone/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0     8838 2023-06-17 20:30:12.955812 pynecone-0.1.34a2/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1636 2023-06-17 20:30:12.956097 pynecone-0.1.34a2/pynecone/__init__.py
+-rw-r--r--   0        0        0      320 2023-06-16 05:09:35.278638 pynecone-0.1.34a2/pynecone/admin.py
+-rw-r--r--   0        0        0    21913 2023-06-19 21:09:12.739037 pynecone-0.1.34a2/pynecone/app.py
+-rw-r--r--   0        0        0     2548 2023-06-16 05:09:35.278940 pynecone-0.1.34a2/pynecone/base.py
+-rw-r--r--   0        0        0       29 2023-06-16 05:09:35.279040 pynecone-0.1.34a2/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     7335 2023-06-19 21:09:12.739412 pynecone-0.1.34a2/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     2739 2023-06-19 21:09:12.739600 pynecone-0.1.34a2/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     7767 2023-06-16 05:09:35.279374 pynecone-0.1.34a2/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     7471 2023-06-16 05:09:35.279688 pynecone-0.1.34a2/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      229 2023-06-16 05:09:35.279922 pynecone-0.1.34a2/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-16 05:09:35.279996 pynecone-0.1.34a2/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-06-16 05:09:35.280073 pynecone-0.1.34a2/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-06-16 05:09:35.280133 pynecone-0.1.34a2/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      265 2023-06-16 05:09:35.280191 pynecone-0.1.34a2/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      933 2023-06-16 05:09:35.280288 pynecone-0.1.34a2/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1412 2023-06-16 05:09:35.280378 pynecone-0.1.34a2/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    24243 2023-06-16 05:09:35.280545 pynecone-0.1.34a2/pynecone/components/component.py
+-rw-r--r--   0        0        0      496 2023-06-16 05:09:35.280902 pynecone-0.1.34a2/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      334 2023-06-16 05:09:35.280992 pynecone-0.1.34a2/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2513 2023-06-16 05:09:35.281074 pynecone-0.1.34a2/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4033 2023-06-16 05:09:35.281150 pynecone-0.1.34a2/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      537 2023-06-16 05:09:35.281254 pynecone-0.1.34a2/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-06-16 05:09:35.281333 pynecone-0.1.34a2/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1430 2023-06-16 05:09:35.281415 pynecone-0.1.34a2/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2157 2023-06-16 05:09:35.281495 pynecone-0.1.34a2/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5793 2023-06-16 05:09:35.281620 pynecone-0.1.34a2/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2188 2023-06-16 05:09:35.281738 pynecone-0.1.34a2/pynecone/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-06-16 05:09:35.281995 pynecone-0.1.34a2/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3517 2023-06-16 05:09:35.282101 pynecone-0.1.34a2/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2777 2023-06-16 05:09:35.282180 pynecone-0.1.34a2/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1741 2023-06-16 05:09:35.282287 pynecone-0.1.34a2/pynecone/components/disclosure/transition.py
+-rw-r--r--   0        0        0      285 2023-06-16 05:09:35.282356 pynecone-0.1.34a2/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-06-16 05:09:35.282647 pynecone-0.1.34a2/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1571 2023-06-16 05:09:35.282727 pynecone-0.1.34a2/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1905 2023-06-16 05:09:35.282811 pynecone-0.1.34a2/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      879 2023-06-16 05:09:35.282890 pynecone-0.1.34a2/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1785 2023-06-16 05:09:35.282969 pynecone-0.1.34a2/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      678 2023-06-16 05:09:35.283039 pynecone-0.1.34a2/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1471 2023-06-16 05:09:35.283322 pynecone-0.1.34a2/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1765 2023-06-16 05:09:35.283424 pynecone-0.1.34a2/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2454 2023-06-16 05:09:35.283533 pynecone-0.1.34a2/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3147 2023-06-16 05:09:35.283651 pynecone-0.1.34a2/pynecone/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      578 2023-06-16 05:09:35.283755 pynecone-0.1.34a2/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      243 2023-06-16 05:09:35.283847 pynecone-0.1.34a2/pynecone/components/forms/date_picker.py
+-rw-r--r--   0        0        0      277 2023-06-16 05:09:35.283931 pynecone-0.1.34a2/pynecone/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     1949 2023-06-16 05:09:35.284031 pynecone-0.1.34a2/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0      243 2023-06-16 05:09:35.284144 pynecone-0.1.34a2/pynecone/components/forms/email.py
+-rw-r--r--   0        0        0     2996 2023-06-16 05:09:35.284270 pynecone-0.1.34a2/pynecone/components/forms/form.py
+-rw-r--r--   0        0        0      802 2023-06-16 05:09:35.284358 pynecone-0.1.34a2/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2880 2023-06-16 05:09:35.284448 pynecone-0.1.34a2/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0    12667 2023-06-16 05:09:35.284573 pynecone-0.1.34a2/pynecone/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3897 2023-06-16 05:09:35.284676 pynecone-0.1.34a2/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      253 2023-06-16 05:09:35.284744 pynecone-0.1.34a2/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2670 2023-06-16 05:09:35.284841 pynecone-0.1.34a2/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3043 2023-06-16 05:09:35.284950 pynecone-0.1.34a2/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2853 2023-06-16 05:09:35.285054 pynecone-0.1.34a2/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3522 2023-06-16 05:09:35.285154 pynecone-0.1.34a2/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     3124 2023-06-16 05:09:35.285251 pynecone-0.1.34a2/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1573 2023-06-16 05:09:35.285337 pynecone-0.1.34a2/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1532 2023-06-16 05:09:35.285439 pynecone-0.1.34a2/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2915 2023-06-16 05:09:35.285534 pynecone-0.1.34a2/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-06-16 05:09:35.285660 pynecone-0.1.34a2/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1357 2023-06-16 05:09:35.285742 pynecone-0.1.34a2/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17360 2023-06-16 05:09:35.285861 pynecone-0.1.34a2/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-06-16 05:09:35.286157 pynecone-0.1.34a2/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      324 2023-06-16 05:09:35.286231 pynecone-0.1.34a2/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      766 2023-06-16 05:09:35.286317 pynecone-0.1.34a2/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0     2859 2023-06-16 05:09:35.286413 pynecone-0.1.34a2/pynecone/components/layout/card.py
+-rw-r--r--   0        0        0      396 2023-06-16 05:09:35.286474 pynecone-0.1.34a2/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3844 2023-06-16 05:09:35.286583 pynecone-0.1.34a2/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      363 2023-06-16 05:09:35.286649 pynecone-0.1.34a2/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      656 2023-06-16 05:09:35.286714 pynecone-0.1.34a2/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     3167 2023-06-16 05:09:35.286852 pynecone-0.1.34a2/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2023-06-16 05:09:35.286940 pynecone-0.1.34a2/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     4327 2023-06-19 21:55:00.208072 pynecone-0.1.34a2/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-06-16 05:09:35.287093 pynecone-0.1.34a2/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-06-16 05:09:35.287165 pynecone-0.1.34a2/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2023-06-16 05:09:35.287232 pynecone-0.1.34a2/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      995 2023-06-16 05:09:35.287294 pynecone-0.1.34a2/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1471 2023-06-16 05:09:35.287357 pynecone-0.1.34a2/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-06-16 05:09:35.287445 pynecone-0.1.34a2/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2023-06-16 05:09:35.287500 pynecone-0.1.34a2/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0     1391 2023-06-16 05:09:35.287587 pynecone-0.1.34a2/pynecone/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-06-16 05:09:35.287825 pynecone-0.1.34a2/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0      197 2023-06-16 05:09:35.287927 pynecone-0.1.34a2/pynecone/components/media/audio.py
+-rw-r--r--   0        0        0     1524 2023-06-16 05:09:35.288014 pynecone-0.1.34a2/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-06-16 05:09:35.288088 pynecone-0.1.34a2/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     2065 2023-06-17 20:30:12.957848 pynecone-0.1.34a2/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      197 2023-06-16 05:09:35.288271 pynecone-0.1.34a2/pynecone/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-06-16 05:09:35.288589 pynecone-0.1.34a2/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2023 2023-06-16 05:09:35.288672 pynecone-0.1.34a2/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1616 2023-06-16 05:09:35.288784 pynecone-0.1.34a2/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      530 2023-06-16 05:09:35.288849 pynecone-0.1.34a2/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      507 2023-06-16 05:09:35.288915 pynecone-0.1.34a2/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2842 2023-06-16 05:09:35.289003 pynecone-0.1.34a2/pynecone/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-06-16 05:09:35.289274 pynecone-0.1.34a2/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5027 2023-06-16 05:09:35.289387 pynecone-0.1.34a2/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1016 2023-06-16 05:09:35.289499 pynecone-0.1.34a2/pynecone/components/overlay/banner.py
+-rw-r--r--   0        0        0     4681 2023-06-16 05:09:35.289600 pynecone-0.1.34a2/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5530 2023-06-16 05:09:35.289712 pynecone-0.1.34a2/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4917 2023-06-16 05:09:35.289815 pynecone-0.1.34a2/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5688 2023-06-16 05:09:35.289921 pynecone-0.1.34a2/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1949 2023-06-16 05:09:35.290030 pynecone-0.1.34a2/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-06-16 05:09:35.290272 pynecone-0.1.34a2/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-16 05:09:35.290353 pynecone-0.1.34a2/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-06-16 05:09:35.290435 pynecone-0.1.34a2/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5018 2023-06-16 05:09:35.290544 pynecone-0.1.34a2/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-06-16 05:09:35.290617 pynecone-0.1.34a2/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      304 2023-06-16 05:09:35.290747 pynecone-0.1.34a2/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      282 2023-06-16 05:09:35.290812 pynecone-0.1.34a2/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      682 2023-06-16 05:09:35.290901 pynecone-0.1.34a2/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     3460 2023-06-16 05:09:35.290998 pynecone-0.1.34a2/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      337 2023-06-16 05:09:35.291063 pynecone-0.1.34a2/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      306 2023-06-16 05:09:35.291128 pynecone-0.1.34a2/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     7132 2023-06-19 21:09:12.739787 pynecone-0.1.34a2/pynecone/config.py
+-rw-r--r--   0        0        0    10422 2023-06-19 21:55:00.208286 pynecone-0.1.34a2/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-06-16 05:09:35.291528 pynecone-0.1.34a2/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-06-16 05:09:35.291627 pynecone-0.1.34a2/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-06-16 05:09:35.291727 pynecone-0.1.34a2/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-06-16 05:09:35.291801 pynecone-0.1.34a2/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-06-16 05:09:35.291904 pynecone-0.1.34a2/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1320 2023-06-16 05:09:35.292004 pynecone-0.1.34a2/pynecone/el/element.py
+-rw-r--r--   0        0        0   108518 2023-06-16 05:09:35.292266 pynecone-0.1.34a2/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2667 2023-06-16 05:09:35.292389 pynecone-0.1.34a2/pynecone/el/precompile.py
+-rw-r--r--   0        0        0    11876 2023-06-17 20:30:12.959513 pynecone-0.1.34a2/pynecone/event.py
+-rw-r--r--   0        0        0      113 2023-06-16 05:09:35.292653 pynecone-0.1.34a2/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     1738 2023-06-16 05:09:35.292762 pynecone-0.1.34a2/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1167 2023-06-16 05:09:35.292844 pynecone-0.1.34a2/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     2388 2023-06-16 05:09:35.292946 pynecone-0.1.34a2/pynecone/model.py
+-rw-r--r--   0        0        0     8815 2023-06-20 17:23:40.592375 pynecone-0.1.34a2/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-06-16 05:09:35.293110 pynecone-0.1.34a2/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-06-16 05:09:35.293208 pynecone-0.1.34a2/pynecone/route.py
+-rw-r--r--   0        0        0    30945 2023-06-16 05:09:35.293398 pynecone-0.1.34a2/pynecone/state.py
+-rw-r--r--   0        0        0     1121 2023-06-16 05:09:35.293539 pynecone-0.1.34a2/pynecone/style.py
+-rw-r--r--   0        0        0       26 2023-06-16 05:09:35.293673 pynecone-0.1.34a2/pynecone/utils/__init__.py
+-rw-r--r--   0        0        0     7863 2023-06-20 17:23:40.592790 pynecone-0.1.34a2/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1759 2023-06-16 05:09:35.294005 pynecone-0.1.34a2/pynecone/utils/console.py
+-rw-r--r--   0        0        0     4793 2023-06-20 17:23:40.593030 pynecone-0.1.34a2/pynecone/utils/exec.py
+-rw-r--r--   0        0        0    11859 2023-06-16 05:09:35.294243 pynecone-0.1.34a2/pynecone/utils/format.py
+-rw-r--r--   0        0        0      587 2023-06-16 05:09:35.294316 pynecone-0.1.34a2/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-06-16 05:09:35.294391 pynecone-0.1.34a2/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0    10905 2023-06-16 05:09:35.294530 pynecone-0.1.34a2/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-06-16 05:09:35.294639 pynecone-0.1.34a2/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     2397 2023-06-16 05:09:35.294743 pynecone-0.1.34a2/pynecone/utils/telemetry.py
+-rw-r--r--   0        0        0     4806 2023-06-16 05:09:35.294850 pynecone-0.1.34a2/pynecone/utils/types.py
+-rw-r--r--   0        0        0     2634 2023-06-16 05:09:35.294923 pynecone-0.1.34a2/pynecone/utils/watch.py
+-rw-r--r--   0        0        0    30928 2023-06-16 05:09:35.295168 pynecone-0.1.34a2/pynecone/vars.py
+-rw-r--r--   0        0        0     1874 2023-06-20 17:23:55.810928 pynecone-0.1.34a2/pyproject.toml
+-rw-r--r--   0        0        0     9620 1970-01-01 00:00:00.000000 pynecone-0.1.34a2/PKG-INFO
```

### Comparing `pynecone-0.1.34a1/LICENSE` & `pynecone-0.1.34a2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/README.md` & `pynecone-0.1.34a2/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/apps/counter/counter.py` & `pynecone-0.1.34a2/pynecone/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/apps/default/default.py` & `pynecone-0.1.34a2/pynecone/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.34a2/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/jinja/web/pages/index.js.jinja2` & `pynecone-0.1.34a2/pynecone/.templates/jinja/web/pages/index.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/jinja/web/pages/utils.js.jinja2` & `pynecone-0.1.34a2/pynecone/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.34a2/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/web/package.json` & `pynecone-0.1.34a2/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.34a2/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.34a2/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.34a2/pynecone/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/__init__.py` & `pynecone-0.1.34a2/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/app.py` & `pynecone-0.1.34a2/pynecone/app.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/base.py` & `pynecone-0.1.34a2/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/compiler/compiler.py` & `pynecone-0.1.34a2/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/compiler/templates.py` & `pynecone-0.1.34a2/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/compiler/utils.py` & `pynecone-0.1.34a2/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/__init__.py` & `pynecone-0.1.34a2/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/base/bare.py` & `pynecone-0.1.34a2/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/base/document.py` & `pynecone-0.1.34a2/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/base/link.py` & `pynecone-0.1.34a2/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/base/meta.py` & `pynecone-0.1.34a2/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/component.py` & `pynecone-0.1.34a2/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/datadisplay/code.py` & `pynecone-0.1.34a2/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.34a2/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.34a2/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/datadisplay/list.py` & `pynecone-0.1.34a2/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.34a2/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/datadisplay/table.py` & `pynecone-0.1.34a2/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/datadisplay/tag.py` & `pynecone-0.1.34a2/pynecone/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.34a2/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.34a2/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/disclosure/transition.py` & `pynecone-0.1.34a2/pynecone/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/feedback/alert.py` & `pynecone-0.1.34a2/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.34a2/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/feedback/progress.py` & `pynecone-0.1.34a2/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.34a2/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/feedback/spinner.py` & `pynecone-0.1.34a2/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/__init__.py` & `pynecone-0.1.34a2/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/button.py` & `pynecone-0.1.34a2/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/checkbox.py` & `pynecone-0.1.34a2/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/colormodeswitch.py` & `pynecone-0.1.34a2/pynecone/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.34a2/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/editable.py` & `pynecone-0.1.34a2/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/form.py` & `pynecone-0.1.34a2/pynecone/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.34a2/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/input.py` & `pynecone-0.1.34a2/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/multiselect.py` & `pynecone-0.1.34a2/pynecone/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/numberinput.py` & `pynecone-0.1.34a2/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/pininput.py` & `pynecone-0.1.34a2/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/radio.py` & `pynecone-0.1.34a2/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.34a2/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/select.py` & `pynecone-0.1.34a2/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/slider.py` & `pynecone-0.1.34a2/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/switch.py` & `pynecone-0.1.34a2/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/textarea.py` & `pynecone-0.1.34a2/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/forms/upload.py` & `pynecone-0.1.34a2/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/graphing/plotly.py` & `pynecone-0.1.34a2/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/graphing/victory.py` & `pynecone-0.1.34a2/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/__init__.py` & `pynecone-0.1.34a2/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/box.py` & `pynecone-0.1.34a2/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/card.py` & `pynecone-0.1.34a2/pynecone/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/cond.py` & `pynecone-0.1.34a2/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/flex.py` & `pynecone-0.1.34a2/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/foreach.py` & `pynecone-0.1.34a2/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/grid.py` & `pynecone-0.1.34a2/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/html.py` & `pynecone-0.1.34a2/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/responsive.py` & `pynecone-0.1.34a2/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/stack.py` & `pynecone-0.1.34a2/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/layout/wrap.py` & `pynecone-0.1.34a2/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/libs/react_player.py` & `pynecone-0.1.34a2/pynecone/components/libs/react_player.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/media/avatar.py` & `pynecone-0.1.34a2/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/media/icon.py` & `pynecone-0.1.34a2/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/media/image.py` & `pynecone-0.1.34a2/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.34a2/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/navigation/link.py` & `pynecone-0.1.34a2/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.34a2/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/navigation/stepper.py` & `pynecone-0.1.34a2/pynecone/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/overlay/__init__.py` & `pynecone-0.1.34a2/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.34a2/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/overlay/banner.py` & `pynecone-0.1.34a2/pynecone/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/overlay/drawer.py` & `pynecone-0.1.34a2/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/overlay/menu.py` & `pynecone-0.1.34a2/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/overlay/modal.py` & `pynecone-0.1.34a2/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/overlay/popover.py` & `pynecone-0.1.34a2/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.34a2/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.34a2/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/tags/tag.py` & `pynecone-0.1.34a2/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/tags/tagless.py` & `pynecone-0.1.34a2/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/typography/highlight.py` & `pynecone-0.1.34a2/pynecone/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/components/typography/markdown.py` & `pynecone-0.1.34a2/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/config.py` & `pynecone-0.1.34a2/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/constants.py` & `pynecone-0.1.34a2/pynecone/constants.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/el/constants/html.py` & `pynecone-0.1.34a2/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/el/constants/pynecone.py` & `pynecone-0.1.34a2/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/el/constants/react.py` & `pynecone-0.1.34a2/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/el/element.py` & `pynecone-0.1.34a2/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/el/elements/__init__.py` & `pynecone-0.1.34a2/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/el/precompile.py` & `pynecone-0.1.34a2/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/event.py` & `pynecone-0.1.34a2/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.34a2/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/middleware/middleware.py` & `pynecone-0.1.34a2/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/model.py` & `pynecone-0.1.34a2/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/pc.py` & `pynecone-0.1.34a2/pynecone/pc.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,34 +125,44 @@
     console.rule("[bold]Starting Pynecone App")
     app = prerequisites.get_app()
 
     # Check the admin dashboard settings.
     prerequisites.check_admin_settings()
 
     # Get the frontend and backend commands, based on the environment.
-    frontend_cmd = backend_cmd = None
+    setup_frontend = frontend_cmd = backend_cmd = None
     if env == constants.Env.DEV:
-        frontend_cmd, backend_cmd = exec.run_frontend, exec.run_backend
+        setup_frontend, frontend_cmd, backend_cmd = (
+            build.setup_frontend,
+            exec.run_frontend,
+            exec.run_backend,
+        )
     if env == constants.Env.PROD:
-        frontend_cmd, backend_cmd = exec.run_frontend_prod, exec.run_backend_prod
-    assert frontend_cmd and backend_cmd, "Invalid env"
+        setup_frontend, frontend_cmd, backend_cmd = (
+            build.setup_frontend_prod,
+            exec.run_frontend_prod,
+            exec.run_backend_prod,
+        )
+    assert setup_frontend and frontend_cmd and backend_cmd, "Invalid env"
 
     # Post a telemetry event.
     telemetry.send(f"run-{env.value}", get_config().telemetry_enabled)
 
     # Run the frontend and backend.
+    if frontend:
+        setup_frontend(Path.cwd(), loglevel)
+        threading.Thread(
+            target=frontend_cmd, args=(Path.cwd(), frontend_port, loglevel)
+        ).start()
     if backend:
+        build.setup_backend()
         threading.Thread(
             target=backend_cmd,
             args=(app.__name__, backend_host, backend_port, loglevel),
         ).start()
-    if frontend:
-        threading.Thread(
-            target=frontend_cmd, args=(app.app, Path.cwd(), frontend_port)
-        ).start()
 
 
 @cli.command()
 def deploy(dry_run: bool = typer.Option(False, help="Whether to run a dry run.")):
     """Deploy the app to the Pynecone hosting service."""
     # Get the app config.
     config = get_config()
@@ -213,17 +223,15 @@
 
     # Compile the app in production mode and export it.
     console.rule("[bold]Compiling production app and preparing for export.")
 
     if frontend:
         build.setup_frontend(Path.cwd())
 
-    app = prerequisites.get_app().app
     build.export_app(
-        app,
         backend=backend,
         frontend=frontend,
         zip=zipping,
         deploy_url=config.deploy_url,
     )
 
     # Post a telemetry event.
```

### Comparing `pynecone-0.1.34a1/pynecone/route.py` & `pynecone-0.1.34a2/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/state.py` & `pynecone-0.1.34a2/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/style.py` & `pynecone-0.1.34a2/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/build.py` & `pynecone-0.1.34a2/pynecone/utils/build.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,25 +3,22 @@
 from __future__ import annotations
 
 import json
 import os
 import random
 import subprocess
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional, Union
+from typing import Optional, Union
 
 from rich.progress import Progress
 
 from pynecone import constants
 from pynecone.config import get_config
 from pynecone.utils import path_ops, prerequisites
 
-if TYPE_CHECKING:
-    from pynecone.app import App
-
 
 def update_json_file(file_path: str, update_dict: dict[str, Union[int, str]]):
     """Update the contents of a json file.
 
     Args:
         file_path: the path to the JSON file.
         update_dict: object to update json.
@@ -87,25 +84,23 @@
     )
 
     with open(constants.SITEMAP_CONFIG_FILE, "w") as f:
         f.write(templates.SITEMAP_CONFIG(config=config))
 
 
 def export_app(
-    app: App,
     backend: bool = True,
     frontend: bool = True,
     zip: bool = False,
     deploy_url: Optional[str] = None,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Zip up the app for deployment.
 
     Args:
-        app: The app.
         backend: Whether to zip up the backend app.
         frontend: Whether to zip up the frontend app.
         zip: Whether to zip the app.
         deploy_url: The URL of the deployed app.
         loglevel: The log level to use.
     """
     # Remove the static folder.
@@ -117,45 +112,42 @@
 
     # Create a progress object
     progress = Progress()
 
     # Add a single task to the progress object
     task = progress.add_task("Building app... ", total=500)
 
-    # Start the progress bar
-    with progress:
-        # Run the subprocess command
-        export_process = subprocess.Popen(
-            [prerequisites.get_package_manager(), "run", "export"],
-            cwd=constants.WEB_DIR,
-            env=os.environ,
-            stderr=subprocess.STDOUT,
-            stdout=subprocess.PIPE,  # Redirect stdout to a pipe
-            universal_newlines=True,  # Set universal_newlines to True for text mode
-        )
-
-        if export_process.stdout:
-            for line in iter(export_process.stdout.readline, ""):
-                if "Linting and checking " in line:
-                    progress.update(task, advance=100)
-                elif "Compiled successfully" in line:
-                    progress.update(task, advance=100)
-                elif "Route (pages)" in line:
-                    progress.update(task, advance=100)
-                elif "automatically rendered as static HTML" in line:
-                    progress.update(task, advance=100)
-                elif "Export successful" in line:
-                    print("DOOE")
-                    progress.update(task, completed=500)
-                    break  # Exit the loop if the completion message is found
-                elif loglevel == constants.LogLevel.DEBUG:
-                    print(line, end="")
+    # Start the subprocess with the progress bar.
+    with progress, subprocess.Popen(
+        [prerequisites.get_package_manager(), "run", "export"],
+        cwd=constants.WEB_DIR,
+        env=os.environ,
+        stderr=subprocess.STDOUT,
+        stdout=subprocess.PIPE,  # Redirect stdout to a pipe
+        universal_newlines=True,  # Set universal_newlines to True for text mode
+    ) as export_process:
+        assert export_process.stdout is not None, "No stdout for export process."
+        for line in export_process.stdout:
+            # Print the line in debug mode.
+            if loglevel == constants.LogLevel.DEBUG:
+                print(line, end="")
+
+            # Check for special strings and update the progress bar.
+            if "Linting and checking " in line:
+                progress.update(task, advance=100)
+            elif "Compiled successfully" in line:
+                progress.update(task, advance=100)
+            elif "Route (pages)" in line:
+                progress.update(task, advance=100)
+            elif "automatically rendered as static HTML" in line:
+                progress.update(task, advance=100)
+            elif "Export successful" in line:
+                progress.update(task, completed=500)
+                break  # Exit the loop if the completion message is found
 
-        # Wait for the subprocess to complete
-        export_process.wait()
         print("Export process completed.")
 
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
@@ -190,21 +182,29 @@
         cmd = r"cd .web/_static && zip -r ../../frontend.zip ./*"
         os.system(cmd)
     if backend:
         cmd = r"zip -r backend.zip ./* -x .web/\* ./assets\* ./frontend.zip\* ./backend.zip\*"
         os.system(cmd)
 
 
-def setup_frontend(root: Path, disable_telemetry: bool = True):
+def setup_frontend(
+    root: Path,
+    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
+    disable_telemetry: bool = True,
+):
     """Set up the frontend.
 
     Args:
-        root: root path of the project.
+        root: The root path of the project.
+        loglevel: The log level to use.
         disable_telemetry: Whether to disable the Next telemetry.
     """
+    # Validate bun version.
+    prerequisites.validate_and_install_bun(initialize=False)
+
     # Initialize the web directory if it doesn't exist.
     web_dir = prerequisites.create_web_directory(root)
 
     # Install frontend packages.
     prerequisites.install_frontend_packages(web_dir)
 
     # Copy asset files to public folder.
@@ -229,14 +229,30 @@
             cwd=constants.WEB_DIR,
             env=os.environ,
             stdout=subprocess.DEVNULL,
             stderr=subprocess.STDOUT,
         )
 
 
+def setup_frontend_prod(
+    root: Path,
+    loglevel: constants.LogLevel = constants.LogLevel.ERROR,
+    disable_telemetry: bool = True,
+):
+    """Set up the frontend for prod mode.
+
+    Args:
+        root: The root path of the project.
+        loglevel: The log level to use.
+        disable_telemetry: Whether to disable the Next telemetry.
+    """
+    setup_frontend(root, loglevel, disable_telemetry)
+    export_app(loglevel=loglevel)
+
+
 def setup_backend():
     """Set up backend.
 
     Specifically ensures backend database is updated when running --no-frontend.
     """
     # Import here to avoid circular imports.
     from pynecone.model import Model
```

### Comparing `pynecone-0.1.34a1/pynecone/utils/console.py` & `pynecone-0.1.34a2/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/exec.py` & `pynecone-0.1.34a2/pynecone/utils/exec.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,48 +3,41 @@
 from __future__ import annotations
 
 import os
 import platform
 import subprocess
 from datetime import datetime
 from pathlib import Path
-from typing import TYPE_CHECKING
 
 from rich import print
 
 from pynecone import constants
 from pynecone.config import get_config
 from pynecone.utils import console, prerequisites, processes
-from pynecone.utils.build import export_app, setup_backend, setup_frontend
 from pynecone.utils.watch import AssetFolderWatch
 
-if TYPE_CHECKING:
-    from pynecone.app import App
-
 
 def start_watching_assets_folder(root):
     """Start watching assets folder.
 
     Args:
         root: root path of the project.
     """
     asset_watch = AssetFolderWatch(root)
     asset_watch.start()
 
 
 def run_process_and_launch_url(
     run_command: list[str],
-    root: Path,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the process and launch the URL.
 
     Args:
         run_command: The command to run.
-        root: root path of the project.
         loglevel: The log level to use.
     """
     process = subprocess.Popen(
         run_command,
         cwd=constants.WEB_DIR,
         env=os.environ,
         stderr=subprocess.STDOUT,
@@ -68,71 +61,55 @@
                     f"[yellow][Updating App][/yellow] Applying changes and refreshing. Time: {current_time}"
                 )
             elif loglevel == constants.LogLevel.DEBUG:
                 print(line, end="")
 
 
 def run_frontend(
-    app: App,
     root: Path,
     port: str,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the frontend.
 
     Args:
-        app: The app.
-        root: root path of the project.
-        port: port of the app.
+        root: The root path of the project.
+        port: The port to run the frontend on.
         loglevel: The log level to use.
     """
-    # validate bun version
-    prerequisites.validate_and_install_bun(initialize=False)
-
-    # Set up the frontend.
-    setup_frontend(root)
-
     # Start watching asset folder.
     start_watching_assets_folder(root)
 
     # Run the frontend in development mode.
     console.rule("[bold green]App Running")
     os.environ["PORT"] = get_config().frontend_port if port is None else port
     run_process_and_launch_url(
-        [prerequisites.get_package_manager(), "run", "dev"], root, loglevel
+        [prerequisites.get_package_manager(), "run", "dev"], loglevel
     )
 
 
 def run_frontend_prod(
-    app: App,
     root: Path,
     port: str,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
 ):
     """Run the frontend.
 
     Args:
-        app: The app.
-        root: root path of the project.
-        port: port of the app.
+        root: The root path of the project (to keep same API as run_frontend).
+        port: The port to run the frontend on.
         loglevel: The log level to use.
     """
-    # Set up the frontend.
-    setup_frontend(root)
-
-    # Export the app.
-    export_app(app, loglevel=loglevel)
-
     # Set the port.
     os.environ["PORT"] = get_config().frontend_port if port is None else port
 
     # Run the frontend in production mode.
     console.rule("[bold green]App Running")
     run_process_and_launch_url(
-        [prerequisites.get_package_manager(), "run", "prod"], root, loglevel
+        [prerequisites.get_package_manager(), "run", "prod"], loglevel
     )
 
 
 def run_backend(
     app_name: str,
     host: str,
     port: int,
@@ -142,16 +119,14 @@
 
     Args:
         host: The app host
         app_name: The app name.
         port: The app port
         loglevel: The log level.
     """
-    setup_backend()
-
     cmd = [
         "uvicorn",
         f"{app_name}:{constants.APP_VAR}.{constants.API_VAR}",
         "--host",
         host,
         "--port",
         str(port),
@@ -177,16 +152,14 @@
 
     Args:
         host: The app host
         app_name: The app name.
         port: The app port
         loglevel: The log level.
     """
-    setup_backend()
-
     num_workers = processes.get_num_workers()
     command = (
         [
             *constants.RUN_BACKEND_PROD_WINDOWS,
             "--host",
             host,
             "--port",
```

### Comparing `pynecone-0.1.34a1/pynecone/utils/format.py` & `pynecone-0.1.34a2/pynecone/utils/format.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/imports.py` & `pynecone-0.1.34a2/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/path_ops.py` & `pynecone-0.1.34a2/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/prerequisites.py` & `pynecone-0.1.34a2/pynecone/utils/prerequisites.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/processes.py` & `pynecone-0.1.34a2/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/telemetry.py` & `pynecone-0.1.34a2/pynecone/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/types.py` & `pynecone-0.1.34a2/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/utils/watch.py` & `pynecone-0.1.34a2/pynecone/utils/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pynecone/vars.py` & `pynecone-0.1.34a2/pynecone/vars.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.34a1/pyproject.toml` & `pynecone-0.1.34a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.34a1"
+version = "0.1.34a2"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.34a1/PKG-INFO` & `pynecone-0.1.34a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.34a1
+Version: 0.1.34a2
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

