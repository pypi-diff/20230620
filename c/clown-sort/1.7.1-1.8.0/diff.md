# Comparing `tmp/clown_sort-1.7.1.tar.gz` & `tmp/clown_sort-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.7.1.tar", max compression
+gzip compressed data, was "clown_sort-1.8.0.tar", max compression
```

## Comparing `clown_sort-1.7.1.tar` & `clown_sort-1.8.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3274 2023-06-15 23:50:36.857435 clown_sort-1.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.7.1/LICENSE
--rw-r--r--   0        0        0     8766 2023-06-03 00:17:25.185210 clown_sort-1.7.1/README.md
--rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.7.1/clown_sort/__init__.py
--rw-r--r--   0        0        0     7987 2023-06-03 00:19:42.985646 clown_sort-1.7.1/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.7.1/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.7.1/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     3069 2023-06-15 23:22:00.182053 clown_sort-1.7.1/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11399 2023-06-02 21:49:12.145554 clown_sort-1.7.1/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.7.1/clown_sort/sort_selector.py
--rw-r--r--   0        0        0    11363 2023-06-15 23:40:16.589247 clown_sort-1.7.1/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.7.1/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.7.1/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.7.1/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3690 2023-06-02 22:06:05.123239 clown_sort-1.7.1/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.7.1/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.7.1/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.7.1/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-06-15 23:50:36.863775 clown_sort-1.7.1/pyproject.toml
--rw-r--r--   0        0        0    10188 1970-01-01 00:00:00.000000 clown_sort-1.7.1/PKG-INFO
+-rw-r--r--   0        0        0     3302 2023-06-20 03:21:16.499883 clown_sort-1.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.8.0/LICENSE
+-rw-r--r--   0        0        0     9088 2023-06-20 03:19:34.505801 clown_sort-1.8.0/README.md
+-rw-r--r--   0        0        0     3347 2023-06-20 03:19:34.506319 clown_sort-1.8.0/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7987 2023-06-03 00:19:42.985646 clown_sort-1.8.0/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.8.0/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.8.0/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     3069 2023-06-15 23:22:00.182053 clown_sort-1.8.0/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    12052 2023-06-20 03:19:34.507174 clown_sort-1.8.0/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.8.0/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    11758 2023-06-20 03:19:34.507783 clown_sort-1.8.0/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.8.0/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.8.0/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.8.0/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3705 2023-06-20 03:19:34.508422 clown_sort-1.8.0/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.8.0/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.8.0/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.8.0/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1619 2023-06-20 03:21:16.505459 clown_sort-1.8.0/pyproject.toml
+-rw-r--r--   0        0        0    10510 1970-01-01 00:00:00.000000 clown_sort-1.8.0/PKG-INFO
```

### Comparing `clown_sort-1.7.1/CHANGELOG.md` & `clown_sort-1.8.0/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # NEXT RELEASE
 
+# 1.8.0
+* Add a script to 
+
 ### 1.7.1
 * Handle 0 byte PDF error
 * More default rules
 
 # 1.7.0
 * Skip comment rows starting with `#` in rules CSVs.
 * New default rules
```

### Comparing `clown_sort-1.7.1/LICENSE` & `clown_sort-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/README.md` & `clown_sort-1.8.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -131,14 +131,24 @@
 ```sh
 pipx install clown_sort[gui]
 ```
 
 ![](doc/manual_select_box.png)
 
 
+## One Offs
+There is a script you can use to extract text from a single file (or a bunch of files, or all the files in a given directory). Just run:
+
+```
+scripts/extract_text_from_files.py MY_FILE1 MY_FILE2 SOME_DIR3
+```
+
+This will parse and display the text in `MY_FILE1`, `MY_FILE2`, and all the files in `SOME_DIR3`.
+
+
 # Contributing
 Feel free to file issues or open pull requests.
 
 This package is managed with [Python Poetry](http://python-poetry.org/). To get going:
 1. Install Poetry.
 1. `git clone` this repo.
 1. `cd clown_sort`
```

### Comparing `clown_sort-1.7.1/clown_sort/__init__.py` & `clown_sort-1.8.0/clown_sort/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # load_dotenv() should be called as soon as possible (before parsing local classes) but not for pytest
 if not environ.get('INVOKED_BY_PYTEST', False):
     for dotenv_file in [path.join(dir, '.clown_sort') for dir in [getcwd(), Path.home()]]:
         if path.exists(dotenv_file):
             load_dotenv(dotenv_path=dotenv_file)
             break
 
-from clown_sort.config import Config, check_for_pymupdf
+from clown_sort.config import Config
 from clown_sort.files.image_file import ImageFile
 from clown_sort.files.pdf_file import PdfFile
 from clown_sort.files.sortable_file import SortableFile
 from clown_sort.sort_selector import process_file_with_popup
 from clown_sort.util.filesystem_helper import (IMAGE_FILE_EXTENSIONS, files_in_dir, is_image,
       is_pdf, set_timestamp_based_on_screenshot_filename)
 from clown_sort.util.logging import log
@@ -60,35 +60,35 @@
             file_paths.extend(glob(str(glob_pattern)))
 
     for file_path in file_paths:
         if Config.screenshots_only and not Config.filename_regex.match(path.basename(file_path)):
             log.debug(f"Skipping '{file_path}' because it doesn't match the filename_regex...")
             continue
 
-        sortable_files.append(_build_sortable_file(file_path))
+        sortable_files.append(build_sortable_file(file_path))
 
     console.print(
         f"Re-processing {len(sortable_files)} files in '{Config.sorted_screenshots_dir}'...",
         style='bright_green'
     )
 
     for file_path in sortable_files:
         file_path.sort_file()
 
 
 def screenshot_paths(dir: Path) -> List[SortableFile]:
     """Returns a list of ImageFiles for all the screenshots to be sorted."""
     screenshots = [
-        _build_sortable_file(f) for f in files_in_dir(Config.screenshots_dir)
+        build_sortable_file(f) for f in files_in_dir(Config.screenshots_dir)
         if not Config.screenshots_only or Config.filename_regex.match(path.basename(f))
     ]
 
     return sorted(screenshots, key=lambda f: f.basename)
 
 
-def _build_sortable_file(file_path: Union[str, Path]) -> SortableFile:
+def build_sortable_file(file_path: Union[str, Path]) -> SortableFile:
     if is_image(file_path):
         return ImageFile(file_path)
     elif is_pdf(file_path):
         return PdfFile(file_path)
     else:
         return SortableFile(file_path)
```

### Comparing `clown_sort-1.7.1/clown_sort/config.py` & `clown_sort-1.8.0/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/clown_sort/filename_extractor.py` & `clown_sort-1.8.0/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/clown_sort/files/image_file.py` & `clown_sort-1.8.0/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/clown_sort/files/pdf_file.py` & `clown_sort-1.8.0/clown_sort/files/pdf_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/clown_sort/files/sortable_file.py` & `clown_sort-1.8.0/clown_sort/files/sortable_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -182,14 +182,37 @@
 
         if platform.system() == 'Windows':
             log.debug("Windows platform detected; attempting to run the file itself...")
             run([self.file_path])
         else:
             run(['open', self.file_path])
 
+    def print_extracted_text(self, max_chars: Optional[int] = None) -> None:
+        console.print(self._filename_panel())
+        console.print(self._extracted_str())
+
+    def _extracted_str(self, max_chars: Optional[int] = None) -> str:
+        """Raw string version of extracted text but truncated to max_chars if provided."""
+        txt = self.extracted_text()
+
+        if txt is None:
+            txt = "<No extracted text>"
+        else:
+            if max_chars is not None:
+                txt = txt[0:MAX_EXTRACTION_LENGTH]
+
+        return txt
+
+    def _extracted_text_panel(self) -> Panel:
+        """Panelized version of the extracted text for display."""
+        return Panel(self._extracted_str(MAX_EXTRACTION_LENGTH), expand=True, style='dim')
+
+    def _filename_panel(self) -> Panel:
+        return Panel(str(self.file_path), expand=False, style='bright_white reverse')
+
     def _log_copy_file(self, destination_path: Path, match: Optional[re.Match] = None) -> None:
         """Log info about a file copy."""
         if Config.debug:
             console.print(copying_file_log_message(self.basename, destination_path))
             return
 
         log_msg = Text('').append('Copying to ', style='dim')
@@ -242,23 +265,18 @@
 
     def __repr__(self) -> str:
         return f"SortableFile('{self.file_path}')"
 
     def __rich_console__(self, console: Console, options: ConsoleOptions) -> RenderResult:
         """Rich text method."""
         yield Text("\n\n")
-        yield Panel(str(self.file_path), expand=False, style='bright_white reverse')
+        yield self._filename_panel()
 
         if Config.debug:
-            if self.extracted_text() is None:
-                txt = "<No extracted text>"
-            else:
-                txt = self.extracted_text()[0:MAX_EXTRACTION_LENGTH]
-
-            yield Panel(txt, expand=True, style='dim')
+            yield self._extracted_text_panel()
 
         if self._filename_extractor is not None:
             if self._filename_extractor._is_tweet():
                 log_txt = bullet_text("It's a tweet by ", style='social_media')
                 log_txt.append(self._filename_extractor.author or 'NO_AUTHOR', style='author')
 
                 if self._filename_extractor.reply_to_account is not None:
```

### Comparing `clown_sort-1.7.1/clown_sort/sort_selector.py` & `clown_sort-1.8.0/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.8.0/clown_sort/sorting_rules/crypto.csv`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 Abra,\bAbra\b|\bPlutus\b|\bBarhydt
 AAX,\baax
 Algorand,\bAlgorand|\b[$#]ALGO\b
 Arbitrum,Arbitrum|[$#]ARB\b
 Amber Group,Amber[-_\s.]*Group|\btiantian\b|\bkullander\b|\btony[-_\s.]*he\b|\bbo[-_\s.]*shen\b
 Aptos,\bAptos\b
 Art,occult
+Atomic Wallet,Atomic[-_\s.]*Wallet
 Avalanche,\bAvax|AVAX\b|avalanche|\bava[-_\s.]*labs
 Banks,SEBA[^a-z]|Credit[-_\s.]*Suisse|SJMBT|Sygnum|Celtic[-_\s.]*Bank|\bMercury\b|Choice[-_\s.]*Financial[-_\s.]*Group|\$FRC|Commercium[-_\s.]*Financial|\bmetabank|\bHBAN\b|Huntington[-_\s.]*Bancshares|United[-_\s.]*Texas|\bUTB\b|Craig[-_\s.]*Sellars
 Bankless,Bankless|David[-_\s.]*Hoffman
 Biconomy,\bBiconomy|Omchain
 Binary Options,binary[-_\s.]*options
 Binance,binance|\bbiconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|\bjoselito\b|\bpaysafe|\bSwipe[-_\s.]*(IO|Wallet)|\bkeyway|\bkey[-_\s.]*vision|\bTrustWallet\b|BUSD\b|\boztures|Kaiser[-_\s.]*Ng|InvestByBit|Swyftx|Guangying[-_\s.]*Chen|\bcoley\b|\bBAM\b|\bFlowbank|\bnuvei\b|\borum\b|Worldpay|Bijie[-_\s.]*(Network|Tech)|Venus[-_\s.]*(Protocol|Community)
 Bitdeer,Bitdeer
@@ -32,15 +33,15 @@
 Bored Ape Yacht Club,BAYC|Bored[-_\s.]*Ape|yuga[-_\s.]*labs
 Bros,cryptomanran|\bRan[-_\s.]*Neuner|trillionUSD|nic[-_\s.]*carter|bitboy|ben[-_\s.]*armstrong|basedkarbon|thecryptolark|adam([-_\s.]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s.]*Alfred|natbrunell|natalie[-_\s.]*brunell|stackersatoshi|Max[-_\s.]*Keiser|Cowboy[-_\s.]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s.]*Paul\b|raoul(gmi|[-_\s.]*pal)|mccormack|andr3w|andrew[-_\s.]*wang|\b(JW)?[-_\s.]*Verret\b|@FlurETH\b|wolf[-_\s.]*of[-_\s.]*all[-_\s.]*streets|scott[-_\s.]*melker
 Broettes,Nicole[-_\s.]*Behnam|natbrunell
 Bybit,\bBybit\b|Ben[-_\s.]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
 Cathie Wood,Cathie[-_\s.]*Wood|\bARK(F|G|K|[-_\s.]*Innovation|[-_\s.]*Invest)|\bIZRL
 Celsius,celsius|mashinsky|levity[-_\s.]*and[-_\s.]*love|\bcelsian|Artur[-_\s.]*Abreu|ronpaulbot|\bnuke[-_\s.]*gold(stein)?
-China,fentanyl|\bchin(a|ese)|Hong[-_\s.]*Kong
+China,fentanyl|\bchin(a|ese)|Hong[-_\s.]*Kong|BANK[-_\s.]*OF[-_\s.]*COMMUNICATIONS
 Circle,[@#]circle|usdc|circle[-_\s.]*internet|disparte|\ballaire|jerallaire|Macromedia
 CMCC Global,CMCC[-_\s.]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s.]*armstrong|grewal\b|Asiff[-_\s.]*Hirji|\bbalaji|Fred[-_\s.]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s.]*Lamb|Roger[-_\s.]*Ver|coinflex|Doug[-_\s.]*Polk|OPNX|flexusd|Leslie[-_\s.]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
 ConsenSys,ConsenSys
@@ -63,27 +64,27 @@
 Euler Finance,\beuler\b
 FalconX,falconx
 First Digital,First[-_\s.]*Digital\b
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
-Friedlander Group,Friedlander|Agro[-_\s.]*Bank|\ball[-_\s.]*year\b|\bbrock\b|brockpierce|litvishhocker
+Friedlander Group,Friedlander|Agro[-_\s.]*Bank|\ball[-_\s.]*year\b|\bbrock\b|brockpierce|litvishhocker|Yecheskel|Swift[-_\s.]*Staffing
 FTX,FTX|\bFTT\b|\bSBF|Trabucco|\bBankman\b|\bEllison|\bNishad|\bAlameda|Moonstone|friedberg|autism[-_\s.]*capital|\bryne\b|clifton[-_\s.]*bay|\bZUBR\b
 Galaxy Digital,novogratz|Alex[-_\s.]*Thorn
 Gate.io,Gate[_.]?IO
 Gelato Network,Gelato[-_\s.]*Network|\bSorbet[-_\s.]*Finance|@gitpusha|hilmar[-_\s.]*x|\bmistx\b|@_alchemistcoin|@ChaosLabs_NFT|Arrakis[-_\s.]*Finance|Dave[-_\s.]*Leibowitz|Hilmar[-_\s.]*Orth|joehquak
 Gemini,Gemini|winklev|@cameron
 Genesis,Genesis|Michael\s?Moro
 Goldfinch,goldfinch
 Hamas,\bHamas\b|Al[-_\s.]*Qassam
 Haru Invest,\bHaru(invest)?\b|\b(happy)?Delio\b
 Hex,\bHex\b|[#$]Hex|Pulsechain|Richard[-_\s.]*Heart|Hexican
 Hoo,Hoo[-_\s.]*(Research|Exchange)|[#$]Hoo\b|Rexy[-_\s.]*(Hoo|Wang)|\bhoo\b
-Huobi,huobi|jiao_newlife|jiaojiao|Leon[-_\s.]*Li
+Huobi,huobi|jiao_newlife|jiaojiao|Leon[-_\s.]*Li\b|\b(GoPlus|Walken)\b
 Iran,\bIran\b|\bIranian\b|Nobitex|\bCoinNik|\bWallex\b|Sarmayex|\bRabex\b
 Jump Trading,Jump[-_\s.]*Trading|@jump_
 Justin Sun,justin[-_\s.]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina|\bR(ebo|ible)\b|Love[-_\s.]*Letters[-_\s.]*Limited|Objectivists[-_\s.]*Limited
 Kazakhstan,\bkazakh|Freedom[-_\s.]*Holding|\balmaty|Timor[-_\s.]*Turlov|\bFFIN[-_\s.]*brokerage
 Kinesis,kinesis|\bKVT\b|\bABX\b|\bKAG\b
 Kraken,kraken|payward|\bjespow\b|Jesse[-_\s.]*Powell
 KuCoin,kucoin
@@ -106,17 +107,17 @@
 Founders Bank,Michael[-_\s.]*Bianchi|Founders[-_\s.]*Bank
 Miles Guo,\bguo\b|\bhcoin|himalaya[-_\s.]*exchange|\bbannon\b|\bfjb|\bkwok\b|brother[-_\s.]*seven|kin[-_\s.]*ming[-_\s.]*je|william[-_\s.]*je\b|\bHaoyun\b|\bLi[-_\s.]*You\b
 Miners,bitcoin[-_\s.]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s.]*Scientific|Iris[-_\s.]*Energy|Blockstream
 Moonpay,\bmoonpay
 MSTR,Saylor|MSTR
 MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s.]*bot
 Near Protocol,NEAR[-_\s.]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s.]*Rettig
-Nexo,\bNexo\b|Antoni[-_\s.]*Trenchev|Georgi[-_\s.]*Shulev|Lydia[-_\s.]*Shuleva
+Nexo,\bNexo\b|Antoni[-_\s.]*Trenchev|Georgi[-_\s.]*Shulev|Lydia[-_\s.]*Shuleva|\bNDS[-_\s.]*EOD\b
 NFTs,crypto[-_\s.]*punk|pudgy[-_\s.]*penguin
-OKX,oke?[cx]|star[-_\s.]*xu|\blennix[-_\s.]*lai\b
+OKX,oke?[cx]|star[-_\s.]*xu|\blennix[-_\s.]*lai\b|\bOKcoin|\bHong[-_\s.]*Fang\b
 Olympus DAO,\bOlympus\b|OlympusDAO|\bOHM\b
 Ooki DAO,\bOoki(DAO)?\b
 OneCoin,\bOne(Coin|Life)\b
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea
 PAG,\bpag\b|Weijian[-_\s.]*Shan
 Paradigm,Fred[-_\s.]*Ehrsam|paradigm\b
@@ -140,24 +141,25 @@
 Silvergate,\$SI|Silvergate|Alan[-_\s.]*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s.]*Rettig
 Skrill,\bskrill
 Solana,Solana|Serum
 Stellar,\bstellar\b
 Stifel Bank,\bStifel\b|[#$]SF\b
 Symbolic Capital,Symbolic[-_\s.]*Capital|Lev[-_\s]Livnev
 Synapse,Synapse(fi|labs|protocol)?\b
-TerraLuna,luna\b|do[-_\s.]*kwon|stablekwon|\bterra\b|Macedo|\bLuna[-_\s.]*Foundation\b
-Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|hoegner|Noble[-_\s.]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Noblex|SJMBT|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s.]*Potter|Stablehouse|Samson[-_\s.]*Mow|Gabor[-_\s.]*Grubacs|XBTO|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s.]*Collins|\bdevasini\b|phil(ip)?[-_\s.]*potter\b|van[-_\s.]*der[-_\s.]*velde|Perpetual[-_\s.]*Action[-_\s.]*Group|\burwhatyouknow|global[-_\s.]*trade[-_\s.]*solutions|reginald[-_\s.]*fowler|renrenbee\b|\bludovicus|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s.]*payments|Five[-_\s.]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec|Mainstreet[-_\s.]*Partners|\bMallers\b
+TerraLuna,\bluna\b|do[-_\s.]*kwon|stablekwon|\bTerra(form|Luna)?\b|Macedo|\bLuna[-_\s.]*Foundation\b|Mirror[-_\s.]*Protocol
+Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|\bhoegner|Noble[-_\s.]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Noblex|SJMBT|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s.]*Potter|Stablehouse|Samson[-_\s.]*Mow|Gabor[-_\s.]*Gurbacs|XBTO|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s.]*Collins|\bdevasini\b|phil(ip)?[-_\s.]*potter\b|van[-_\s.]*der[-_\s.]*velde|Perpetual[-_\s.]*Action[-_\s.]*Group|\burwhatyouknow|global[-_\s.]*trade[-_\s.]*solutions|reginald[-_\s.]*fowler|renrenbee\b|\bludovicus|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s.]*payments|Five[-_\s.]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec|Mainstreet[-_\s.]*Partners|\bMallers\b|Far[-_\s.]*Eastern[-_\s.]*International|\b(Chesham|Sinopec|SFP)\b|White[-_\s.]*Plains[-_\s.]*Capital|BANK[-_\s.]*OF[-_\s.]*COMMUNICATIONS
 Tornado Cash,tornado[-_\s.]*cash
 Transactive Systems UAB,Transactive
 Tron,\btron\b|tron(block|[-_\s.]*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
 VCs,venture[-_\s.]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s.]*sacks|\bthiel\b|sequoia|founders[-_\s.]*fund|Valar[-_\s.]*Ventures|6th[-_\s.]*Man[-_\s.]*Ventures|Northzone|Warburg[-_\s.]*Serres|Alan[-_\s.]*Howard|Tiger[-_\s.]*Global
 Vitalik Buterin,\bvitalik\b
 Voyager,voyager
+Wanxiang Group,wanxiang|\bFeng[-_\s.]*Xiao
 Wallet Addresses BCH,bitcoincash:q.*\b
 Wallet Addresses Bitcoin,\b(bc1|[13])[a-zA-HJ-NP-Z0-9]{25,39}\b
 Wallet Addresses Cardano,\baddr1[a-z0-9]+\b
 Wallet Addresses Cosmos,\bcosmos[a-zA-Z0-9_.-]{10,}\b
 Wallet Addresses Dash,\bX[1-9A-HJ-NP-Za-km-z]{33}
 Wallet Addresses Doge,\bD[a-zA-Z0-9_.-]{33}
 Wallet Addresses Ethereum,0x[a-fA-F0-9]{40}
```

### Comparing `clown_sort-1.7.1/clown_sort/util/argument_parser.py` & `clown_sort-1.8.0/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/clown_sort/util/constants.py` & `clown_sort-1.8.0/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/clown_sort/util/filesystem_helper.py` & `clown_sort-1.8.0/clown_sort/util/filesystem_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 IMAGE_FILE_EXTENSIONS = [f".{ext}" for ext in 'tiff jpg jpeg png heic'.split()]
 MOVIE_FILE_EXTENSIONS = ['.mov', '.flv', '.avi']
 SORTABLE_FILE_EXTENSIONS = IMAGE_FILE_EXTENSIONS + [PDF_EXTENSION, '.mov']
 MAC_SCREENSHOT_TIMESTAMP_FORMAT = '%Y-%m-%d at %I.%M.%S %p'
 
 
 def files_in_dir(dir: Union[os.PathLike, str], with_extname: Optional[str] = None) -> List[str]:
-    """Paths for non-hidden files, optionally ending in 'with_extname'"""
+    """Paths for non-hidden, non-directory files, optionally ending in 'with_extname'"""
     files = [file for file in _non_hidden_files_in_dir(dir) if not path.isdir(file)]
 
     if with_extname:
         files = [f for f in files if f.endswith(f".{with_extname}")]
 
     return files
```

### Comparing `clown_sort-1.7.1/clown_sort/util/rich_helper.py` & `clown_sort-1.8.0/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/clown_sort/util/string_helper.py` & `clown_sort-1.8.0/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.1/pyproject.toml` & `clown_sort-1.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.7.1"
+version = "1.8.0"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.7.1/PKG-INFO` & `clown_sort-1.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.7.1
+Version: 1.8.0
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
@@ -164,14 +164,24 @@
 ```sh
 pipx install clown_sort[gui]
 ```
 
 ![](doc/manual_select_box.png)
 
 
+## One Offs
+There is a script you can use to extract text from a single file (or a bunch of files, or all the files in a given directory). Just run:
+
+```
+scripts/extract_text_from_files.py MY_FILE1 MY_FILE2 SOME_DIR3
+```
+
+This will parse and display the text in `MY_FILE1`, `MY_FILE2`, and all the files in `SOME_DIR3`.
+
+
 # Contributing
 Feel free to file issues or open pull requests.
 
 This package is managed with [Python Poetry](http://python-poetry.org/). To get going:
 1. Install Poetry.
 1. `git clone` this repo.
 1. `cd clown_sort`
```

