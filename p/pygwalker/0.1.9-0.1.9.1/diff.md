# Comparing `tmp/pygwalker-0.1.9.tar.gz` & `tmp/pygwalker-0.1.9.1.tar.gz`

## Comparing `pygwalker-0.1.9.tar` & `pygwalker-0.1.9.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/index.html
--rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/package.json
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/postcss.config.js
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/tailwind.config.js
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/tsconfig.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/vite.config.ts
--rw-r--r--   0        0        0   124966 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/yarn.lock
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/index.css
--rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/index.tsx
--rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/components/defaultTab.tsx
--rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/components/modal.tsx
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/components/options.tsx
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/components/button/base.ts
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/components/button/default.tsx
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/components/button/primary.tsx
--rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/components/codeExportModal/index.tsx
--rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/components/codeExportModal/saveConfigButton.tsx
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/dataSource/index.ts
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/interfaces/index.ts
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/utils/save.ts
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pygwalker-0.1.9/app/src/utils/userConfig.ts
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/__version__.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/base.py
--rw-r--r--   0        0        0    10110 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/gwalker.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/index.html
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/walk.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  1852666 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0    27735 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/style.css
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/components/defaultTab.d.ts
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/components/modal.d.ts
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/components/button/base.d.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/components/button/default.d.ts
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/components/button/primary.d.ts
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/components/codeExportModal/index.d.ts
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/components/codeExportModal/saveConfigButton.d.ts
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/dataSource/index.d.ts
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/utils/save.d.ts
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/templates/dist/utils/userConfig.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/utils/check_update.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/utils/errors.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/utils/fname_encodings.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/utils/format_invoke_walk_code.py
--rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/utils/gwalker_props.py
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/utils/render.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker/utils/spec.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker_utils/__init__.py
--rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker_utils/__main__.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker_utils/config.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pygwalker_utils/defaults.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.9/scripts/__init__.py
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.1.9/scripts/compile.sh
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.1.9/scripts/develop.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.1.9/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.1.9/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.1.9/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.1.9/LICENSE
--rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 pygwalker-0.1.9/README.md
--rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 pygwalker-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    14077 2020-02-02 00:00:00.000000 pygwalker-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/index.html
+-rw-r--r--   0        0        0     1256 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/package.json
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/postcss.config.js
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/tailwind.config.js
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/tsconfig.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/vite.config.ts
+-rw-r--r--   0        0        0   124966 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/yarn.lock
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/index.css
+-rw-r--r--   0        0        0     5170 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/index.tsx
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/components/defaultTab.tsx
+-rw-r--r--   0        0        0     2917 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/components/modal.tsx
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/components/options.tsx
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/components/button/base.ts
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/components/button/default.tsx
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/components/button/primary.tsx
+-rw-r--r--   0        0        0     4359 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/components/codeExportModal/index.tsx
+-rw-r--r--   0        0        0     5885 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/components/codeExportModal/saveConfigButton.tsx
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/dataSource/index.ts
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/utils/save.ts
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/app/src/utils/userConfig.ts
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/__version__.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/base.py
+-rw-r--r--   0        0        0    10133 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/gwalker.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/walk.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  1852666 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0    27735 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/style.css
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/components/defaultTab.d.ts
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/components/modal.d.ts
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/components/button/base.d.ts
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/components/button/default.d.ts
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/components/button/primary.d.ts
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/components/codeExportModal/index.d.ts
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/components/codeExportModal/saveConfigButton.d.ts
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/dataSource/index.d.ts
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/utils/save.d.ts
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/templates/dist/utils/userConfig.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/utils/check_update.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/utils/errors.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/utils/fname_encodings.py
+-rw-r--r--   0        0        0     1430 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/utils/format_invoke_walk_code.py
+-rw-r--r--   0        0        0     9097 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/utils/gwalker_props.py
+-rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/utils/render.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker/utils/spec.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker_utils/__init__.py
+-rw-r--r--   0        0        0     2045 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker_utils/__main__.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker_utils/config.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pygwalker_utils/defaults.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/scripts/__init__.py
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/scripts/compile.sh
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/scripts/develop.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/LICENSE
+-rw-r--r--   0        0        0    12915 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/README.md
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/pyproject.toml
+-rw-r--r--   0        0        0    14079 2020-02-02 00:00:00.000000 pygwalker-0.1.9.1/PKG-INFO
```

### Comparing `pygwalker-0.1.9/app/package.json` & `pygwalker-0.1.9.1/app/package.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/tsconfig.json` & `pygwalker-0.1.9.1/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/vite.config.ts` & `pygwalker-0.1.9.1/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/yarn.lock` & `pygwalker-0.1.9.1/app/yarn.lock`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/index.tsx` & `pygwalker-0.1.9.1/app/src/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/components/defaultTab.tsx` & `pygwalker-0.1.9.1/app/src/components/defaultTab.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/components/modal.tsx` & `pygwalker-0.1.9.1/app/src/components/modal.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/components/options.tsx` & `pygwalker-0.1.9.1/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/components/button/default.tsx` & `pygwalker-0.1.9.1/app/src/components/button/default.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/components/button/primary.tsx` & `pygwalker-0.1.9.1/app/src/components/button/primary.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/components/codeExportModal/index.tsx` & `pygwalker-0.1.9.1/app/src/components/codeExportModal/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/components/codeExportModal/saveConfigButton.tsx` & `pygwalker-0.1.9.1/app/src/components/codeExportModal/saveConfigButton.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/dataSource/index.ts` & `pygwalker-0.1.9.1/app/src/dataSource/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/interfaces/index.ts` & `pygwalker-0.1.9.1/app/src/interfaces/index.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/app/src/utils/save.ts` & `pygwalker-0.1.9.1/app/src/utils/save.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/__init__.py` & `pygwalker-0.1.9.1/pygwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/base.py` & `pygwalker-0.1.9.1/pygwalker/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/gwalker.py` & `pygwalker-0.1.9.1/pygwalker/gwalker.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         gid = global_gid
         global_gid += 1
     df = df.sample(frac=1)
     kwargs["sourceInvokeCode"] = get_formated_spec_params_code(
         inspect.stack()[1].code_context[0]
     )
     kwargs["spec"] = get_spec_json(kwargs.get("spec", ""))
+    kwargs["id"] = gid
     html = to_html(
         df, gid, env=env, fieldSpecs=fieldSpecs, 
         hideDataSourceConfig=hideDataSourceConfig, themeKey=themeKey, dark=dark, **kwargs
     )
     import html as m_html
     srcdoc = m_html.escape(html)
     iframe = \
```

### Comparing `pygwalker-0.1.9/pygwalker/templates/walk.js` & `pygwalker-0.1.9.1/pygwalker/templates/walk.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.1.9.1/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/templates/dist/style.css` & `pygwalker-0.1.9.1/pygwalker/templates/dist/style.css`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/utils/check_update.py` & `pygwalker-0.1.9.1/pygwalker/utils/check_update.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/utils/format_invoke_walk_code.py` & `pygwalker-0.1.9.1/pygwalker/utils/format_invoke_walk_code.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,11 +36,11 @@
     else:
         func.keywords.insert(0, ast.keyword(arg='spec', value=replace_value))
 
     return astor.to_source(func)
 
 
 def get_formated_spec_params_code(code: str) -> str:
-    call_func = _find_walk_func_node(code)
+    call_func = _find_walk_func_node(code.strip())
     if call_func is None:
         return ''
     return _repalce_spec_params_code(call_func)
```

### Comparing `pygwalker-0.1.9/pygwalker/utils/gwalker_props.py` & `pygwalker-0.1.9.1/pygwalker/utils/gwalker_props.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/utils/render.py` & `pygwalker-0.1.9.1/pygwalker/utils/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker/utils/spec.py` & `pygwalker-0.1.9.1/pygwalker/utils/spec.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker_utils/__main__.py` & `pygwalker-0.1.9.1/pygwalker_utils/__main__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pygwalker_utils/config.py` & `pygwalker-0.1.9.1/pygwalker_utils/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/scripts/test-init.py` & `pygwalker-0.1.9.1/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/scripts/test-init.sh` & `pygwalker-0.1.9.1/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/.gitignore` & `pygwalker-0.1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/LICENSE` & `pygwalker-0.1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/README.md` & `pygwalker-0.1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/pyproject.toml` & `pygwalker-0.1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.9/PKG-INFO` & `pygwalker-0.1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygwalker
-Version: 0.1.9
+Version: 0.1.9.1
 Summary: pygwalker: Combining Jupyter Notebook with a Tableau-like UI
 Project-URL: homepage, https://github.com/Kanaries/pygwalker
 Project-URL: repository, https://github.com/Kanaries/pygwalker
 Author-email: "Asm.Def" <woojson@zju.edu.cn>
 License-File: LICENSE
 Keywords: data-analysis,data-exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pygwalker Version: 0.1.9 Summary: pygwalker:
+Metadata-Version: 2.1 Name: pygwalker Version: 0.1.9.1 Summary: pygwalker:
 Combining Jupyter Notebook with a Tableau-like UI Project-URL: homepage, https:
 //github.com/Kanaries/pygwalker Project-URL: repository, https://github.com/
 Kanaries/pygwalker Author-email: "Asm.Def"
 zju.edu.cn> License-File: LICENSE Keywords: data-analysis,data-
 exploration,dataframe,jupyter,pandas,tableau,tableau-alternative,visualization
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Requires-Python: >=3.6 Requires-Dist:
```

