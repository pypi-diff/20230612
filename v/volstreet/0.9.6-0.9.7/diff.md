# Comparing `tmp/volstreet-0.9.6.tar.gz` & `tmp/volstreet-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volstreet-0.9.6.tar", last modified: Fri Jun  9 10:18:52 2023, max compression
+gzip compressed data, was "volstreet-0.9.7.tar", last modified: Mon Jun 12 13:05:09 2023, max compression
```

## Comparing `volstreet-0.9.6.tar` & `volstreet-0.9.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 10:18:52.505343 volstreet-0.9.6/
--rw-rw-rw-   0        0        0      497 2023-06-09 10:18:52.505343 volstreet-0.9.6/PKG-INFO
--rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.6/README.md
--rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.6/pyproject.toml
--rw-rw-rw-   0        0        0     1375 2023-06-09 10:18:52.506838 volstreet-0.9.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 10:18:52.496495 volstreet-0.9.6/volstreet/
--rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.6/volstreet/SmartWebSocketV2.py
--rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.6/volstreet/__init__.py
--rw-rw-rw-   0        0        0     8133 2023-06-07 07:39:33.000000 volstreet-0.9.6/volstreet/blackscholes.py
--rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.6/volstreet/constants.py
--rw-rw-rw-   0        0        0    24214 2023-06-07 14:47:58.000000 volstreet-0.9.6/volstreet/datamodule.py
--rw-rw-rw-   0        0        0   161941 2023-06-09 10:14:18.000000 volstreet-0.9.6/volstreet/dealingroom.py
--rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.6/volstreet/discord_bot.py
--rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.6/volstreet/exceptions.py
--rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.6/volstreet/nsefunctions.py
--rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.6/volstreet/strategies.py
-drwxrwxrwx   0        0        0        0 2023-06-09 10:18:52.504342 volstreet-0.9.6/volstreet.egg-info/
--rw-rw-rw-   0        0        0      497 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      447 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      787 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-09 10:18:52.000000 volstreet-0.9.6/volstreet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 13:05:09.174687 volstreet-0.9.7/
+-rw-rw-rw-   0        0        0      497 2023-06-12 13:05:09.174687 volstreet-0.9.7/PKG-INFO
+-rw-rw-rw-   0        0        0      124 2023-06-07 14:47:58.000000 volstreet-0.9.7/README.md
+-rw-rw-rw-   0        0        0       91 2023-05-24 02:09:11.000000 volstreet-0.9.7/pyproject.toml
+-rw-rw-rw-   0        0        0     1375 2023-06-12 13:05:09.176046 volstreet-0.9.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-12 13:05:09.166493 volstreet-0.9.7/volstreet/
+-rw-rw-rw-   0        0        0    16121 2023-05-24 02:09:11.000000 volstreet-0.9.7/volstreet/SmartWebSocketV2.py
+-rw-rw-rw-   0        0        0       37 2023-06-07 15:08:38.000000 volstreet-0.9.7/volstreet/__init__.py
+-rw-rw-rw-   0        0        0     8133 2023-06-07 07:39:33.000000 volstreet-0.9.7/volstreet/blackscholes.py
+-rw-rw-rw-   0        0        0     2694 2023-06-07 14:47:58.000000 volstreet-0.9.7/volstreet/constants.py
+-rw-rw-rw-   0        0        0    25475 2023-06-12 13:04:14.000000 volstreet-0.9.7/volstreet/datamodule.py
+-rw-rw-rw-   0        0        0   167244 2023-06-12 13:04:14.000000 volstreet-0.9.7/volstreet/dealingroom.py
+-rw-rw-rw-   0        0        0     1683 2023-05-24 02:09:11.000000 volstreet-0.9.7/volstreet/discord_bot.py
+-rw-rw-rw-   0        0        0      209 2023-06-06 15:42:44.000000 volstreet-0.9.7/volstreet/exceptions.py
+-rw-rw-rw-   0        0        0    39664 2023-05-24 02:09:11.000000 volstreet-0.9.7/volstreet/nsefunctions.py
+-rw-rw-rw-   0        0        0    14536 2023-06-07 14:47:58.000000 volstreet-0.9.7/volstreet/strategies.py
+drwxrwxrwx   0        0        0        0 2023-06-12 13:05:09.173654 volstreet-0.9.7/volstreet.egg-info/
+-rw-rw-rw-   0        0        0      497 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      447 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      787 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-12 13:05:09.000000 volstreet-0.9.7/volstreet.egg-info/top_level.txt
```

### Comparing `volstreet-0.9.6/setup.cfg` & `volstreet-0.9.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6f6c 7374 7265 6574 0d0a 7665   = volstreet..ve
-00000020: 7273 696f 6e20 3d20 302e 392e 360d 0a61  rsion = 0.9.6..a
+00000020: 7273 696f 6e20 3d20 302e 392e 370d 0a61  rsion = 0.9.7..a
 00000030: 7574 686f 7220 3d20 5261 6875 6c20 5468  uthor = Rahul Th
 00000040: 616b 6b61 720d 0a61 7574 686f 725f 656d  akkar..author_em
 00000050: 6169 6c20 3d20 722e 7468 616b 6b61 7231  ail = r.thakkar1
 00000060: 3540 676d 6169 6c2e 636f 6d0d 0a64 6573  5@gmail.com..des
 00000070: 6372 6970 7469 6f6e 203d 2056 6f6c 5374  cription = VolSt
 00000080: 7265 6574 2069 7320 6120 5079 7468 6f6e  reet is a Python
 00000090: 206c 6962 7261 7279 2066 6f72 2061 7574   library for aut
```

### Comparing `volstreet-0.9.6/volstreet/SmartWebSocketV2.py` & `volstreet-0.9.7/volstreet/SmartWebSocketV2.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.6/volstreet/blackscholes.py` & `volstreet-0.9.7/volstreet/blackscholes.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.6/volstreet/constants.py` & `volstreet-0.9.7/volstreet/constants.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.6/volstreet/datamodule.py` & `volstreet-0.9.7/volstreet/datamodule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 import volstreet as vs
 from volstreet.exceptions import ApiKeyNotFound
 from eod import EodHistoricalData
 import pandas as pd
 from dateutil.relativedelta import relativedelta, MO, TU, WE, TH, FR
 import numpy as np
+from datetime import datetime, timedelta
 
 
 class DataClient:
     def __init__(self, api_key):
         if api_key is None:
             raise ApiKeyNotFound("EOD API Key not found")
         self.api_key = api_key
         self.client = EodHistoricalData(api_key=api_key)
 
-    def get_data(self, symbol, from_date="2011-01-01", return_columns=None):
+    @staticmethod
+    def parse_symbol(symbol):
+
         symbol_dict = {
             "NIFTY": "NSEI.INDX",
             "BANKNIFTY": "NSEBANK.INDX",
             "FINNIFTY": "CNXFIN.INDX",
         }
         symbol = symbol.upper()
-        name = symbol.split(".")[0]
         if "." not in symbol:
             if symbol in symbol_dict:
                 symbol = symbol_dict[symbol]
             else:
                 symbol = symbol + ".NSE"
+        return symbol
+
+    def get_data(self, symbol, from_date="2011-01-01", return_columns=None):
+
+        name = symbol.split(".")[0] if "." in symbol else symbol
+
+        symbol = self.parse_symbol(symbol)
 
         if return_columns is None:
             return_columns = ["open", "close", "gap", "intra", "abs_gap", "abs_intra"]
 
         resp = self.client.get_prices_eod(
             symbol, period="d", order="a", from_=from_date
         )
@@ -41,14 +50,44 @@
         df["intra"] = (df.close / df.open - 1) * 100
         df["abs_gap"] = abs(df.gap)
         df["abs_intra"] = abs(df.intra)
         df = df.loc[:, return_columns]
         df.name = name
         return df
 
+    def get_intraday_data(self, symbol, interval, from_date="2011-01-01", return_columns=None):
+
+        name = symbol.split(".")[0] if "." in symbol else symbol
+
+        symbol = self.parse_symbol(symbol)
+
+        if return_columns is None:
+            return_columns = ['open', 'high', 'low', 'close']
+
+        resp_list = []
+        from_date = pd.to_datetime(from_date)
+        while datetime.now().date() > from_date.date():
+            to_date = from_date + timedelta(days=120)
+            resp = self.client.get_prices_intraday(
+                symbol, interval=interval,
+                from_=str(int(from_date.timestamp())),
+                to=str(int(to_date.timestamp()))
+            )
+
+            resp_list.extend(resp)
+            from_date += timedelta(days=120)
+
+        df = pd.DataFrame(resp_list)
+        df.index = pd.to_datetime(df['datetime'])
+        df = df.drop_duplicates()
+        df.index = df.index + timedelta(hours=5, minutes=30)
+        df = df[return_columns]
+        df.name = name
+        return df
+
 
 def retain_name(func):
     def wrapper(df, *args, **kwargs):
         try:
             name = df.name
         except AttributeError:
             name = None
```

### Comparing `volstreet-0.9.6/volstreet/dealingroom.py` & `volstreet-0.9.7/volstreet/dealingroom.py`

 * *Files 1% similar despite different names*

```diff
@@ -2585,14 +2585,16 @@
     @log_errors
     def intraday_strangle(
         self,
         quantity_in_lots,
         call_strike_offset=0,
         put_strike_offset=0,
         stop_loss=1.6,
+        call_stop_loss=None,
+        put_stop_loss=None,
         exit_time=(15, 29),
         sleep_time=5,
         catch_trend=False,
         trend_qty_ratio=1,
         trend_strike_offset=0,
         trend_sl=0.003,
         place_sl_orders=False
@@ -2605,14 +2607,18 @@
             Quantity in lots
         call_strike_offset : float, optional
             Call strike offset in percentage terms, by default 0
         put_strike_offset : float, optional
             Put strike offset in percentage terms, by default 0
         stop_loss : float, optional
             Stop loss percentage, by default 1.6
+        call_stop_loss : float, optional
+            Call stop loss percentage, by default None. If None then stop loss is same as stop_loss.
+        put_stop_loss : float, optional
+            Put stop loss percentage, by default None. If None then stop loss is same as stop_loss.
         exit_time : tuple, optional
             Exit time, by default (15, 29)
         sleep_time : int, optional
             Sleep time in seconds for updating prices, by default 60
         catch_trend : bool, optional
             Catch trend or not, by default False
         trend_qty_ratio : int, optional
@@ -2713,28 +2719,35 @@
             )
 
             # Setting up the stop loss
             sl_multiplier = 1 - sl if sl_type == "call" else 1 + sl
             sl_price = spot_price * sl_multiplier
             trend_sl_hit = False
 
+            notifier(
+                f"{self.name} strangle {sl_type} trend catcher starting. "
+                + f"Placed {qty_in_lots} lots of {strike} {opt_type} at {trend_option.fetch_ltp()}. "
+                + f"Stoploss price: {sl_price}, Underlying Price: {spot_price}",
+                self.webhook_url,
+            )
+
             last_print_time = currenttime()
             print_interval = timedelta(seconds=10)
             while all([currenttime().time() < time(*exit_time), not info_dict["exit_triggers"]["trade_complete"]]):
                 spot_price = info_dict["underlying_ltp"]
                 trend_sl_hit = spot_price < sl_price if sl_type == "call" else spot_price > sl_price
                 if trend_sl_hit:
                     break
                 sleep(1)
                 if currenttime() - last_print_time > print_interval:
                     last_print_time = currenttime()
                     print(
-                        f"{self.name} {sl_type} trend catcher running.\n"
+                        f"{self.name} {sl_type} trend catcher running\n"
                         + f"Stoploss price: {sl_price}, Underlying Price: {spot_price}\n"
-                        + f"Stoploss hit: {trend_sl_hit}.\n"
+                        + f"Stoploss hit: {trend_sl_hit}\n"
                     )
 
             if trend_sl_hit:
                 notifier(
                     f"{self.name} strangle {sl_type} trend catcher stoploss hit.", self.webhook_url
                 )
             else:
@@ -2823,16 +2836,16 @@
         )
 
         # Calculating average prices
         call_avg_price = lookup_and_return(orderbook, 'orderid', call_order_ids, 'averageprice').astype(float).mean()
         put_avg_price = lookup_and_return(orderbook, 'orderid', put_order_ids, 'averageprice').astype(float).mean()
         total_avg_price = call_avg_price + put_avg_price
 
-        call_stop_loss_price = call_avg_price * stop_loss
-        put_stop_loss_price = put_avg_price * stop_loss
+        call_stop_loss_price = call_avg_price * call_stop_loss if call_stop_loss else call_avg_price * stop_loss
+        put_stop_loss_price = put_avg_price * put_stop_loss if put_stop_loss else put_avg_price * stop_loss
 
         # Logging information and sending notification
         self.log_combined_order(
             call_strike=call_strike,
             put_strike=put_strike,
             expiry=expiry,
             buy_or_sell="SELL",
@@ -2958,32 +2971,32 @@
             pass
 
         # Calculate profit
         total_exit_price = shared_info_dict["call_exit_price"] + shared_info_dict["put_exit_price"]
         exit_message = (
             f"{self.name} strangle exited.\n"
             f"Time: {currenttime():%d-%m-%Y %H:%M:%S}\n"
-            f"Underlying LTP: {underlying_ltp}\n"
-            f"Call Price: {call_ltp}\n"
-            f"Put Price: {put_ltp}\n"
-            f"Call SL: {call_sl}\n"
-            f"Put SL: {put_sl}\n"
+            f"Underlying LTP: {shared_info_dict['underlying_ltp']}\n"
+            f"Call Price: {shared_info_dict['call_ltp']}\n"
+            f"Put Price: {shared_info_dict['put_ltp']}\n"
+            f"Call SL: {shared_info_dict['call_sl']}\n"
+            f"Put SL: {shared_info_dict['put_sl']}\n"
             f"Call Exit Price: {shared_info_dict['call_exit_price']}\n"
             f"Put Exit Price: {shared_info_dict['put_exit_price']}\n"
             f"Total Exit Price: {total_exit_price}\n"
             f"Total Entry Price: {total_avg_price}\n"
             f"Profit Pts: {total_avg_price - total_exit_price}\n"
         )
         exit_dict = {
             "Call exit price": shared_info_dict["call_exit_price"],
             "Put exit price": shared_info_dict["put_exit_price"],
             "Total exit price": total_exit_price,
             "Points captured": total_avg_price - total_exit_price,
-            "Call SL": call_sl,
-            "Put SL": put_sl,
+            "Call SL": shared_info_dict["call_sl"],
+            "Put SL": shared_info_dict["put_sl"],
         }
         try:
             self.order_log[order_tag][0].update(exit_dict)
         except Exception as e:
             notifier(
                 f"{self.name}: Error updating order list with exit details. {e}",
                 self.webhook_url,
@@ -3199,14 +3212,44 @@
     data.append(serializable_data)
 
     # Write the updated data back to the JSON file with indentation
     with open(file_name, "w") as file:
         json.dump(data, file, indent=4, default=str)
 
 
+def word_to_num(s):
+    word = {
+        'one': 1, 'two': 2, 'three': 3, 'four': 4, 'five': 5,
+        'six': 6, 'seven': 7, 'eight': 8, 'nine': 9, 'ten': 10,
+        'eleven': 11, 'twelve': 12, 'thirteen': 13, 'fourteen': 14,
+        'fifteen': 15, 'sixteen': 16, 'seventeen': 17, 'eighteen': 18, 'nineteen': 19,
+        'twenty': 20, 'thirty': 30, 'forty': 40, 'fifty': 50,
+        'sixty': 60, 'seventy': 70, 'eighty': 80, 'ninety': 90
+    }
+    multiplier = {'thousand': 1000, 'hundred': 100, 'million': 1000000, 'billion': 1000000000}
+
+    words = s.lower().split()
+    if words[0] == 'a':
+        words[0] = 'one'
+    total = 0
+    current = 0
+    for w in words:
+        if w in word:
+            current += word[w]
+        if w in multiplier:
+            current *= multiplier[w]
+        if w == 'and':
+            continue
+        if w == 'thousand' or w == 'million' or w == 'billion':
+            total += current
+            current = 0
+    total += current
+    return total
+
+
 def login(user, pin, apikey, authkey, webhook_url=None):
     global obj, login_data
     authkey = pyotp.TOTP(authkey)
     obj = SmartConnect(api_key=apikey)
     login_data = obj.generateSession(user, pin, authkey.now())
     if login_data["message"] != "SUCCESS":
         for attempt in range(2, 7):
@@ -3425,20 +3468,41 @@
         return avg_price
 
     return order_ids
 
 
 # Market Hours
 def markethours():
-    if time(9, 10) < currenttime().time() < time(15, 30):
+    if time(9, 15) <= currenttime().time() <= time(15, 30):
         return True
     else:
         return False
 
 
+def last_market_close_time():
+
+    if currenttime().time() < time(9, 15):
+        wip_time = currenttime() - timedelta(days=1)
+        wip_time = wip_time.replace(hour=15, minute=30, second=0, microsecond=0)
+    elif currenttime().time() > time(15, 30):
+        wip_time = currenttime().replace(hour=15, minute=30, second=0, microsecond=0)
+    else:
+        wip_time = currenttime()
+
+    if wip_time.weekday() not in [5, 6] and wip_time.date() not in holidays:
+        return wip_time
+    else:
+        # Handling weekends and holidays
+        while wip_time.weekday() in [5, 6] or wip_time.date() in holidays:
+            wip_time = wip_time - timedelta(days=1)
+
+    last_close_day_time = wip_time.replace(hour=15, minute=30, second=0, microsecond=0)
+    return last_close_day_time
+
+
 # Defining current time
 def currenttime():
     # Adjusting for timezones
     ist = timezone(timedelta(hours=5, minutes=30))
     return datetime.now(ist).replace(tzinfo=None)
 
 
@@ -3580,35 +3644,35 @@
         token_df = scrips.loc[scrips["token"].isin(tokens)]
         symbol_token_pairs = [
             (token_df.loc[token_df["token"] == token, "symbol"].values[0], token)
             for token in tokens
         ]
         return symbol_token_pairs
 
-    if expiry is None and strike is None and option_type is None:
-        if name in ["BANKNIFTY", "NIFTY", "NIFTY FIN SERVICE"]:
+    if expiry is None and strike is None and option_type is None:  # Cash segment
+        if name in ["BANKNIFTY", "NIFTY", "NIFTY FIN SERVICE"]:  # Index scrips
             symbol, token = scrips.loc[
                 (scrips.name == name) & (scrips.exch_seg == "NSE"), ["symbol", "token"]
             ].values[0]
-        elif name == "FINNIFTY":
+        elif name == "FINNIFTY":  # Specific additional case for finnifty since cash segment price is not available
             futures = scrips.loc[
                 (scrips.name == name) & (scrips.instrumenttype == "FUTIDX"),
                 ["expiry", "symbol", "token"],
             ]
             futures["expiry"] = pd.to_datetime(futures["expiry"], format="%d%b%Y")
             futures = futures.sort_values(by="expiry")
             symbol, token = futures.iloc[0][["symbol", "token"]].values
-        else:
+        else:  # For all other equity scrips
             symbol, token = scrips.loc[
                 (scrips.name == name)
                 & (scrips.exch_seg == "NSE")
                 & (scrips.symbol.str.endswith("EQ")),
                 ["symbol", "token"],
             ].values[0]
-    elif expiry is not None and strike is not None and option_type is not None:
+    elif expiry is not None and strike is not None and option_type is not None:  # Options segment
         strike = str(int(strike))  # Handle float strikes, convert to integer first
         symbol = name + expiry + strike + option_type
         token = scrips[scrips.symbol == symbol]["token"].tolist()[0]
     else:
         raise ValueError("Invalid arguments")
 
     return symbol, token
@@ -3681,14 +3745,87 @@
                 raise Exception(f"Error in fetching LTP: {e}")
             else:
                 print(f"Error {attempt} in fetching LTP: {e}")
                 sleep(1)
                 continue
 
 
+def get_historical_prices(
+        interval,
+        last_n_intervals=None,
+        from_date=None,
+        to_date=None,
+        token=None,
+        name=None,
+        expiry=None,
+        strike=None,
+        option_type=None
+):
+
+    """ Available intervals:
+
+        ONE_MINUTE	1 Minute
+        THREE_MINUTE 3 Minute
+        FIVE_MINUTE	5 Minute
+        TEN_MINUTE	10 Minute
+        FIFTEEN_MINUTE	15 Minute
+        THIRTY_MINUTE	30 Minute
+        ONE_HOUR	1 Hour
+        ONE_DAY	1 Day
+
+        """
+
+    if token is None and name is None:
+        raise ValueError("Either name or token must be specified.")
+
+    if last_n_intervals is None and from_date is None:
+        raise ValueError("Either last_n_intervals or from_date must be specified.")
+
+    if last_n_intervals is not None and from_date is not None:
+        raise ValueError("Only one of last_n_intervals or from_date must be specified.")
+
+    if to_date is None:
+        to_date = last_market_close_time()
+    else:
+        to_date = pd.to_datetime(to_date)
+
+    if from_date is None and last_n_intervals is not None:
+        interval_digit, interval_unit = interval.lower().split("_")
+        interval_unit = interval_unit + "s" if interval_unit[-1] != "s" else interval_unit
+        interval_digit = word_to_num(interval_digit)
+        time_delta = interval_digit*last_n_intervals
+        from_date = to_date - timedelta(**{interval_unit: time_delta})
+    else:
+        from_date = pd.to_datetime(from_date)
+
+    to_date = to_date.strftime("%Y-%m-%d %H:%M")
+    from_date = from_date.strftime("%Y-%m-%d %H:%M")
+
+    if token is None:
+        _, token = fetch_symbol_token(name, expiry, strike, option_type)
+
+    exchange_seg = scrips.loc[scrips.token == token, "exch_seg"].values[0]
+
+    historic_param = {
+        "exchange": exchange_seg,
+        "symboltoken": token,
+        "interval": interval,
+        "fromdate": from_date,
+        "todate": to_date,
+    }
+    data = obj.getCandleData(historic_param)
+    data = pd.DataFrame(data["data"])
+    data.set_index(pd.Series(data.iloc[:, 0], name='date'), inplace=True)
+    data.index = pd.to_datetime(data.index)
+    data.index = data.index.tz_localize(None)
+    data.drop(data.columns[0], axis=1, inplace=True)
+    data.columns = ["open", "high", "low", "close", "volume"]
+    return data
+
+
 def fetchpreviousclose(exchange_seg, symbol, token):
     for attempt in range(3):
         try:
             previousclose = obj.ltpData(exchange_seg, symbol, token)["data"]["close"]
             return previousclose
         except Exception as e:
             if attempt == 2:
```

### Comparing `volstreet-0.9.6/volstreet/discord_bot.py` & `volstreet-0.9.7/volstreet/discord_bot.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.6/volstreet/nsefunctions.py` & `volstreet-0.9.7/volstreet/nsefunctions.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.6/volstreet/strategies.py` & `volstreet-0.9.7/volstreet/strategies.py`

 * *Files identical despite different names*

### Comparing `volstreet-0.9.6/volstreet.egg-info/requires.txt` & `volstreet-0.9.7/volstreet.egg-info/requires.txt`

 * *Files identical despite different names*

