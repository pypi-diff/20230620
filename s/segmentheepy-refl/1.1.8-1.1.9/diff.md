# Comparing `tmp/segmentheepy_refl-1.1.8-py3-none-any.whl.zip` & `tmp/segmentheepy_refl-1.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11037 bytes, number of entries: 9
+Zip file size: 11048 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jan-31 09:33 segmenthee/__init__.py
--rw-rw-r--  2.0 unx    25566 b- defN 23-Mar-28 06:48 segmenthee/cart_api.py
+-rw-rw-r--  2.0 unx    25625 b- defN 23-Mar-31 11:07 segmenthee/cart_api.py
 -rw-rw-r--  2.0 unx      766 b- defN 23-Mar-02 12:58 segmenthee/config.py
--rw-rw-r--  2.0 unx     2023 b- defN 23-Mar-24 16:01 segmenthee/parser_api.py
--rw-rw-r--  2.0 unx    13742 b- defN 23-Mar-28 06:54 segmenthee/shop.py
--rw-rw-r--  2.0 unx      261 b- defN 23-Mar-28 12:34 segmentheepy_refl-1.1.8.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Mar-28 12:34 segmentheepy_refl-1.1.8.dist-info/WHEEL
--rw-rw-r--  2.0 unx       11 b- defN 23-Mar-28 12:34 segmentheepy_refl-1.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      726 b- defN 23-Mar-28 12:34 segmentheepy_refl-1.1.8.dist-info/RECORD
-9 files, 43187 bytes uncompressed, 9783 bytes compressed:  77.3%
+-rw-rw-r--  2.0 unx     2023 b- defN 23-Mar-31 10:27 segmenthee/parser_api.py
+-rw-rw-r--  2.0 unx    13736 b- defN 23-Mar-31 11:08 segmenthee/shop.py
+-rw-rw-r--  2.0 unx      261 b- defN 23-Mar-31 12:23 segmentheepy_refl-1.1.9.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Mar-31 12:23 segmentheepy_refl-1.1.9.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       11 b- defN 23-Mar-31 12:23 segmentheepy_refl-1.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      726 b- defN 23-Mar-31 12:23 segmentheepy_refl-1.1.9.dist-info/RECORD
+9 files, 43240 bytes uncompressed, 9794 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: segmenthee/parser_api.py
 Comment: 
 
 Filename: segmenthee/shop.py
 Comment: 
 
-Filename: segmentheepy_refl-1.1.8.dist-info/METADATA
+Filename: segmentheepy_refl-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: segmentheepy_refl-1.1.8.dist-info/WHEEL
+Filename: segmentheepy_refl-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: segmentheepy_refl-1.1.8.dist-info/top_level.txt
+Filename: segmentheepy_refl-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: segmentheepy_refl-1.1.8.dist-info/RECORD
+Filename: segmentheepy_refl-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## segmenthee/cart_api.py

```diff
@@ -282,14 +282,17 @@
 
 
 class CouponRejectedEvent(UserActionEvent):
     def __init__(self, time: int, event_label: str):
         super().__init__(time)
         self.event_label = event_label
 
+    def Update(self, prevstate):
+        return prevstate
+
     def skip_update(self) -> bool:
         return True
 
     def is_pageview(self) -> bool:
         return False
```

## segmenthee/shop.py

```diff
@@ -109,20 +109,20 @@
     event_name: str = item.get('en')
 
     if event_name == 'scroll':
         return ProductPageScrollEvent(**kwargs)
 
     if event_name == 'add_to_cart':
         delta_count: int = int(item.get('qty'))
-        delta_total: int = round(float(item.get('val')), 2)
+        delta_total: int = round(float(item.get('val')))
         return CartModifyEvent(hit_time, delta_count, delta_total)
 
     if event_name == 'remove_from_cart':
         delta_count: int = -1 * int(item.get('qty'))
-        delta_total: int = -1 * round(float(item.get('val')), 2)
+        delta_total: int = -1 * round(float(item.get('val')))
         return CartModifyEvent(hit_time, delta_count, delta_total)
 
     if event_name == 'coupon_offered':
         return CouponOfferedEvent(hit_time, item.get('el'))
 
     if event_name == 'coupon_accepted':
         return CouponAcceptedEvent(hit_time, item.get('el'))
```

## Comparing `segmentheepy_refl-1.1.8.dist-info/RECORD` & `segmentheepy_refl-1.1.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 segmenthee/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-segmenthee/cart_api.py,sha256=C2pKUw2tGowp1FcYfqaTZdwhoKwgx1Z95_drowmBxp0,25566
+segmenthee/cart_api.py,sha256=8pKraROA186ETTO83Ivv2P8K_is7uIWdqN9r2HDwOyo,25625
 segmenthee/config.py,sha256=lXea6JINCK44eZP38JaQOlfgVerzFx0e9wDxObuw54c,766
 segmenthee/parser_api.py,sha256=TB-Q8roqNAV_wwYSrdJYchNoC3zTGRKI0die0sN-K-8,2023
-segmenthee/shop.py,sha256=7d7LrIpRAlgF40XxSSzhRDOJ2s8U0-Cr81lK6jMRPqE,13742
-segmentheepy_refl-1.1.8.dist-info/METADATA,sha256=mbiWdzFr_wZpMlpHfyZEVcElopuOGfRfHdSvQyWUI8w,261
-segmentheepy_refl-1.1.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-segmentheepy_refl-1.1.8.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
-segmentheepy_refl-1.1.8.dist-info/RECORD,,
+segmenthee/shop.py,sha256=2X0vL-SqQ2JQqLw2slEpaLrezUb4WmRL3YQ6xQCD2zY,13736
+segmentheepy_refl-1.1.9.dist-info/METADATA,sha256=qzkK3EWojbVkxvj6jnqM8E5fTaA1DVbiLd40mlYe8zk,261
+segmentheepy_refl-1.1.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+segmentheepy_refl-1.1.9.dist-info/top_level.txt,sha256=ESnfgSm7LAnmWZiJ4HDmTbd5B0AemZ20M9sFA5X59IU,11
+segmentheepy_refl-1.1.9.dist-info/RECORD,,
```

