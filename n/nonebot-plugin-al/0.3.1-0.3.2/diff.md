# Comparing `tmp/nonebot_plugin_al-0.3.1.tar.gz` & `tmp/nonebot_plugin_al-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_al-0.3.1.tar", max compression
+gzip compressed data, was "nonebot_plugin_al-0.3.2.tar", max compression
```

## Comparing `nonebot_plugin_al-0.3.1.tar` & `nonebot_plugin_al-0.3.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2023-06-19 16:16:50.043033 nonebot_plugin_al-0.3.1/LICENSE
--rw-r--r--   0        0        0     3793 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/README.md
--rw-r--r--   0        0        0     6478 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/__init__.py
--rw-r--r--   0        0        0    69751 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/api.py
--rw-r--r--   0        0        0     3348 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/bili.py
--rw-r--r--   0        0        0    69109 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/data/eq.json
--rw-r--r--   0        0        0    41850 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/data/ship.json
--rw-r--r--   0        0        0    10152 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/draw.py
--rw-r--r--   0        0        0     7427 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/name.py
--rw-r--r--   0        0        0    13372 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/send_message.py
--rw-r--r--   0        0        0     5995 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/nonebot_plugin_al/utils.py
--rw-r--r--   0        0        0     1028 2023-06-19 16:16:50.047033 nonebot_plugin_al-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3778 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/README.md
+-rw-r--r--   0        0        0     6487 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/nonebot_plugin_al/__init__.py
+-rw-r--r--   0        0        0    70845 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/nonebot_plugin_al/api.py
+-rw-r--r--   0        0        0     3348 2023-06-20 05:01:07.930343 nonebot_plugin_al-0.3.2/nonebot_plugin_al/bili.py
+-rw-r--r--   0        0        0    69109 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/data/eq.json
+-rw-r--r--   0        0        0    41850 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/data/ship.json
+-rw-r--r--   0        0        0    10152 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/draw.py
+-rw-r--r--   0        0        0     7691 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/name.py
+-rw-r--r--   0        0        0    13667 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/send_message.py
+-rw-r--r--   0        0        0     6878 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/nonebot_plugin_al/utils.py
+-rw-r--r--   0        0        0     1028 2023-06-20 05:01:07.934342 nonebot_plugin_al-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4912 1970-01-01 00:00:00.000000 nonebot_plugin_al-0.3.2/PKG-INFO
```

### Comparing `nonebot_plugin_al-0.3.1/LICENSE` & `nonebot_plugin_al-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.1/README.md` & `nonebot_plugin_al-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 ### 【总】碧蓝帮助 | 碧蓝指令
 
 - 1、碧蓝+['强度榜','装备榜','金部件榜','萌新榜','兵器榜','专武榜',
         '兑换榜','研发榜','改造榜','跨队榜','pt榜','氪金榜','打捞主线榜','打捞作战榜']
 - 2、碧蓝角色【角色名称】
 - 3、碧蓝装备【装备名称】
 
-### 【blhx_wiki】（除了查船，其他不用空格）
+### 【blhx_wiki】（强制检查空格）
 
 0.帮助信息
 
 命令示范：blhx 帮助
 
 1.根据船名查舰船信息
```

#### html2text {}

```diff
@@ -15,19 +15,19 @@
 `è¿ç¹ååéè¦ï¼blhx_wikiåè½90%ä¾èµè¿ä¸ªèµæºåï¼è¯·èªè¡çæå®çæ´æ°
 ç¾åº¦äºçï¼é¾æ¥ï¼https://pan.baidu.com/s/
 1ppLW3rkygLovXIG_Y58Qrg?pwd=57uk æåç ï¼57uk ## æä»¤ ###
 ãæ»ãç¢§èå¸®å© | ç¢§èæä»¤ - 1ãç¢§è+
 ['å¼ºåº¦æ¦','è£å¤æ¦','éé¨ä»¶æ¦','èæ°æ¦','åµå¨æ¦','ä¸æ­¦æ¦',
 'åæ¢æ¦','ç åæ¦','æ¹é æ¦','è·¨éæ¦','ptæ¦','æ°ªéæ¦','ææä¸»çº¿æ¦','ææä½ææ¦']
 - 2ãç¢§èè§è²ãè§è²åç§°ã - 3ãç¢§èè£å¤ãè£å¤åç§°ã ###
-ãblhx_wikiãï¼é¤äºæ¥è¹ï¼å¶ä»ä¸ç¨ç©ºæ ¼ï¼ 0.å¸®å©ä¿¡æ¯
-å½ä»¤ç¤ºèï¼blhx å¸®å© 1.æ ¹æ®è¹åæ¥è°è¹ä¿¡æ¯ å½ä»¤ç¤ºèï¼ blhx
-é¿é¨ 2.æ ¹æ®è¹ååç®è¤åæ¥è¯¢ç®è¤ç«ç» å½ä»¤ç¤ºèï¼blhx
-å£è·¯ææ¯ Luxury_Handle å½ä»¤ç¤ºèï¼blhx é¿é¨ å¾¡ççè¾æ¯è¢
-å½ä»¤ç¤ºèï¼blhx é¿é¨ åç® å½ä»¤ç¤ºèï¼blhx é¿é¨ å©çº±
+ãblhx_wikiãï¼å¼ºå¶æ£æ¥ç©ºæ ¼ï¼ 0.å¸®å©ä¿¡æ¯ å½ä»¤ç¤ºèï¼blhx
+å¸®å© 1.æ ¹æ®è¹åæ¥è°è¹ä¿¡æ¯ å½ä»¤ç¤ºèï¼ blhx é¿é¨
+2.æ ¹æ®è¹ååç®è¤åæ¥è¯¢ç®è¤ç«ç» å½ä»¤ç¤ºèï¼blhx å£è·¯ææ¯
+Luxury_Handle å½ä»¤ç¤ºèï¼blhx é¿é¨ å¾¡ççè¾æ¯è¢ å½ä»¤ç¤ºèï¼blhx
+é¿é¨ åç® å½ä»¤ç¤ºèï¼blhx é¿é¨ å©çº±
 3.éæºè¿åæ¸¸æå è½½é¡µé¢çæç» å½ä»¤ç¤ºèï¼blhx è¿åº
 4.è¿åbwikiçPVEå¼ºåº¦æ¦ä¿¡æ¯ å½ä»¤ç¤ºèï¼blhx å¼ºåº¦æ¦ 7.å¼ºå¶æ´æ°
 (ç®åå·²ä½¿ç¨ä»£çæ´æ°apiæ°æ®ä¸ºç¦»çº¿æ¨¡å¼æç¨ï¼å¦æåºé®é¢åæ¶issue)
 å½ä»¤ç¤ºèï¼blhx å¼ºå¶æ´æ° 8.è·åææ°æ´»å¨ä¿¡æ¯
 (æé®é¢åæ¶issue) å½ä»¤ç¤ºèï¼blhx ææ°æ´»å¨ 9.ä¸ºè°è¹åæµç§°
 (ä»¥åä½ å°±å¯ä»¥ç¨æµç§°æ¥è¯¢äº) å½ä»¤ç¤ºèï¼blhxå¤æ³¨ åè¾ å¤ªå¤ª
 ä»¥åå°±å¯ä»¥ç¨ blhx å¤ªå¤ª å©çº± è¿ç§æµç§°åä»£æ­£å¼åç§°æ¥è¯¢
```

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/__init__.py` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -129,64 +129,64 @@
     "blhx", 
     block=True, 
     priority=50,
     handlers=[blhx.send_ship_skin_or_info]
 )
 
 on_command(
-    "blhx过场", 
+    "blhx 过场", 
     block=True, 
     priority=10,
     handlers=[blhx.send_random_gallery]
 )
 
 on_command(
-    "blhx帮助", 
+    "blhx 帮助", 
     block=True, 
     priority=10,
     handlers=[blhx.send_blhx_help]
 )
 on_command(
-    "blhx强度榜", 
+    "blhx 强度榜", 
     block=True, 
     priority=10,
     handlers=[blhx.send_pve_recommendation]
 )
 on_command(
-    "blhx强制更新", 
+    "blhx 强制更新", 
     block=True, 
     priority=10,
     permission=SUPERUSER,
     handlers=[blhx.force_update]
 )
 on_command(
-    "blhx最新活动", 
+    "blhx 最新活动", 
     block=True, 
     priority=10,
     handlers=[blhx.get_recently_event]
 )
 on_command(
-    "blhx备注", 
+    "blhx 备注", 
     block=True, 
     priority=10,
     permission=ADMIN,
     handlers=[blhx.set_nickname]
 )
 on_command(
-    "blhx移除备注", 
+    "blhx 移除备注", 
     block=True, 
     priority=10,
     permission=ADMIN,
     handlers=[blhx.remove_nickname]
 )
 on_command(
-    "blhx皮肤", 
+    "blhx 皮肤", 
     block=True, 
     priority=10,
     handlers=[blhx.quick_search_skin]
 )
 on_command(
-    "blhx大建", 
+    "blhx 大建", 
     block=True, 
     priority=10,
     handlers=[blhx.building]
 )
```

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/api.py` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 
 
 async def get_ship_id_by_name(name):
     async with aiofiles.open(DATA_PATH.joinpath('azurapi_data', 'ships.json'),mode='r',encoding='utf-8'
                              )as load_f:
         load_dict = await load_f.read()
-        load_dict = json.loads(load_dict)
+        load_dict = await str_to_json(load_dict)
         id = None
 
         for result in load_dict:
             if str(result['names']['cn']) == str(name):
                 id = (result['id'])
             else:
                 continue
@@ -58,15 +58,15 @@
 """
 
 
 async def get_ship_data_by_name(name):
     async with aiofiles.open(DATA_PATH.joinpath('azurapi_data', 'ships.json'),mode='r',encoding='utf-8'
                              )as load_f:
         load_dict = await load_f.read()
-        load_dict = json.loads(load_dict)
+        load_dict = await str_to_json(load_dict)
     for result in load_dict:
         if str(result['names']['cn']) == str(name):
             return result
         else:
             continue
     return None
 
@@ -78,15 +78,15 @@
 说明：该方法作用是通过碧蓝航线api，用舰船id获取舰船数据，返回一个数据字典供html适配数据调用
 """
 
 async def get_ship_data_by_id(id):
     async with aiofiles.open(DATA_PATH.joinpath('azurapi_data', 'ships.json'),mode='r',encoding='utf-8'
                              )as load_f:
         load_dict = await load_f.read()
-        load_dict = json.loads(load_dict)
+        load_dict = await str_to_json(load_dict)
     for result in load_dict:
         if str(result['id']) == str(id):
             return result
         else:
             continue
     return None
 """
@@ -97,19 +97,20 @@
 """
 
 
 async def format_data_into_html(data):
     # 读入html备用
     soup = BeautifulSoup(open(DATA_PATH.joinpath('ship_html', 'ship_temp.html'), encoding='UTF-8'), "lxml")
     # 读入bwiki数据
-
+    with open('test.json','w') as f:
+        json.dump(data,f, ensure_ascii=True,indent=4)
     async with aiofiles.open(DATA_PATH.joinpath('ship_html', 'ships_plus.json'),mode='r',encoding='utf-8'
                             )as load_f:
         load_dict = await load_f.read()
-        load_dict = json.loads(load_dict)
+        load_dict = await str_to_json(load_dict)
     data_plus = {}
     try:
         for i in range(0, len(load_dict)):
             if str(data['id']) == str(load_dict[i]['编号']):
                 data_plus = load_dict[i]
                 break
     except:
@@ -772,17 +773,18 @@
     soup.find(id='total').append(str(data['fleetTech']['techPoints']['total']))
     # 退役，有的船不能退役,能退役的就三种返现：油，钱，章
     scrapValues = data['scrapValue']
     coin = ""
     oil = ""
     medal = ""
     if scrapValues is not None:
+        # 退役不再返油
         coin = str(data['scrapValue']['coin'])
         soup.find(id='coin').string = coin
-        oil = str(data['scrapValue']['oil'])
+        # oil = str(data['scrapValue']['oil'])
         soup.find(id='oil').string = oil
         medal = str(data['scrapValue']['medal'])
         soup.find(id='medal').string = medal
     else:
         soup.find(id='coin').string = soup.find(id='oil').string = soup.find(id='medal').string = "不可食用"
 
     # 皮肤列表
@@ -1029,20 +1031,30 @@
     result = await get_ship_data_by_id(str(id))
     ship_skin_list = result['skins']
     image_path = ''
     background_path = ''
     chibi_path = ''
     # 处理原皮
     if skin_name == '原皮':
+        # image_path = str(ship_skin_list[0]['image']).replace(
+        #     "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", "data/al/ship_html/")
+        # background_path = str(ship_skin_list[0]['background']).replace(
+        #     "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", "data/al/ship_html/")
+        # chibi_path = str(ship_skin_list[0]['chibi']).replace(
+        #     "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", "data/al/ship_html/")
+        # 在线
         image_path = str(ship_skin_list[0]['image']).replace(
-            "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", "")
+            "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", 
+            "https://ghproxy.com/https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/")
         background_path = str(ship_skin_list[0]['background']).replace(
-            "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", "")
+            "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", 
+            "https://ghproxy.com/https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/")
         chibi_path = str(ship_skin_list[0]['chibi']).replace(
-            "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", "")
+            "https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/", 
+            "https://ghproxy.com/https://raw.githubusercontent.com/AzurAPI/azurapi-js-setup/master/")
 
         soup.find(id='img-content')['style'] = "background-image: url('" + background_path + "')"
         soup.find(id='img-content').string = ''
         soup.find(id='img-content').append(soup.new_tag('img', src=image_path, style="height: 720px"))
         soup.find(id='img-content').append(
             soup.new_tag('img', src=chibi_path, style="position: fixed;bottom: 0;left: 0;"))
         DATA_PATH.joinpath('ship_html', 'ship_skin.html')
@@ -1195,22 +1207,23 @@
 参数列表：name(string)
 用处：根据船名获取bwiki的推荐装备，生成html
 返回值：无
 """
 
 
 async def get_ship_weapon_by_ship_name(name):
-    url = "https://wiki.biligame.com/blhx/" + str(name)
-    response_text:str = await get_data(url,mode='text')
-    soup = BeautifulSoup(response_text, "lxml")
-    div_list = soup.find(class_='row zb-table')
+    # 这里不知道怎么改，先注释问原作者
+    # url = "https://wiki.biligame.com/blhx/" + str(name)
+    # response_text:str = await get_data(url,mode='text')
+    # soup = BeautifulSoup(response_text, "lxml")
+    # div_list = soup.find(class_='row zb-table')
     target_soup = BeautifulSoup(
         open(DATA_PATH.joinpath('ship_html', 'ship_weapon_temp.html'),
              encoding='UTF-8'), "lxml")
-    target_soup.find('body').append(div_list)
+    # target_soup.find('body').append(div_list)
     async with aiofiles.open(DATA_PATH.joinpath('ship_html', 'ship_weapon.html'),
               'w', encoding="utf-8") as fp:
         await fp.write(str(target_soup.prettify()))
 
 
 async def force_update_offline():
     Path(SAVE_PATH, 'azurapi_data').mkdir(parents=True, exist_ok=True)
@@ -1233,28 +1246,28 @@
 
 
 async def get_recent_event():
     base_url='https://wiki.biligame.com'
     url = "https://wiki.biligame.com/blhx/首页"
     response_text:str = await get_data(url,mode='text')
     soup = BeautifulSoup(response_text, "lxml")
-    div_list=soup.find(class_='sy-left')
+    div_list=soup.find(class_='wikitable eventCalendar noselect')
     if div_list.a['href'] is not None and str( div_list.a['href'])!='':
         return base_url+str(div_list.a['href'])
     else:
         return None
 
 
 async def gacha_heavy_10():
     gacha_result = []
     async with aiofiles.open(DATA_PATH.joinpath('gacha_data', 'pools.json'),
                              'r',
                              encoding='UTF-8') as load_f:
         load_dict = await load_f.read()
-        load_dict = json.loads(load_dict)
+        load_dict = await str_to_json(load_dict)
         for i in range(0,10):
             flag = random.randint(0,999)
             if flag < 70:
                 superRare= await get_ship_id_by_name (choice(load_dict['HeavyShipBuildingListSuperRare']))
                 gacha_result.append({'id':superRare})
             if 70 <= flag < 190:
                 elite = await get_ship_id_by_name (choice(load_dict['HeavyShipBuildingListElite']))
@@ -1271,15 +1284,15 @@
 
 async def gacha_special_10():
     gacha_result = []
     async with aiofiles.open(DATA_PATH.joinpath('gacha_data', 'pools.json'),
                              'r',
                              encoding='UTF-8') as load_f:
         load_dict = await load_f.read()
-        load_dict = json.loads(load_dict)
+        load_dict = await str_to_json(load_dict)
         for i in range(0,10):
             flag = random.randint(0,999)
             if flag < 70:
                 superRare= await get_ship_id_by_name (choice(load_dict['SpecialShipBuildingListSuperRare']))
                 gacha_result.append({'id':superRare})
             if 70 <= flag < 190:
                 elite = await get_ship_id_by_name (choice(load_dict['SpecialShipBuildingListElite']))
@@ -1296,15 +1309,15 @@
 
 async def gacha_light_10():
     gacha_result = []
     async with aiofiles.open(DATA_PATH.joinpath('gacha_data', 'pools.json'),
                              'r',
                              encoding='UTF-8') as load_f:
         load_dict = await load_f.read()
-        load_dict = json.loads(load_dict)
+        load_dict = await str_to_json(load_dict)
         for i in range(0,10):
             flag = random.randint(0,999)
             if flag < 70:
                 superRare= await get_ship_id_by_name (choice(load_dict['LightShipBuildingListSuperRare']))
                 gacha_result.append({'id':superRare})
             if 70 <= flag < 190:
                 elite = await get_ship_id_by_name (choice(load_dict['LightShipBuildingListElite']))
```

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/bili.py` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/bili.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/data/eq.json` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/data/eq.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/data/ship.json` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/data/ship.json`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/draw.py` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/name.py` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/name.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,16 +23,20 @@
 PATH_CHAR_GACHA = DATA_PATH.joinpath('gacha_data', 'character_image')       # 角色立绘目录
 PATH_STAR_GACHA = DATA_PATH.joinpath('gacha_data', 'star')                  # 星星图片目录
 PATH_TYPE_GACHA = DATA_PATH.joinpath('gacha_data', 'type_icon')             # 舰种图片目录
 PATH_BG_GACHA = DATA_PATH.joinpath('gacha_data', 'level_background')        # 背景图片目录
 
 import aiofiles
 import difflib
-import json
-import os
+
+try:
+    import ujson as json
+except:
+    import json
+
 
 '''
 这个模块定义了名字系统及其对应的操作方法。引入的库都是py的标准库，无需额外安装
 id: [
     cn_name,
     jp_name,
     kr_name,
@@ -69,22 +73,23 @@
 '''
 async def UpdateName():
     ships = {}
 
     # 判断文件是否存在，不存在的话就不进行读取
     try:
         async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
-            load_dict = await fp.read()
-            ships = json.loads(load_dict)
+            load_dict = str(await fp.read())
+            ships = await str_to_json(load_dict)
     except:
         pass
 
     async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/ships.json', 'r', encoding='utf-8') as fp:
-        load_dict = await fp.read()
-        data = json.loads(load_dict)
+        load_dict = str(await fp.read())
+        data = await str_to_json(load_dict)
+        print(f'data的类型是{type(data)}')
 
     for item in data:
         if item['id'] in ships.keys():
             continue
         ships[item['id']] = [item['names']['cn'], item['names']['jp'], item['names']['kr'], item['names']['en']]
 
     # print(ships)
@@ -104,16 +109,16 @@
 
 为舰船上传新的别名，在调用这个方法的时候用该特别注意权限控制
 '''
 ERR_NAMEALREADYEXISTS = -1
 async def AddName(id: str, nickname: str):
 
     async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
-        load_dict = await fp.read()
-        data = json.loads(load_dict)
+        load_dict = str(await fp.read())
+        data = await str_to_json(load_dict)
 
     if nickname in data[str(id)]:
         return ERR_NAMEALREADYEXISTS
     data[id].append(nickname)
 
     async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'w', encoding='utf-8') as fp:
         await fp.write(json.dumps(data, indent=2, ensure_ascii=False))
@@ -130,16 +135,16 @@
 
 为舰船删除已有的别名，在调用这个方法的时候用该特别注意权限控制
 '''
 ERR_NICKNAMENOTFOUND = -1
 async def DelName(id: str, nickname: str):
 
     async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
-        load_dict = await fp.read()
-        data = json.loads(load_dict)
+        load_dict = str(await fp.read())
+        data = await str_to_json(load_dict)
 
     try:
         data[id].remove(nickname)
     except:
         return ERR_NICKNAMENOTFOUND
 
     async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'w', encoding='utf-8') as fp:
@@ -158,16 +163,16 @@
 
 根据船只的标准名或者别名，查找船只的id和标准名
 '''
 ERR_SHIPNOTFOUND = -1
 async def GetIDByNickname(nickname: str):
 
     async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
-        load_dict = await fp.read()
-        data = json.loads(load_dict)
+        load_dict = str(await fp.read())
+        data = await str_to_json(load_dict)
 
     # data = {}
     retvalue = {}
     for item in data.items():
         if nickname in item[1]:
             retvalue = {
                 'id': item[0],
@@ -208,13 +213,16 @@
     返回一个数组，里面包含这个舰船的所有名称
 
 根据舰船的标准名，返回这个舰船的所有名称
 '''
 async def GetAllNickname(id: str):
 
     async with aiofiles.open(DATA_PATH_STR + '/azurapi_data/names.json', 'r', encoding='utf-8') as fp:
-        load_dict = await fp.read()
-        data = json.loads(load_dict)
+        load_dict = str(await fp.read())
+        data = await str_to_json(load_dict)
 
     return data[id]
 
-
+async def str_to_json(data:str):
+    while isinstance(data,str):
+        data = json.loads(data)
+    return data
```

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/send_message.py` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/send_message.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import shutil
 
 from nonebot.adapters.onebot.v11 import (Bot, GroupMessageEvent, Message,
                                          MessageSegment,Event)
 from nonebot.params import CommandArg
 from nonebot.matcher import Matcher
 from nonebot.log import logger
+from nonebot_plugin_htmlrender import html_to_pic
 
 from .api import *
 from .utils import *
 from .draw import *
 from .name import *
 
 
@@ -19,15 +20,15 @@
 
     async def send_ship_skin_or_info(
         matcher:Matcher,
         event:Event,
         bot:Bot,
         arg:Message = CommandArg()
         ):
-        SAVE_PATH = Path().cwd().joinpath('data/al')
+        SAVE_PATH = Path().cwd().joinpath('data/al/ship_html')
         try:
             args = arg.extract_plain_text().split()
             if len(args) == 2:
                 ship_name = str(args[0])
                 skin_name = str(args[1]).replace("_", (" "))
                 ship_nickname_data = await GetIDByNickname(ship_name)
                 if ship_nickname_data == -1 :
@@ -37,63 +38,69 @@
                     ship_id = ship_nickname_data['id']
 
                 flag = await get_ship_skin_by_id(str(ship_id), skin_name)
                 if flag == 4:
                     msg = "她没有这个皮肤！"
                     await bot.send(event=event,message=msg, at_sender=True)
                 if flag == 0:
-                    print_img_skin()
-                    msg = MessageSegment.image("file:///" + SAVE_PATH + "/images/ship_skin_mix/ship_skin.png")
+                    # print_img_skin()
+                    await save_img_ship('skin',temp=False)
+                    msg = MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_skin.png")))
                     await bot.send(event=event,message=msg, at_sender=True)
                 if flag == 1:
                     msg = "她只有原皮！"
                     await bot.send(event=event,message=msg, at_sender=True)
             if len(args) == 1:
                 nickname_list = ''
                 ship_name = str(args[0])
                 ship_nickname_data = await GetIDByNickname(ship_name)
                 ship_nickname_list = await GetAllNickname(ship_nickname_data['id'])
                 for string in ship_nickname_list:
                     nickname_list+=(str(string)+"\n")
 
                 index = await format_data_into_html(await get_ship_data_by_id(ship_nickname_data['id']))
                 await get_ship_weapon_by_ship_name(ship_nickname_data['standred_name'])
-                print_img_ship()
-                print_img_ship_weapon()
+                
+                # print_img_ship()
+                # print_img_ship_weapon()
+
+                await save_img_ship()
+                await save_img_ship('weapon')
                 img_process_ship_info()
                 img_process_ship_weapon()
+                
                 if index == 0:
-                    msg = "舰船信息\n" + MessageSegment.image("file:///" + SAVE_PATH + "/images/ship_info.png") \
-                        + "\n推荐出装\n" + MessageSegment.image("file:///" + SAVE_PATH + "/images/ship_weapon.png")+ "\n此船备注昵称有：\n"+nickname_list
+                    msg = "舰船信息\n" + MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_info.png"))) \
+                        + "\n推荐出装\n" + MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_weapon.png")))+ "\n此船备注昵称有：\n"+nickname_list
                 else:
                     print_img_ship_retrofit()
                     img_process_ship_retrofit()
-                    msg = "舰船信息\n" + MessageSegment.image("file:///" + SAVE_PATH + "/images/ship_info.png") \
-                        + "\n此船可改\n" + MessageSegment.image("file:///" + SAVE_PATH + "/images/ship_retrofit.png") \
-                        + "\n推荐出装\n" + MessageSegment.image("file:///" + SAVE_PATH + "/images/ship_weapon.png")\
+                    msg = "舰船信息\n" + MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_info.png"))) \
+                        + "\n此船可改\n" + MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_retrofit.png"))) \
+                        + "\n推荐出装\n" + MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_weapon.png")))\
                         + "\n此船备注昵称有：\n"+nickname_list
 
                 msg_list = []
                 msg_list.append(msg)
                 forward_msg = render_forward_msg(msg_list)
                 if isinstance(event,GroupMessageEvent):
                     await bot.call_api('send_group_forward_msg',group_id=event.group_id, messages=forward_msg)
                     return
             if len(args) == 0:
                 await bot.send(event=event,message='请在命令之后提供精确舰船名称和皮肤昵称哦~', at_sender=True)
         except Exception as e:
             traceback.print_exc()
-            await bot.send(event=event,message="查询出错", at_sender=True)
+            await bot.send(event=event,message=f"查询出错,{e}", at_sender=True)
 
     async def send_random_gallery(
         matcher:Matcher,
         event:Event,
         bot:Bot
         ):
-        SAVE_PATH = Path().cwd().joinpath('data/al/ship_html/images/gallery/' / get_random_gallery())
+        SAVE_PATH = Path().cwd().joinpath('data/al/ship_html/images/gallery/',get_random_gallery())
         msg = MessageSegment.image("file:///" + str(SAVE_PATH))
         await bot.send(event=event,message=msg, at_sender=True)
 
 
     async def send_blhx_help(
         matcher:Matcher,
         event:Event,
@@ -257,15 +264,15 @@
                 flag = await get_ship_skin_by_id_with_index(str(ship_id), skin_index)
                 if flag == -1:
                     msg = "她没有这个皮肤！"
                     await bot.send(event=event,message=msg, at_sender=True)
                     return
                 if flag == 0:
                     print_img_skin()
-                    msg = MessageSegment.image("file:///" + SAVE_PATH + "/images/ship_skin_mix/ship_skin.png")
+                    msg = MessageSegment.image("file:///" + str(SAVE_PATH.joinpath("images/ship_skin.png")))
                     await bot.send(event=event,message=msg, at_sender=True)
                     return
         except:
             msg = '处理出错，请看日志'
             traceback.print_exc()
             await bot.send(event=event,message=str(msg), at_sender=True)
             return
@@ -274,15 +281,15 @@
     async def building(        
         matcher:Matcher,
         event:Event,
         bot:Bot,
         arg:Message = CommandArg()
         ):
         try:
-            args = arg.message.extract_plain_text().split()
+            args = arg.extract_plain_text().split()
             if len(args) == 1:
                 if str(args[0]) == '轻型':
                     data = await gacha_light_10()
                     img = GachaImage(data)
                     cq = await img.Make()
                     await bot.send(event=event,message=cq,at_sender=True)
                 if str(args[0]) == '重型':
```

### Comparing `nonebot_plugin_al-0.3.1/nonebot_plugin_al/utils.py` & `nonebot_plugin_al-0.3.2/nonebot_plugin_al/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,56 @@
 import imgkit
 import cv2
 import pypinyin
 import json
 import aiofiles
 
+from typing import Optional
 from pathlib import Path
 from nonebot.adapters.onebot.v11 import Bot
+from nonebot_plugin_htmlrender import html_to_pic
 
 SAVE_PATH = Path().joinpath('data/al')
 tool_path = SAVE_PATH.joinpath('wkhtmltopdf', 'bin', 'wkhtmltoimage.exe')
 """
 方法名：print_img
 参数列表：无
 用处：调用打印工具，打印ship_info.html成图片
 返回值：无返回值，从html文件夹里读取html文件，打印的图片输出到images文件夹
 """
 
-
+async def save_img_ship(tag:Optional[str] = None,temp:bool = True):
+    tep = '_temp' if temp else ''
+    if not tag:
+        with open(SAVE_PATH.joinpath('ship_html', 'ship_info.html'),'r',encoding='utf-8')as f:
+            html = f.read()
+        pic = await html_to_pic(html=html)
+        with open(SAVE_PATH.joinpath('ship_html','images', 'ship_temp.png'),'wb')as f:
+            f.write(pic)
+    else:
+        with open(SAVE_PATH.joinpath('ship_html', f'ship_{tag}.html'),'r',encoding='utf-8')as f:
+            html = f.read()
+        pic = await html_to_pic(html=html)
+        with open(SAVE_PATH.joinpath('ship_html','images', f'ship_{tag}{tep}.png'),'wb')as f:
+            f.write(pic)
+            
 def print_img_ship():
     # path_wkimg = SAVE_PATH + '/\\wkhtmltopdf/\\bin/\\wkhtmltoimage.exe'  # 工具路径
     path_wkimg = tool_path
     cfg = imgkit.config(wkhtmltoimage=path_wkimg)
     options = {
         "encoding": "UTF-8",
         "enable-local-file-access": None
     }
     print("开始")
     imgkit.from_file(SAVE_PATH.joinpath('ship_html', 'ship_info.html'),
                      SAVE_PATH.joinpath('images', 'ship_temp.png'),
                      options=options, config=cfg)  # 不管怎么样都打印这张图片
     print("结束")
 
-
 def print_img_ship_retrofit():
     # path_wkimg = SAVE_PATH + '/\\wkhtmltopdf/\\bin/\\wkhtmltoimage.exe'  # 工具路径
     path_wkimg = tool_path
     cfg = imgkit.config(wkhtmltoimage=path_wkimg)
     options = {
         "encoding": "UTF-8",
         "enable-local-file-access": None
@@ -47,18 +62,18 @@
     print("结束")
 
 
 
 
 def img_process_ship_retrofit():
     # SAVE_PATH.joinpath('images', 'ship_temp.png'))
-    img = cv2.imread(SAVE_PATH.joinpath('images', 'ship_retrofit_temp.png'))
+    img = cv2.imread(SAVE_PATH.joinpath('ship_html','images', 'ship_retrofit_temp.png'))
     image = img.shape
     cropped = img[0:image[0], 0:620]  # 裁剪坐标为[y0:y1, x0:x1]
-    cv2.imwrite(SAVE_PATH.joinpath('images', 'ship_retrofit.png'), cropped)
+    cv2.imwrite(SAVE_PATH.joinpath('ship_html','images', 'ship_retrofit.png'), cropped)
 
 """
 方法名：print_img_skin
 参数列表：无
 用处：调用打印工具，打印ship_skin.html成图片
 返回值：无返回值，从html文件夹里读取html文件，打印的图片输出到images文件夹
 """
@@ -68,59 +83,60 @@
     path_wkimg = tool_path  # 工具路径
     cfg = imgkit.config(wkhtmltoimage=path_wkimg)
     options = {
         "encoding": "UTF-8",
         "enable-local-file-access": None
     }
     imgkit.from_file(SAVE_PATH.joinpath('ship_html', 'ship_skin.html'),
-                     SAVE_PATH.joinpath('images', 'ship_skin_mix', 'ship_skin.png'),
+                     SAVE_PATH.joinpath('ship_html', 'images','ship_skin.png'),
                      options=options, config=cfg)  # 不管怎么样都打印这张图片
 
 
 def print_img_ship_weapon():
     path_wkimg = tool_path  # 工具路径
     cfg = imgkit.config(wkhtmltoimage=path_wkimg)
     options = {
         "encoding": "UTF-8",
         "enable-local-file-access": None
     }
     imgkit.from_file(SAVE_PATH.joinpath('ship_html', 'ship_weapon.html'),
-                     SAVE_PATH.joinpath('images', 'ship_weapon_temp.png'),
+                     SAVE_PATH.joinpath('ship_html', 'images', 'ship_weapon_temp.png'),
                      options=options, config=cfg)  # 不管怎么样都打印这张图片
 
 
+
 """
 方法名：img_process_ship_info
 参数列表：无
 用处：裁剪图片
 返回值：无返回值
 """
 
 
 def img_process_ship_info():
     # SAVE_PATH.joinpath('images', 'ship_temp.png'))
-    img = cv2.imread(SAVE_PATH.joinpath('images', 'ship_temp.png'))
+    img = cv2.imread(str(SAVE_PATH.joinpath('ship_html','images', 'ship_temp.png')))
     image = img.shape
     cropped = img[0:image[0], 0:620]  # 裁剪坐标为[y0:y1, x0:x1]
-    cv2.imwrite(SAVE_PATH.joinpath('images', 'ship_info.png'), cropped)
+    cv2.imwrite(str(SAVE_PATH.joinpath('ship_html','images', 'ship_info.png')), cropped)
 
     """
     方法名：img_process_ship_weapon
     参数列表：无
     用处：裁剪图片
     返回值：无返回值
     """
 
 
 def img_process_ship_weapon():
     # SAVE_PATH.joinpath('images', 'ship_weapon_temp.png'))
-    img = cv2.imread(SAVE_PATH.joinpath('images', 'ship_weapon_temp.png'))
+    img = cv2.imread(str(SAVE_PATH.joinpath('ship_html','images', 'ship_weapon_temp.png')))
     image = img.shape
     cropped = img[0:image[0], 0:620]  # 裁剪坐标为[y0:y1, x0:x1]
-    cv2.imwrite(SAVE_PATH.joinpath('images', 'ship_weapon.png'), cropped)
+    cv2.imwrite(str(SAVE_PATH.joinpath('ship_html','images', 'ship_weapon.png')), cropped)
 
 
 def translate_ship_type(english):
     if english == 'Aircraft Carrier':
         return ['航空母舰', 'CV']
     if english == 'Destroyer':
         return ['驱逐舰', 'DD']
```

### Comparing `nonebot_plugin_al-0.3.1/pyproject.toml` & `nonebot_plugin_al-0.3.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot_plugin_al"
-version = "0.3.1"
+version = "0.3.2"
 description = "Azuer L plugin for NoneBot2"
 authors = ["Agnes_Digital <Z735803792@163.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Agnes4m/nonebot_plugin_AL"
 repository = "https://github.com/Agnes4m/nonebot_plugin_AL"
 keywords = ["game", "nonebot2", "plugin","bilibili"]
```

### Comparing `nonebot_plugin_al-0.3.1/PKG-INFO` & `nonebot_plugin_al-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-al
-Version: 0.3.1
+Version: 0.3.2
 Summary: Azuer L plugin for NoneBot2
 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT
 Keywords: game,nonebot2,plugin,bilibili
 Author: Agnes_Digital
 Author-email: Z735803792@163.com
 Requires-Python: >=3.9,<4.0
@@ -97,15 +97,15 @@
 ### 【总】碧蓝帮助 | 碧蓝指令
 
 - 1、碧蓝+['强度榜','装备榜','金部件榜','萌新榜','兵器榜','专武榜',
         '兑换榜','研发榜','改造榜','跨队榜','pt榜','氪金榜','打捞主线榜','打捞作战榜']
 - 2、碧蓝角色【角色名称】
 - 3、碧蓝装备【装备名称】
 
-### 【blhx_wiki】（除了查船，其他不用空格）
+### 【blhx_wiki】（强制检查空格）
 
 0.帮助信息
 
 命令示范：blhx 帮助
 
 1.根据船名查舰船信息
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.1 Summary: Azuer L
+Metadata-Version: 2.1 Name: nonebot-plugin-al Version: 0.3.2 Summary: Azuer L
 plugin for NoneBot2 Home-page: https://github.com/Agnes4m/nonebot_plugin_AL
 License: MIT Keywords: game,nonebot2,plugin,bilibili Author: Agnes_Digital
 Author-email: Z735803792@163.com Requires-Python: >=3.9,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
@@ -31,19 +31,19 @@
 `è¿ç¹ååéè¦ï¼blhx_wikiåè½90%ä¾èµè¿ä¸ªèµæºåï¼è¯·èªè¡çæå®çæ´æ°
 ç¾åº¦äºçï¼é¾æ¥ï¼https://pan.baidu.com/s/
 1ppLW3rkygLovXIG_Y58Qrg?pwd=57uk æåç ï¼57uk ## æä»¤ ###
 ãæ»ãç¢§èå¸®å© | ç¢§èæä»¤ - 1ãç¢§è+
 ['å¼ºåº¦æ¦','è£å¤æ¦','éé¨ä»¶æ¦','èæ°æ¦','åµå¨æ¦','ä¸æ­¦æ¦',
 'åæ¢æ¦','ç åæ¦','æ¹é æ¦','è·¨éæ¦','ptæ¦','æ°ªéæ¦','ææä¸»çº¿æ¦','ææä½ææ¦']
 - 2ãç¢§èè§è²ãè§è²åç§°ã - 3ãç¢§èè£å¤ãè£å¤åç§°ã ###
-ãblhx_wikiãï¼é¤äºæ¥è¹ï¼å¶ä»ä¸ç¨ç©ºæ ¼ï¼ 0.å¸®å©ä¿¡æ¯
-å½ä»¤ç¤ºèï¼blhx å¸®å© 1.æ ¹æ®è¹åæ¥è°è¹ä¿¡æ¯ å½ä»¤ç¤ºèï¼ blhx
-é¿é¨ 2.æ ¹æ®è¹ååç®è¤åæ¥è¯¢ç®è¤ç«ç» å½ä»¤ç¤ºèï¼blhx
-å£è·¯ææ¯ Luxury_Handle å½ä»¤ç¤ºèï¼blhx é¿é¨ å¾¡ççè¾æ¯è¢
-å½ä»¤ç¤ºèï¼blhx é¿é¨ åç® å½ä»¤ç¤ºèï¼blhx é¿é¨ å©çº±
+ãblhx_wikiãï¼å¼ºå¶æ£æ¥ç©ºæ ¼ï¼ 0.å¸®å©ä¿¡æ¯ å½ä»¤ç¤ºèï¼blhx
+å¸®å© 1.æ ¹æ®è¹åæ¥è°è¹ä¿¡æ¯ å½ä»¤ç¤ºèï¼ blhx é¿é¨
+2.æ ¹æ®è¹ååç®è¤åæ¥è¯¢ç®è¤ç«ç» å½ä»¤ç¤ºèï¼blhx å£è·¯ææ¯
+Luxury_Handle å½ä»¤ç¤ºèï¼blhx é¿é¨ å¾¡ççè¾æ¯è¢ å½ä»¤ç¤ºèï¼blhx
+é¿é¨ åç® å½ä»¤ç¤ºèï¼blhx é¿é¨ å©çº±
 3.éæºè¿åæ¸¸æå è½½é¡µé¢çæç» å½ä»¤ç¤ºèï¼blhx è¿åº
 4.è¿åbwikiçPVEå¼ºåº¦æ¦ä¿¡æ¯ å½ä»¤ç¤ºèï¼blhx å¼ºåº¦æ¦ 7.å¼ºå¶æ´æ°
 (ç®åå·²ä½¿ç¨ä»£çæ´æ°apiæ°æ®ä¸ºç¦»çº¿æ¨¡å¼æç¨ï¼å¦æåºé®é¢åæ¶issue)
 å½ä»¤ç¤ºèï¼blhx å¼ºå¶æ´æ° 8.è·åææ°æ´»å¨ä¿¡æ¯
 (æé®é¢åæ¶issue) å½ä»¤ç¤ºèï¼blhx ææ°æ´»å¨ 9.ä¸ºè°è¹åæµç§°
 (ä»¥åä½ å°±å¯ä»¥ç¨æµç§°æ¥è¯¢äº) å½ä»¤ç¤ºèï¼blhxå¤æ³¨ åè¾ å¤ªå¤ª
 ä»¥åå°±å¯ä»¥ç¨ blhx å¤ªå¤ª å©çº± è¿ç§æµç§°åä»£æ­£å¼åç§°æ¥è¯¢
```

