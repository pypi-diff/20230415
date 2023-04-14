# Comparing `tmp/clown_sort-1.3.0.tar.gz` & `tmp/clown_sort-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clown_sort-1.3.0.tar", max compression
+gzip compressed data, was "clown_sort-1.3.1.tar", max compression
```

## Comparing `clown_sort-1.3.0.tar` & `clown_sort-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1515 2023-04-08 19:53:14.230615 clown_sort-1.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.3.0/LICENSE
--rw-r--r--   0        0        0     6799 2023-04-07 00:33:31.752002 clown_sort-1.3.0/README.md
--rw-r--r--   0        0        0     3243 2023-03-01 08:49:45.644326 clown_sort-1.3.0/clown_sort/__init__.py
--rw-r--r--   0        0        0     6481 2023-04-07 00:35:30.510105 clown_sort-1.3.0/clown_sort/config.py
--rw-r--r--   0        0        0     7607 2023-04-07 00:25:54.119824 clown_sort-1.3.0/clown_sort/filename_extractor.py
--rw-r--r--   0        0        0     4090 2023-03-25 04:05:46.024955 clown_sort-1.3.0/clown_sort/files/image_file.py
--rw-r--r--   0        0        0      811 2023-03-01 06:48:04.940218 clown_sort-1.3.0/clown_sort/files/pdf_file.py
--rw-r--r--   0        0        0     9023 2023-04-07 00:36:43.260639 clown_sort-1.3.0/clown_sort/files/sortable_file.py
--rwxr-xr-x   0        0        0     3109 2023-02-27 05:37:46.609295 clown_sort-1.3.0/clown_sort/sort_selector.py
--rw-r--r--   0        0        0     5392 2023-04-07 17:58:30.359470 clown_sort-1.3.0/clown_sort/sorting_rules/crypto.csv
--rw-r--r--   0        0        0     3343 2023-04-07 00:34:34.095790 clown_sort-1.3.0/clown_sort/util/argument_parser.py
--rw-r--r--   0        0        0     1455 2023-02-27 03:16:08.096928 clown_sort-1.3.0/clown_sort/util/constants.py
--rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.3.0/clown_sort/util/dict_helper.py
--rw-r--r--   0        0        0     3372 2023-02-27 01:29:17.019569 clown_sort-1.3.0/clown_sort/util/filesystem_helper.py
--rw-r--r--   0        0        0      372 2023-02-22 15:45:18.161513 clown_sort-1.3.0/clown_sort/util/logging.py
--rw-r--r--   0        0        0     2725 2023-02-27 12:32:42.820775 clown_sort-1.3.0/clown_sort/util/rich_helper.py
--rw-r--r--   0        0        0      167 2023-02-20 21:09:37.440942 clown_sort-1.3.0/clown_sort/util/string_helper.py
--rw-r--r--   0        0        0     1441 2023-04-08 19:53:08.440362 clown_sort-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     8205 1970-01-01 00:00:00.000000 clown_sort-1.3.0/setup.py
--rw-r--r--   0        0        0     8047 1970-01-01 00:00:00.000000 clown_sort-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1759 2023-04-14 23:33:23.641199 clown_sort-1.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1078 2023-02-19 21:54:39.742371 clown_sort-1.3.1/LICENSE
+-rw-r--r--   0        0        0     7434 2023-04-14 22:57:58.586571 clown_sort-1.3.1/README.md
+-rw-r--r--   0        0        0     3243 2023-03-01 08:49:45.644326 clown_sort-1.3.1/clown_sort/__init__.py
+-rw-r--r--   0        0        0     6991 2023-04-14 22:38:02.184270 clown_sort-1.3.1/clown_sort/config.py
+-rw-r--r--   0        0        0     7607 2023-04-07 00:25:54.119824 clown_sort-1.3.1/clown_sort/filename_extractor.py
+-rw-r--r--   0        0        0     4090 2023-03-25 04:05:46.024955 clown_sort-1.3.1/clown_sort/files/image_file.py
+-rw-r--r--   0        0        0     1356 2023-04-14 22:52:16.476471 clown_sort-1.3.1/clown_sort/files/pdf_file.py
+-rw-r--r--   0        0        0     9225 2023-04-14 23:29:52.404808 clown_sort-1.3.1/clown_sort/files/sortable_file.py
+-rwxr-xr-x   0        0        0     3109 2023-04-14 22:23:25.165083 clown_sort-1.3.1/clown_sort/sort_selector.py
+-rw-r--r--   0        0        0     5954 2023-04-14 23:31:10.625862 clown_sort-1.3.1/clown_sort/sorting_rules/crypto.csv
+-rw-r--r--   0        0        0     3298 2023-04-14 23:18:26.928346 clown_sort-1.3.1/clown_sort/util/argument_parser.py
+-rw-r--r--   0        0        0     1455 2023-02-27 03:16:08.096928 clown_sort-1.3.1/clown_sort/util/constants.py
+-rw-r--r--   0        0        0      196 2023-03-25 04:04:12.967064 clown_sort-1.3.1/clown_sort/util/dict_helper.py
+-rw-r--r--   0        0        0     3372 2023-02-27 01:29:17.019569 clown_sort-1.3.1/clown_sort/util/filesystem_helper.py
+-rw-r--r--   0        0        0      372 2023-04-14 22:24:41.414299 clown_sort-1.3.1/clown_sort/util/logging.py
+-rw-r--r--   0        0        0     2876 2023-04-14 23:10:01.312077 clown_sort-1.3.1/clown_sort/util/rich_helper.py
+-rw-r--r--   0        0        0       52 2023-04-14 23:08:55.335981 clown_sort-1.3.1/clown_sort/util/string_helper.py
+-rw-r--r--   0        0        0     1558 2023-04-14 23:33:23.644817 clown_sort-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8995 1970-01-01 00:00:00.000000 clown_sort-1.3.1/setup.py
+-rw-r--r--   0        0        0     8798 1970-01-01 00:00:00.000000 clown_sort-1.3.1/PKG-INFO
```

### Comparing `clown_sort-1.3.0/CHANGELOG.md` & `clown_sort-1.3.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # NEXT RELEASE
 
+### 1.3.1
+* Handle unparseable PDFs with a warning instead of a crash.
+* `--yes-overwrite` option should not default to true
+* New crypto sort rules (MCB and CUBI now sorted to their own directories instead of 'Banks')
+
 ## 1.3.0
 * Ask for confirmation before overwriting files (`--yes-overwrite` option to skip the check)
 * Check if image's extracted text is already in the filename (important if rescanning)
+* New crypto sort rules
 
 ## 1.2.0
 * `--only-if-match` option
 * New crypto sort rules
 
 ## 1.1.0
 * Filenames for retweets
```

### Comparing `clown_sort-1.3.0/LICENSE` & `clown_sort-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.0/README.md` & `clown_sort-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -58,14 +58,21 @@
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
 ```
 pipx install clown_sort
 ```
 
+Some (not many) PDFs require the `pycryptodome` package. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with:
+
+```sh
+pipx install clown_sort[pycryptodome]
+```
+
+
 ### Configuring With `.clown_sort` File
 If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
 
 1. The current directory
 2. Your home directory
 
 See [the example](.clown_sort.example) for more information on what can be configured this way.
@@ -96,19 +103,33 @@
 
 
 ## Manually Sorting (Experimental)
 **This is an experimental feature.** It's only been tested on macOS.
 
 If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
 
+To use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:
+```sh
+pipx install clown_sort[PySimpleGUI]
+```
+
 ![](doc/manual_select_box.png)
 
 
 # Contributing
-Feel free to file issues or open pull requests. Only requirement is that tests should pass before you open it, which you can check with
+Feel free to file issues or open pull requests.
+
+This package is managed with [Python Poetry](http://python-poetry.org/). To get going:
+1. Install Poetry.
+1. `git clone` this repo.
+1. `cd clown_sort`
+1. `poetry install`
+1. Optional components can be install with `poetry install -E pdf -E gui`
+
+Only requirement is that tests should pass before you open it, which you can check with
 
 ```
 pytest
 ```
 
 [^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.
```

### Comparing `clown_sort-1.3.0/clown_sort/__init__.py` & `clown_sort-1.3.1/clown_sort/__init__.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.0/clown_sort/config.py` & `clown_sort-1.3.1/clown_sort/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Global configuration.
 """
 import csv
-import logging
 import re
 import sys
 from argparse import Namespace
 from collections import namedtuple
 from importlib.metadata import version
 from os import environ
 from pathlib import Path
-from typing import List, Union
+from typing import List, Optional, Union
 
 from rich import box
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 
 from clown_sort.util.argument_parser import CRYPTO, parser
@@ -165,16 +164,33 @@
         log.debug(f"processed_screenshots_dir: {cls.processed_screenshots_dir}")
 
 
 def _check_for_pysimplegui():
     try:
         import PySimpleGUI as sg
     except ModuleNotFoundError:
-        console = Console()
         msg = Text('ERROR: ', style='bright_red')
-        msg.append('PySimpleGUI package must be installed before you can use the manual selector. Try running:', style='bright_white')
-        console.line(2)
-        console.print(msg)
-        console.line(2)
-        console.print("     pipx install clown_sort[PySimpleGUI]", style='bright_cyan')
-        console.line(2)
+
+        msg.append(
+            'PySimpleGUI package must be installed before you can use the manual selector. Try running:',
+            style='bright_white'
+        )
+        log_optional_module_warning('PySimpleGUI', msg)
         sys.exit()
+
+
+# TODO: it sucks that this is here but it's dependency hell otherwise
+def log_optional_module_warning(module_name: str, msg: Optional[Text] = None) -> None:
+    """msg is optional argument for a custom message, otherwise it's a warning"""
+    if msg is None:
+        msg = Text('WARNING: ', style='bright_red').append(
+            f"Optional package '{module_name}' not installed. . Try running:",
+            style='bright_white'
+        )
+
+    console = Console()
+    console.line(2)
+    console.print(msg)
+    console.line(2)
+    console.print(f"     pipx install clown_sort[{module_name}]", style='bright_cyan')
+    console.line(2)
+
```

### Comparing `clown_sort-1.3.0/clown_sort/filename_extractor.py` & `clown_sort-1.3.1/clown_sort/filename_extractor.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.0/clown_sort/files/image_file.py` & `clown_sort-1.3.1/clown_sort/files/image_file.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.0/clown_sort/files/sortable_file.py` & `clown_sort-1.3.1/clown_sort/files/sortable_file.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 from rich.prompt import Confirm
 from rich.text import Text
 
 from clown_sort.config import Config
 from clown_sort.filename_extractor import FilenameExtractor
 from clown_sort.util.filesystem_helper import copy_file_creation_time
 from clown_sort.util.logging import log
-from clown_sort.util.rich_helper import (bullet_text, indented_bullet, console,
+from clown_sort.util.rich_helper import (bullet_text, comma_join, indented_bullet, console,
      copying_file_log_message, moving_file_log_message)
-from clown_sort.util.string_helper import comma_join
 
 MAX_EXTRACTION_LENGTH = 4096
 NOT_MOVING_FILE = "Not moving file to processed dir because it's"
 NO_SORT_FOLDERS_MSG = bullet_text('No sort folders matched so copying to base sorted dir...', style='color(209)')
 
 
 class SortableFile:
@@ -56,33 +55,37 @@
             if Config.only_if_match:
                 console.print('No folder match and --only-if-match option selected. Skipping...')
                 return
 
             console.print(NO_SORT_FOLDERS_MSG)
             sort_folders = [None]
         else:
-            console.print(bullet_text(Text('Sort folders: ') + comma_join(sort_folders)))
+            console.print(bullet_text(Text('Sort folders: ') + comma_join(sort_folders, 'sort_folder')))
 
         # Copy the renamed file to all the folders whose sorting rules were matched.
         for folder in sort_folders:
             # Create the subdir if it doesn't exist.
             if folder is not None:
                 destination_dir = Config.sorted_screenshots_dir.joinpath(folder)
 
                 if not destination_dir.is_dir() and not Config.dry_run:
                     log.info(f"Creating subdirectory '{destination_dir}'...")
                     destination_dir.mkdir()
 
             destination_path = self.sort_destination_path(folder)
 
             if destination_path.exists():
-                console.print(f"\nFile '{destination_path.name}' already exists in '{folder}/'!", style='blink')
+                console.line()
+                msg = Text('').append(f"WARNING", style='bright_yellow').append(f": File ")
+                msg.append(destination_path.name, style='cyan').append(" already exists in ")
+                msg.append(folder, style='sort_folder')
+                console.print(msg)
 
                 if not (Config.yes_overwrite or Confirm.ask(f"Overwrite?")):
-                    console.print("Skipping...")
+                    console.print("Skipping...", style='dim')
                     continue
 
             self._paths_of_sorted_copies.append(destination_path)
             self.copy_file_to_sorted_dir(destination_path)
 
         if Config.leave_in_place:
             console.print(bullet_text(Text('Leaving in place...', style='dim')))
@@ -141,15 +144,15 @@
 
     def _log_copy_file(self, destination_path: Path) -> None:
         """Log info about a file copy."""
         if Config.debug:
             console.print(copying_file_log_message(self.basename, destination_path))
             return
 
-        log_msg = Text('Copying to ')
+        log_msg = Text('').append('Copying to ', style='dim')
 
         if destination_path.parent == Config.destination_dir:
             console.print(indented_bullet(log_msg.append('root sorted dir...')))
         else:
             log_msg.append(str(destination_path.parent), style='sort_destination')
             console.print(indented_bullet(log_msg.append('...')))
 
@@ -209,13 +212,13 @@
                     log_txt.append("\n    -> Replying to ", style='color(23)')
                     log_txt.append(self._filename_extractor.reply_to_account, style='author')
 
                 yield log_txt
             elif self._filename_extractor._is_reddit():
                 yield Text("It's a reddit post", style='social_media')
 
-        log_msg = Text('Destination filename: ').append(self.new_basename(), style='cyan dim')
+        log_msg = Text('Destination filename: ').append(self.new_basename(), style='cyan')
         yield bullet_text(log_msg)
 
         if Config.debug:
             yield bullet_text('EXIF: ')
             yield f"   {self.exif_dict()}\n\n"
```

### Comparing `clown_sort-1.3.0/clown_sort/sort_selector.py` & `clown_sort-1.3.1/clown_sort/sort_selector.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.0/clown_sort/sorting_rules/crypto.csv` & `clown_sort-1.3.1/clown_sort/sorting_rules/crypto.csv`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 folder,regex
 1mdb,1mdb|jho[-_\s]*low|Victor[-_\s]*Hoo
-3ac,3ac|Three[-_\s]*Arrows[-_\s]*Capital|su[-_\s]*zhu|zhu[-_\s]*su|kyle[-_\s]*davies
+3ac,3ac|Three[-_\s]*Arrows[-_\s]*Capital|su[-_\s]*zhu|zhu[-_\s]*su|kyle[-_\s]*davies|OPNX
 A16Z,a16z|andreessen|packym|arianna[-_\s1]*simpson
 Aave,aave
 AAX,\baax
 Arbitrum,Arbitrum|[$#]ARB\b
+Amber Group,Amber[-_\s]*Group|\btiantian\b|\bkullander\b|\btony[-_\s]*he\b|\bbo[-_\s]*shen\b
+Aptos,\bAptos\b
 Art,occult
 Avalanche,\bAvax|avalanche
-Banks,\$CUBI|Customers[-_\s]*Ban(k|corp)|SEBA[^a-z]|MCB\b|MCBankNY|Metropolitan[-_\s]*Community|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group
+Banks,SEBA[^a-z]|Credit[-_\s]*Suisse|SJMBT|Sygnum|Celtic[-_\s]*Bank|\bMercury\b|Choice[-_\s]*Financial[-_\s]*Group|\$FRC
 Bankless,Bankless
+Biconomy,Biconomy|Omchain
 Binary Options,binary[-_\s]*options
-Binance,binance|biconomy|bnb|bsc|cz|bifinity|binaryx|billance|changpeng|joselito|paysafe|SwipeIO|Swipe\s*Wallet|keyway|\bkey[-_\s]*vision|TrustWallet|BUSD|\boztures|Kaiser[-_\s]*Ng
+Binance,binance|biconomy|bnb|bsc|cz|bifinity|binaryx|billance|changpeng|joselito|paysafe|SwipeIO|Swipe\s*Wallet|keyway|\bkey[-_\s]*vision|TrustWallet|BUSD|\boztures|Kaiser[-_\s]*Ng|InvestByBit
 Bitdeer,Bitdeer
 BitGet,Bitget
 Bitmain,Bitmain
 Bitstamp,Bitstamp
 Bittrex,Bittrex|Ritchie[-_\s]*Lai
 Bitzlato,Bitzlato
-Blockchain8,Blockchain8|tom[-_\s]*emmer|ritchie[-_\s]*torres|repritchie|Warren[-_\s]*Davidson|Byron[-_\s]*Donalds|Ted[-_\s]*Budd|Josh[-_\s]*Gotheimer|Jake[-_\s]*Auchincloss|Darren[-_\s]*Soto|ro[-_\s]*khanna
+Blockchain8,Blockchain8|tom[-_\s]*emmer|ritchie[-_\s]*torres|repritchie|Warren[-_\s]*Davidson|Byron[-_\s]*Donalds|Ted[-_\s]*Budd|Josh[-_\s]*Gotheimer|Jake[-_\s]*Auchincloss|Darren[-_\s]*Soto|ro[-_\s]*khanna|KMSmithDC|Kristin[-_\s]*Smith\b
 Blockchain Capital,Blockchain[-_\s]*Capital|\bbrock\b|brockpierce
 BlockFi,BlockFi
 Bored Ape Yacht Club,BAYC|Bored[-_\s]*Ape|yuga[-_\s]*labs
-Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell
+Bros,cryptomanran|trillionUSD|nic[-_\s]*carter|bitboy|ben[-_\s]*armstrong|basedkarbon|thecryptolark|adam([-_\s]*back|3us)|@DegenSp|APompliano|IIICapital|\bMeltem\b|algodtrading|whatbitcoindid|CryptoKaleo|Mike[-_\s]*Alfred|natbrunell|natalie[-_\s]*brunell|stackersatoshi
+Bybit,\bBybit\b|Ben[-_\s]*Zhou|InvestByBit
 Cardano,Cardano|[$\s]ADA[^\w]|Hoskinson
-Cathie Wood,Cathie\s*Wood|\bARK(K|\s*Innovation|\s*Invest)
+Cathie Wood,Cathie\s*Wood|\bARK(F|G|K|\s*Innovation|\s*Invest)
 Celsius,celsius|mashinsky|levity[-_\s]*and[-_\s]*love|celsian
 Circle,[@#]circle|usdc|circle[-_\s]*internet|disparte|\ballaire|jerallaire
 Coinbase,Coinbase|\$COIN|brian[-_\s]*armstrong|grewal\b
-Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk
+Coinflex,Mark[-_\s]*Lamb|Roger[-_\s]*Ver|coinflex|Doug[-_\s]*Polk|OPNX
 CompoundFi,compoundfi|leshner|\bgonen\b
 Cross River Bank,CRB|Cross[-_\s]*River|Prestige[-_\s]*Capital|bae[-_\s]*communications|Zenfi|PeerIQ|\bupstart\b|\bUPST\b|\bLeumi\b|Hapoalim
 Crypto.com,crypto[._]?com|CDC|[$#]CRO|\sCRO\s
+CUBI,\$CUBI|Customers[-_\s]*Ban(k|corp)
 Custodia,custodia|caitlin[-_\s]*long
 DCG,DCG|digital\s*currency\s*group|sh?ill?bert|Grayscale|GBTC
+DWF,DWF|Andrey[-_\s]*Grachev|\bgrachev\b
 El Salvador,El[-_\s]*Salvador|Bukele
 EOS,[^\w]EOS|\s*Blumer[^\w]
 Euler Finance,\beuler\b
 FalconX,falconx
 Flip Filipkowski,filipkowski
 Finblox,finblox
 Fireblocks,fireblocks
@@ -45,55 +51,59 @@
 Gemini,Gemini|winklev|@cameron
 Genesis,Genesis|Michael\s?Moro
 Goldfinch,goldfinch
 Hex,\bHex\b|[#$]Hex|Pulsechain|Richard\s*Heart|Hexican
 Hoo,Hoo[-_\s]*Exchange|#Hoo\s|Rexy\s*(Hoo|Wang)
 Huobi,huobi
 Jump Trading,Jump[-_\s]*Trading|@jump_
-Justin Sun,justin[-_\s]*sun|pgala|sunswap|sunyuchentron
+Justin Sun,justin[-_\s]*sun|pgala|sunswap|sunyuchentron|poloniex|web3nina
 Kinesis,kinesis|kvt|ABX|KAG
 Kraken,kraken|payward
 KuCoin,kucoin
 LBRY,LBRY
 North Korea,lazarus|North\s*Korea|pyongyang
 Paul LeRoux,leroux
 MakerDAO,makerdao|[$#\s]DAI[^\w]
 Marathon,\$MARA|marathon
 Matthew Roszak,[^\w]roszak
 Mario Nawfal,marionawfal
-Messari,Ryan\s*Selkis|twobitidiot|messari
+Messari,Ryan\s*Selkis|twobitidiot|messari|@robustus|Dan[-_\s]*McArdle
 Memes,\smeme
 Metallicus,FBBT|Nauvoo|Metallicus|Bitcoinwalking|Bruce[-_\s]*Stewart
+Metropolitan Commercial Bank,MCB\b|MCBankNY|Metropolitan[-_\s]*Commercial
 Founders Bank,Michael[-_\s]*Bianchi|Founders[-_\s]*Bank
 Miles Guo,\bguo\b|hcoin|himalaya[-_\s]*exchange|bannon|fjb|miles[-_\s]*kwok|brother[-_\s]*seven|kin[-_\s]*ming[-_\s]*je|william[-_\s]*je\b|\bHaoyun\b
 Miners,bitcoin[-_\s]*min(ing|er)|\$(CORZ|IRIS|ARGO|HUT|HIVE|CAN|BLOK|BTCM)|Core[-_\s]*Scientific|Iris[-_\s]*Energy|Blockstream
 Moonpay,moonpay
 MSTR,Saylor|MSTR
 Near Protocol,NEAR[-_\s]*Protocol|[$#]near\b|\bavichal\b|Rebecca[-_\s]*Rettig
 Nexo,Nexo
 NFTs,crypto[-_\s]*punk|pudgy[-_\s]*penguin
-OKX,oke?[cx]|star xu
+OKX,oke?[cx]|star[-_\s]*xu
 OpenPayd,openpayd|CFD\s?Team
 OpenSea,OpenSea
+Paxful,paxful|Ray[-_\s]*Youssef|Artur[-_\s]*Schaback
 Paxos,paxos|BUSD|USDP|PAXG
 Payrnet,payrnet|railsr|railsbank
 Pi,\$PI[^\w]|Pi[-_\s]*Network
 Prime Trust,Prime[-\s_]?Trust
 PVBC,PVBC|BankProv
 Quadriga,Quadriga|Gerald[-_\s]*Cotten
 Revolut,revolut[^\w]
 Ripple,XRP|garlinghouse|\bripple\b
 RIOT,\$RIOT|Riot[-\s_]*Block
 Safemoon,Safemoon
 Satoshi,Satoshi|Nakamoto
 SEC,\bSEC(\b|Gov)|Gensler|Securities.{0,6}Exchange.{0,6}Commission
 Signature Bank,SBNY|Signature[-_\s]*Bank|Signet
 Silicon Valley Bank,si?vb|Silicon[-_\s]*Valley[-_\s]*Bank
+Silk Road,Silk[-_\s]*Road|\bulbricht|\bDPR\b
 Silvergate,\$SI|Silvergate|Alan\s*Lane|Eisele|[\s#]SEN[^\w]|Rebecca[-_\s]*Rettig
 Solana,Solana|Serum
+Symbolic Capital,Symbolic[-_\s]*Capital|Lev[-_\s]Livnev
 TerraLuna,luna\b|do[-_\s]*kwon|stablekwon|\bterra\b|LFG|Macedo|\bLuna[-_\s]*Foundation\b
 Tether,tether|usdt|paolo|friedberg|hoegner|Noble\s?Bank|Deltec[^\']|bitfinex[^e]|\bbrock\b|brockpierce|Capital[-_\s]*Union|Noblex|SJMBT
 Tornado Cash,tornado\s*cash
 Transactive Systems UAB,Transactive
 Tron,\btron\b|tron(block|\s*)?chain|trondao|TRX\b
 TrueUSD,TUSD|TrueUSD|TrueFi|TrustExplorer|Techteryx
 Vauld,Vauld
@@ -106,10 +116,10 @@
 Wallet Addresses Dash,X[1–9A-HJ-NP-Za-km-z]{33}
 Wallet Addresses Doge,\sD[a-zA-Z0–9_.-]{33}
 Wallet Addresses Ethereum,0x[a-fA-F0–9]{40}
 Wallet Addresses Monero,[48][0–9AB][1–9A-HJ-NP-Za-km-z]{93}
 Wallet Addresses Polkadot,1[0–9a-zA-Z]{47}
 Wallet Addresses Ripple,r[0–9a-zA-Z]{33}
 Wallet Addresses Stellar,G[0–9A-Z]{40,60}\b
-Wintermute,wintermute
-Wirecard,wirecard
+Wintermute,wintermute|\bbebop\b
+Wirecard,wirecard|\bmarsalek\b
 Wyre,wyre
```

### Comparing `clown_sort-1.3.0/clown_sort/util/argument_parser.py` & `clown_sort-1.3.1/clown_sort/util/argument_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,28 +39,27 @@
 
 parser.add_argument('-d', '--destination-dir',
                     metavar='DESTINATION_DIR',
                     help='destination folder to place the Sorted/ and Processed/ dirs (default: SCREENSHOTS_DIR)',
                     default=str(DEFAULT_DESTINATION_DIR).replace(str(Path.home()), '~'))
 
 parser.add_argument('-m', '--manual-sort', action='store_true',
-                    help='causes a popup to be presented for each file where it can be manually named and a sorting destination selected')
+                    help='causes a popup to be presented for each file where it can be manually named and a sorting destination selected (experimental)')
 
 parser.add_argument('-r', '--rules-csv',
                     action='append',
                     metavar='RULES_FILE.CSV',
                     help=f"sorting rules can be supplied more than once (use string '{CRYPTO}' to use the defaults)")
 
 parser.add_argument('-f', '--filename-regex',
                     help='filename regular expression',
                     default=DEFAULT_FILENAME_REGEX.pattern)
 
 parser.add_argument('-y', '--yes-overwrite', action='store_true',
-                    help='skip confirmation prompt and always overwrite if a file with the same name already exists',
-                    default=DEFAULT_FILENAME_REGEX.pattern)
+                    help='skip confirmation prompt and always overwrite if a file with the same name already exists')
 
 parser.add_argument('--rescan-sorted', action='store_true',
                     help="rescan already sorted files (useful if you updated your sorting rules)")
 
 parser.add_argument('--delete-originals', action='store_true',
                     help="don't preserve the original screenshots in the Processed/ folder")
```

### Comparing `clown_sort-1.3.0/clown_sort/util/constants.py` & `clown_sort-1.3.1/clown_sort/util/constants.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.0/clown_sort/util/filesystem_helper.py` & `clown_sort-1.3.1/clown_sort/util/filesystem_helper.py`

 * *Files identical despite different names*

### Comparing `clown_sort-1.3.0/clown_sort/util/rich_helper.py` & `clown_sort-1.3.1/clown_sort/util/rich_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pathlib import Path
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from rich.console import Console
 from rich.panel import Panel
 from rich.text import Text
 from rich.theme import Theme
 
 from clown_sort.config import Config
@@ -33,14 +33,15 @@
     'grey.darker_italic': 'color(8) dim italic',
     'grey.darkest': 'color(235) dim',
     'grey.light': 'color(248)',
     'off_white': 'color(245)',
     'social_media': 'color(82)',
     'author': 'color(178)',
     'sort_destination': 'magenta',
+    'sort_folder': 'color(62)'
 }
 
 COLOR_THEME = Theme(COLOR_THEME_DICT)
 INDENT_SPACES = 4
 
 # Main rich text output object.
 console = Console(theme=COLOR_THEME, color_system='256')
@@ -83,14 +84,18 @@
     return _file_operation_log_message(basename, new_file, 'Copying')
 
 
 def moving_file_log_message(basename: str, new_file: Path) -> Text:
     return _file_operation_log_message(basename, new_file, 'Moving processed file')
 
 
+def comma_join(strs: List[str], style: str) -> Text:
+    return Text(", ").join([Text(s, style) for s in strs])
+
+
 def _file_operation_log_message(basename: str, new_file: Path, log_msg: str) -> Text:
     log_msg += ' '
     log_msg = Text(log_msg)
 
     if Config.dry_run:
         log_msg = NOT + log_msg
```

### Comparing `clown_sort-1.3.0/pyproject.toml` & `clown_sort-1.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "clown_sort"
-version = "1.3.0"
+version = "1.3.1"
 description = "Sort screenshots based on rules or through individual review."
 authors = ["Michel de Cryptadamus <michel@cryptadamus.com>"]
 readme = "README.md"
 packages = [{include = "clown_sort"}]
 homepage = "https://github.com/michelcrypt4d4mus/clown_sort"
 
 include = [
@@ -39,16 +39,19 @@
 piexif = "^1.1.3"
 pillow = "^9.4.0"
 filedate = "^2.0"
 python-dotenv = "^0.21.1"
 rich-argparse-plus = "^0.3.1.4"
 pyexiftool = "^0.5.5"
 pypdf = "^3.4.1"
+pycryptodome = {version = "^3.17", optional = true}
 
-
+[tool.poetry.extras]
+pdf = ['pycryptodome']
+gui = ['PySimpleGUI']
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 bpython = "^0.24"
 
 [tool.pytest.ini_options]
 addopts = [
```

### Comparing `clown_sort-1.3.0/setup.py` & `clown_sort-1.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,31 +15,35 @@
  'pyexiftool>=0.5.5,<0.6.0',
  'pypdf>=3.4.1,<4.0.0',
  'pytesseract>=0.3.10,<0.4.0',
  'python-dotenv>=0.21.1,<0.22.0',
  'rich-argparse-plus>=0.3.1.4,<0.4.0.0',
  'rich>=13.0.1,<14.0.0']
 
+extras_require = \
+{'gui': ['PySimpleGUI>=4.60.4,<5.0.0'], 'pdf': ['pycryptodome>=3.17,<4.0']}
+
 entry_points = \
 {'console_scripts': ['set_screenshot_timestamps = '
                      'clown_sort:set_screenshot_timestamps',
                      'sort_screenshots = clown_sort:sort_screenshots']}
 
 setup_kwargs = {
     'name': 'clown-sort',
-    'version': '1.3.0',
+    'version': '1.3.1',
     'description': 'Sort screenshots based on rules or through individual review.',
-    'long_description': '# CLOWN SORT\nSometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can\'t find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.\n\nClown Sort[^1] solves this.\n\n\n## What It Do\nIt sorts screenshots, PDFs, etc. based on their name and/or their textual contents into folders based on a list of rules. The contents of the tweet/reddit post/whatever are prepended to the filename and the `ImageDescription` EXIF tag is set to the OCR text. As you can configure your own arbitrary rules and run it against any set of images it works on many things other than screenshots of social media clowns, though the default configuration is for cryptocurrency clowns.\n\nFor example this screenshot of a tweet by a noteworthy cryptocurrency "reporter"[^2] on the eve of FTX\'s implosion:\n\n![](doc/larry_cermak_on_alameda_and_ftx.png)\n\nWould be renamed from `Screen Shot 2023-02-17 at 7.11.37 PM.png` to\n\n```\nTweet by @lawmaster: "I will say though before this thread gets taken over: 1. I do believe Alameda has the size to easily buy Binance\\\'s FIT OTC 2. I think the chance of FTX insolvency is near" Screen Shot 2023-02-17 at 7.11.37 PM.png\n```\n\nOther stuff that happens:\n* The `ImageDescription` EXIF tag will be written (for images).\n* All timestamps will be preserved.\n* Files that match multiple patterns will be copied to multiple destination folders.\n* The original file will be moved into a `Processed/` directory after it has been handled.\n\nNote also that:\n* This works on images that are more substantive than just self-clowning screenshots.\n* So far only Tweets and Reddit screenshots have special handling beyond OCR text extraction.\n* PDFs can be sorted by contents or filename, e.g. a PDF named `Norton Anthology of Crypto Bro Poetry.pdf` containing iambic verse like _["Fuck u justin sun  and fuck ur dick face... u all play with investing and money of the people !!!!"](https://universeodon.com/@cryptadamist/109642431382653023)_ by the noted bard JOKER_OF_CRYPTO will be copied to the `Justin Sun/` folder but not renamed.\n* Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.\n\n## Quick Start\n```sh\n# Installation with pipx is preferred if you have it but you can also use pip which comes standard\n# on almost all systems. pipx is only a noticeably better answer if you\'re a python programmer who\n# is concerned about side effects of pip upgrading system python packages.\npip install clown_sort\n\n# Get help\nsort_screenshots -h\n\n# Dry run with default cryptocurrency sort rules (dry runs don\'t actually move anything,\n# they just show you what will happen if you run again with the --execute flag)\nsort_screenshots\n\n# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots\nsort_screenshots --execute\n\n# Sort a different directory of screenshots\nsort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute\n\n# Sort with custom rules\nsort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute\n\n# Sort pdfs\nsort_screenshots -f \'.*pdf$\' -e\n```\n\n# Setup\n[pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.\n```\npipx install clown_sort\n```\n\n### Configuring With `.clown_sort` File\nIf there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:\n\n1. The current directory\n2. Your home directory\n\nSee [the example](.clown_sort.example) for more information on what can be configured this way.\n\n### Optional Components\nIf you want to use the popup window to manually tag you _may_ need to install:\n* Python TK: `brew install python-tk@3.10` (if you don\'t have [homebrew](https://brew.sh/) you need to install it to run `brew install`)\n\nNot required for standard PNG, JPG, etc. images but you may optionally install `exiftool` for other file types if you want excessive debugging.\n* ExifTool: `brew install exiftool` or download from https://exiftool.org\n\n\n# Usage\nThe default is for the tool to run in "dry run" mode, meaning it doesn\'t actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**\n\nWhile every effort has been made to use Python\'s cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.\n\n### Help Screen\n![](doc/sort_screenshots_help.png)\n\n(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)\n\n### Custom Sorting Rules\nThe default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you\'re not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.\n\n### Example Output (Automated Sorting)\n![](doc/output_example.png)\n\n\n## Manually Sorting (Experimental)\n**This is an experimental feature.** It\'s only been tested on macOS.\n\nIf you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.\n\n![](doc/manual_select_box.png)\n\n\n# Contributing\nFeel free to file issues or open pull requests. Only requirement is that tests should pass before you open it, which you can check with\n\n```\npytest\n```\n\n[^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.\n\n[^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried\'s various scams as part of his commitment to "unrivaled transparency".\n',
+    'long_description': '# CLOWN SORT\nSometimes someone is being a clown on the internet. Somewhere on your hard drive is the perfect screenshot to prove to the world that the clown in question is a fool, a hypocrite, a criminal, or worse. But then - horrors - you can\'t find the screenshot! It has been lost in your vast archive of screenshots of clowns clowning themselves on the internet.\n\nClown Sort[^1] solves this.\n\n\n## What It Do\nIt sorts screenshots, PDFs, etc. based on their name and/or their textual contents into folders based on a list of rules. The contents of the tweet/reddit post/whatever are prepended to the filename and the `ImageDescription` EXIF tag is set to the OCR text. As you can configure your own arbitrary rules and run it against any set of images it works on many things other than screenshots of social media clowns, though the default configuration is for cryptocurrency clowns.\n\nFor example this screenshot of a tweet by a noteworthy cryptocurrency "reporter"[^2] on the eve of FTX\'s implosion:\n\n![](doc/larry_cermak_on_alameda_and_ftx.png)\n\nWould be renamed from `Screen Shot 2023-02-17 at 7.11.37 PM.png` to\n\n```\nTweet by @lawmaster: "I will say though before this thread gets taken over: 1. I do believe Alameda has the size to easily buy Binance\\\'s FIT OTC 2. I think the chance of FTX insolvency is near" Screen Shot 2023-02-17 at 7.11.37 PM.png\n```\n\nOther stuff that happens:\n* The `ImageDescription` EXIF tag will be written (for images).\n* All timestamps will be preserved.\n* Files that match multiple patterns will be copied to multiple destination folders.\n* The original file will be moved into a `Processed/` directory after it has been handled.\n\nNote also that:\n* This works on images that are more substantive than just self-clowning screenshots.\n* So far only Tweets and Reddit screenshots have special handling beyond OCR text extraction.\n* PDFs can be sorted by contents or filename, e.g. a PDF named `Norton Anthology of Crypto Bro Poetry.pdf` containing iambic verse like _["Fuck u justin sun  and fuck ur dick face... u all play with investing and money of the people !!!!"](https://universeodon.com/@cryptadamist/109642431382653023)_ by the noted bard JOKER_OF_CRYPTO will be copied to the `Justin Sun/` folder but not renamed.\n* Videos are not OCRed and can only be moved based on filename matches, e.g. a file called `SBF is a big fat liar.mov` will be moved to the `FTX/` folder but otherwise left alone.\n\n## Quick Start\n```sh\n# Installation with pipx is preferred if you have it but you can also use pip which comes standard\n# on almost all systems. pipx is only a noticeably better answer if you\'re a python programmer who\n# is concerned about side effects of pip upgrading system python packages.\npip install clown_sort\n\n# Get help\nsort_screenshots -h\n\n# Dry run with default cryptocurrency sort rules (dry runs don\'t actually move anything,\n# they just show you what will happen if you run again with the --execute flag)\nsort_screenshots\n\n# Execute default cryptocurrency sort rules against ~/Pictures/Screenshots\nsort_screenshots --execute\n\n# Sort a different directory of screenshots\nsort_screenshots --screenshots-dir /Users/hrollins/Pictures/get_in_the_van/tourphotos --execute\n\n# Sort with custom rules\nsort_screenshots --rules-csv /Users/hrollins/my_war.csv --execute\n\n# Sort pdfs\nsort_screenshots -f \'.*pdf$\' -e\n```\n\n# Setup\n[pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.\n```\npipx install clown_sort\n```\n\nSome (not many) PDFs require the `pycryptodome` package. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with:\n\n```sh\npipx install clown_sort[pycryptodome]\n```\n\n\n### Configuring With `.clown_sort` File\nIf there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:\n\n1. The current directory\n2. Your home directory\n\nSee [the example](.clown_sort.example) for more information on what can be configured this way.\n\n### Optional Components\nIf you want to use the popup window to manually tag you _may_ need to install:\n* Python TK: `brew install python-tk@3.10` (if you don\'t have [homebrew](https://brew.sh/) you need to install it to run `brew install`)\n\nNot required for standard PNG, JPG, etc. images but you may optionally install `exiftool` for other file types if you want excessive debugging.\n* ExifTool: `brew install exiftool` or download from https://exiftool.org\n\n\n# Usage\nThe default is for the tool to run in "dry run" mode, meaning it doesn\'t actually do anything - it just shows you what it _would_ do if you added the `--execute` flag. **YOU ARE ADVISED TO MAKE A BACKUP OF YOUR SCREENSHOTS FOLDER BEFORE HITTING THE `--execute` FLAG.**\n\nWhile every effort has been made to use Python\'s cross platform `Pathlib` module as much as possible sometimes shit gets wonky on other platforms. This is 100x as true on Windows - Clown Sort has never been tested on a Windows platform.\n\n### Help Screen\n![](doc/sort_screenshots_help.png)\n\n(In my personal usuage I tend to run the tool with the `--all` and `--only-if-match` options.)\n\n### Custom Sorting Rules\nThe default is to sort cryptocurrency related content but you can define your own CSV of rules with two columns `folder` and `regex`. The value in `folder` specifies the subdirectory to sort into and `regex` is the pattern to match against. See [the default crypto related configuration](clown_sort/sorting_rules/crypto.csv) for an example. An explanation of regular expressions is beyond the scope of this README but many resources are available to help. If you\'re not good at regexes just remember that any alphanumeric string is a regex that will match that string. [pythex](http://pythex.org/) is a great website for testing your regexes.\n\n### Example Output (Automated Sorting)\n![](doc/output_example.png)\n\n\n## Manually Sorting (Experimental)\n**This is an experimental feature.** It\'s only been tested on macOS.\n\nIf you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.\n\nTo use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:\n```sh\npipx install clown_sort[PySimpleGUI]\n```\n\n![](doc/manual_select_box.png)\n\n\n# Contributing\nFeel free to file issues or open pull requests.\n\nThis package is managed with [Python Poetry](http://python-poetry.org/). To get going:\n1. Install Poetry.\n1. `git clone` this repo.\n1. `cd clown_sort`\n1. `poetry install`\n1. Optional components can be install with `poetry install -E pdf -E gui`\n\nOnly requirement is that tests should pass before you open it, which you can check with\n\n```\npytest\n```\n\n[^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.\n\n[^2]: Perhaps notable that the "reporter" in question for years maintained a private list of the blockchain addresses of Sam Bankman-Fried\'s various scams as part of his commitment to "unrivaled transparency".\n',
     'author': 'Michel de Cryptadamus',
     'author_email': 'michel@cryptadamus.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/michelcrypt4d4mus/clown_sort',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.10,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `clown_sort-1.3.0/PKG-INFO` & `clown_sort-1.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 Metadata-Version: 2.1
 Name: clown-sort
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sort screenshots based on rules or through individual review.
 Home-page: https://github.com/michelcrypt4d4mus/clown_sort
 Keywords: ocr,organization,organizer,screenshot,rename,sort
 Author: Michel de Cryptadamus
 Author-email: michel@cryptadamus.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Desktop Environment :: File Managers
 Classifier: Topic :: Multimedia :: Graphics :: Capture
 Classifier: Topic :: Multimedia :: Graphics :: Capture :: Screen Capture
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0)
+Provides-Extra: gui
+Provides-Extra: pdf
+Requires-Dist: PySimpleGUI (>=4.60.4,<5.0.0) ; extra == "gui"
 Requires-Dist: exif (>=1.5.0,<2.0.0)
 Requires-Dist: filedate (>=2.0,<3.0)
 Requires-Dist: piexif (>=1.1.3,<2.0.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: pycryptodome (>=3.17,<4.0) ; extra == "pdf"
 Requires-Dist: pyexiftool (>=0.5.5,<0.6.0)
 Requires-Dist: pypdf (>=3.4.1,<4.0.0)
 Requires-Dist: pytesseract (>=0.3.10,<0.4.0)
 Requires-Dist: python-dotenv (>=0.21.1,<0.22.0)
 Requires-Dist: rich (>=13.0.1,<14.0.0)
 Requires-Dist: rich-argparse-plus (>=0.3.1.4,<0.4.0.0)
 Description-Content-Type: text/markdown
@@ -87,14 +90,21 @@
 
 # Setup
 [pipx](https://pypa.github.io/pipx/) is recommended because it keeps your system python environment safe but you can also just use `pip`.
 ```
 pipx install clown_sort
 ```
 
+Some (not many) PDFs require the `pycryptodome` package. To avoid complicating the dependency situation this is offered as an optional installation which can be accomplished with:
+
+```sh
+pipx install clown_sort[pycryptodome]
+```
+
+
 ### Configuring With `.clown_sort` File
 If there are command line options you find yourself specifying repeatedly you can place them in a `.clown_sort` file. When you invoke `sort_screenshots` the following locations will be checked for `.clown_sort`:
 
 1. The current directory
 2. Your home directory
 
 See [the example](.clown_sort.example) for more information on what can be configured this way.
@@ -125,19 +135,33 @@
 
 
 ## Manually Sorting (Experimental)
 **This is an experimental feature.** It's only been tested on macOS.
 
 If you run with the `--manual-sort` command line the behavior is quite different. Rather than automatically sort files for you, instead for every file you will be greeted with a popup asking you for a desired filename and a radio button select of possible subdirectories off your `Sorted/` directory.
 
+To use this feature you must install the optional `PySimpleGUI` package which can be accomplished like this:
+```sh
+pipx install clown_sort[PySimpleGUI]
+```
+
 ![](doc/manual_select_box.png)
 
 
 # Contributing
-Feel free to file issues or open pull requests. Only requirement is that tests should pass before you open it, which you can check with
+Feel free to file issues or open pull requests.
+
+This package is managed with [Python Poetry](http://python-poetry.org/). To get going:
+1. Install Poetry.
+1. `git clone` this repo.
+1. `cd clown_sort`
+1. `poetry install`
+1. Optional components can be install with `poetry install -E pdf -E gui`
+
+Only requirement is that tests should pass before you open it, which you can check with
 
 ```
 pytest
 ```
 
 [^1]: The name `clown_sort` was suggested by [ParrotCapital](http://twitter.com/ParrotCapital) and while the tool can work on any kind of screenshot it was too good not to use.
```

