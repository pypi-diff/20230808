# Comparing `tmp/uwuipy-0.1.6.tar.gz` & `tmp/uwuipy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwuipy-0.1.6.tar", max compression
+gzip compressed data, was "uwuipy-0.1.7.tar", max compression
```

## Comparing `uwuipy-0.1.6.tar` & `uwuipy-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rwxr-xr-x   0        0        0     1084 2022-07-30 16:51:45.360190 uwuipy-0.1.6/LICENSE
--rwxr-xr-x   0        0        0     2018 2023-04-30 21:25:36.914918 uwuipy-0.1.6/README.md
--rwxr-xr-x   0        0        0      505 2023-04-30 22:22:54.298305 uwuipy-0.1.6/pyproject.toml
--rwxr-xr-x   0        0        0       26 2022-07-30 17:42:55.320171 uwuipy-0.1.6/uwuipy/__init__.py
--rwxr-xr-x   0        0        0     1834 2023-04-30 21:25:36.915912 uwuipy-0.1.6/uwuipy/__main__.py
--rwxr-xr-x   0        0        0     7620 2023-04-30 21:15:42.019576 uwuipy-0.1.6/uwuipy/uwuipy.py
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 uwuipy-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1084 2022-07-30 16:51:45.360190 uwuipy-0.1.7/LICENSE
+-rwxr-xr-x   0        0        0     3817 2023-08-07 22:29:12.374619 uwuipy-0.1.7/README.md
+-rwxr-xr-x   0        0        0      505 2023-04-30 22:44:46.030767 uwuipy-0.1.7/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2023-08-07 22:02:35.713706 uwuipy-0.1.7/uwuipy/__init__.py
+-rwxr-xr-x   0        0        0     2079 2023-08-07 22:02:35.717141 uwuipy-0.1.7/uwuipy/__main__.py
+-rwxr-xr-x   0        0        0     8354 2023-08-07 22:02:35.718140 uwuipy-0.1.7/uwuipy/uwuipy.py
+-rw-r--r--   0        0        0     4392 2023-08-07 22:57:54.078544 uwuipy-0.1.7/setup.py
+-rw-r--r--   0        0        0     4187 2023-08-07 22:57:54.078751 uwuipy-0.1.7/PKG-INFO
```

### Comparing `uwuipy-0.1.6/LICENSE` & `uwuipy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `uwuipy-0.1.6/uwuipy/__main__.py` & `uwuipy-0.1.7/uwuipy/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from uwuipy import uwuipy
 from os import getenv
-import readline
 import argparse
 
 
+try:
+    import readline
+
+except:
+    pass
+
+
 def main():
     parser = argparse.ArgumentParser(
         prog="uwuipy",
         description="UwUiPy uwuifies text. Runs a REPL if there is no message specified at CLI",
     )
 
     parser.add_argument(
@@ -46,23 +52,32 @@
         "-e",
         "--exclamationchance",
         type=float,
         default=1,
         help="The chance of replacing ! with an exclamation. [default: 1]",
     )
 
+    parser.add_argument(
+        "-n",
+        "--nsfwactions",
+        default=False,
+        action="store_true",
+        help="Enable NFSW actions. [default: False]"
+    )
+
     parser.add_argument("message", nargs=argparse.REMAINDER, help="The text to uwuify")
     args = parser.parse_args()
 
     uwu = uwuipy(
         args.seed,
         args.stutterchance,
         args.facechance,
         args.actionchance,
         args.exclamationchance,
+        args.nsfwactions
     )
 
     if len(args.message):
         print(uwu.uwuify(" ".join(args.message)))
         return
 
     while True:
```

### Comparing `uwuipy-0.1.6/uwuipy/uwuipy.py` & `uwuipy-0.1.7/uwuipy/uwuipy.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,79 @@
 import re
-import random as rand
+import random
 
 
 class uwuipy:
-    
     __uwu_pattern = [
-        (r'[rl]', 'w'),
-        (r'[RL]', 'W'),
-        (r'n([aeiou])', 'ny\g<1>'),
-        (r'N([aeiou])', 'Ny\g<1>'),
-        (r'N([AEIOU])', 'NY\g<1>'),
-        (r'ove', 'uv'),
-        (r'pog', 'poggies'),
+        (r"[rl]", "w"),
+        (r"[RL]", "W"),
+        (r"n([aeiou])", r"ny\g<1>"),
+        (r"N([aeiou])", r"Ny\g<1>"),
+        (r"N([AEIOU])", r"NY\g<1>"),
+        (r"ove", "uv"),
+        (r"pog", "poggies"),
     ]
 
     __actions = [
-        '***blushes***',
-        '***whispers to self***',
-        '***cries***',
-        '***screams***',
-        '***sweats***',
-        '***twerks***',
-        '***runs away***',
-        '***screeches***',
-        '***walks away***',
-        '***sees bulge***',
-        '***looks at you***',
-        '***notices buldge***',
-        '***starts twerking***',
-        '***huggles tightly***',
-        '***boops your nose***',
-        '***wags my tail***',
-        '***pounces on you***',
-        '***nuzzles your necky wecky***',
-        '***unzips your pants***',
-        '***licks lips***',
-        '***glomps and huggles***',
-        '***glomps***',
-        '***looks around suspiciously***',
-        '***smirks smuggly***',
-        '***pounces on your buldge***',
-        '***breaks into your house and aliases neofetch to rm -rf --no-preserve-root /***',
+        "***blushes***",
+        "***whispers to self***",
+        "***cries***",
+        "***screams***",
+        "***sweats***",
+        "***runs away***",
+        "***screeches***",
+        "***walks away***",
+        "***looks at you***",
+        "***huggles tightly***",
+        "***boops your nose***",
+        "***wags my tail***",
+        "***pounces on you***",
+        "***nuzzles your necky wecky***",
+        "***licks lips***",
+        "***glomps and huggles***",
+        "***glomps***",
+        "***looks around suspiciously***",
+        "***smirks smuggly***",
+        "***breaks into your house and aliases neofetch to rm -rf --no-preserve-root /***",
+    ]
+
+    # Because I got annoyed at them not being toggleable.
+    __nsfw_actions = [
+        "***twerks***",  # arguably nsfw
+        "***sees bulge***",
+        "***notices buldge***",
+        "***starts twerking***",  # also arguable.
+        "***unzips your pants***",
+        "***pounces on your buldge***",
     ]
 
     __exclamations = [
-        '!?',
-        '?!!',
-        '?!?1',
-        '!!11',
-        '!!1!',
-        '?!?!',
+        "!?",
+        "?!!",
+        "?!?1",
+        "!!11",
+        "!!1!",
+        "?!?!",
     ]
 
     __faces = [
-        "(・\`ω\´・)",
+        r"(・\`ω\´・)",
         ";;w;;",
         "OwO",
         "owo",
         "UwU",
-        "\>w\<",
+        r"\>w\<",
         "^w^",
         "ÚwÚ",
         "^-^",
         ":3",
         "x3",
-        'Uwu',
-        'uwU',
-        '(uwu)',
+        "Uwu",
+        "uwU",
+        "(uwu)",
         "(ᵘʷᵘ)",
         "(ᵘﻌᵘ)",
         "(◡ ω ◡)",
         "(◡ ꒳ ◡)",
         "(◡ w ◡)",
         "(◡ ሠ ◡)",
         "(˘ω˘)",
@@ -102,119 +105,152 @@
         "( ͡o ꒳ ͡o )",
         "( ˊ.ᴗˋ )",
         "(ᴜ‿ᴜ✿)",
         "~(˘▾˘~)",
         "(｡ᴜ‿‿ᴜ｡)",
     ]
 
-    def __init__(self, seed: int = None, stutter_chance: float = 0.1, face_chance: float = 0.05,
-                 action_chance: float = 0.075, exclamation_chance: float = 1):
-
+    def __init__(
+        self,
+        seed: int | None = None,
+        stutter_chance: float = 0.1,
+        face_chance: float = 0.05,
+        action_chance: float = 0.075,
+        exclamation_chance: float = 1,
+        nsfw_actions: bool = False,
+    ):
         # input protection to make sure the user stays within allowed parameters
         if not 0.0 <= stutter_chance <= 1.0:
-            raise ValueError("Invalid input value for stutterChance, supported range is 0-1.0")
-        elif not 0.0 <= face_chance <= 1.0:
-            raise ValueError("Invalid input value for faceChance, supported range is 0-1.0")
-        elif not 0.0 <= action_chance <= 1.0:
-            raise ValueError("Invalid input value for actionChance, supported range is 0-1.0")
-        elif not 0.0 <= exclamation_chance <= 1.0:
-            raise ValueError("Invalid input value for exclamationChance, supported range is 0-1.0")
+            raise ValueError(
+                "Invalid input value for stutterChance, supported range is 0-1.0"
+            )
+        if not 0.0 <= face_chance <= 1.0:
+            raise ValueError(
+                "Invalid input value for faceChance, supported range is 0-1.0"
+            )
+        if not 0.0 <= action_chance <= 1.0:
+            raise ValueError(
+                "Invalid input value for actionChance, supported range is 0-1.0"
+            )
+        if not 0.0 <= exclamation_chance <= 1.0:
+            raise ValueError(
+                "Invalid input value for exclamationChance, supported range is 0-1.0"
+            )
 
-        rand.seed(seed)
+        random.seed(seed)
         self._stutter_chance = stutter_chance
         self._face_chance = face_chance
         self._action_chance = action_chance
         self._exclamation_chance = exclamation_chance
+        self._nsfw_actions = nsfw_actions
 
     def _uwuify_words(self, _msg):
         # split the message into words
-        words = _msg.split(' ')
-        
+        words = _msg.split(" ")
+
         # iterate over each individual word
         # sure you could regex the entire thing, but then you lose
         # the ability to ignore certain cases, like pings and urls
         for idx, word in enumerate(words):
             # skip empty entries
             if not word:
                 continue
             # skip URLs
-            if re.search(r'((http:|https:)//[^ \<]*[^ \<\.])', word):
+            if re.search(r"((http:|https:)//[^ \<]*[^ \<\.])", word):
                 continue
             # skip pings
-            if word[0] == '@':
+            if word[0] == "@" or word[0] == "#" or word[0] == ":" or word[0] == "<":
                 continue
             # for each pattern in the array
             for pattern, substitution in self.__uwu_pattern:
                 # attempt to use the pattern on the word
                 word = re.sub(pattern, substitution, word)
-            
+
             # add the modified word to the original words array
             words[idx] = word
 
         # return the joined string
-        return ' '.join(words)
+        return " ".join(words)
 
     def _uwuify_spaces(self, _msg):
         # split the message into words
-        words = _msg.split(' ')
+        words = _msg.split(" ")
 
         # iterate over each individual word
         for idx, word in enumerate(words):
             # skip empty entries
             if not word:
                 continue
-            
+            # skip pings
+            if word[0] == "@" or word[0] == "#" or word[0] == ":" or word[0] == "<":
+                continue
+
             # get the character case for the second letter in the word
             next_char_case = word[1].isupper() if len(word) > 1 else False
-            _word = ''
-            
+            _word = ""
+
             # if we are to add stutters, do it
-            if rand.random() <= self._stutter_chance:
+            if random.random() <= self._stutter_chance:
                 # creates a random number between 1 and 2
-                stutter_len = rand.randrange(1, 3)
+                stutter_len = random.randrange(1, 3)
                 # add as many characters to the stutter as stutter_len dictates
                 for j in range(stutter_len + 1):
-                    _word += (word[0] if j == 0 else (word[0].upper() if next_char_case else word[0].lower())) + "-"
-                    
+                    _word += (
+                        word[0]
+                        if j == 0
+                        else (word[0].upper() if next_char_case else word[0].lower())
+                    ) + "-"
+
                 # add in the whole word, but make sure the case matches the next rest of the word
-                _word += (word[0].upper() if next_char_case else word[0].lower()) + word[1:]
-                
+                _word += (
+                    word[0].upper() if next_char_case else word[0].lower()
+                ) + word[1:]
+
             # if we are to add a face, do it
-            if rand.random() <= self._face_chance:
-                _word = (_word or word) + ' ' + self.__faces[rand.randrange(0, len(self.__faces))]
-                
+            if random.random() <= self._face_chance:
+                _word = (_word or word) + " " + random.choice(self.__faces)
+
             # if we are to add an action, do it
-            if rand.random() <= self._action_chance:
-                _word = (_word or word) + ' ' + self.__actions[rand.randrange(0, len(self.__actions))]
-                
+            if random.random() <= self._action_chance:
+                _word = (
+                    (_word or word)
+                    + " "
+                    + random.choice(
+                        self.__actions
+                        if not self._nsfw_actions
+                        else self.__actions + self.__nsfw_actions
+                    )
+                )
+
             # replace the word in the array with the modified if it exists, if not add the original word back
-            words[idx] = (_word or word)
+            words[idx] = _word or word
+
+        return " ".join(words)
 
-        return ' '.join(words)
-            
     def _uwuify_exclamations(self, _msg):
         # split the message into words
-        words = _msg.split(' ')
-        
+        words = _msg.split(" ")
+
         # iterate over each individual word
         for idx, word in enumerate(words):
             # skip empty entries
             if not word:
                 continue
             # skip if an exclamation is not present or the random number is greater than the chance
-            if (not re.search(r'[?!]+$', word)) or rand.random() > self._exclamation_chance:
+            if (
+                not re.search(r"[?!]+$", word)
+            ) or random.random() > self._exclamation_chance:
                 continue
-            
+
             # strip the exclamation from the word, add new exclamations and return it to the words array
-            index = rand.randrange(0, len(self.__exclamations))
-            word = re.sub(r'[?!]+$', '', word) + self.__exclamations[index]
+            word = re.sub(r"[?!]+$", "", word) + random.choice(self.__exclamations)
             words[idx] = word
-        
+
         # return the joined string
-        return ' '.join(words)
+        return " ".join(words)
 
     def uwuify(self, msg):
         msg = self._uwuify_words(msg)
         msg = self._uwuify_spaces(msg)
         msg = self._uwuify_exclamations(msg)
 
         return msg
```

