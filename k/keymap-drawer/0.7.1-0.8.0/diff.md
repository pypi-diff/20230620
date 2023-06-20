# Comparing `tmp/keymap_drawer-0.7.1-py3-none-any.whl.zip` & `tmp/keymap_drawer-0.8.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 46564 bytes, number of entries: 29
+Zip file size: 48686 bytes, number of entries: 30
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 keymap_drawer/__init__.py
 -rw-r--r--  2.0 unx     6741 b- defN 80-Jan-01 00:00 keymap_drawer/__main__.py
--rw-r--r--  2.0 unx     9260 b- defN 80-Jan-01 00:00 keymap_drawer/config.py
--rw-r--r--  2.0 unx    13227 b- defN 80-Jan-01 00:00 keymap_drawer/draw.py
+-rw-r--r--  2.0 unx     9464 b- defN 80-Jan-01 00:00 keymap_drawer/config.py
+-rw-r--r--  2.0 unx    13787 b- defN 80-Jan-01 00:00 keymap_drawer/draw.py
+-rw-r--r--  2.0 unx     5784 b- defN 80-Jan-01 00:00 keymap_drawer/dts.py
 -rw-r--r--  2.0 unx     5798 b- defN 80-Jan-01 00:00 keymap_drawer/glyph.py
 -rw-r--r--  2.0 unx     9388 b- defN 80-Jan-01 00:00 keymap_drawer/keymap.py
--rw-r--r--  2.0 unx    16947 b- defN 80-Jan-01 00:00 keymap_drawer/parse.py
+-rw-r--r--  2.0 unx    15866 b- defN 80-Jan-01 00:00 keymap_drawer/parse.py
 -rw-r--r--  2.0 unx    12301 b- defN 80-Jan-01 00:00 keymap_drawer/physical_layout.py
 -rw-r--r--  2.0 unx     4183 b- defN 80-Jan-01 00:00 resources/qmk_layouts/adv360.json
 -rw-r--r--  2.0 unx     2114 b- defN 80-Jan-01 00:00 resources/qmk_layouts/berylline.json
 -rw-r--r--  2.0 unx     2267 b- defN 80-Jan-01 00:00 resources/qmk_layouts/chocofi.json
 -rw-r--r--  2.0 unx     2437 b- defN 80-Jan-01 00:00 resources/qmk_layouts/clog.json
 -rw-r--r--  2.0 unx     3502 b- defN 80-Jan-01 00:00 resources/qmk_layouts/corne_rotated.json
 -rw-r--r--  2.0 unx     3684 b- defN 80-Jan-01 00:00 resources/qmk_layouts/fingerpunch@ffkb.json
@@ -19,13 +20,13 @@
 -rw-r--r--  2.0 unx     2537 b- defN 80-Jan-01 00:00 resources/qmk_layouts/klotz.json
 -rw-r--r--  2.0 unx     1783 b- defN 80-Jan-01 00:00 resources/qmk_layouts/osprey.json
 -rw-r--r--  2.0 unx     2466 b- defN 80-Jan-01 00:00 resources/qmk_layouts/paroxysm.json
 -rw-r--r--  2.0 unx     3728 b- defN 80-Jan-01 00:00 resources/qmk_layouts/revxlp.json
 -rw-r--r--  2.0 unx     2838 b- defN 80-Jan-01 00:00 resources/qmk_layouts/rufous.json
 -rw-r--r--  2.0 unx     2803 b- defN 80-Jan-01 00:00 resources/qmk_layouts/totem.json
 -rw-r--r--  2.0 unx     6244 b- defN 80-Jan-01 00:00 resources/zmk_keyboard_layouts.yaml
--rw-r--r--  2.0 unx    26355 b- defN 80-Jan-01 00:00 keymap_drawer-0.7.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 keymap_drawer-0.7.1.dist-info/WHEEL
--rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 keymap_drawer-0.7.1.dist-info/LICENSE
--rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 keymap_drawer-0.7.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2542 b- defN 16-Jan-01 00:00 keymap_drawer-0.7.1.dist-info/RECORD
-29 files, 159846 bytes uncompressed, 42446 bytes compressed:  73.4%
+-rw-r--r--  2.0 unx    26110 b- defN 80-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1069 b- defN 80-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2619 b- defN 16-Jan-01 00:00 keymap_drawer-0.8.0.dist-info/RECORD
+30 files, 165145 bytes uncompressed, 44452 bytes compressed:  73.1%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: keymap_drawer/config.py
 Comment: 
 
 Filename: keymap_drawer/draw.py
 Comment: 
 
+Filename: keymap_drawer/dts.py
+Comment: 
+
 Filename: keymap_drawer/glyph.py
 Comment: 
 
 Filename: keymap_drawer/keymap.py
 Comment: 
 
 Filename: keymap_drawer/parse.py
@@ -66,23 +69,23 @@
 
 Filename: resources/qmk_layouts/totem.json
 Comment: 
 
 Filename: resources/zmk_keyboard_layouts.yaml
 Comment: 
 
-Filename: keymap_drawer-0.7.1.dist-info/METADATA
+Filename: keymap_drawer-0.8.0.dist-info/METADATA
 Comment: 
 
-Filename: keymap_drawer-0.7.1.dist-info/WHEEL
+Filename: keymap_drawer-0.8.0.dist-info/WHEEL
 Comment: 
 
-Filename: keymap_drawer-0.7.1.dist-info/LICENSE
+Filename: keymap_drawer-0.8.0.dist-info/LICENSE
 Comment: 
 
-Filename: keymap_drawer-0.7.1.dist-info/entry_points.txt
+Filename: keymap_drawer-0.8.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: keymap_drawer-0.7.1.dist-info/RECORD
+Filename: keymap_drawer-0.8.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## keymap_drawer/config.py

```diff
@@ -141,14 +141,18 @@
         .icon-tabler > path[stroke="none"][fill="none"] {
             visibility: collapse;
         }
         /* End Tabler Icons Cleanup */
         """
     )
 
+    # shrink font size for legends wider than this many chars, set to 0 to disable
+    # ideal value depends on the font size defined in svg_style and width of the boxes
+    shrink_wide_legends: int = 7
+
     # height in pixels for glyphs in different key fields
     glyph_tap_size: int = 14
     glyph_hold_size: int = 12
     glyph_shifted_size: int = 10
 
     # mapping of glyph names to be used in key fields to their SVG definitions
     glyphs: dict[str, str] = {}
```

## keymap_drawer/draw.py

```diff
@@ -39,21 +39,31 @@
 
     def _draw_rect(self, p: Point, w: float, h: float, classes: Sequence[str]) -> None:
         self.out.write(
             f'<rect rx="{self.cfg.key_rx}" ry="{self.cfg.key_ry}" x="{p.x - w / 2}" y="{p.y - h / 2}" '
             f'width="{w}" height="{h}"{self._to_class_str(classes)}/>\n'
         )
 
+    def _get_scaling(self, width: int) -> str:
+        if not self.cfg.shrink_wide_legends or width <= self.cfg.shrink_wide_legends:
+            return ""
+        return f' style="font-size: {max(60.0, 100 * self.cfg.shrink_wide_legends / width):.0f}%"'
+
     def _draw_text(self, p: Point, word: str, classes: Sequence[str]) -> None:
         if not word:
             return
-        self.out.write(f'<text x="{p.x}" y="{p.y}"{self._to_class_str(classes)}>{escape(word)}</text>\n')
+        self.out.write(
+            f'<text x="{p.x}" y="{p.y}"{self._to_class_str(classes)}{self._get_scaling(len(word))}>'
+            f"{escape(word)}</text>\n"
+        )
 
     def _draw_textblock(self, p: Point, words: Sequence[str], classes: Sequence[str], shift: float = 0) -> None:
-        self.out.write(f'<text x="{p.x}" y="{p.y}"{self._to_class_str(classes)}>\n')
+        self.out.write(
+            f'<text x="{p.x}" y="{p.y}"{self._to_class_str(classes)}{self._get_scaling(max(len(w) for w in words))}>\n'
+        )
         dy_0 = (len(words) - 1) * (self.cfg.line_spacing * (1 + shift) / 2)
         self.out.write(f'<tspan x="{p.x}" dy="-{dy_0}em">{escape(words[0])}</tspan>')
         for word in words[1:]:
             self.out.write(f'<tspan x="{p.x}" dy="{self.cfg.line_spacing}em">{escape(word)}</tspan>')
         self.out.write("</text>\n")
 
     def _draw_glyph(self, p: Point, name: str, legend_type: LegendType, classes: Sequence[str]) -> None:
@@ -89,14 +99,20 @@
         start = f"M{p_1.x},{p_1.y}"
         diff = p_2 - p_1
         if shorten and shorten < (magn := abs(diff)):
             diff = (1 - shorten / magn) * diff
         line = f"l{diff.x},{diff.y}"
         self.out.write(f'<path d="{start} {line}" class="combo"/>\n')
 
+    def print_layer_header(self, p: Point, header: str) -> None:
+        """Print a layer header that precedes the layer visualization."""
+        if self.cfg.append_colon_to_layer_header:
+            header += ":"
+        self.out.write(f'<text x="{p.x}" y="{p.y}" class="label">{escape(header)}</text>\n')
+
     def print_key(self, p_0: Point, p_key: PhysicalKey, l_key: LayoutKey) -> None:
         """
         Given anchor coordinates p_0, print SVG code for a rectangle with text representing
         the key, which is described by its physical representation (p_key) and what it does in
         the given layer (l_key).
         """
         p, w, h, r = (
@@ -285,18 +301,15 @@
 
         p = Point(self.cfg.outer_pad_w, 0.0)
         for name, layer_keys in layers.items():
             # per-layer class group
             self.out.write(f'<g class="layer-{name}">\n')
 
             # draw layer name
-            layer_header = name
-            if self.cfg.append_colon_to_layer_header:
-                layer_header += ":"
-            self._draw_text(p + Point(0, self.cfg.outer_pad_h / 2), layer_header, classes=["label"])
+            self.print_layer_header(p + Point(0, self.cfg.outer_pad_h / 2), name)
 
             # get offsets added by combo alignments, draw keys and combos
             p += Point(0, self.cfg.outer_pad_h + offsets_per_layer[name][0])
             self.print_layer(p, layer_keys, combos_per_layer[name], empty_layer=combos_only)
             p += Point(0, self.layout.height + offsets_per_layer[name][1])
 
             self.out.write("</g>\n")
```

## keymap_drawer/parse.py

```diff
@@ -1,22 +1,21 @@
 """Module to parse QMK/ZMK keymaps into KeymapData and then dump them to dict."""
 import re
 import json
-from io import StringIO, TextIOWrapper
+from io import TextIOWrapper
 from pathlib import Path
 from abc import ABC
 from itertools import chain
 from typing import Sequence
 
 import yaml
-import pyparsing as pp
-from pcpp.preprocessor import Preprocessor, OutputDirective, Action  # type: ignore
 
 from .keymap import LayoutKey, ComboSpec, KeymapData
 from .config import ParseConfig
+from .dts import DeviceTree
 
 
 ZMK_LAYOUTS_PATH = Path(__file__).parent.parent / "resources" / "zmk_keyboard_layouts.yaml"
 
 
 class KeymapParser(ABC):
     """Abstract base class for parsing firmware keymap representations."""
@@ -30,14 +29,15 @@
     ):
         self.cfg = config
         self.columns = columns if columns is not None else 0
         self.layer_names: list[str] | None = layer_names
         self.base_keymap = base_keymap
         self.layer_activated_from: dict[int, set[int]] = {}
         self.trans_key = LayoutKey.from_key_spec(self.cfg.trans_legend)
+        self.raw_binding_map = self.cfg.raw_binding_map.copy()
 
     def update_layer_activated_from(self, from_layer: int | None, to_layer: int, key_positions: Sequence[int]) -> None:
         """
         Update the data structure that keeps track of what keys were held (i.e. momentary layer keys)
         in order to activate a given layer. Also considers what keys were already being held in order
         to activate the `from_layer` that the `to_layer` is being activated from.
 
@@ -93,16 +93,16 @@
     _lt_re = re.compile(r"LT\((\d+), *(\S+)\)")
     _osm_re = re.compile(r"OSM\(MOD_(\S+)\)")
     _osl_re = re.compile(r"OSL\((\d+)\)")
 
     def _str_to_key(  # pylint: disable=too-many-return-statements
         self, key_str: str, current_layer: int, key_positions: Sequence[int]
     ) -> LayoutKey:
-        if key_str in self.cfg.raw_binding_map:
-            return LayoutKey.from_key_spec(self.cfg.raw_binding_map[key_str])
+        if key_str in self.raw_binding_map:
+            return LayoutKey.from_key_spec(self.raw_binding_map[key_str])
         if self.cfg.skip_binding_parsing:
             return LayoutKey(tap=key_str)
 
         assert self.layer_names is not None
 
         def mapped(key: str) -> LayoutKey:
             return LayoutKey.from_key_spec(self.cfg.qmk_keycode_map.get(key, key.replace("_", " ")))
@@ -169,37 +169,44 @@
 
         return layout, keymap_data
 
 
 class ZmkKeymapParser(KeymapParser):
     """Parser for ZMK devicetree keymaps, using C preprocessor and hacky pyparsing-based parsers."""
 
-    _bindings_re = re.compile(r"(?<!sensor-)bindings = <(.*?)>")
-    _keypos_re = re.compile(r"key-positions = <(.*?)>")
-    _layers_re = re.compile(r"layers = <(.*?)>")
-    _label_re = re.compile(r'label = "(.*?)"')
-    _compatible_re = re.compile(r'compatible = "(.*?)"')
-    _nodelabel_re = re.compile(r"([\w-]+) *: *([\w-]+) *{")
     _numbers_re = re.compile(r"N(UM(BER)?_)?(\d)")
 
     def __init__(
         self,
         config: ParseConfig,
         columns: int | None,
         base_keymap: KeymapData | None = None,
         layer_names: list[str] | None = None,
     ):
         super().__init__(config, columns, base_keymap, layer_names)
-        self.hold_tap_labels = {"&mt", "&lt"}
+        self.hold_taps = {"&mt": ["&kp", "&kp"], "&lt": ["&mo", "&kp"]}
+        self.mod_morphs: dict[str, list[str]] = {}
+        self.sticky_keys = {"&sk": ["&kp"], "&sl": ["&mo"]}
+
+    def _update_raw_binding_map(self, dts: DeviceTree) -> None:
+        raw_keys = list(self.raw_binding_map.keys())
+        prep_keys = dts.preprocess_extra_data("\n".join(raw_keys)).splitlines()
+        assert len(raw_keys) == len(
+            prep_keys
+        ), "Keys in parse_config.raw_binding_map did not preprocess properly, please check for issues"
+        for old, new in zip(raw_keys, prep_keys):
+            if new != old:
+                self.raw_binding_map[new] = self.raw_binding_map[old]
+                del self.raw_binding_map[old]
 
-    def _str_to_key(  # pylint: disable=too-many-return-statements
+    def _str_to_key(  # pylint: disable=too-many-return-statements,too-many-locals
         self, binding: str, current_layer: int | None, key_positions: Sequence[int], no_shifted: bool = False
     ) -> LayoutKey:
-        if binding in self.cfg.raw_binding_map:
-            return LayoutKey.from_key_spec(self.cfg.raw_binding_map[binding])
+        if binding in self.raw_binding_map:
+            return LayoutKey.from_key_spec(self.raw_binding_map[binding])
         if self.cfg.skip_binding_parsing:
             return LayoutKey(tap=binding)
 
         assert self.layer_names is not None
 
         def mapped(key: str) -> LayoutKey:
             mapped = LayoutKey.from_key_spec(
@@ -208,158 +215,119 @@
                 )
             )
             if no_shifted:
                 mapped.shifted = ""
             return mapped
 
         match binding.split():
-            case ["&none"]:
+            case ["&none", *_]:
                 return LayoutKey()
             case ["&trans"]:
                 return self.trans_key
-            case [ref]:
-                return LayoutKey(tap=ref)
+            case [ref, *_] if ref in self.mod_morphs:
+                tap_key = self._str_to_key(self.mod_morphs[ref][0], current_layer, key_positions)
+                shifted_key = self._str_to_key(self.mod_morphs[ref][1], current_layer, key_positions)
+                return LayoutKey(tap=tap_key.tap, hold=tap_key.hold, shifted=shifted_key.tap)
             case ["&kp", par]:
                 return mapped(par)
-            case ["&sk", par]:
-                l_key = mapped(par)
+            case [ref, par] if ref in self.sticky_keys:
+                l_key = self._str_to_key(f"{self.sticky_keys[ref][0]} {par}", current_layer, key_positions)
                 return LayoutKey(tap=l_key.tap, hold=self.cfg.sticky_label, shifted=l_key.shifted)
             case [("&out" | "&bt" | "&ext_power" | "&rgb_ug"), *pars]:
                 return LayoutKey(tap=" ".join(pars).replace("_", " ").replace(" SEL ", " "))
-            case [("&mo" | "&to" | "&tog" | "&sl") as behavior, par]:
-                if behavior in ("&mo", "&sl"):
+            case [("&mo" | "&to" | "&tog") as behavior, par]:
+                if behavior in ("&mo",):
                     self.update_layer_activated_from(current_layer, int(par), key_positions)
-                return LayoutKey(
-                    tap=self.layer_names[int(par)], hold=self.cfg.sticky_label if behavior == "&sl" else ""
-                )
-            case [ref, hold_par, tap_par] if ref in self.hold_tap_labels:
-                try:
-                    hold = self.layer_names[int(hold_par)]
-                    self.update_layer_activated_from(current_layer, int(hold_par), key_positions)
-                except (ValueError, IndexError):  # not a layer-tap, so maybe a keycode?
-                    hold = mapped(hold_par).tap
-                tap_key = mapped(tap_par)
-                return LayoutKey(tap=tap_key.tap, hold=hold, shifted=tap_key.shifted)
+                return LayoutKey(tap=self.layer_names[int(par)])
+            case [ref, hold_par, tap_par] if ref in self.hold_taps:
+                hold_key = self._str_to_key(f"{self.hold_taps[ref][0]} {hold_par}", current_layer, key_positions)
+                tap_key = self._str_to_key(f"{self.hold_taps[ref][1]} {tap_par}", current_layer, key_positions)
+                return LayoutKey(tap=tap_key.tap, hold=hold_key.tap, shifted=tap_key.shifted)
+            case [ref] | [ref, "0"]:
+                return LayoutKey(tap=ref)
         return LayoutKey(tap=binding)
 
-    def _get_prepped(self, in_str: str, file_name: str | None = None) -> str:
-        if self.cfg.preprocess:
-
-            def include_handler(*args):
-                raise OutputDirective(Action.IgnoreAndPassThrough)
-
-            preprocessor = Preprocessor()
-            preprocessor.line_directive = None
-            preprocessor.on_include_not_found = include_handler
-            preprocessor.parse(in_str, source=file_name)
-            with StringIO() as f_out:
-                preprocessor.write(f_out)
-                prepped = f_out.getvalue()
-        else:
-            prepped = in_str
-        return re.sub(r"^\s*#.*?$", "", prepped)
+    def _update_behaviors(self, dts: DeviceTree) -> None:
+        def get_behavior_bindings(compatible_value: str, n_bindings: int) -> dict[str, list[str]]:
+            out = {}
+            for node in dts.get_compatible_nodes(compatible_value):
+                if not (bindings := node.get_phandle_array("(?<!sensor-)bindings")):
+                    raise RuntimeError(f'Cannot parse bindings for behavior "{node.name}"')
+                if node.label is None:
+                    raise RuntimeError(f'Cannot find label for behavior "{node.name}"')
+                out[f"&{node.label}"] = bindings[:n_bindings]
+            return out
+
+        self.hold_taps |= get_behavior_bindings("zmk,behavior-hold-tap", 2)
+        self.mod_morphs |= get_behavior_bindings("zmk,behavior-mod-morph", 2)
+        self.sticky_keys |= get_behavior_bindings("zmk,behavior-sticky-key", 1)
+
+    def _get_layers(self, dts: DeviceTree) -> dict[str, list[LayoutKey]]:
+        if not (layer_parents := dts.get_compatible_nodes("zmk,keymap")):
+            raise RuntimeError('Could not find any keymap nodes with "zmk,keymap" compatible property')
 
-    def _find_nodes_with_name(
-        self, parsed: pp.ParseResults, node_name: str | None = None
-    ) -> list[tuple[str, pp.ParseResults]]:
-        found_nodes = []
-        for elt_p, elt_n in zip(parsed[:-1], parsed[1:]):
-            if (
-                isinstance(elt_p, str)
-                and isinstance(elt_n, pp.ParseResults)
-                and (node_name is None or elt_p.rsplit(":", maxsplit=1)[-1] == node_name)
-            ):
-                found_nodes.append((elt_p, elt_n))
-        return found_nodes
-
-    def _update_hold_tap_labels(self, parsed: Sequence[pp.ParseResults]) -> None:
-        behavior_parents = chain.from_iterable(self._find_nodes_with_name(node, "behaviors") for node in parsed)
-        behavior_nodes = {
-            node_name: " ".join(item for item in node.as_list() if isinstance(item, str))
-            for node_name, node in chain.from_iterable(self._find_nodes_with_name(node) for _, node in behavior_parents)
-        }
-        for name, node_str in behavior_nodes.items():
-            if ":" not in name:
-                continue
-            if (m := self._compatible_re.search(node_str)) and m.group(1) == "zmk,behavior-hold-tap":
-                self.hold_tap_labels.add("&" + name.split(":", 1)[0])
-
-    def _get_layers(self, parsed: Sequence[pp.ParseResults]) -> dict[str, list[LayoutKey]]:
-        layer_parents = chain.from_iterable(self._find_nodes_with_name(node, "keymap") for node in parsed)
-        layer_nodes = {
-            node_name: " ".join(item for item in node.as_list() if isinstance(item, str))
-            for node_name, node in chain.from_iterable(self._find_nodes_with_name(node) for _, node in layer_parents)
-        }
+        layer_nodes = [node for parent in layer_parents for node in parent.children]
         if self.layer_names is None:
             self.layer_names = [
-                m.group(1) if (m := self._label_re.search(node_str)) else node_name
-                for node_name, node_str in layer_nodes.items()
+                node.get_string("label") or node.name.removeprefix("layer_").removesuffix("_layer")
+                for node in layer_nodes
             ]
         else:
             assert (l_u := len(self.layer_names)) == (
                 l_p := len(layer_nodes)
             ), f"Length of provided layer name list ({l_u}) does not match the number of parsed layers ({l_p})"
 
         layers = {}
-        for layer_ind, node_str in enumerate(layer_nodes.values()):
-            layer_name = self.layer_names[layer_ind]
-            try:
-                key_strs = [
-                    f"&{stripped}"
-                    for binding in self._bindings_re.search(node_str).group(1).split("&")  # type: ignore
-                    if (stripped := binding.strip().removeprefix("&"))
+        for layer_ind, node in enumerate(layer_nodes):
+            if bindings := node.get_phandle_array(r"(?<!sensor-)bindings"):
+                layers[self.layer_names[layer_ind]] = [
+                    self._str_to_key(binding, layer_ind, [i]) for i, binding in enumerate(bindings)
                 ]
-                layers[layer_name] = [self._str_to_key(binding, layer_ind, [i]) for i, binding in enumerate(key_strs)]
-            except AttributeError:
-                continue
+            else:
+                raise RuntimeError(f'Could not parse `bindings` property under layer node "{node.name}"')
         return layers
 
-    def _get_combos(self, parsed: Sequence[pp.ParseResults]) -> list[ComboSpec]:
+    def _get_combos(self, dts: DeviceTree) -> list[ComboSpec]:
         assert self.layer_names is not None
-        combo_parents = chain.from_iterable(self._find_nodes_with_name(node, "combos") for node in parsed)
-        combo_nodes = chain.from_iterable(self._find_nodes_with_name(node) for _, node in combo_parents)
+        if not (combo_parents := dts.get_compatible_nodes("zmk,combos")):
+            return []
+        combo_nodes = chain.from_iterable(parent.children for parent in combo_parents)
 
         combos = []
-        for name, node in combo_nodes:
-            try:
-                node_str = " ".join(item for item in node.as_list() if isinstance(item, str))
-                binding = self._bindings_re.search(node_str).group(1)  # type: ignore
-                key_pos = [int(pos) for pos in self._keypos_re.search(node_str).group(1).split()]  # type: ignore
-                combo = {
-                    "k": self._str_to_key(binding, None, key_pos, no_shifted=True),  # ignore current layer for combos
-                    "p": key_pos,
-                }
-                if m := self._layers_re.search(node_str):
-                    combo["l"] = [self.layer_names[int(layer)] for layer in m.group(1).split()]
-
-                # see if combo had additional properties specified in the config, if so merge them in
-                cfg_combo = ComboSpec.normalize_fields(self.cfg.zmk_combos.get(name, {}))
-                combos.append(ComboSpec(**(combo | cfg_combo)))
-            except (AttributeError, ValueError):
-                continue
+        for node in combo_nodes:
+            if not (bindings := node.get_phandle_array("bindings")):
+                raise RuntimeError(f'Could not parse `bindings` for combo node "{node.name}"')
+            if not (key_pos_strs := node.get_array("key-positions")):
+                raise RuntimeError(f'Could not parse `key-positions` for combo node "{node.name}"')
+
+            key_pos = [int(pos) for pos in key_pos_strs]
+            combo = {
+                "k": self._str_to_key(bindings[0], None, key_pos, no_shifted=True),  # ignore current layer for combos
+                "p": key_pos,
+            }
+            if layers := node.get_array("layers"):
+                combo["l"] = [self.layer_names[int(layer)] for layer in layers]
+
+            # see if combo had additional properties specified in the config, if so merge them in
+            cfg_combo = ComboSpec.normalize_fields(self.cfg.zmk_combos.get(node.name, {}))
+            combos.append(ComboSpec(**(combo | cfg_combo)))
         return combos
 
     def _parse(self, in_str: str, file_name: str | None = None) -> tuple[dict, KeymapData]:
         """
         Parse a ZMK keymap with its content and path and return the layout spec and KeymapData to be dumped to YAML.
         """
-        prepped = self._get_prepped(in_str, file_name)
-        parsed = [
-            node
-            for node in (
-                pp.nested_expr("{", "};")
-                .ignore("//" + pp.SkipTo(pp.lineEnd))
-                .ignore(pp.c_style_comment)
-                .parse_string("{ " + self._nodelabel_re.sub(r"\1:\2 {", prepped) + " };")[0]
-            )
-            if isinstance(node, pp.ParseResults)
-        ]
-        self._update_hold_tap_labels(parsed)
-        layers = self._get_layers(parsed)
-        combos = self._get_combos(parsed)
+        dts = DeviceTree(in_str, file_name, self.cfg.preprocess)
+
+        if self.cfg.preprocess and self.raw_binding_map:
+            self._update_raw_binding_map(dts)
+
+        self._update_behaviors(dts)
+        layers = self._get_layers(dts)
+        combos = self._get_combos(dts)
         layers = self.add_held_keys(layers)
 
         keymap_data = KeymapData(layers=layers, combos=combos, layout=None, config=None)
 
         if not file_name:
             return {}, keymap_data
```

## Comparing `keymap_drawer-0.7.1.dist-info/METADATA` & `keymap_drawer-0.8.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keymap-drawer
-Version: 0.7.1
+Version: 0.8.0
 Summary: A module and CLI tool to help parse and draw keyboard layouts.
 Home-page: https://github.com/caksoylar/keymap-drawer
 License: MIT
 Author: Cem Aksoylar
 Author-email: caksoylar@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -85,22 +85,17 @@
 
 - **ZMK**: `.keymap` files are used for parsing. These will be preprocessed similar to the ZMK build system, so `#define`'s and `#include`s will be expanded.
 
   ```sh
   keymap parse -c 10 -z ~/zmk-config/config/cradio.keymap >sweep_keymap.yaml
   ```
 
-  Currently combos, hold-taps (including custom ones), layer names and sticky keys (`&sk`/`&sl`) can be determined via parsing.
+  Currently combos, hold-taps, mod-morphs, sticky keys and layer names can be determined via parsing.
   For layer names, the value of the `label` property will take precedence over the layer's node name if provided.
 
-  > **Warning**
-  >
-  > Parsing rules currently require that your keymap have nodes named `keymap` and `combos` that are nested one level-deep from the root.
-  > (These conditions hold for most keymaps by convention.)
-
 As an alternative to parsing, you can also check out the [examples](examples/) to find a layout similar to yours to use as a starting point.
 
 ### Tweaking the produced keymap representation
 
 While the parsing step aims to create a decent starting point, you will likely want to make certain tweaks to the produced keymap representation.
 Please refer to [the keymap schema specification](KEYMAP_SPEC.md) while making changes:
```

## Comparing `keymap_drawer-0.7.1.dist-info/LICENSE` & `keymap_drawer-0.8.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `keymap_drawer-0.7.1.dist-info/RECORD` & `keymap_drawer-0.8.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 keymap_drawer/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 keymap_drawer/__main__.py,sha256=k-j2SVcBBfoJ-zRW8rrDuH0nr2GzEhScadabb0HnREM,6741
-keymap_drawer/config.py,sha256=YGZLdRNo4pWLirYOiFdvPmSjlYdMQhKLnKfAXmkvOSk,9260
-keymap_drawer/draw.py,sha256=wbSsxRezfsgcZCm3f7_KfkwyvfeuU1EmiC9tRJvYeUM,13227
+keymap_drawer/config.py,sha256=XvhCymSdfeWj7Vt2WePigyeIyPKnODFYqqpArRxzsYw,9464
+keymap_drawer/draw.py,sha256=xPMt0meDsywAjA1V4GfwsBhDj-KRmOJunBjPX-FdsOY,13787
+keymap_drawer/dts.py,sha256=bBrkdwDxfNYcag5ppyp5KoemZ1SJjMsFqsLbDs5I0zo,5784
 keymap_drawer/glyph.py,sha256=bLDtb_Zcl6fHMCxJ6JGcgogcXhb-U84fkEHDckDvR1s,5798
 keymap_drawer/keymap.py,sha256=saEQG30NgVftS7cax60aHmx9i1WHiEm4RZdm1p0yGSk,9388
-keymap_drawer/parse.py,sha256=LKMrrhSqVwEJuNJrmBQF-mIoMZWhS2Y8isd0_W-2ll0,16947
+keymap_drawer/parse.py,sha256=wGWeY9D3YVYZWh_dOjZY9-jeFi7h9T2GuRDejIKTh74,15866
 keymap_drawer/physical_layout.py,sha256=xKtFg3p9DjVBURHdA0KpU6vPKFr3gkxmaDc0cjoo1v0,12301
 resources/qmk_layouts/adv360.json,sha256=MM5xOXcn9-O4hzei6RPJoFhLbqz86fEqczdqGU6N2uE,4183
 resources/qmk_layouts/berylline.json,sha256=lsTJzCcQ78TeYUYoBa67fAb4cm6_phrwL9eHphw4qq4,2114
 resources/qmk_layouts/chocofi.json,sha256=Lsayi_fcsljEGGmQwmI_KLUf7snLy_qEqSSVbFcpEkQ,2267
 resources/qmk_layouts/clog.json,sha256=wzkTRyevr0OkZoFNJkWRQ8APpKQ3S5cBiuwdxSnTRt8,2437
 resources/qmk_layouts/corne_rotated.json,sha256=8hTZZSuP4C2p9ywDtnW4o8ThNC9Zw0ue9qwGX1aaOXk,3502
 resources/qmk_layouts/fingerpunch@ffkb.json,sha256=toAtmnP65nnEGE-alZUGShf5E-l58vvl3nipRBBh9hQ,3684
@@ -18,12 +19,12 @@
 resources/qmk_layouts/klotz.json,sha256=jV-tpL1FixKxk78_EnW4UvfricUYsFfFbWf-j1SeY7Y,2537
 resources/qmk_layouts/osprey.json,sha256=_2qw3uVKeuZNybUEhWpcy0U831lldj1LfH6szXeh_j4,1783
 resources/qmk_layouts/paroxysm.json,sha256=y17689V0dqnDhmDgxlzw1kPnNaQub-GHgrsa4-kEV_8,2466
 resources/qmk_layouts/revxlp.json,sha256=FRFgeD6PAQAwDg1gVEZPJl7-tPdTFv7HSQ7Pc-62hgI,3728
 resources/qmk_layouts/rufous.json,sha256=6VtvTikJtgEYx0xfkSTT9_KaLdW5TfmoFoaz0uf5GYQ,2838
 resources/qmk_layouts/totem.json,sha256=HXKwNwjT9lByzFhqlAFhxhhp_SYerOsTasJwUppCh4U,2803
 resources/zmk_keyboard_layouts.yaml,sha256=jC_CzZWmyIXWAIxSER877imSqI0u_0trMzxBLQDIsL0,6244
-keymap_drawer-0.7.1.dist-info/METADATA,sha256=ty8R5cQDZTyHNU5a1MOiQcygJ8fbS0utz9wtNbwBUB8,26355
-keymap_drawer-0.7.1.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-keymap_drawer-0.7.1.dist-info/LICENSE,sha256=ym_5D56d6k2MroMU8y9ZDt1ZUI4H7PYgbfa87rNFCaM,1069
-keymap_drawer-0.7.1.dist-info/entry_points.txt,sha256=kog7wHfRs-vFQWhh8V3H-Ra4UPbW1nINE9VHJZ1aK2w,54
-keymap_drawer-0.7.1.dist-info/RECORD,,
+keymap_drawer-0.8.0.dist-info/METADATA,sha256=3rFGcmy7cEIaY9grVDm8lNsZ05eb75rxAA7Ld1dT7ko,26110
+keymap_drawer-0.8.0.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
+keymap_drawer-0.8.0.dist-info/LICENSE,sha256=ym_5D56d6k2MroMU8y9ZDt1ZUI4H7PYgbfa87rNFCaM,1069
+keymap_drawer-0.8.0.dist-info/entry_points.txt,sha256=kog7wHfRs-vFQWhh8V3H-Ra4UPbW1nINE9VHJZ1aK2w,54
+keymap_drawer-0.8.0.dist-info/RECORD,,
```

