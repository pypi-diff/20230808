# Comparing `tmp/yeref-0.2.95.tar.gz` & `tmp/yeref-0.2.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.2.95.tar", last modified: Tue Aug  8 15:18:18 2023, max compression
+gzip compressed data, was "yeref-0.2.97.tar", last modified: Tue Aug  8 16:19:22 2023, max compression
```

## Comparing `yeref-0.2.95.tar` & `yeref-0.2.97.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 15:18:18.045060 yeref-0.2.95/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 15:18:18.045292 yeref-0.2.95/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 15:18:18.046454 yeref-0.2.95/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 15:18:05.000000 yeref-0.2.95/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 15:18:18.041149 yeref-0.2.95/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.95/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.95/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   237742 2023-08-08 15:18:05.000000 yeref-0.2.95/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 15:18:18.044467 yeref-0.2.95/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 15:18:18.000000 yeref-0.2.95/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 15:18:18.000000 yeref-0.2.95/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 15:18:18.000000 yeref-0.2.95/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 15:18:18.000000 yeref-0.2.95/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:19:22.928993 yeref-0.2.97/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 16:19:22.929237 yeref-0.2.97/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-08-08 16:19:22.930151 yeref-0.2.97/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1552 2023-08-08 16:18:49.000000 yeref-0.2.97/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:19:22.920324 yeref-0.2.97/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.2.97/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   583683 2023-08-06 16:53:26.000000 yeref-0.2.97/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   238932 2023-08-08 16:16:45.000000 yeref-0.2.97/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-08-08 16:19:22.928145 yeref-0.2.97/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-08-08 16:19:22.000000 yeref-0.2.97/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-08-08 16:19:22.000000 yeref-0.2.97/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-08-08 16:19:22.000000 yeref-0.2.97/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-08-08 16:19:22.000000 yeref-0.2.97/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.2.95/setup.py` & `yeref-0.2.97/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.2.95',
+      version='0.2.97',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
```

### Comparing `yeref-0.2.95/yeref/l_.py` & `yeref-0.2.97/yeref/l_.py`

 * *Files identical despite different names*

### Comparing `yeref-0.2.95/yeref/yeref.py` & `yeref-0.2.97/yeref/yeref.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     InviteHashExpired, InviteHashInvalid, ChatAdminRequired, UserDeactivated, UsernameNotOccupied, ChannelBanned
 from pyrogram.raw import functions
 from stegano import lsb, exifHeader
 from telegraph.aio import Telegraph
 
 import yeref
 
-
 elly_a = 5900268983
 my_tid = 5491025132
 my_tids = [
     '5900268983',
     '6179455648',
     '6236215930',
 
@@ -94,15 +93,14 @@
 old_tid_del = 1_000_000_000
 lat_company = 59.395881
 long_company = 24.658980
 bin_empty = b'\xe2\x81\xa0\xe2\x81\xa0'  # .encode("utf-8")
 hex_empty = 'e281a0e281a0'  # .encode("utf-8").hex()  || bytes.fromhex()
 str_empty = bin_empty.decode('utf-8')
 
-
 SECTION = 'CONFIG'
 LINES_ON_PAGE = 5
 short_name = 'me'
 const_url = 'https://t.me/'
 phone_number = '79999999999'
 vk_group = 'https://vk.com'
 vk_account = 'https://vk.com'
@@ -150,15 +148,19 @@
 ferey_wp = 'https://t.me/bg/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 ferey_set = 'https://t.me/addstickers/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 ferey_emoji = 'https://t.me/addemoji/Mr2tXPkzQUoGAgAAv-ssUh01-P4'
 reactions_ = ['👍', '❤', '🔥', '🥰', '👏', '😁', '🤔', '🤯', '😱', '🤬', '😢', '🎉', '🤩', '🙏',
               '👌', '🕊', '🤡', '🥱', '🥴', '😍', '🐳', '❤\u200d🔥', '🌚', '🌭', '💯', '🤣', '⚡', '🍌', '🏆',
               '💔', '🤨', '😐', '🍓', '🍾', '💋', '😈', '😴', '😭', '🤓', '👻', '👨\u200d💻', '👀', '🎃',
               '🙈', '😇', '😨', '🤝', '✍', '🤗', '\U0001fae1', '😂', '🎄', '⛄', ' 🆒', '🗿']
-emojis_ = ['🙂', '😶‍🌫️', '🫥', '🎃', '😻', '🫶🏽', '🙌🏽', '👍🏽', '🤌🏾', '🫳🏽', '👉🏼', '☝🏽', '👋🏽', '✍🏽', '🙏🏼', '👣', '🫀', '👤', '👥', '👮🏽', '👩🏽‍💻', '🥷🏽', '💁🏽‍♂️', '🤷🏽‍♂️', '👕', '🧢', '🎓', '👓', '🐳', '🐋', '🌱', '🌿', '☘️', '🍀', '🍃', '🍂', '🍁', '🌚', '🌗', '🌏', '⭐️', '⚡️', '🔥', '☀️', '🌤️', '❄️', '🫧', '🌬️', '🧊', '🥏', '🎗️', '🧩', '🚀', '🗽', '🗿', '⛰️', '🏔️', '🗻', '🏠', '🏙️', '💻', '🎥', '🧭', '⏳', '🔋', '💡', '💵', '💰', '💳', '⚒️', '🛡️', '📍', '🪬', '🛋️', '🎉', '✉️', '📬', '📜', '📄', '📅', '🧾', '📇', '📋', '🗄️', '📁', '📰', '📘', '📖', '🖤', '〽️', '🔆', '✅', '🌐', '💠', '🔹', '💭', '🚩']
+emojis_ = ['🙂', '😶‍🌫️', '🫥', '🎃', '😻', '🫶🏽', '🙌🏽', '👍🏽', '🤌🏾', '🫳🏽', '👉🏼', '☝🏽', '👋🏽', '✍🏽', '🙏🏼', '👣', '🫀', '👤', '👥',
+           '👮🏽', '👩🏽‍💻', '🥷🏽', '💁🏽‍♂️', '🤷🏽‍♂️', '👕', '🧢', '🎓', '👓', '🐳', '🐋', '🌱', '🌿', '☘️', '🍀', '🍃', '🍂', '🍁', '🌚',
+           '🌗', '🌏', '⭐️', '⚡️', '🔥', '☀️', '🌤️', '❄️', '🫧', '🌬️', '🧊', '🥏', '🎗️', '🧩', '🚀', '🗽', '🗿', '⛰️', '🏔️', '🗻',
+           '🏠', '🏙️', '💻', '🎥', '🧭', '⏳', '🔋', '💡', '💵', '💰', '💳', '⚒️', '🛡️', '📍', '🪬', '🛋️', '🎉', '✉️', '📬', '📜', '📄',
+           '📅', '🧾', '📇', '📋', '🗄️', '📁', '📰', '📘', '📖', '🖤', '〽️', '🔆', '✅', '🌐', '💠', '🔹', '💭', '🚩']
 themes_ = ['🐥', '⛄', '💎', '👨\u200d🏫', '🌷', '💜', '🎄', '🎮']  # все в порядке, все ставятся, если не стояли
 bot_father = "@BotFather"
 text_jpeg = 'https://telegra.ph/file/0c675e5a3724deff3b2e1.jpg'
 bot_logo_jpeg = 'https://telegra.ph/file/99d4f150a52dcf78b3e8a.jpg'
 channel_logo_jpeg = 'https://telegra.ph/file/8418e1cd70484eac89477.jpg'
 group_logo_jpeg = 'https://telegra.ph/file/807e0d4fc4f271899272a.jpg'
 payment_photo = 'https://telegra.ph/file/75747cf7bc68f45a0e8b8.jpg'
@@ -185,15 +187,14 @@
      types.KeyboardButton(text='➡️️ Next')]], resize_keyboard=True, selective=True, row_width=3)
 
 BOT_VARS_ = '{"BOT_PROMO": "#911", "BOT_CHANNEL": 0, "BOT_CHANNELTID": 0, "BOT_GROUP": 0, "BOT_GROUPTID": 0, "BOT_TZ": "+00:00", "BOT_DT": "", "BOT_LZ": "en", "BOT_LC": "en"}'
 BOT_LSTS_ = '{"BOT_ADMINS": []}'
 USER_VARS_ = '{"USER_TEXT": "", "USER_PUSH": "", "USER_EMAIL": "", "USER_PROMO": "", "USER_PHONE": "", "USER_GEO": "", "USER_UTM": "", "USER_ID": 0, "USER_DT": "", "USER_TZ": "+00:00", "USER_LC": "en", "USER_ISADMIN": 0, "USER_ISPREMIUM": 0, "USER_BALL": 0, "USER_RAND": 0, "USER_QUIZ": 0, "USER_DICE": 0, "USER_PAY": 0, "DATE_TIME": 0}'
 USER_LSTS_ = '{"USER_UTMREF": []}'
 
-
 html_404 = f"""<!DOCTYPE html>
 <html lang="en">
 <head>
     <meta charset="UTF-8"><meta name="viewport" content="width=device-width, initial-scale=1.0">
     <style>
         body {{ background-image: url('https://telegra.ph/file/4b093c7e2b68f9f2915b0.jpg'); background-size: cover; background-position: center; font-family: Arial, sans-serif; display: flex; justify-content: center; align-items: center; height: 100vh; margin: 0; }}
         .container {{ text-align: center; padding: 30px; background-color: rgba(255, 255, 255, 0.8); border-radius: 10px; }}
@@ -219,15 +220,16 @@
         *,*::before, *::after {{ box-sizing: inherit; font-family: Arial, sans-serif; color: rgba(40, 40, 40, 0.99);}}
         a {{ text-decoration: none; }}
         span {{ color: #007bff; }}
         body {{ margin: 0; padding: 0; overflow-x: hidden; }}
         
         .text b, .text u, .text i, .text a, .text code, .text span {{ display: inline; }}
         .text code {{ font-family: 'Courier New', monospace; background-color: #f5f5f5; }}
-        .text {{ width: 100%; text-align: justify; }}
+        .text {{ width: 100%; text-align: justify; }}   
+        .text span { margin: -1px; }
 
         .container-wrapper {{ max-width: 1270px; height: 100vh;  padding: 4px; margin: 0 auto; display: flex; flex-direction: column; justify-content: space-between; gap: 4px; }}
         .container {{ display: flex; flex-direction: column; align-items: center; justify-content: flex-start; font-size: 14px; gap: 4px; }}
         
         .media-wrapper {{ -webkit-text-stroke: 0.5px rgba(50, 50, 50, 0.99); position: relative; width: 100%; min-height: 33vh; display: flex; justify-content: center; align-items: flex-start; }}
         .media {{ width: 100%; max-height: 33vh; object-fit: cover; }}
         .media:not(.rounded-media) {{ border-radius: 4px; }}
@@ -418,14 +420,16 @@
         fetchData(startUrl);
 
         for (let i = 0; i < buttonsClass.length; i++)  buttonsClass[i].addEventListener('click', async () => {{ await handleButtonClick(buttonsClass[i]); }});
     </script>
 </body>
 </html>
 """
+
+
 # endregion
 
 
 # region db
 def sqlite_lower(value_):
     return value_.lower() if value_ else None
 
@@ -738,15 +742,16 @@
 
 
 async def get_buttons_main(lz, bot_un, BASE_D):
     result = []
     try:
         result = [
             types.InlineKeyboardButton(text="👩🏽‍💼Acc", url=f"tg://user?id={my_tid}"),
-            types.InlineKeyboardButton(text="🙌🏽Tgph", web_app=types.WebAppInfo(url='https://telegra.ph/Links-07-05-462')),
+            types.InlineKeyboardButton(text="🙌🏽Tgph",
+                                       web_app=types.WebAppInfo(url='https://telegra.ph/Links-07-05-462')),
             types.InlineKeyboardButton(text="🔗Share",
                                        url=f'https://t.me/share/url?url=https%3A%2F%2Ft.me%2F{bot_un}&text=%40{bot_un}'),
             types.InlineKeyboardButton(text=f"{(await read_likes(BASE_D))}♥️Like", callback_data=f"like"),
             types.InlineKeyboardButton(text="🦋Chan", url=f"https://t.me/{get_tg_channel(lz)}"),
             types.InlineKeyboardButton(text="🫥Bots", switch_inline_query_current_chat=f"~"),
         ]
     except Exception as e:
@@ -1053,14 +1058,16 @@
         elif tid in b_ids:
             result = True
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
+
+
 # endregion
 
 
 # region admin
 async def pre_upload(bot, chat_id, media_name, media_type, EXTRA_D, BASE_D):
     result = None
     try:
@@ -1441,15 +1448,16 @@
             OFFER_TEXT = OFFER_TEXT if OFFER_TEXT and OFFER_TEXT != '' else str_empty
             OFFER_TEXT = f"<a href='{OFFER_TGPHLINK}'>​</a>{OFFER_TEXT}"
 
             if OFFER_ISGALLERY:
                 OFFER_TEXT = '' if OFFER_TEXT == str_empty and OFFER_MEDIATYPE != 'text' else OFFER_TEXT
                 buttons = [
                     types.InlineKeyboardButton(text="←", callback_data=f'gallery_prev_{offer_id}_{current}_{len_}'),
-                    types.InlineKeyboardButton(text=f"{current}/{len_}", switch_inline_query_current_chat=f"{offer_id} ~"),
+                    types.InlineKeyboardButton(text=f"{current}/{len_}",
+                                               switch_inline_query_current_chat=f"{offer_id} ~"),
                     types.InlineKeyboardButton(text="→", callback_data=f'gallery_next_{offer_id}_{current}_{len_}'),
                 ]
                 reply_markup.row(*buttons)
 
         if '[' in OFFER_MEDIATYPE and not message_id:
             media = []
             for i in range(0, len(OFFER_FILEID)):
@@ -2471,15 +2479,16 @@
 
 
 # endregion
 
 
 # region functions
 async def upper_register(txt):
-    result = str(txt).replace('0', '⁰').replace('1', '¹').replace('2', '²').replace('3', '³').replace('4', '⁴').replace('5', '⁵').replace('6', '⁶').replace('7', '⁷').replace('8', '⁸').replace('9', '⁹')
+    result = str(txt).replace('0', '⁰').replace('1', '¹').replace('2', '²').replace('3', '³').replace('4', '⁴').replace(
+        '5', '⁵').replace('6', '⁶').replace('7', '⁷').replace('8', '⁸').replace('9', '⁹')
     try:
         if len(result) >= 3:
             result = f"{result[0]}˙{result[1]}ᵏ"
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
@@ -2528,15 +2537,17 @@
                 if int(btn['i']) >= finish:
                     result = f"{row_html}</div>"
                     print(f"! res limit = {finish}, {result}")
                     break
 
                 sql = "SELECT PUSH_ID FROM PUSH WHERE POST_ID=? AND BUTTON_ID=?"
                 data_push = await db_select(sql, (int(MSG_VID), int(btn["i"]),), BASE_BOT)
-                btn_cnt_click = str(len(data_push)).replace('0', '⁰').replace('1', '¹').replace('2', '²').replace('3', '³').replace('4', '⁴').replace('5', '⁵').replace('6', '⁶').replace('7', '⁷').replace('8', '⁸').replace('9', '⁹')
+                btn_cnt_click = str(len(data_push)).replace('0', '⁰').replace('1', '¹').replace('2', '²').replace('3',
+                                                                                                                  '³').replace(
+                    '4', '⁴').replace('5', '⁵').replace('6', '⁶').replace('7', '⁷').replace('8', '⁸').replace('9', '⁹')
 
                 if btn['knd'] == 'payment':
                     invoice_link = await create_invoice_link(BOT_TID, BOT_LC, msg_text, msg_btns, BASE_D)
                     if not invoice_link: continue
 
                     btn_html = f'<a id="btn-{btn["knd"]}-{btn["i"]}-{str(len(data_push))}" class="button" data-url="{invoice_link}">{btn_cnt_click} {btn["lbl"]}</a>'
                     row_html = f"{row_html}{btn_html}"
@@ -2573,15 +2584,16 @@
         # msg_text = await replace_user_vars(chat_id, msg_text)
         msg_text = msg_text if msg_text and msg_text != '' else btn_name
         soup = BeautifulSoup(msg_text, 'html.parser')
         msg_text = soup.get_text()
 
         currency = await convert_domain_to_currency(BOT_LC)
         price = msg_btns[0]['lnk']
-        amount = int(price.replace('.', '').replace(',', '')) if '.' in price or ',' in price else int(f"{msg_btns[0]['lnk']}00")
+        amount = int(price.replace('.', '').replace(',', '')) if '.' in price or ',' in price else int(
+            f"{msg_btns[0]['lnk']}00")
         prices = [types.LabeledPrice(label=btn_name, amount=amount)]
 
         msg_media = {
             'title': btn_name,
             'description': msg_text,
             'payload': f"{BOT_TID}_{amount}",
             'provider_token': BOT_TOKENPAY,
@@ -3546,25 +3558,28 @@
                 if v[0]:
                     if len(tmp) > 0 and tmp[-1] is None:
                         result.row(*buttons)
                         if 'ᴵ' in v[0]:
                             buttons = [types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat='')]
                             cnt_k += 1
                         elif str(v[1]).startswith("btn_"):
-                            buttons = [types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{cnt_k}")]
+                            buttons = [types.InlineKeyboardButton(text=str(v[0]),
+                                                                  callback_data=f"btn_{type_}_{offer_id}_{cnt_k}")]
                             cnt_k += 1
                         else:
                             buttons = [types.InlineKeyboardButton(text=str(v[0]), url=v[1])]
                             cnt_k += 1
                     else:
                         if 'ᴵ' in v[0]:
-                            buttons.append(types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat=''))
+                            buttons.append(
+                                types.InlineKeyboardButton(text=str(v[0]), switch_inline_query_current_chat=''))
                             cnt_k += 1
                         elif str(v[1]).startswith("btn_"):
-                            buttons.append(types.InlineKeyboardButton(text=str(v[0]), callback_data=f"btn_{type_}_{offer_id}_{cnt_k}"))
+                            buttons.append(types.InlineKeyboardButton(text=str(v[0]),
+                                                                      callback_data=f"btn_{type_}_{offer_id}_{cnt_k}"))
                             cnt_k += 1
                         else:
                             buttons.append(types.InlineKeyboardButton(text=str(v[0]), url=v[1]))
                             cnt_k += 1
                 tmp.append(v[0])
             except Exception as e:
                 logger.info(log_ % str(e))
@@ -5178,15 +5193,15 @@
 # rm -rf /etc/letsencrypt/renewal/
 # rm -rf /etc/letsencrypt/archive/
 # rm -rf /etc/letsencrypt/live/
 # rm -rf /opt/letsencrypt
 # rm -rf /etc/letsencrypt
 # snap install --classic certbot
 # ln -s /snap/bin/certbot /usr/bin/certbot
- # POST
+# POST
 # cur.execute('''CREATE TABLE IF NOT EXISTS POST (
 #     POST_ID            INTEGER      PRIMARY KEY AUTOINCREMENT
 #                                     UNIQUE
 #                                     NOT NULL,
 #     POST_CHATTID       BIGINT       NOT NULL,
 #     POST_USERTID       BIGINT       NOT NULL,
 #     POST_TARGET        VARCHAR,
@@ -5245,29 +5260,31 @@
 
         for item in data:
             try:
                 await asyncio.sleep(round(random.uniform(1, 2), 2))
                 USER_TID, USER_LZ, USER_DTPAID, USER_ISPAID = item
                 get_ = await bot.get_chat(chat_id=USER_TID)
 
-                if USER_ISPAID == 1 and USER_DTPAID and (dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
+                if USER_ISPAID == 1 and USER_DTPAID and (
+                        dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
                     chan_private_donate = channel_library_ru if USER_LZ == 'ru' else channel_library_en
                     extra_bot = Bot(token=BOT_TOKEN_E18B)
                     get_chat_member_ = await extra_bot.get_chat_member(chat_id=chan_private_donate, user_id=USER_TID)
                     await extra_bot.session.close()
 
                     if get_chat_member_.status in ['member', 'administrator', 'creator']:
                         USER_DTPAID = datetime.datetime.utcnow().strftime('%d-%m-%Y_%H-%M-%S')
                         sql = "UPDATE USER SET USER_ISPAID=1, USER_USERNAME=?, USER_FULLNAME=?, USER_DTPAID=? " \
                               "WHERE USER_TID=?"
                         await db_change(sql, (get_.username, get_.full_name, USER_DTPAID, USER_TID,), BASE_D)
                     else:
                         sql = "UPDATE USER SET USER_ISPAID=0, USER_USERNAME=?, USER_FULLNAME=? WHERE USER_TID=?"
-                        await db_change(sql, (get_.username, get_.full_name, USER_TID, ), BASE_D)
-                elif USER_ISPAID == -1 and USER_DTPAID and (dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
+                        await db_change(sql, (get_.username, get_.full_name, USER_TID,), BASE_D)
+                elif USER_ISPAID == -1 and USER_DTPAID and (
+                        dt_ - datetime.datetime.strptime(USER_DTPAID, '%d-%m-%Y_%H-%M-%S')).days > 31:
                     result.append(item)
                 else:
                     sql = "UPDATE USER SET USER_USERNAME=?, USER_FULLNAME=? WHERE USER_TID=?"
                     await db_change(sql, (get_.username, get_.full_name, USER_TID,), BASE_D)
             except TelegramRetryAfter as e:
                 logger.info(log_ % f"TelegramRetryAfter {e.retry_after}")
                 await asyncio.sleep(e.retry_after + 1)
@@ -5279,28 +5296,30 @@
         await asyncio.sleep(e.retry_after + 1)
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
 
+
 # endregion
 
 
 # region web
-async def region_web(BOT_TID, POST_ID, POST_TYPE, POST_TEXT, POST_LNK, POST_BUTTON, ENT_TYPE, MEDIA_D, BASE_D, bot_username):
+async def region_web(BOT_TID, POST_ID, POST_TYPE, POST_TEXT, POST_LNK, POST_BUTTON, ENT_TYPE, MEDIA_D, BASE_D,
+                     bot_username):
     result = None
     try:
         POST_TEXT = POST_TEXT.replace('<tg-spoiler>', '').replace('</tg-spoiler>', '')
         BASE_BOT = os.path.join(MEDIA_D, str(BOT_TID), f"{str(BOT_TID)}.db")
         os.makedirs(os.path.join(MEDIA_D, str(BOT_TID)), exist_ok=True, mode=0o777)
         await db_bot_create(BASE_BOT)
-        sql = "SELECT BOT_TOKENTGPH, BOT_USERNAME, BOT_FIRSTNAME FROM BOT WHERE BOT_TID=?"
+        sql = "SELECT BOT_TOKENTGPH, BOT_USERNAME, BOT_FIRSTNAME, BOT_LC FROM BOT WHERE BOT_TID=?"
         data_bot = await db_select(sql, (BOT_TID,), BASE_D)
-        BOT_TOKENTGPH, BOT_USERNAME, BOT_FIRSTNAME = data_bot[0]
+        BOT_TOKENTGPH, BOT_USERNAME, BOT_FIRSTNAME, BOT_LC = data_bot[0]
 
         WEB_D = os.path.join(MEDIA_D, str(BOT_TID), 'WEB')
         os.makedirs(WEB_D, exist_ok=True, mode=0o777)
         file_html = os.path.join(WEB_D, f"{POST_ID}.html")
         msg_text = POST_TEXT
 
         m_html = ''
@@ -5330,69 +5349,80 @@
             m_html = f'''<div class="media-wrapper">{add_number}{add_media}{add_prev}{add_next}{add_dots}</div>'''
         print(m_html)
 
         txt_html = ''
         if msg_text and msg_text.strip() != '' and msg_text != str_empty:
             msg_text = msg_text.strip()
             msg_arr = re.split(r'\s+', msg_text)
-            print(msg_arr)
+            # print(msg_arr)
 
             for msg_item in msg_arr:
                 if msg_item.startswith('#') or msg_item.startswith('$'):
                     msg_text = msg_text.replace(msg_item, f"<span>{msg_item}</span>")
-
             txt_html = f'<div class="text">{msg_text}</div>'
 
         btn_html = ''
         if POST_BUTTON:
-            extra_id = 0
-            btns_html = ''
-            row_html = '<div class="buttons-row">'
-            dic_btns = await check_buttons2(POST_BUTTON, True)
-
-            for k, v in dic_btns.items():
-                if not v[0] or (len(v) > 0 and v[-1] is None):
-                    if len(row_html) > len('<div class="buttons-row">'):
-                        btns_html = f"{btns_html}{row_html}</div>"
-                        row_html = '<div class="buttons-row">'
-                    continue
-
-                btn_ix = extra_id
-                btn_knd = 'like' if v[-1] == 'btn_' else 'link'
-                btn_lbl = str(v[0]).strip('⁰')
-                btn_lnk = v[-1]
-                row_html = f'{row_html}<a id="btn-{btn_knd}-{btn_ix}-0" class="button" data-url="{btn_lnk}">⁰ {btn_lbl}</a>'
-                extra_id += 1
-
-            if len(row_html) > len('<div class="buttons-row">'):
-                btns_html = f"{btns_html}{row_html}</div>"
-            btn_html = f'<div class="buttons-wrapper">{btns_html}</div>'
+            if ENT_TYPE == 'PST':
+                extra_id = 0
+                btns_html = ''
+                row_html = '<div class="buttons-row">'
+                dic_btns = await check_buttons2(POST_BUTTON, True)
+
+                for k, v in dic_btns.items():
+                    if not v[0] or (len(v) > 0 and v[-1] is None):
+                        if len(row_html) > len('<div class="buttons-row">'):
+                            btns_html = f"{btns_html}{row_html}</div>"
+                            row_html = '<div class="buttons-row">'
+                        continue
+
+                    btn_ix = extra_id
+                    btn_knd = 'like' if v[-1] == 'btn_' else 'link'
+                    btn_lbl = str(v[0]).strip('⁰')
+                    btn_lnk = v[-1]
+                    row_html = f'{row_html}<a id="btn-{btn_knd}-{btn_ix}-0" class="button" data-url="{btn_lnk}">⁰ {btn_lbl}</a>'
+                    extra_id += 1
+
+                if len(row_html) > len('<div class="buttons-row">'):
+                    btns_html = f"{btns_html}{row_html}</div>"
+                btn_html = f'<div class="buttons-wrapper">{btns_html}</div>'
+            else:
+                msg_btns = ast.literal_eval(POST_BUTTON)
+                btns_html = ''
+                for i in range(1, 4):
+                    b_html = await get_row_html(msg_text, msg_btns, i * 3 - 3, i * 3, POST_ID, BOT_TID, BOT_LC,
+                                                BASE_BOT, BASE_D)
+                    btns_html = f"{btns_html}{b_html}"
+                btn_html = f'<div class="buttons-wrapper">{btns_html}</div>'
             print(f"btn_html = {btn_html}")
 
         sql = "SELECT VIEW_ID FROM VIEW WHERE ENT_VID=? AND ENT_TYPE=?"
         data_views = await db_select(sql, (POST_ID, ENT_TYPE,), BASE_BOT)
         msg_views = str(len(data_views))
         print(f"data_views={msg_views}")
 
         if POST_LNK:
             POST_LNKS = POST_LNK if '[' in POST_LNK else str([POST_LNK])
         else:
             POST_LNKS = '[]'
 
-        html_web = html_template.format(m_html, txt_html, btn_html, msg_views, BOT_USERNAME, BOT_TID, POST_ID, POST_LNKS)
+        html_web = html_template.format(m_html, txt_html, btn_html, msg_views, BOT_USERNAME, BOT_TID, POST_ID,
+                                        POST_LNKS)
         if POST_ID:
             with open(file_html, 'w', encoding='utf-8') as f:
                 f.write(html_web)
             result = f"https://t.me/{bot_username}/web?startapp={BOT_TID}_{POST_ID}"
             logger.info(f"{BOT_TID} ({POST_ID}): {result}")
     except Exception as e:
         logger.info(log_ % str(e))
         await asyncio.sleep(round(random.uniform(0, 1), 2))
     finally:
         return result
+
+
 # endregion
 
 
 def main():
     pass
```

