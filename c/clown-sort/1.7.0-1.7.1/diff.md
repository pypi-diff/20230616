# Comparing `tmp/clown_sort-1.7.0.tar.gz` & `tmp/clown_sort-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.7.0.tar", max compression
+gzip compressed data, was "clown_sort-1.7.1.tar", max compression
```

## Comparing `clown_sort-1.7.0.tar` & `clown_sort-1.7.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     3216 2023-06-03 00:37:57.393324 clown_sort-1.7.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.7.0/LICENSE
--rw-r--r--   0        0        0     8766 2023-06-03 00:17:25.185210 clown_sort-1.7.0/README.md
--rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.7.0/clown_sort/__init__.py
--rw-r--r--   0        0        0     7987 2023-06-03 00:19:42.985646 clown_sort-1.7.0/clown_sort/config.py
--rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.7.0/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.7.0/clown_sort/files/image_file.py
--rw-r--r--   0        0        0     2756 2023-06-02 21:34:09.379034 clown_sort-1.7.0/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0    11399 2023-06-02 21:49:12.145554 clown_sort-1.7.0/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3310 2023-06-02 21:07:10.228823 clown_sort-1.7.0/clown_sort/sort_selector.py
--rw-r--r--   0        0        0    10323 2023-06-03 00:36:44.463991 clown_sort-1.7.0/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.7.0/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.7.0/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.7.0/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3690 2023-06-02 22:06:05.123239 clown_sort-1.7.0/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.7.0/clown_sort/util/logging.py
--rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.7.0/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.7.0/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1619 2023-06-03 00:37:57.396990 clown_sort-1.7.0/pyproject.toml
--rw-r--r--   0        0        0    10188 1970-01-01 00:00:00.000000 clown_sort-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0     3274 2023-06-15 23:50:36.857435 clown_sort-1.7.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.7.1/LICENSE
+-rw-r--r--   0        0        0     8766 2023-06-03 00:17:25.185210 clown_sort-1.7.1/README.md
+-rw-r--r--   0        0        0     3369 2023-05-27 22:11:48.831591 clown_sort-1.7.1/clown_sort/__init__.py
+-rw-r--r--   0        0        0     7987 2023-06-03 00:19:42.985646 clown_sort-1.7.1/clown_sort/config.py
+-rw-r--r--   0        0        0     9021 2023-06-02 20:58:04.234216 clown_sort-1.7.1/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4711 2023-05-27 16:06:01.553047 clown_sort-1.7.1/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     3069 2023-06-15 23:22:00.182053 clown_sort-1.7.1/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0    11399 2023-06-02 21:49:12.145554 clown_sort-1.7.1/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3456 2023-06-15 23:17:52.887054 clown_sort-1.7.1/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0    11363 2023-06-15 23:40:16.589247 clown_sort-1.7.1/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3506 2023-04-24 00:53:03.331251 clown_sort-1.7.1/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1559 2023-05-09 18:20:37.531689 clown_sort-1.7.1/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.7.1/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3690 2023-06-02 22:06:05.123239 clown_sort-1.7.1/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.7.1/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     3427 2023-05-27 22:16:38.822426 clown_sort-1.7.1/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0      667 2023-05-27 16:06:01.554255 clown_sort-1.7.1/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1619 2023-06-15 23:50:36.863775 clown_sort-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0    10188 1970-01-01 00:00:00.000000 clown_sort-1.7.1/PKG-INFO
```

### Comparing `clown_sort-1.7.0/CHANGELOG.md` & `clown_sort-1.7.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # NEXT RELEASE
 
+### 1.7.1
+* Handle 0 byte PDF error
+* More default rules
+
 # 1.7.0
 * Skip comment rows starting with `#` in rules CSVs.
 * New default rules
 
 ### 1.6.4
 * Crop very long PDF pages when previewing in manual select window
 * Fix regexes for wallet addresses
```

### Comparing `clown_sort-1.7.0/LICENSE` & `clown_sort-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/README.md` & `clown_sort-1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/__init__.py` & `clown_sort-1.7.1/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/config.py` & `clown_sort-1.7.1/clown_sort/config.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/filename_extractor.py` & `clown_sort-1.7.1/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/files/image_file.py` & `clown_sort-1.7.1/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/files/pdf_file.py` & `clown_sort-1.7.1/clown_sort/files/pdf_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Wrapper for PDF files.
 """
 import logging
 from sys import exit
 from typing import Optional
 
 from pypdf import PdfReader
-from pypdf.errors import DependencyError
+from pypdf.errors import DependencyError, EmptyFileError
 
 from clown_sort.config import check_for_pymupdf, log_optional_module_warning
 from clown_sort.util.rich_helper import WARNING, console
 from clown_sort.util.logging import log
 from clown_sort.files.sortable_file import SortableFile
 
 MAX_DISPLAY_HEIGHT = 600
@@ -22,35 +22,44 @@
 
     def extracted_text(self) -> Optional[str]:
         """Use Tesseract to OCR the text in the image, which is returned as a string."""
         if self.text_extraction_attempted:
             return self._extracted_text
 
         self._extracted_text = None
+        log.debug(f"Extracting text from '{self.file_path}'...")
 
         try:
             pdf_reader = PdfReader(self.file_path)
             self._extracted_text = '\\n\\n'.join([page.extract_text() for page in pdf_reader.pages])
         except DependencyError:
             log_optional_module_warning('pdf')
+        except EmptyFileError:
+            log.warn("Skipping empty file!")
         except (KeyError, TypeError):
             # TODO: failure on KeyError: '/Root' seems to have been fixed but not released yet
             # https://github.com/py-pdf/pypdf/pull/1784
             log.warn("Failed to parse PDF!")
 
         if self._extracted_text is not None:
             self._extracted_text = self._extracted_text.strip()
 
         self.text_extraction_attempted = True
         return self._extracted_text
 
-    def thumbnail_bytes(self) -> bytes:
+    def thumbnail_bytes(self) -> Optional[bytes]:
         """Return bytes for a thumbnail."""
         import fitz
-        doc = fitz.open(self.file_path)
+        log.debug(f"Getting bytes for '{self.file_path}'...")
+
+        try:
+            doc = fitz.open(self.file_path)
+        except fitz.fitz.EmptyFileError:
+            return None
+
         zoom_matrix = fitz.Matrix(fitz.Identity).prescale(SCALE_FACTOR, SCALE_FACTOR)
         page = doc[0]
         bottom_right = page.rect.br
         page_height = bottom_right[1]
         page_width = bottom_right[0]
 
         # Check for PDFs with very long pages and crop them
```

### Comparing `clown_sort-1.7.0/clown_sort/files/sortable_file.py` & `clown_sort-1.7.1/clown_sort/files/sortable_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/sort_selector.py` & `clown_sort-1.7.1/clown_sort/sort_selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,17 +24,22 @@
 def process_file_with_popup(image: Union['ImageFile', 'PdfFile']) -> None:
     # Do the import here so as to allow usage without installing PySimpleGUI
     import PySimpleGUI as psg
     psg.theme('SystemDefault1')
     suggested_filename = FilenameExtractor(image).filename()
     sort_dirs = [path.basename(dir) for dir in Config.get_sort_dirs()]
     max_dirname_length = max([len(dir) for dir in sort_dirs])
+    thumbnail_bytes = image.thumbnail_bytes()
+
+    if thumbnail_bytes is None:
+        log.warn(f"Failed to get a thumbnail; skipping...")
+        return
 
     layout = [
-        [psg.Column([[psg.Image(data=image.thumbnail_bytes(), key="-IMAGE-")]], justification='center')],
+        [psg.Column([[psg.Image(data=thumbnail_bytes, key="-IMAGE-")]], justification='center')],
         [psg.HSep()],
         [psg.Text("Choose Filename:")],
         [psg.Input(suggested_filename, size=(len(suggested_filename), 1))],# font=("Courier New", 12))],
         [
             psg.Text(f"Choose Directory:"),
             psg.Combo(sort_dirs, size=(max_dirname_length, SELECT_SIZE)),
             psg.Text(f"(Enter custom text to create new directory. If no directory is chosen file will be copied to '{Config.sorted_screenshots_dir}'.)")
```

### Comparing `clown_sort-1.7.0/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.7.1/clown_sort/sorting_rules/crypto.csv`

 * *Files 9% similar despite different names*

```diff
@@ -1,101 +1,106 @@
 folder,regex
 1mdb,1mdb|jho[-_\s.]*low|Victor[-_\s.]*Hoo
 3ac,3ac|Three[-_\s.]*Arrows[-_\s.]*Capital|su[-_\s.]*zhu|zhu[-_\s.]*su|kyle[-_\s.]*davies|OPNX
-A16Z,a16z|Andreessen|Packym|Arianna[-_\s1]*Simpson
+A16Z,a16z|Andreessen|Packym|Arianna[-_\s1]*Simpson|Ben[-_\s.]*Horowitz|\bAXS\b
 Aave,\bAave
+Abra,\bAbra\b|\bPlutus\b|\bBarhydt
 AAX,\baax
 Algorand,\bAlgorand|\b[$#]ALGO\b
 Arbitrum,Arbitrum|[$#]ARB\b
 Amber Group,Amber[-_\s.]*Group|\btiantian\b|\bkullander\b|\btony[-_\s.]*he\b|\bbo[-_\s.]*shen\b
 Aptos,\bAptos\b
 Art,occult
 Avalanche,\bAvax|AVAX\b|avalanche|\bava[-_\s.]*labs
 Banks,SEBA[^a-z]|Credit[-_\s.]*Suisse|SJMBT|Sygnum|Celtic[-_\s.]*Bank|\bMercury\b|Choice[-_\s.]*Financial[-_\s.]*Group|\$FRC|Commercium[-_\s.]*Financial|\bmetabank|\bHBAN\b|Huntington[-_\s.]*Bancshares|United[-_\s.]*Texas|\bUTB\b|Craig[-_\s.]*Sellars
 Bankless,Bankless|David[-_\s.]*Hoffman
 Biconomy,\bBiconomy|Omchain
 Binary Options,binary[-_\s.]*options
-Binance,binance|\bbiconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|\bjoselito\b|\bpaysafe|\bSwipe[-_\s.]*(IO|Wallet)|\bkeyway|\bkey[-_\s.]*vision|\bTrustWallet\b|BUSD\b|\boztures|Kaiser[-_\s.]*Ng|InvestByBit|Swyftx
+Binance,binance|\bbiconomy|\bbnb\b|\bbsc\b|\bcz\b|\bbifinity\b|binaryx|\bbillance|changpeng|\bjoselito\b|\bpaysafe|\bSwipe[-_\s.]*(IO|Wallet)|\bkeyway|\bkey[-_\s.]*vision|\bTrustWallet\b|BUSD\b|\boztures|Kaiser[-_\s.]*Ng|InvestByBit|Swyftx|Guangying[-_\s.]*Chen|\bcoley\b|\bBAM\b|\bFlowbank|\bnuvei\b|\borum\b|Worldpay|Bijie[-_\s.]*(Network|Tech)|Venus[-_\s.]*(Protocol|Community)
 Bitdeer,Bitdeer
 BitGet,Bitget
 Bithumb,\bbithumb
 Bitmain,Bitmain
+BitMex,Bitmex|Arthur[-_\s.]*Hayes
 Bitstamp,Bitstamp
 Bittrex,Bittrex|Ritchie[-_\s.]*Lai|Kiran[-_\s.]*Raj|John[-_\s.]*Roth\b|\bAquila\b
 Bitzlato,Bitzlato
 Blockchain.com,\bblockchain\.com\b|@blockchain\b|@AskBlockchain\b|Patrick[-_\s.]*McHenry
 Blockchain8,Blockchain8|tom[-_\s.]*emmer|ritchie[-_\s.]*torres|repritchie|Warren[-_\s.]*Davidson|Byron[-_\s.]*Donalds|Ted[-_\s.]*Budd|Josh[-_\s.]*Gotheimer|Jake[-_\s.]*Auchincloss|Darren[-_\s.]*Soto|ro[-_\s.]*khanna|KMSmithDC|Kristin[-_\s.]*Smith\b|Warren[-_\s.]*Davidson
 Blockchain Capital,Blockchain[-_\s.]*Capital|\bbrock\b|brockpierce
 BlockFi,BlockFi|Zac[-_\s.]*Prince|Brian[-_\s.]*Oliver
 Blockstream,Blockstream
 Bored Ape Yacht Club,BAYC|Bored[-_\s.]*Ape|yuga[-_\s.]*labs
-Bros,cryptomanran|trillionUSD|nic[-_\s.]*carter|bitboy|ben[-_\s.]*armstrong|basedkarbon|thecryptolark|adam([-_\s.]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s.]*Alfred|natbrunell|natalie[-_\s.]*brunell|stackersatoshi|Max[-_\s.]*Keiser|Cowboy[-_\s.]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s.]*Paul\b|raoul(gmi|[-_\s.]*pal)|mccormack|andr3w|andrew[-_\s.]*wang|\b(JW)?[-_\s.]*Verret\b|@FlurETH\b
+Bros,cryptomanran|\bRan[-_\s.]*Neuner|trillionUSD|nic[-_\s.]*carter|bitboy|ben[-_\s.]*armstrong|basedkarbon|thecryptolark|adam([-_\s.]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s.]*Alfred|natbrunell|natalie[-_\s.]*brunell|stackersatoshi|Max[-_\s.]*Keiser|Cowboy[-_\s.]*Crypto|minimalcsgo|greg16676935420|@Aridavidpaul|\bAri[-_\s.]*Paul\b|raoul(gmi|[-_\s.]*pal)|mccormack|andr3w|andrew[-_\s.]*wang|\b(JW)?[-_\s.]*Verret\b|@FlurETH\b|wolf[-_\s.]*of[-_\s.]*all[-_\s.]*streets|scott[-_\s.]*melker
 Broettes,Nicole[-_\s.]*Behnam|natbrunell
 Bybit,\bBybit\b|Ben[-_\s.]*Zhou|InvestByBit|TravelByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson|\bIOHK
 Cathie Wood,Cathie[-_\s.]*Wood|\bARK(F|G|K|[-_\s.]*Innovation|[-_\s.]*Invest)|\bIZRL
 Celsius,celsius|mashinsky|levity[-_\s.]*and[-_\s.]*love|\bcelsian|Artur[-_\s.]*Abreu|ronpaulbot|\bnuke[-_\s.]*gold(stein)?
 China,fentanyl|\bchin(a|ese)|Hong[-_\s.]*Kong
-Circle,[@#]circle|usdc|circle[-_\s.]*internet|disparte|\ballaire|jerallaire
+Circle,[@#]circle|usdc|circle[-_\s.]*internet|disparte|\ballaire|jerallaire|Macromedia
 CMCC Global,CMCC[-_\s.]*Global
 Coinbase,Coinbase|\$COIN|brian[-_\s.]*armstrong|grewal\b|Asiff[-_\s.]*Hirji|\bbalaji|Fred[-_\s.]*Ehrsam|\bremitly\b|\$RELY\b
 Coinflex,Mark[-_\s.]*Lamb|Roger[-_\s.]*Ver|coinflex|Doug[-_\s.]*Polk|OPNX|flexusd|Leslie[-_\s.]*Lamb|dougpolkvids
 CoinLoan,coinloan|Faliushin\b
 CompoundFi,compoundfi|leshner|\bgonen\b
 ConsenSys,ConsenSys
-Cross River Bank,\bCRB|Cross[-_\s.]*River|Prestige[-_\s.]*Capital|\bbae[-_\s.]*communications|Zenfi\b|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv|\bKabbage|\bAFRM\b
-Cumberland,cumberland
-Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s
+Cross River Bank,\bCRB|Cross[-_\s.]*River|Prestige[-_\s.]*Capital|\bbae[-_\s.]*communications|Zenfi\b|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim|BetterFin|\bMANTL\b|\bLvnv|\bKabbage|\bAFRM\b|\bMomnt
+Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s|Doug(las)?[-_\s.]*Ching\b
 CUBI,\bCUBI\b|Customers[-_\s.]*Ban(k|corp)
+Cumberland,cumberland
 Custodia,custodia\b|caitlin[-_\s.]*long
 dalle,craiyon|midjourney|\bdall[-_\s.]*e\b
-DCG,DCG|digital[-_\s.]*currency[-_\s.]*group|sh?ill?bert|Grayscale|GBTC|\bkraines\b
+DCG,DCG|digital[-_\s.]*currency[-_\s.]*group|sh?ill?bert|Grayscale|GBTC|\bkraines\b|hq[-_\s.]*digital|Alana[-_\s.]*Ackerson|Jennifer[-_\s.]*Mitrenga|Emily[-_\s.]*(Heather[-_\s.]*)?Goodman|Founders[-_\s.]*Liquidity[-_\s.]*Fund
 DeFi,\bdefi\b|decentralized[-_\s.]*finance
 Dragonfly Capital,Dragonfly[-_\s.]*Capital
 DWF,DWF|Andrey[-_\s.]*Grachev|\bgrachev\b
 Evolve Bank,getevolved|\bevolve[-_\s.]*bank\b
 Effective Altruism,\bE\.?A\.?\b|effective[-_\s.]*altruism
 El Salvador,El[-_\s.]*Salvador|Bukele|Max[-_\s.]*Keiser
 Elon Musk,\bTesla\b|\bTSLA\b|\bElon\b|\bElmo\b
 EOS,\bEOS\b|\bBlumer\b|\bLarimer\b|@B1\b|Block[-_\.\s]One
 Evertas,\bEvertas\b|Ryan[-_\s.]*Lackey
 Euler Finance,\beuler\b
 FalconX,falconx
+First Digital,First[-_\s.]*Digital\b
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
 Frax,\bFrax\b|\bFRX|[\b#$]FXS
 Friedlander Group,Friedlander|Agro[-_\s.]*Bank|\ball[-_\s.]*year\b|\bbrock\b|brockpierce|litvishhocker
 FTX,FTX|\bFTT\b|\bSBF|Trabucco|\bBankman\b|\bEllison|\bNishad|\bAlameda|Moonstone|friedberg|autism[-_\s.]*capital|\bryne\b|clifton[-_\s.]*bay|\bZUBR\b
 Galaxy Digital,novogratz|Alex[-_\s.]*Thorn
+Gate.io,Gate[_.]?IO
 Gelato Network,Gelato[-_\s.]*Network|\bSorbet[-_\s.]*Finance|@gitpusha|hilmar[-_\s.]*x|\bmistx\b|@_alchemistcoin|@ChaosLabs_NFT|Arrakis[-_\s.]*Finance|Dave[-_\s.]*Leibowitz|Hilmar[-_\s.]*Orth|joehquak
 Gemini,Gemini|winklev|@cameron
 Genesis,Genesis|Michael\s?Moro
 Goldfinch,goldfinch
 Hamas,\bHamas\b|Al[-_\s.]*Qassam
+Haru Invest,\bHaru(invest)?\b|\b(happy)?Delio\b
 Hex,\bHex\b|[#$]Hex|Pulsechain|Richard[-_\s.]*Heart|Hexican
 Hoo,Hoo[-_\s.]*(Research|Exchange)|[#$]Hoo\b|Rexy[-_\s.]*(Hoo|Wang)|\bhoo\b
 Huobi,huobi|jiao_newlife|jiaojiao|Leon[-_\s.]*Li
 Iran,\bIran\b|\bIranian\b|Nobitex|\bCoinNik|\bWallex\b|Sarmayex|\bRabex\b
 Jump Trading,Jump[-_\s.]*Trading|@jump_
-Justin Sun,justin[-_\s.]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina
+Justin Sun,justin[-_\s.]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina|\bR(ebo|ible)\b|Love[-_\s.]*Letters[-_\s.]*Limited|Objectivists[-_\s.]*Limited
 Kazakhstan,\bkazakh|Freedom[-_\s.]*Holding|\balmaty|Timor[-_\s.]*Turlov|\bFFIN[-_\s.]*brokerage
 Kinesis,kinesis|\bKVT\b|\bABX\b|\bKAG\b
-Kraken,kraken|payward
+Kraken,kraken|payward|\bjespow\b|Jesse[-_\s.]*Powell
 KuCoin,kucoin
 Lead Bank,\bLead[-_\s.]*Bank\b|Finzly
 LBRY,LBRY|\bLBC\b
 Lexpunk Army,lexpunk|gabriel[-_\s.]*shapiro|_gabrielShapir0|\blex_node\b
 Lifeboat Foundation,Lifeboat[-_\s.]*Foundation
 North Korea,lazarus|North[-_\s.]*Korea|pyongyang|\bDPRK|puuurtbubv|@fast4release
 Paul LeRoux,leroux
 Polygon Labs,polygon[-_\s.]*labs|ryan[-_\s.]*watt\b|@Fwiz|Rebecca[-_\s.]*Rettig|[#$]DOT\b
 MakerDAO,makerdao|[$#\s]DAI[^\w]
 Marathon,\$MARA|marathon
-Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s.]*Cheng|\bBeauregard\b|\bGoCoin\b|Advent[-_\s.]*International|Keystone[-_\s.]*Capital[-_\s.]*Partners
+Matthew Roszak,\broszak|matthewroszak|Calvin[-_\s.]*Cheng|\bBeauregard\b|\bGoCoin\b|Advent[-_\s.]*International|Keystone[-_\s.]*Capital[-_\s.]*Partners|\bGarzik\b
 Mario Nawfal,mario[-_\s.]*nawfal
 Messari,Ryan[-_\s.]*Selkis|twobitidiot|messari|@robustus|Dan[-_\s.]*McArdle
 Memes,\smeme
 Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s.]*Stewart|\bHayner\b
 Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s.]*(Bank|Commercial)|Mission[-_\s.]*Gateway|Aryeh[-_\s.]*Realty
 Multichain,Multichain\b
 Founders Bank,Michael[-_\s.]*Bianchi|Founders[-_\s.]*Bank
@@ -105,42 +110,46 @@
 MSTR,Saylor|MSTR
 MtGox,Mt[-_\s.]*Gox|\bwilly[-_\s.]*bot
 Near Protocol,NEAR[-_\s.]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s.]*Rettig
 Nexo,\bNexo\b|Antoni[-_\s.]*Trenchev|Georgi[-_\s.]*Shulev|Lydia[-_\s.]*Shuleva
 NFTs,crypto[-_\s.]*punk|pudgy[-_\s.]*penguin
 OKX,oke?[cx]|star[-_\s.]*xu|\blennix[-_\s.]*lai\b
 Olympus DAO,\bOlympus\b|OlympusDAO|\bOHM\b
+Ooki DAO,\bOoki(DAO)?\b
+OneCoin,\bOne(Coin|Life)\b
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea
 PAG,\bpag\b|Weijian[-_\s.]*Shan
 Paradigm,Fred[-_\s.]*Ehrsam|paradigm\b
 Paxful,paxful|Ray[-_\s.]*(Youssef|Savant)|Artur[-_\s.]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
 Payrnet,payrnet|railsr|railsbank
 Pi,\$PI[^\w]|Pi[-_\s.]*Network
 Politics,\bted[-_\s.]*cruz
-Prime Trust,Prime[-\s_]?Trust
+Prime Trust,Prime[-\s_]*Trust|\bBanq\b|Scott\bPurcell|(Planet|Fortress)[-\s_]*(Xyz|Trust|NFT)|George[-\s_]*Georgiades|Kevin[-\s_]*Lehtiniitty|PrimeX\b|\bSroge\b|\banonalyx
 PVBC,PVBC|BankProv
 Quadriga,Quadriga|Gerald[-_\s.]*Cotten|0xsifu\b|michael[-_\s.]*patryn|wonderland|daniele[-_\s.]*sesta\b
 Revolut,revolut[^\w]
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,[$#]RIOT\b|Riot[-\s_]*(Block|Platform)|Bioptix
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
-SEC,\bSEC(\b|Gov)|\bGensler|CFTC|Securities.{0,6}Exchange.{0,6}Commission
+SEC,\bSEC(\b|Gov)|\b(Gary)?Gensler|CFTC|Securities.{0,6}Exchange.{0,6}Commission
 Signature Bank,SBNY|Signature[-_\s.]*Bank|Signet|Scott[-_\s.]*Shay\b|(Joseph|Joe)[-_\s.]*DePaolo|\bKushner\b
 Silicon Valley Bank,si?vb|Silicon[-_\s.]*Valley[-_\s.]*Bank
 Silk Road,Silk[-_\s.]*Road|\bulbricht|\bDPR\b
 Silvergate,\$SI|Silvergate|Alan[-_\s.]*Lane|Eisele|\bSEN\b|SENnetwork|Rebecca[-_\s.]*Rettig
 Skrill,\bskrill
 Solana,Solana|Serum
+Stellar,\bstellar\b
+Stifel Bank,\bStifel\b|[#$]SF\b
 Symbolic Capital,Symbolic[-_\s.]*Capital|Lev[-_\s]Livnev
 Synapse,Synapse(fi|labs|protocol)?\b
-TerraLuna,luna\b|do[-_\s.]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s.]*Foundation\b
-Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|hoegner|Noble[-_\s.]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Noblex|SJMBT|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s.]*Potter|Stablehouse|Samson[-_\s.]*Mow|Gabor[-_\s.]*Grubacs|XBTO|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s.]*Collins|\bdevasini\b|phil(ip)?[-_\s.]*potter\b|van[-_\s.]*der[-_\s.]*velde|Perpetual[-_\s.]*Action[-_\s.]*Group|\burwhatyouknow|global[-_\s.]*trade[-_\s.]*solutions|reginald[-_\s.]*fowler|renrenbee\b|\bludovicus|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s.]*payments|Five[-_\s.]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec|Mainstreet[-_\s.]*Partners
+TerraLuna,luna\b|do[-_\s.]*kwon|stablekwon|\bterra\b|Macedo|\bLuna[-_\s.]*Foundation\b
+Tether,\btether\b|usdt|paolo\b|paoloardoino|friedberg|hoegner|Noble[-_\s.]*Bank|\bDeltec[^\']|b(e|i)tfinex[^e]|\bbrock([-_\s.]*pierce)?\b|Clearstone[-_\s.]*Global|Capital[-_\s.]*Union|Noblex|SJMBT|Global[-_\s.]*Trad(ing|e)[-_\s.]*Solutions|(dig|i)finex|BFXNA|BFXWW|[$#]Leo\b|Phil[-_\s.]*Potter|Stablehouse|Samson[-_\s.]*Mow|Gabor[-_\s.]*Grubacs|XBTO|Paul[-_\s.]*Eisma|Philippe[-_\s.]*Bekhazi|\b(Master|Real)coin\b|Reeve[-_\s.]*Collins|\bdevasini\b|phil(ip)?[-_\s.]*potter\b|van[-_\s.]*der[-_\s.]*velde|Perpetual[-_\s.]*Action[-_\s.]*Group|\burwhatyouknow|global[-_\s.]*trade[-_\s.]*solutions|reginald[-_\s.]*fowler|renrenbee\b|\bludovicus|Amos[-_\s.]*Ltd|William[-_\s.]*Quigley|Sunlot\b|\bD10e\b|\bGoCoin\b|Blade[-_\s.]*payments|Five[-_\s.]*Delta|\bXfire\b|\bPlaysino\b|\bEvertune|\bGamesTV|\bethfinex|coinapult|gabriel[-_\s.]*sukenik|R(ondell|[ho][ho]n)[-_\s.]*(Clyde)?[-_\s.]*Monroe|\bTuxia\b|\bIGEL\b|\bInfomatec|Mainstreet[-_\s.]*Partners|\bMallers\b
 Tornado Cash,tornado[-_\s.]*cash
 Transactive Systems UAB,Transactive
 Tron,\btron\b|tron(block|[-_\s.]*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
 VCs,venture[-_\s.]*capital|\bVCs?\b|calacanis|@jason\b|david[-_\s.]*sacks|\bthiel\b|sequoia|founders[-_\s.]*fund|Valar[-_\s.]*Ventures|6th[-_\s.]*Man[-_\s.]*Ventures|Northzone|Warburg[-_\s.]*Serres|Alan[-_\s.]*Howard|Tiger[-_\s.]*Global
 Vitalik Buterin,\bvitalik\b
@@ -155,8 +164,9 @@
 Wallet Addresses Monero,\b[48][0-9AB][1-9A-HJ-NP-Za-km-z]{93}
 Wallet Addresses Polkadot,\b1[0-9a-zA-Z]{47}
 Wallet Addresses Ripple,\br[0-9a-zA-Z]{33}
 Wallet Addresses Stellar,\bG[0-9A-Z]{40,60}\b
 Waves,sasha35625|sasha\.waves|\bvires|sasha[-_\s.]*ivanov|boris[-_\s.]*titov|[$#]waves\b
 Wintermute,wintermute|\bbebop\b
 Wirecard,wirecard|\bmarsalek\b|\bBafin\b
-Wyre,\bwyre|sendwyre|\bLead[-_\s.]*Bank\b
+Worldcoin,Worldcoin|\borb\b
+Wyre,\bwyre|sendwyre|\bLead[-_\s.]*Bank\b|Steven[-_\s.]*Huynh
```

### Comparing `clown_sort-1.7.0/clown_sort/util/argument_parser.py` & `clown_sort-1.7.1/clown_sort/util/argument_parser.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/util/constants.py` & `clown_sort-1.7.1/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/util/filesystem_helper.py` & `clown_sort-1.7.1/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/util/rich_helper.py` & `clown_sort-1.7.1/clown_sort/util/rich_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/clown_sort/util/string_helper.py` & `clown_sort-1.7.1/clown_sort/util/string_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.7.0/pyproject.toml` & `clown_sort-1.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.7.0"
+version = "1.7.1"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
```

### Comparing `clown_sort-1.7.0/PKG-INFO` & `clown_sort-1.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.7.0
+Version: 1.7.1
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

