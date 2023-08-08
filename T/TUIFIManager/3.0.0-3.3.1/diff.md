# Comparing `tmp/TUIFIManager-3.0.0.tar.gz` & `tmp/TUIFIManager-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TUIFIManager-3.0.0.tar", last modified: Wed Jan 18 17:43:36 2023, max compression
+gzip compressed data, was "TUIFIManager-3.3.1.tar", last modified: Tue Aug  8 07:45:47 2023, max compression
```

## Comparing `TUIFIManager-3.0.0.tar` & `TUIFIManager-3.3.1.tar`

### file list

```diff
@@ -1,21 +1,38 @@
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-01-18 17:43:36.661411 TUIFIManager-3.0.0/
--rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-01-18 17:33:41.000000 TUIFIManager-3.0.0/LICENSE
--rw-r--r--   0 xou       (1000) xou       (1000)     8149 2023-01-18 17:43:36.661411 TUIFIManager-3.0.0/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)     7051 2023-01-18 17:29:00.000000 TUIFIManager-3.0.0/README.md
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-01-18 17:43:36.661411 TUIFIManager-3.0.0/TUIFIManager/
--rw-r--r--   0 xou       (1000) xou       (1000)    27087 2023-01-18 16:09:39.000000 TUIFIManager-3.0.0/TUIFIManager/TUIFIProfile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     5499 2023-01-03 16:30:58.000000 TUIFIManager-3.0.0/TUIFIManager/TUIFile.py
--rw-r--r--   0 xou       (1000) xou       (1000)     6460 2023-01-16 19:12:35.000000 TUIFIManager-3.0.0/TUIFIManager/TUIMenu.py
--rw-r--r--   0 xou       (1000) xou       (1000)     8659 2023-01-07 23:51:10.000000 TUIFIManager-3.0.0/TUIFIManager/TUItilities.py
--rw-r--r--   0 xou       (1000) xou       (1000)    55453 2023-01-18 17:37:11.000000 TUIFIManager-3.0.0/TUIFIManager/__init__.py
--rw-r--r--   0 xou       (1000) xou       (1000)     3107 2023-01-18 17:39:06.000000 TUIFIManager-3.0.0/TUIFIManager/__main__.py
-drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-01-18 17:43:36.661411 TUIFIManager-3.0.0/TUIFIManager.egg-info/
--rw-r--r--   0 xou       (1000) xou       (1000)     8149 2023-01-18 17:43:36.000000 TUIFIManager-3.0.0/TUIFIManager.egg-info/PKG-INFO
--rw-r--r--   0 xou       (1000) xou       (1000)      424 2023-01-18 17:43:36.000000 TUIFIManager-3.0.0/TUIFIManager.egg-info/SOURCES.txt
--rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-01-18 17:43:36.000000 TUIFIManager-3.0.0/TUIFIManager.egg-info/dependency_links.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       53 2023-01-18 17:43:36.000000 TUIFIManager-3.0.0/TUIFIManager.egg-info/entry_points.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-01-18 17:43:36.000000 TUIFIManager-3.0.0/TUIFIManager.egg-info/requires.txt
--rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-01-18 17:43:36.000000 TUIFIManager-3.0.0/TUIFIManager.egg-info/top_level.txt
--rw-r--r--   0 xou       (1000) xou       (1000)     1093 2023-01-18 17:36:32.000000 TUIFIManager-3.0.0/pyproject.toml
--rw-r--r--   0 xou       (1000) xou       (1000)     1272 2023-01-18 17:43:36.661411 TUIFIManager-3.0.0/setup.cfg
--rw-r--r--   0 xou       (1000) xou       (1000)       69 2023-01-04 08:02:28.000000 TUIFIManager-3.0.0/setup.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-08-08 07:45:47.745486 TUIFIManager-3.3.1/
+-rw-r--r--   0 xou       (1000) xou       (1000)      132 2023-08-04 06:46:27.000000 TUIFIManager-3.3.1/.gitattributes
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-08-08 07:45:47.735486 TUIFIManager-3.3.1/.github/
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-08-08 07:45:47.742153 TUIFIManager-3.3.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 xou       (1000) xou       (1000)      437 2023-08-05 01:45:08.000000 TUIFIManager-3.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 xou       (1000) xou       (1000)      604 2023-08-05 01:47:30.000000 TUIFIManager-3.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-08-08 07:45:47.742153 TUIFIManager-3.3.1/.github/workflows/
+-rw-r--r--   0 xou       (1000) xou       (1000)      652 2023-01-04 08:02:28.000000 TUIFIManager-3.3.1/.github/workflows/nox_ci.yml
+-rw-r--r--   0 xou       (1000) xou       (1000)      605 2022-12-31 18:56:42.000000 TUIFIManager-3.3.1/.gitignore
+-rw-r--r--   0 xou       (1000) xou       (1000)      464 2023-01-04 08:02:28.000000 TUIFIManager-3.3.1/.scrutinizer.yml
+-rw-r--r--   0 xou       (1000) xou       (1000)      492 2023-01-04 08:02:28.000000 TUIFIManager-3.3.1/.sourcery.yaml
+-rw-r--r--   0 xou       (1000) xou       (1000)     7729 2023-01-18 17:40:22.000000 TUIFIManager-3.3.1/CHANGELOG.md
+-rw-r--r--   0 xou       (1000) xou       (1000)    35149 2023-01-18 17:33:41.000000 TUIFIManager-3.3.1/LICENSE
+-rw-r--r--   0 xou       (1000) xou       (1000)     8767 2023-08-08 07:45:47.745486 TUIFIManager-3.3.1/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)  1285986 2023-08-04 23:04:46.000000 TUIFIManager-3.3.1/Peek.gif
+-rw-r--r--   0 xou       (1000) xou       (1000)     7669 2023-08-08 07:41:31.000000 TUIFIManager-3.3.1/README.md
+-rw-r--r--   0 xou       (1000) xou       (1000)   246555 2022-12-31 18:56:42.000000 TUIFIManager-3.3.1/TUIFI.png
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-08-08 07:45:47.745486 TUIFIManager-3.3.1/TUIFIManager/
+-rw-r--r--   0 xou       (1000) xou       (1000)    29042 2023-08-07 15:10:23.000000 TUIFIManager-3.3.1/TUIFIManager/TUIFIProfile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     6025 2023-08-08 06:39:14.000000 TUIFIManager-3.3.1/TUIFIManager/TUIFile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     6460 2023-08-06 09:01:10.000000 TUIFIManager-3.3.1/TUIFIManager/TUIMenu.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    11402 2023-08-07 05:50:19.000000 TUIFIManager-3.3.1/TUIFIManager/TUItilities.py
+-rw-r--r--   0 xou       (1000) xou       (1000)    60738 2023-08-08 07:06:29.000000 TUIFIManager-3.3.1/TUIFIManager/__init__.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     3109 2023-08-08 07:11:17.000000 TUIFIManager-3.3.1/TUIFIManager/__main__.py
+drwxr-xr-x   0 xou       (1000) xou       (1000)        0 2023-08-08 07:45:47.745486 TUIFIManager-3.3.1/TUIFIManager.egg-info/
+-rw-r--r--   0 xou       (1000) xou       (1000)     8767 2023-08-08 07:45:47.000000 TUIFIManager-3.3.1/TUIFIManager.egg-info/PKG-INFO
+-rw-r--r--   0 xou       (1000) xou       (1000)      671 2023-08-08 07:45:47.000000 TUIFIManager-3.3.1/TUIFIManager.egg-info/SOURCES.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)        1 2023-08-08 07:45:47.000000 TUIFIManager-3.3.1/TUIFIManager.egg-info/dependency_links.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       53 2023-08-08 07:45:47.000000 TUIFIManager-3.3.1/TUIFIManager.egg-info/entry_points.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       36 2023-08-08 07:45:47.000000 TUIFIManager-3.3.1/TUIFIManager.egg-info/requires.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)       13 2023-08-08 07:45:47.000000 TUIFIManager-3.3.1/TUIFIManager.egg-info/top_level.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)     1004 2023-08-04 06:46:27.000000 TUIFIManager-3.3.1/flake.lock
+-rw-r--r--   0 xou       (1000) xou       (1000)      695 2023-08-04 06:46:27.000000 TUIFIManager-3.3.1/flake.nix
+-rw-r--r--   0 xou       (1000) xou       (1000)      201 2023-01-04 08:02:28.000000 TUIFIManager-3.3.1/noxfile.py
+-rw-r--r--   0 xou       (1000) xou       (1000)     1093 2023-08-08 07:08:16.000000 TUIFIManager-3.3.1/pyproject.toml
+-rw-r--r--   0 xou       (1000) xou       (1000)       40 2023-01-04 08:02:28.000000 TUIFIManager-3.3.1/requirements.txt
+-rw-r--r--   0 xou       (1000) xou       (1000)     1272 2023-08-08 07:45:47.745486 TUIFIManager-3.3.1/setup.cfg
+-rw-r--r--   0 xou       (1000) xou       (1000)       69 2023-01-04 08:02:28.000000 TUIFIManager-3.3.1/setup.py
```

### Comparing `TUIFIManager-3.0.0/LICENSE` & `TUIFIManager-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.0.0/PKG-INFO` & `TUIFIManager-3.3.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TUIFIManager
-Version: 3.0.0
+Version: 3.3.1
 Summary: A cross-platform terminal-based termux-oriented file manager.
 Home-page: https://github.com/GiorgosXou/TUIFIManager
 Author: George Chousos
 Author-email: gxousos@gmail.com
 License: General Public License v3.0
 Project-URL: Github, https://github.com/GiorgosXou/TUIFIManager
 Keywords: file-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-platform
@@ -40,146 +40,155 @@
 	</a>
 </p>
 </div>
 
 A cross-platform terminal-based termux-oriented file manager *(and component)*, meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses) project or as is. This project is mainly an attempt to get more attention to the [Uni-Curses](https://github.com/unicurses/unicurses) project.
 
 
-## Installation
+# ⚙️ Installation
 ```terminal
 sudo pip3 install tuifimanager --upgrade
 ```
 ```terminal
 pip3 install TUIFIManager --upgrade
 ```
 or just ^^^ if it works for you. *(eg. on termux?)*
 
 
-## Usage
+# 💥 Usage
 Run `tuifi` in your terminal to use it as is or import it in one of your [Uni-Curses](https://github.com/unicurses/unicurses) project as a component like:
 ```python
 from TUIFIManager import *
 ```
 for more details look into the `__main__.py`
 
 <img src="./Peek.gif">
 <sub>FONT: Cartograph CF</sub>
 
-## Features & Shortcuts  
-### *Current:*
+# 📦 Features 
+### • 📌 *Current:*
 - Supports most of the common mouse events so far
 - It is somewhat fully customizable?
 - Can be used as a component
 - Uses only ~30MB of RAM
 - It is pretty snappy <!-- Kinda lol -->
 - Supports [Termux](https://github.com/termux) 
 - Cross Platform 
 - and more
 
-### *Desired:*
+### • 🔮 *Desired:*
 - Undo\Redo
 - tool-tips
 - Scroll bar
 - Sixel support
 - Multiple tabs
 - Better performance
 - Effect on cutted Files
 - [Drop files into GUI apps](https://github.com/GiorgosXou/TUIFIManager/issues/21)
 
-### *Common Shortcuts\Keybindings*
+# ⌨️ Keybindings
 In `vim_mode` both normal and vim shortcuts work 
 | Normal      | vim_mode | Action                                        |
 |----         | ---- |:----                                          |
 |`SHIFT + TAB`  |   |Moves selected file to the previous directory |
 |`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory          |
 |`ALT + DOWN`   |   |Opens\Closes the "right-click menu"           |
 |`KEY_HOME`     | `H`  |Navigates to the $HOME directory              |
 |`KEY_F5`       |   |Reload\Refresh current directory              |
 |`CTRL + V`     | `p` |Pastes the Copied or Cuted files              |
 |`DEL`          | `CTRL+d`  |Deletes the selected files                    |
 |`CTRL + F`     | `i`  |Find Files *(if not auto_find_on_typing)*     |
 |`CTRL + O`     | `O`  |Open whole directory in editor                |
+|`CTRL + A`     |  |Select all files in current folder|
 |`CTRL + C`     | `yy`  |Copies the selected files                     |
 |`CTRL + K`     |   |Copies the selected files                     |
 |`CTRL + X`     | `c`  |Cuts the selected files                       |
 |`CTRL + R`     | `r` |Rename selected file                          | 
+|`CTRL + T`     | | Toggle hidden files|
 |`CTRL + N`     | `W` |Create new folder                             |
 |`CTRL + W`     | `w` |Create new file                               |
 |`ARROW KEYS`   | `l` `k` `j` `h`  |Navigates files                               |
 |`KEY_ENTER`    | `K`|Opens files                                   |
 |`CTRL + E`     | `e` |Exit with `cd`                                  |
 |`ESCAPE`       |   |Exit                                          |
 
+**(*TIP:** 🐁 use `ALT + CLICK` for multiple mouse selection if `SHIFT` not working)*
 
-### *TERMUX only Shortcuts\Keybindings*
+***TERMUX only Shortcuts\Keybindings***
 | Shortcut    | Action                                                                         |
 |----         |:----                                                                           |
 |`CTRL + DOWN`| Goes in&out of select-mode while also automatically copies the selected file(s)|
 |`CTRL + LEFT`| Goes out of select-mode while also cuts the seleccted file(s)                  |
 |`CTRL + END` | Goes out of select-mode while also deleting the selected file(s)               |
 |`CTRL + UP`  | Same as `CTRL + V`, Pastes the Copied or Cuted files                           |
 |`END`        | Deletes selected files                                                         |
 
 
-### *Default & Custom - Commands*
-To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing`-env variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
+# 👨‍💻 Commands
+**(Default & Custom Comands)** - To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
 
 | Cmd | Type | Attributes | Label Comment|
 |---|---|---|---|
 |`gt` | open | 'directory':'~/.config/tuifi'           | - tuifi -|
 |`gh` | open | 'directory':'~/'                        | - Home -|
 |`owv` | open | 'directory':None,'\_with':'vim'         |Opened With Vim|
 |`yat` | copy | 'pattern':'.+\.txt'                     ||
 |`yy` | copy | 'pattern':None                          ||
 
 There are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character 
 
 
-# Documentation
+# 📜 Documentation
 <sub>Work in progress 🛠️🏗 ...</sub>
 
 
-## Customization 
-***How do I enable vim_mode?***
+# 💭 Customization 
+*How do I enable vim_mode?*
 > Set `tuifi_vim_mode` enviroment variable to `True`
 
-***How do I change the default keys (besides commands)?***
+*How do I change the default keys (besides commands)?*
 > This is not possible right now althought you could play around with the content of `toggle_vim_mode` function under `__init__.py`
 
-***How do I set the default editor?***
+*How do I set the default editor?*
 > Set `tuifi_default_editor` enviroment variable to `vim` or whatever you prefer
 
-***How do I disable the auto-find-mode?***
+*How do I disable the auto-find-mode?*
 > You can just set `tuifi_auto_find_on_typing` enviroment variable to `False`
 
-***How do I change the default configuration path?***
+*How do I change the scroll sensitivity?*
+> You can set either or both `tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number of characters per scroll action *(they default to 1 and 7)*
+
+How do I change the number of visible lines of filenames that are visible?
+> You can set how mnay lines you want using `tuifi_visible_filename_lines` *(Defaults to 4)*
+
+*How do I change the default configuration path?*
 > Set `tuifi_config_path` enviroment variable to whatever you prefer most
 
-***How do I toggle hidden files/folders?***
+*How do I toggle hidden files/folders?*
 > You can either `CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True`
 
-***How do I change the default colors?***
+*How do I change the default colors?*
 > [look here for more informations](https://github.com/GiorgosXou/TUIFIManager/issues/38)
 
 
-# Donation
+# 💗 Donation
 I do really need money to survive, I have no job, living in a basement, making things for free, because I love to.
 - [***Paypal Address***](https://www.paypal.com/donate/?hosted_button_id=QNQN23M55EJVS)
 - ***Monero Address:*** `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
 
 <div align="center">
 <img src='./TUIFI.png'>
 </div>
 
 
-# Special thanks to
+# 🫶 Special thanks to
 - [Bryan Lunduke for this article](https://lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the)
 - [Brodie Robertson for this video](https://youtu.be/9laxdMKTZLA)
 - [r/linux community for their comments](https://www.reddit.com/r/linux/comments/zzf5rx)
 - [r/cyberDeck community for their comments](https://www.reddit.com/r/cyberDeck/comments/zttur0)
 - [r/commandline community for their comments](https://www.reddit.com/r/commandline/comments/zt30v9)
 
-# Help
+# 🕳️ Help
 Any Idea with this issue https://github.com/unicurses/unicurses/issues/21 ?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TUIFIManager Version: 3.0.0 Summary: A cross-
+Metadata-Version: 2.1 Name: TUIFIManager Version: 3.3.1 Summary: A cross-
 platform terminal-based termux-oriented file manager. Home-page: https://
 github.com/GiorgosXou/TUIFIManager Author: George Chousos Author-email:
 gxousos@gmail.com License: General Public License v3.0 Project-URL: Github,
 https://github.com/GiorgosXou/TUIFIManager Keywords: file-
 manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-
 platform Platform: unix Platform: linux Platform: osx Platform: cygwin
 Platform: windows Classifier: Intended Audience :: Developers Classifier:
@@ -17,78 +17,86 @@
             [https://img.shields.io/github/last-commit/GiorgosXou/
 TUIFIManager?color=%4dc71f&label=Last%20Commit&logo=github&style=flat-square]
               [https://img.shields.io/github/license/GiorgosXou/
             TUIFIManager?label=License&logo=GNU&style=flat-square]
 A cross-platform terminal-based termux-oriented file manager *(and component)*,
 meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses)
 project or as is. This project is mainly an attempt to get more attention to
-the [Uni-Curses](https://github.com/unicurses/unicurses) project. ##
+the [Uni-Curses](https://github.com/unicurses/unicurses) project. # âï¸
 Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
 ```terminal pip3 install TUIFIManager --upgrade ``` or just ^^^ if it works for
-you. *(eg. on termux?)* ## Usage Run `tuifi` in your terminal to use it as is
-or import it in one of your [Uni-Curses](https://github.com/unicurses/
+you. *(eg. on termux?)* # ð¥ Usage Run `tuifi` in your terminal to use it as
+is or import it in one of your [Uni-Curses](https://github.com/unicurses/
 unicurses) project as a component like: ```python from TUIFIManager import *
 ``` for more details look into the `__main__.py` [./Peek.gif] FONT: Cartograph
-CF ## Features & Shortcuts ### *Current:* - Supports most of the common mouse
+CF # ð¦ Features ### â¢ ð *Current:* - Supports most of the common mouse
 events so far - It is somewhat fully customizable? - Can be used as a component
 - Uses only ~30MB of RAM - It is pretty snappy  - Supports [Termux](https://
-github.com/termux) - Cross Platform - and more ### *Desired:* - Undo\Redo -
-tool-tips - Scroll bar - Sixel support - Multiple tabs - Better performance -
-Effect on cutted Files - [Drop files into GUI apps](https://github.com/
-GiorgosXou/TUIFIManager/issues/21) ### *Common Shortcuts\Keybindings* In
+github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* -
+Undo\Redo - tool-tips - Scroll bar - Sixel support - Multiple tabs - Better
+performance - Effect on cutted Files - [Drop files into GUI apps](https://
+github.com/GiorgosXou/TUIFIManager/issues/21) # â¨ï¸ Keybindings In
 `vim_mode` both normal and vim shortcuts work | Normal | vim_mode | Action | |-
 --- | ---- |:---- | |`SHIFT + TAB` | |Moves selected file to the previous
 directory | |`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory | |`ALT
 + DOWN` | |Opens\Closes the "right-click menu" | |`KEY_HOME` | `H` |Navigates
 to the $HOME directory | |`KEY_F5` | |Reload\Refresh current directory | |`CTRL
 + V` | `p` |Pastes the Copied or Cuted files | |`DEL` | `CTRL+d` |Deletes the
 selected files | |`CTRL + F` | `i` |Find Files *(if not auto_find_on_typing)* |
-|`CTRL + O` | `O` |Open whole directory in editor | |`CTRL + C` | `yy` |Copies
-the selected files | |`CTRL + K` | |Copies the selected files | |`CTRL + X` |
-`c` |Cuts the selected files | |`CTRL + R` | `r` |Rename selected file | |`CTRL
-+ N` | `W` |Create new folder | |`CTRL + W` | `w` |Create new file | |`ARROW
-KEYS` | `l` `k` `j` `h` |Navigates files | |`KEY_ENTER` | `K`|Opens files |
-|`CTRL + E` | `e` |Exit with `cd` | |`ESCAPE` | |Exit | ### *TERMUX only
-Shortcuts\Keybindings* | Shortcut | Action | |---- |:---- | |`CTRL + DOWN`|
-Goes in&out of select-mode while also automatically copies the selected file
-(s)| |`CTRL + LEFT`| Goes out of select-mode while also cuts the seleccted file
-(s) | |`CTRL + END` | Goes out of select-mode while also deleting the selected
-file(s) | |`CTRL + UP` | Same as `CTRL + V`, Pastes the Copied or Cuted files |
-|`END` | Deletes selected files | ### *Default & Custom - Commands* To perform
-a command under the normal-mode, you first have to press the space-bar and then
-type the command. Alternatively, use `vim_mode` or enable the
-`tuifi_auto_command_on_typing`-env variable *(notice: it disables
-`tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can
-be found under the `~/.config/tuifi/cmds.conf` where you can add your custom
-ones too:** | Cmd | Type | Attributes | Label Comment| |---|---|---|---| |`gt`
-| open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` | open | 'directory':
-'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':'vim' |Opened With
-Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy | 'pattern':None ||
-There are also some "static" ones like the `m`+character which marks the
-current directory into the character, so you can navigate back to it by using
-\` or `;`+that_character # Documentation Work in progress ð ï¸ð ... ##
-Customization ***How do I enable vim_mode?*** > Set `tuifi_vim_mode` enviroment
-variable to `True` ***How do I change the default keys (besides commands)?*** >
-This is not possible right now althought you could play around with the content
-of `toggle_vim_mode` function under `__init__.py` ***How do I set the default
-editor?*** > Set `tuifi_default_editor` enviroment variable to `vim` or
-whatever you prefer ***How do I disable the auto-find-mode?*** > You can just
-set `tuifi_auto_find_on_typing` enviroment variable to `False` ***How do I
-change the default configuration path?*** > Set `tuifi_config_path` enviroment
-variable to whatever you prefer most ***How do I toggle hidden files/
-folders?*** > You can either `CTRL + T` or set `tuifi_show_hidden` enviroment
-variable to `True` ***How do I change the default colors?*** > [look here for
-more informations](https://github.com/GiorgosXou/TUIFIManager/issues/38) #
+|`CTRL + O` | `O` |Open whole directory in editor | |`CTRL + A` | |Select all
+files in current folder| |`CTRL + C` | `yy` |Copies the selected files | |`CTRL
++ K` | |Copies the selected files | |`CTRL + X` | `c` |Cuts the selected files
+| |`CTRL + R` | `r` |Rename selected file | |`CTRL + T` | | Toggle hidden
+files| |`CTRL + N` | `W` |Create new folder | |`CTRL + W` | `w` |Create new
+file | |`ARROW KEYS` | `l` `k` `j` `h` |Navigates files | |`KEY_ENTER` |
+`K`|Opens files | |`CTRL + E` | `e` |Exit with `cd` | |`ESCAPE` | |Exit | **
+(*TIP:** ð use `ALT + CLICK` for multiple mouse selection if `SHIFT` not
+working)* ***TERMUX only Shortcuts\Keybindings*** | Shortcut | Action | |---
+- |:---- | |`CTRL + DOWN`| Goes in&out of select-mode while also automatically
+copies the selected file(s)| |`CTRL + LEFT`| Goes out of select-mode while also
+cuts the seleccted file(s) | |`CTRL + END` | Goes out of select-mode while also
+deleting the selected file(s) | |`CTRL + UP` | Same as `CTRL + V`, Pastes the
+Copied or Cuted files | |`END` | Deletes selected files | # ð¨âð»
+Commands **(Default & Custom Comands)** - To perform a command under the
+normal-mode, you first have to press the space-bar and then type the command.
+Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-
+variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default
+commands can be seen below and can be found under the `~/.config/tuifi/
+cmds.conf` where you can add your custom ones too:** | Cmd | Type | Attributes
+| Label Comment| |---|---|---|---| |`gt` | open | 'directory':'~/.config/tuifi'
+| - tuifi -| |`gh` | open | 'directory':'~/' | - Home -| |`owv` | open |
+'directory':None,'\_with':'vim' |Opened With Vim| |`yat` | copy | 'pattern':
+'.+\.txt' || |`yy` | copy | 'pattern':None || There are also some "static" ones
+like the `m`+character which marks the current directory into the character, so
+you can navigate back to it by using \` or `;`+that_character # ð
+Documentation Work in progress ð ï¸ð ... # ð­ Customization *How do I
+enable vim_mode?* > Set `tuifi_vim_mode` enviroment variable to `True` *How do
+I change the default keys (besides commands)?* > This is not possible right now
+althought you could play around with the content of `toggle_vim_mode` function
+under `__init__.py` *How do I set the default editor?* > Set
+`tuifi_default_editor` enviroment variable to `vim` or whatever you prefer *How
+do I disable the auto-find-mode?* > You can just set
+`tuifi_auto_find_on_typing` enviroment variable to `False` *How do I change the
+scroll sensitivity?* > You can set either or both `tuifi_scroll_sensitivity`,
+`tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number
+of characters per scroll action *(they default to 1 and 7)* How do I change the
+number of visible lines of filenames that are visible? > You can set how mnay
+lines you want using `tuifi_visible_filename_lines` *(Defaults to 4)* *How do I
+change the default configuration path?* > Set `tuifi_config_path` enviroment
+variable to whatever you prefer most *How do I toggle hidden files/folders?* >
+You can either `CTRL + T` or set `tuifi_show_hidden` enviroment variable to
+`True` *How do I change the default colors?* > [look here for more
+informations](https://github.com/GiorgosXou/TUIFIManager/issues/38) # ð
 Donation I do really need money to survive, I have no job, living in a
 basement, making things for free, because I love to. - [***Paypal Address***]
 (https://www.paypal.com/donate/?hosted_button_id=QNQN23M55EJVS) - ***Monero
 Address:***
 `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
                                  [./TUIFI.png]
-# Special thanks to - [Bryan Lunduke for this article](https://
+# ð«¶ Special thanks to - [Bryan Lunduke for this article](https://
 lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the) - [Brodie Robertson
 for this video](https://youtu.be/9laxdMKTZLA) - [r/linux community for their
 comments](https://www.reddit.com/r/linux/comments/zzf5rx) - [r/cyberDeck
 community for their comments](https://www.reddit.com/r/cyberDeck/comments/
 zttur0) - [r/commandline community for their comments](https://www.reddit.com/
-r/commandline/comments/zt30v9) # Help Any Idea with this issue https://
+r/commandline/comments/zt30v9) # ð³ï¸ Help Any Idea with this issue https://
 github.com/unicurses/unicurses/issues/21 ?
```

### Comparing `TUIFIManager-3.0.0/README.md` & `TUIFIManager-3.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -11,146 +11,155 @@
 	</a>
 </p>
 </div>
 
 A cross-platform terminal-based termux-oriented file manager *(and component)*, meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses) project or as is. This project is mainly an attempt to get more attention to the [Uni-Curses](https://github.com/unicurses/unicurses) project.
 
 
-## Installation
+# ⚙️ Installation
 ```terminal
 sudo pip3 install tuifimanager --upgrade
 ```
 ```terminal
 pip3 install TUIFIManager --upgrade
 ```
 or just ^^^ if it works for you. *(eg. on termux?)*
 
 
-## Usage
+# 💥 Usage
 Run `tuifi` in your terminal to use it as is or import it in one of your [Uni-Curses](https://github.com/unicurses/unicurses) project as a component like:
 ```python
 from TUIFIManager import *
 ```
 for more details look into the `__main__.py`
 
 <img src="./Peek.gif">
 <sub>FONT: Cartograph CF</sub>
 
-## Features & Shortcuts  
-### *Current:*
+# 📦 Features 
+### • 📌 *Current:*
 - Supports most of the common mouse events so far
 - It is somewhat fully customizable?
 - Can be used as a component
 - Uses only ~30MB of RAM
 - It is pretty snappy <!-- Kinda lol -->
 - Supports [Termux](https://github.com/termux) 
 - Cross Platform 
 - and more
 
-### *Desired:*
+### • 🔮 *Desired:*
 - Undo\Redo
 - tool-tips
 - Scroll bar
 - Sixel support
 - Multiple tabs
 - Better performance
 - Effect on cutted Files
 - [Drop files into GUI apps](https://github.com/GiorgosXou/TUIFIManager/issues/21)
 
-### *Common Shortcuts\Keybindings*
+# ⌨️ Keybindings
 In `vim_mode` both normal and vim shortcuts work 
 | Normal      | vim_mode | Action                                        |
 |----         | ---- |:----                                          |
 |`SHIFT + TAB`  |   |Moves selected file to the previous directory |
 |`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory          |
 |`ALT + DOWN`   |   |Opens\Closes the "right-click menu"           |
 |`KEY_HOME`     | `H`  |Navigates to the $HOME directory              |
 |`KEY_F5`       |   |Reload\Refresh current directory              |
 |`CTRL + V`     | `p` |Pastes the Copied or Cuted files              |
 |`DEL`          | `CTRL+d`  |Deletes the selected files                    |
 |`CTRL + F`     | `i`  |Find Files *(if not auto_find_on_typing)*     |
 |`CTRL + O`     | `O`  |Open whole directory in editor                |
+|`CTRL + A`     |  |Select all files in current folder|
 |`CTRL + C`     | `yy`  |Copies the selected files                     |
 |`CTRL + K`     |   |Copies the selected files                     |
 |`CTRL + X`     | `c`  |Cuts the selected files                       |
 |`CTRL + R`     | `r` |Rename selected file                          | 
+|`CTRL + T`     | | Toggle hidden files|
 |`CTRL + N`     | `W` |Create new folder                             |
 |`CTRL + W`     | `w` |Create new file                               |
 |`ARROW KEYS`   | `l` `k` `j` `h`  |Navigates files                               |
 |`KEY_ENTER`    | `K`|Opens files                                   |
 |`CTRL + E`     | `e` |Exit with `cd`                                  |
 |`ESCAPE`       |   |Exit                                          |
 
+**(*TIP:** 🐁 use `ALT + CLICK` for multiple mouse selection if `SHIFT` not working)*
 
-### *TERMUX only Shortcuts\Keybindings*
+***TERMUX only Shortcuts\Keybindings***
 | Shortcut    | Action                                                                         |
 |----         |:----                                                                           |
 |`CTRL + DOWN`| Goes in&out of select-mode while also automatically copies the selected file(s)|
 |`CTRL + LEFT`| Goes out of select-mode while also cuts the seleccted file(s)                  |
 |`CTRL + END` | Goes out of select-mode while also deleting the selected file(s)               |
 |`CTRL + UP`  | Same as `CTRL + V`, Pastes the Copied or Cuted files                           |
 |`END`        | Deletes selected files                                                         |
 
 
-### *Default & Custom - Commands*
-To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing`-env variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
+# 👨‍💻 Commands
+**(Default & Custom Comands)** - To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
 
 | Cmd | Type | Attributes | Label Comment|
 |---|---|---|---|
 |`gt` | open | 'directory':'~/.config/tuifi'           | - tuifi -|
 |`gh` | open | 'directory':'~/'                        | - Home -|
 |`owv` | open | 'directory':None,'\_with':'vim'         |Opened With Vim|
 |`yat` | copy | 'pattern':'.+\.txt'                     ||
 |`yy` | copy | 'pattern':None                          ||
 
 There are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character 
 
 
-# Documentation
+# 📜 Documentation
 <sub>Work in progress 🛠️🏗 ...</sub>
 
 
-## Customization 
-***How do I enable vim_mode?***
+# 💭 Customization 
+*How do I enable vim_mode?*
 > Set `tuifi_vim_mode` enviroment variable to `True`
 
-***How do I change the default keys (besides commands)?***
+*How do I change the default keys (besides commands)?*
 > This is not possible right now althought you could play around with the content of `toggle_vim_mode` function under `__init__.py`
 
-***How do I set the default editor?***
+*How do I set the default editor?*
 > Set `tuifi_default_editor` enviroment variable to `vim` or whatever you prefer
 
-***How do I disable the auto-find-mode?***
+*How do I disable the auto-find-mode?*
 > You can just set `tuifi_auto_find_on_typing` enviroment variable to `False`
 
-***How do I change the default configuration path?***
+*How do I change the scroll sensitivity?*
+> You can set either or both `tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number of characters per scroll action *(they default to 1 and 7)*
+
+How do I change the number of visible lines of filenames that are visible?
+> You can set how mnay lines you want using `tuifi_visible_filename_lines` *(Defaults to 4)*
+
+*How do I change the default configuration path?*
 > Set `tuifi_config_path` enviroment variable to whatever you prefer most
 
-***How do I toggle hidden files/folders?***
+*How do I toggle hidden files/folders?*
 > You can either `CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True`
 
-***How do I change the default colors?***
+*How do I change the default colors?*
 > [look here for more informations](https://github.com/GiorgosXou/TUIFIManager/issues/38)
 
 
-# Donation
+# 💗 Donation
 I do really need money to survive, I have no job, living in a basement, making things for free, because I love to.
 - [***Paypal Address***](https://www.paypal.com/donate/?hosted_button_id=QNQN23M55EJVS)
 - ***Monero Address:*** `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
 
 <div align="center">
 <img src='./TUIFI.png'>
 </div>
 
 
-# Special thanks to
+# 🫶 Special thanks to
 - [Bryan Lunduke for this article](https://lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the)
 - [Brodie Robertson for this video](https://youtu.be/9laxdMKTZLA)
 - [r/linux community for their comments](https://www.reddit.com/r/linux/comments/zzf5rx)
 - [r/cyberDeck community for their comments](https://www.reddit.com/r/cyberDeck/comments/zttur0)
 - [r/commandline community for their comments](https://www.reddit.com/r/commandline/comments/zt30v9)
 
-# Help
+# 🕳️ Help
 Any Idea with this issue https://github.com/unicurses/unicurses/issues/21 ?
```

#### html2text {}

```diff
@@ -2,78 +2,86 @@
             [https://img.shields.io/github/last-commit/GiorgosXou/
 TUIFIManager?color=%4dc71f&label=Last%20Commit&logo=github&style=flat-square]
               [https://img.shields.io/github/license/GiorgosXou/
             TUIFIManager?label=License&logo=GNU&style=flat-square]
 A cross-platform terminal-based termux-oriented file manager *(and component)*,
 meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses)
 project or as is. This project is mainly an attempt to get more attention to
-the [Uni-Curses](https://github.com/unicurses/unicurses) project. ##
+the [Uni-Curses](https://github.com/unicurses/unicurses) project. # âï¸
 Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
 ```terminal pip3 install TUIFIManager --upgrade ``` or just ^^^ if it works for
-you. *(eg. on termux?)* ## Usage Run `tuifi` in your terminal to use it as is
-or import it in one of your [Uni-Curses](https://github.com/unicurses/
+you. *(eg. on termux?)* # ð¥ Usage Run `tuifi` in your terminal to use it as
+is or import it in one of your [Uni-Curses](https://github.com/unicurses/
 unicurses) project as a component like: ```python from TUIFIManager import *
 ``` for more details look into the `__main__.py` [./Peek.gif] FONT: Cartograph
-CF ## Features & Shortcuts ### *Current:* - Supports most of the common mouse
+CF # ð¦ Features ### â¢ ð *Current:* - Supports most of the common mouse
 events so far - It is somewhat fully customizable? - Can be used as a component
 - Uses only ~30MB of RAM - It is pretty snappy  - Supports [Termux](https://
-github.com/termux) - Cross Platform - and more ### *Desired:* - Undo\Redo -
-tool-tips - Scroll bar - Sixel support - Multiple tabs - Better performance -
-Effect on cutted Files - [Drop files into GUI apps](https://github.com/
-GiorgosXou/TUIFIManager/issues/21) ### *Common Shortcuts\Keybindings* In
+github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* -
+Undo\Redo - tool-tips - Scroll bar - Sixel support - Multiple tabs - Better
+performance - Effect on cutted Files - [Drop files into GUI apps](https://
+github.com/GiorgosXou/TUIFIManager/issues/21) # â¨ï¸ Keybindings In
 `vim_mode` both normal and vim shortcuts work | Normal | vim_mode | Action | |-
 --- | ---- |:---- | |`SHIFT + TAB` | |Moves selected file to the previous
 directory | |`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory | |`ALT
 + DOWN` | |Opens\Closes the "right-click menu" | |`KEY_HOME` | `H` |Navigates
 to the $HOME directory | |`KEY_F5` | |Reload\Refresh current directory | |`CTRL
 + V` | `p` |Pastes the Copied or Cuted files | |`DEL` | `CTRL+d` |Deletes the
 selected files | |`CTRL + F` | `i` |Find Files *(if not auto_find_on_typing)* |
-|`CTRL + O` | `O` |Open whole directory in editor | |`CTRL + C` | `yy` |Copies
-the selected files | |`CTRL + K` | |Copies the selected files | |`CTRL + X` |
-`c` |Cuts the selected files | |`CTRL + R` | `r` |Rename selected file | |`CTRL
-+ N` | `W` |Create new folder | |`CTRL + W` | `w` |Create new file | |`ARROW
-KEYS` | `l` `k` `j` `h` |Navigates files | |`KEY_ENTER` | `K`|Opens files |
-|`CTRL + E` | `e` |Exit with `cd` | |`ESCAPE` | |Exit | ### *TERMUX only
-Shortcuts\Keybindings* | Shortcut | Action | |---- |:---- | |`CTRL + DOWN`|
-Goes in&out of select-mode while also automatically copies the selected file
-(s)| |`CTRL + LEFT`| Goes out of select-mode while also cuts the seleccted file
-(s) | |`CTRL + END` | Goes out of select-mode while also deleting the selected
-file(s) | |`CTRL + UP` | Same as `CTRL + V`, Pastes the Copied or Cuted files |
-|`END` | Deletes selected files | ### *Default & Custom - Commands* To perform
-a command under the normal-mode, you first have to press the space-bar and then
-type the command. Alternatively, use `vim_mode` or enable the
-`tuifi_auto_command_on_typing`-env variable *(notice: it disables
-`tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can
-be found under the `~/.config/tuifi/cmds.conf` where you can add your custom
-ones too:** | Cmd | Type | Attributes | Label Comment| |---|---|---|---| |`gt`
-| open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` | open | 'directory':
-'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':'vim' |Opened With
-Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy | 'pattern':None ||
-There are also some "static" ones like the `m`+character which marks the
-current directory into the character, so you can navigate back to it by using
-\` or `;`+that_character # Documentation Work in progress ð ï¸ð ... ##
-Customization ***How do I enable vim_mode?*** > Set `tuifi_vim_mode` enviroment
-variable to `True` ***How do I change the default keys (besides commands)?*** >
-This is not possible right now althought you could play around with the content
-of `toggle_vim_mode` function under `__init__.py` ***How do I set the default
-editor?*** > Set `tuifi_default_editor` enviroment variable to `vim` or
-whatever you prefer ***How do I disable the auto-find-mode?*** > You can just
-set `tuifi_auto_find_on_typing` enviroment variable to `False` ***How do I
-change the default configuration path?*** > Set `tuifi_config_path` enviroment
-variable to whatever you prefer most ***How do I toggle hidden files/
-folders?*** > You can either `CTRL + T` or set `tuifi_show_hidden` enviroment
-variable to `True` ***How do I change the default colors?*** > [look here for
-more informations](https://github.com/GiorgosXou/TUIFIManager/issues/38) #
+|`CTRL + O` | `O` |Open whole directory in editor | |`CTRL + A` | |Select all
+files in current folder| |`CTRL + C` | `yy` |Copies the selected files | |`CTRL
++ K` | |Copies the selected files | |`CTRL + X` | `c` |Cuts the selected files
+| |`CTRL + R` | `r` |Rename selected file | |`CTRL + T` | | Toggle hidden
+files| |`CTRL + N` | `W` |Create new folder | |`CTRL + W` | `w` |Create new
+file | |`ARROW KEYS` | `l` `k` `j` `h` |Navigates files | |`KEY_ENTER` |
+`K`|Opens files | |`CTRL + E` | `e` |Exit with `cd` | |`ESCAPE` | |Exit | **
+(*TIP:** ð use `ALT + CLICK` for multiple mouse selection if `SHIFT` not
+working)* ***TERMUX only Shortcuts\Keybindings*** | Shortcut | Action | |---
+- |:---- | |`CTRL + DOWN`| Goes in&out of select-mode while also automatically
+copies the selected file(s)| |`CTRL + LEFT`| Goes out of select-mode while also
+cuts the seleccted file(s) | |`CTRL + END` | Goes out of select-mode while also
+deleting the selected file(s) | |`CTRL + UP` | Same as `CTRL + V`, Pastes the
+Copied or Cuted files | |`END` | Deletes selected files | # ð¨âð»
+Commands **(Default & Custom Comands)** - To perform a command under the
+normal-mode, you first have to press the space-bar and then type the command.
+Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-
+variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default
+commands can be seen below and can be found under the `~/.config/tuifi/
+cmds.conf` where you can add your custom ones too:** | Cmd | Type | Attributes
+| Label Comment| |---|---|---|---| |`gt` | open | 'directory':'~/.config/tuifi'
+| - tuifi -| |`gh` | open | 'directory':'~/' | - Home -| |`owv` | open |
+'directory':None,'\_with':'vim' |Opened With Vim| |`yat` | copy | 'pattern':
+'.+\.txt' || |`yy` | copy | 'pattern':None || There are also some "static" ones
+like the `m`+character which marks the current directory into the character, so
+you can navigate back to it by using \` or `;`+that_character # ð
+Documentation Work in progress ð ï¸ð ... # ð­ Customization *How do I
+enable vim_mode?* > Set `tuifi_vim_mode` enviroment variable to `True` *How do
+I change the default keys (besides commands)?* > This is not possible right now
+althought you could play around with the content of `toggle_vim_mode` function
+under `__init__.py` *How do I set the default editor?* > Set
+`tuifi_default_editor` enviroment variable to `vim` or whatever you prefer *How
+do I disable the auto-find-mode?* > You can just set
+`tuifi_auto_find_on_typing` enviroment variable to `False` *How do I change the
+scroll sensitivity?* > You can set either or both `tuifi_scroll_sensitivity`,
+`tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number
+of characters per scroll action *(they default to 1 and 7)* How do I change the
+number of visible lines of filenames that are visible? > You can set how mnay
+lines you want using `tuifi_visible_filename_lines` *(Defaults to 4)* *How do I
+change the default configuration path?* > Set `tuifi_config_path` enviroment
+variable to whatever you prefer most *How do I toggle hidden files/folders?* >
+You can either `CTRL + T` or set `tuifi_show_hidden` enviroment variable to
+`True` *How do I change the default colors?* > [look here for more
+informations](https://github.com/GiorgosXou/TUIFIManager/issues/38) # ð
 Donation I do really need money to survive, I have no job, living in a
 basement, making things for free, because I love to. - [***Paypal Address***]
 (https://www.paypal.com/donate/?hosted_button_id=QNQN23M55EJVS) - ***Monero
 Address:***
 `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
                                  [./TUIFI.png]
-# Special thanks to - [Bryan Lunduke for this article](https://
+# ð«¶ Special thanks to - [Bryan Lunduke for this article](https://
 lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the) - [Brodie Robertson
 for this video](https://youtu.be/9laxdMKTZLA) - [r/linux community for their
 comments](https://www.reddit.com/r/linux/comments/zzf5rx) - [r/cyberDeck
 community for their comments](https://www.reddit.com/r/cyberDeck/comments/
 zttur0) - [r/commandline community for their comments](https://www.reddit.com/
-r/commandline/comments/zt30v9) # Help Any Idea with this issue https://
+r/commandline/comments/zt30v9) # ð³ï¸ Help Any Idea with this issue https://
 github.com/unicurses/unicurses/issues/21 ?
```

### Comparing `TUIFIManager-3.0.0/TUIFIManager/TUIFIProfile.py` & `TUIFIManager-3.3.1/TUIFIManager/TUIFIProfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,14 +137,20 @@
     ),2, DEFAULT_EDITOR),
     '/cpp':TUIFIProfile((
         ' ┏━━━━++┓ \n'
         ' ┇ █▀▀▀ ┃ \n'
         ' ┃ █▄▄▄ ┃ \n'
         ' ┗━━━━━━┛ '
     ),2, DEFAULT_EDITOR),
+    '/toml':TUIFIProfile((
+        ' ┏┏━━━━┓┓ \n'
+        ' ┃░░┃┃░░┃ \n' 
+        ' ┃░░┇┃░░┃ \n'
+        ' ┗━━ ┛━━┛ '
+    ),3, DEFAULT_EDITOR),
     '/js':TUIFIProfile((
         ' ┌━━━━━━┐ \n'
         ' │▀█▀▒▀▀│ \n'
         ' │▃█ ▃▃▓│ \n'
         ' ╰━━━━━━╯ '
     ),2, DEFAULT_EDITOR),
     '/ts':TUIFIProfile((
@@ -265,15 +271,21 @@
         '          '
     ),2, DEFAULT_EDITOR),
     '/pyc':TUIFIProfile((
         ' ▃▃▃ ▃ ▃. \n'
         ' █▃█▒█▃█▒ \n'
         ' █▒.101█▒ \n'
         '          '
-        ),1, DEFAULT_EDITOR),
+    ),1, DEFAULT_EDITOR),
+    '/pyw':TUIFIProfile((
+        ' ▃▃▃ ▃ ▃. \n'
+        ' █▃█▒█▃█▒ \n'
+        ' █▒.wW.█▒ \n'
+        '          '
+    ),1, DEFAULT_EDITOR),
     '/txt':TUIFIProfile((
         ' ┏━━┓┓┓┓┓ \n'
         ' ┃┏┇┃☵☲┃┇ \n'
         ' ┃┇┛┃☲☵┃┃ \n'
         ' ┗━━┛━━┛┛ '
     ),1, DEFAULT_EDITOR),
     '/log':TUIFIProfile((
@@ -302,14 +314,48 @@
     ),2, DEFAULT_EDITOR),
     '/pdf':TUIFIProfile((
         ' ╭━━━━╮━╮ \n'
         ' ┃PDF┃==│ \n'
         ' ┃┇▒█┃▒▒│ \n'
         ' ┗━━━━━━╯ '
     ),3, DEFAULT_OPENER),
+
+
+    '/stl':TUIFIProfile((
+        ' ╭─╭┰─╮─╮ \n'
+        ' │╭╰┸─╯╮│ \n'
+        ' │╰.STL╯│ \n'
+        ' ╰━━━━━━╯ '
+    ),4, DEFAULT_OPENER),
+    '/gcode':TUIFIProfile((
+        ' ╭─╭─┰╮─┒ \n'
+        ' │[╰┬┸╯]┇ \n'
+        ' │GCODE:┃ \n'
+        ' ╰━━━━━━┛ '
+    ),1, DEFAULT_OPENER),
+    '/fcstd':TUIFIProfile((
+        ' ┏━━━━━━┓ \n'
+        ' ┃░█▀▀/:┃ \n'
+        ' ┃░█▀CAD┇ \n'
+        ' ┗━━━━━━┛ '
+    ),3, DEFAULT_EDITOR),
+    '/fcstd1':TUIFIProfile((
+        ' ╭────━━┓ \n'
+        ' │░█▀▀ER┃ \n'
+        ' │░█▀STO┇ \n'
+        ' ╰━━━━━━┛ '
+    ),1, DEFAULT_EDITOR),
+
+
+    '/lock':TUIFIProfile((
+        ' ┏┏━━━━┓┓ \n'
+        ' ┣┗LOCK┛┫ \n'
+        ' ┃┋┇[]┇┋┃ \n'
+        ' ┗━━━━━━┛ '
+    ),2, DEFAULT_EDITOR),
     '/bin':TUIFIProfile((
         ' ╭━━━━━━╮ \n'
         ' │OIIOIO│ \n'
         ' │━━━BIN│ \n'
         ' ╰━━━━━━╯ '
     ),1, DEFAULT_OPENER),
     '/sh':TUIFIProfile((
@@ -392,20 +438,34 @@
         ' ┍━━━┳┳┳┓ \n'
         ' │GIF:∵◖┇ \n'
         ' ┝┓░▃_▓▆┇ \n'
         ' ╰━━━┻┻┻┛ '
     ),2, DEFAULT_OPENER),
 
 
+    '/torrent':TUIFIProfile((
+        ' ╭──────╮ \n'
+        ' │TORENT│ \n'
+        ' │░▓██▓░│ \n'
+        ' ╰━━━━━━╯ '
+    ),5, DEFAULT_OPENER),
+
+
     '/mp4':TUIFIProfile((
         ' ┏┳┳┳┳┳┳┓ \n'
         ' ┇MP4∴∵◖┇ \n'
         ' ┇_░▃_▓▆┇ \n'
         ' ┗┻┻┻┻┻┻┛ '
     ),2, DEFAULT_OPENER),
+    '/mkv':TUIFIProfile((
+        ' ┏┳┳┳┳┳┳┓ \n'
+        ' ┇MKV∴∵◖┇ \n'
+        ' ┇_░▃_▓▆┇ \n'
+        ' ┗┻┻┻┻┻┻┛ '
+    ),2, DEFAULT_OPENER),
     '/3gp':TUIFIProfile((
         ' ┏┳┳┳┳┳┳┓ \n'
         ' ┇3GP∴∵◖┇ \n'
         ' ┇_░▃_▓▆┇ \n'
         ' ┗┻┻┻┻┻┻┛ '
     ),2, DEFAULT_OPENER),
     '/avi':TUIFIProfile((
@@ -468,14 +528,16 @@
     ),4, DEFAULT_EDITOR),
     '/exe':TUIFIProfile((
         ' ┏━━┳━┳━┓ \n'
         ' ┃▓█┣━╋━┫ \n'
         ' ┇EXE━┻━┫ \n'
         ' ╰━━┻━━━┛ '
     ),1, DEFAULT_OPENER),
+
+
     '/jpg':TUIFIProfile((
         ' ┏━━━JPG╮ \n'
         ' ┇*.∴:∵◖┃ \n'
         ' ┣┓░▃┏▓▆┇ \n'
         ' ╰━━━━━━┛ '
     ),2, DEFAULT_OPENER),
     '/png':TUIFIProfile((
@@ -575,26 +637,34 @@
         ' ┇.:.AAC┫ \n'
         ' ╋┻╋┻╋┻━┇ \n'
         ' ┗━━━━━━┛ '
     ),8, DEFAULT_OPENER),
 
 
     '/psd':TUIFIProfile((
-        ' ╭▃▃▃ ▃▃╮ \n'
-        ' │█▂█ █▃┃ \n'
-        ' │█   ▃█┃ \n'
-        ' ┕━PSD━━┛ '
+        ' ┏▃▃▃▃▃▃┓ \n'
+        ' ┃█▂█▒▃▃┃ \n'
+        ' ┃█  ▃▃▒┃ \n'
+        ' ┗━━━━━━┛ '
     ),4, DEFAULT_OPENER),
 
     '/mdf':TUIFIProfile((
-        ' ╭━━━━━━╮ \n'
-        ' ┃┇DB╭▒█┫ \n'
-        ' ┠┇██┻▓▒┃ \n'
-        ' ┗━━━╯━━╯ '
-    ),2, DEFAULT_OPENER),
+        ' ┏━━━━━━  \n'
+        ' ┃MDF┏▄ ┇ \n'
+        ' ┇█▓░┣┻▄┇ \n'
+        ' ┗━━ ▀  ┛ '
+    ),8, DEFAULT_EDITOR),
+    '/db':TUIFIProfile((
+        ' ┏━━┳━━━  \n'
+        ' ┃DB┃┏▄ ┇ \n'
+        ' ┇█▓░┣┻▄┇ \n'
+        ' ┗━━ ▀  ┛ '
+    ),8, DEFAULT_EDITOR),
+
+
     '/tuifi':TUIFIProfile((
         '             \                                      [            \n'
         '              @                 ⟡                  ╢             \n'
         '      /       ╣▒                                  ]▒       \     \n'
         '     ╔       ]Ñ▒                                  ╟╣┐       ▓    \n'
         '    ╢╣       ╣▓            √          t            ▓╣       ▓╣   \n'
         '   ▓╣▒╖    ╓╫╜           ╥▓   #TUIFI   ▓@           ╙▓╖    ╔╣╢║  \n'
```

### Comparing `TUIFIManager-3.0.0/TUIFIManager/TUIFile.py` & `TUIFIManager-3.3.1/TUIFIManager/TUIFile.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import unicurses
-
 from .TUIFIProfile import TUIFIProfile, LINK_SYMBOL, LINK_SYMBOL_COLOR, DEFAULT_PROFILE
+from os import getenv
+
+
+VISIBLE_FILENAME_LINES  = int(getenv('tuifi_visible_filename_lines', 4))
+
 
 
 class TUIFile:
     profile = DEFAULT_PROFILE
     #h,w = 4,11 # 10
     x,y         = 0,0
     name_height = 1
     is_selected = False
     is_cut      = False # This is pointless for now, until i find a way of efficiently drawing/managing cuted  files
 
 
     def chunk_str(self, text, n):
         base = '\n'.join(text[i:i+n] for i in range(0, len(text), n))
-        self.name_height = base.count('\n') + 1
+        self.name_height = base.count('\n') + 1 if base.count('\n') + 1 < VISIBLE_FILENAME_LINES  else VISIBLE_FILENAME_LINES
         return base
 
 
     def __init__(self, name, y=0, x=0, profile=DEFAULT_PROFILE, name_color=1, is_link=False):
         assert isinstance(profile, TUIFIProfile),'profile needs to be of type class TUIFIProfile'
         self.name_color  = name_color
         self.profile     = profile
@@ -34,27 +38,34 @@
         pass
 
 
     def draw_name(self, atpad, name, prename, chgatXY, attr=unicurses.A_NORMAL, color_pair_offset=0):  # fuck, lol
         """
         DON'T USE IT
         """
+        offXY = (VISIBLE_FILENAME_LINES * self.profile.width)
+        if VISIBLE_FILENAME_LINES and chgatXY >= offXY:
+            prename = prename[chgatXY - offXY +1:]
+            name = name[chgatXY - offXY +1:]
+            chgatXY = 0 + offXY -1
+
         y = chgatXY // self.profile.width
         x = chgatXY - y * (self.profile.width)
-        for offY, ln in enumerate(self.chunk_str(f'{prename} ', self.profile.width).split('\n'), self.profile.height):
+
+        for offY, ln in enumerate(self.chunk_str(f'{prename} ', self.profile.width).split('\n')[:VISIBLE_FILENAME_LINES], self.profile.height):
             unicurses.mvwaddwstr(atpad,offY + self.y,self.x, ' ' * len(ln)) # A_BOLD | 
-        for offY, ln in enumerate(self.chunk_str(name,self.profile.width).split('\n'), self.profile.height):
+        for offY, ln in enumerate(self.chunk_str(name,self.profile.width).split('\n')[:VISIBLE_FILENAME_LINES], self.profile.height):
             unicurses.mvwaddwstr(atpad,offY + self.y,self.x, ln, unicurses.COLOR_PAIR(self.name_color + color_pair_offset) | attr) # A_BOLD | 
         unicurses.mvwchgat(atpad,self.y + self.profile.height + y, self.x +x, 1, unicurses.A_NORMAL, 6 + color_pair_offset)
 
 
     def __draw_file(self, atpad, color_pair_offset=0):
         for offY, ln in enumerate((self.profile.text + '\n').split('\n')):
             unicurses.mvwaddwstr(atpad,offY + self.y,self.x, ln, unicurses.COLOR_PAIR(self.profile.color_map + color_pair_offset) ) 
-        for offY, ln in enumerate(self.chunk_str(self.name,self.profile.width).split('\n'), offY):
+        for offY, ln in enumerate(self.chunk_str(self.name,self.profile.width).split('\n')[:VISIBLE_FILENAME_LINES], offY):
             unicurses.mvwaddwstr(atpad,offY + self.y,self.x, ln, unicurses.COLOR_PAIR(self.name_color + color_pair_offset) )                  
 
         if self.is_link: # no idea why but mvwadd_wch misbehaves ...
             unicurses.mvwaddwstr(atpad, self.y + self.profile.height -1 , self.x + self.profile.width -1, LINK_SYMBOL, unicurses.COLOR_PAIR(LINK_SYMBOL_COLOR + color_pair_offset))  # | A_BOLD
 
 
     def __perform_effect(self, atpad, effect, color_map, redraw_icon=False, include_name=False):
@@ -62,15 +73,15 @@
         for y in range(self.y, self.y + self.profile.height):
             unicurses.mvwchgat(atpad,y, self.x, self.profile.width, effect, color_map)
 
         if not include_name: # meh
             effect    = unicurses.A_NORMAL
             color_map = self.name_color
 
-        for offY, ln in enumerate(self.chunk_str(self.name,self.profile.width).split('\n'), self.profile.height):
+        for offY, ln in enumerate(self.chunk_str(self.name,self.profile.width).split('\n')[:VISIBLE_FILENAME_LINES], self.profile.height):
             unicurses.mvwchgat(atpad,offY + self.y, self.x, len(ln), effect, color_map)
         # unicurses.mvwchgat(atpad,self.y + self.profile.height + y, self.x +x, 1, unicurses.A_NORMAL, 6 + color_pair_offset)
 
 
     def reverse_effect   (self, atpad, redraw_icon=False, color_pair_offset=0, include_name=False): self.__perform_effect(atpad, unicurses.A_REVERSE, 7 + color_pair_offset                      , redraw_icon, include_name)
     def dim_effect       (self, atpad, redraw_icon=False, color_pair_offset=0, include_name=False): self.__perform_effect(atpad, unicurses.A_DIM    , 1 + color_pair_offset                      , redraw_icon, include_name)
     def dim_color_effect (self, atpad,                    color_pair_offset=0, include_name=False): self.__perform_effect(atpad, unicurses.A_DIM    , self.profile.color_map + color_pair_offset , False      , include_name)
```

### Comparing `TUIFIManager-3.0.0/TUIFIManager/TUIMenu.py` & `TUIFIManager-3.3.1/TUIFIManager/TUIMenu.py`

 * *Files identical despite different names*

### Comparing `TUIFIManager-3.0.0/TUIFIManager/TUItilities.py` & `TUIFIManager-3.3.1/TUIFIManager/TUItilities.py`

 * *Files 18% similar despite different names*

```diff
@@ -84,32 +84,67 @@
     (uc.COLOR_GREEN  ,uc.COLOR_BLACK  ),
     (uc.COLOR_BLACK  ,uc.COLOR_WHITE  ),
     (uc.COLOR_BLUE   ,uc.COLOR_WHITE  ),
     (uc.COLOR_CYAN   ,uc.COLOR_BLACK  ),
     (uc.COLOR_BLACK  ,uc.COLOR_YELLOW ),
 )
 
+
+
+@dataclass
+class Border:
+    left                : int = uc.ACS_VLINE
+    right               : int = uc.ACS_VLINE
+    top                 : int = uc.ACS_HLINE
+    bottom              : int = uc.ACS_HLINE
+    top_left_corner     : int = uc.ACS_ULCORNER
+    top_right_corner    : int = uc.ACS_URCORNER
+    bottom_left_corner  : int = uc.ACS_LLCORNER
+    bottom_right_corner : int = uc.ACS_LRCORNER
+
+    def __post_init__(self):
+        self.left                = uc.CCHAR(self.left               )
+        self.right               = uc.CCHAR(self.right              )
+        self.top                 = uc.CCHAR(self.top                )
+        self.bottom              = uc.CCHAR(self.bottom             )
+        self.top_left_corner     = uc.CCHAR(self.top_left_corner    )
+        self.top_right_corner    = uc.CCHAR(self.top_right_corner   )
+        self.bottom_left_corner  = uc.CCHAR(self.bottom_left_corner )
+        self.bottom_right_corner = uc.CCHAR(self.bottom_right_corner)
+
+    def clear(self, win): uc.wborder(win, uc.CCHAR(' '), uc.CCHAR(' '), uc.CCHAR(' '), uc.CCHAR(' '), uc.CCHAR(' '), uc.CCHAR(' '), uc.CCHAR(' '), uc.CCHAR(' '))
+    def draw (self, win): uc.wborder(win, self.left, self.right, self.top, self.bottom, self.top_left_corner, self.top_right_corner, self.bottom_left_corner, self.bottom_right_corner)
+
+    def update(self, win):
+        self.clear(win)
+        self.draw (win)
+
+
+
 class Component():
-    def __init__(self, win, y, x, height, width, anchor, is_focused=False, color_pair_offset=0, iheight=None, iwidth=None ) -> None:
+    def __init__(self, win, y, x, height, width, anchor, is_focused=False, color_pair_offset=0, iheight=None, iwidth=None, warp=True, border:Border=None) -> None:
         self.pad               = uc.newpad(height, width)
         self.parent            = Parent(win or uc.stdscr)
         self.position          = Position (y, x)
         self.size              = Size(height, width, iheight or height, iwidth or width)
         self.anchor            = Anchor   (*anchor)
         self.is_focused        = is_focused
         self.color_pair_offset = color_pair_offset
+        self.warp              = warp
+        self.border            = border # TODO: to check
+        if border: self.border.draw(self.pad)
         for i in range(1, 10):                                            # Initializing color pairs of (FOREGROUND, BACKGROUND) colors.
             if uc.pair_content(i+color_pair_offset) in ((0,0),(7,0)):     # if it exists in some way | also TODO: https://github.com/GiorgosXou/TUIFIManager/issues/48
                 uc.init_pair(i+color_pair_offset, *MY_COLOR_PAIRS[i-1] )
 
 
     def refresh(self, redraw_parent=False):
         if redraw_parent:
             uc.touchwin(self.parent.win) # Do i need this? YES
-        uc.wrefresh(self.parent.win) # Do i need this? YES
+        uc.wrefresh(self.parent.win) # Do i need this? YES | IMPORTANT: wrefresh works only with windows, not pads also look at https://stackoverflow.com/a/35351060/11465149
         uc.prefresh(self.pad, self.position.iy, self.position.ix, self.position.y, self.position.x, self.position.y + self.size.height -1, self.position.x + self.size.width -1)
 
 
     @property #TODO: ADD descrition like use `self.position.x` instead if you don't want to redraw the `parent.win` immediately after
     def x(self): return self.position.x
 
     @x.setter
@@ -141,47 +176,70 @@
 
     @property
     def height(self): return self.size.height
 
     @height.setter
     def height(self, height): self.size.height = height; self.refresh(redraw_parent=True)
 
+    @property
+    def iwidth(self): return self.size.iwidth
+
+    @iwidth.setter
+    def iwidth(self, iwidth): self.size.iwidth = iwidth; uc.wresize(self.pad, self.iheight, iwidth); self.refresh(redraw_parent=True)
+
+    @property
+    def iheight(self): return self.size.iheight
+
+    @iheight.setter
+    def iheight(self, iheight): self.size.iheight = iheight; uc.wresize(self.pad, iheight, self.iwidth); self.refresh(redraw_parent=True)
 
     def get_mouse(self):
         id, x, y, z, bstate = uc.getmouse()
         in_range = (
             self.x <= x < self.x + self.width
             and self.y <= y < self.y + self.height
         )
         return (in_range, id, x, y, z, bstate )
 
 
-    def handle_resize(self, redraw_parent=True): # TODO: max min sizes
+    def handle_resize(self, redraw_parent=True, redraw_border=True): # TODO: max min sizes
+        if self.border and redraw_border: self.border.clear(self.pad)
         new_lines, new_columns = uc.getmaxyx(self.parent.win)
         if self.anchor.bottom:
             if self.anchor.top:
-                self.size.height += (new_lines - self.parent.lines)
-                uc.wresize(self.pad, self.height, self.width)
+                delta = (new_lines - self.parent.lines)
+                self.size.height  += delta
+                if self.warp or self.size.height > self.size.iheight: # That means that it won't contract the inside width unless you do so
+                    self.size.iheight += delta
+                    uc.wresize(self.pad, self.iheight, self.iwidth)
             else:
                 deltaY           = (new_lines - self.parent.lines)
                 self.position.y  += deltaY
                 # self.size.height += deltaY
         if self.anchor.right:
             if self.anchor.left:
-                self.size.width += (new_columns - self.parent.columns)
-                uc.wresize(self.pad, self.height, self.width)
+                delta = (new_columns - self.parent.columns)
+                self.size.width  += delta
+                if self.warp or self.size.width > self.size.iwidth:
+                    self.size.iwidth += delta
+                    uc.wresize(self.pad, self.iheight, self.iwidth)
             else:
                 deltaX           = (new_columns - self.parent.columns)
                 self.position.x += deltaX
                 # self.size.width += deltaX
 
         self.parent.lines   = new_lines
         self.parent.columns = new_columns
         if redraw_parent:
             uc.touchwin(self.parent.win)
+        if self.border and redraw_border: self.border.draw(self.pad)
+
+
+    def add_component(self, obj):
+        self.components.append(obj)
 
 
     def handle_events(self, event, redraw_parent=True):
         if event == uc.KEY_RESIZE: self.handle_resize(redraw_parent)
```

### Comparing `TUIFIManager-3.0.0/TUIFIManager/__init__.py` & `TUIFIManager-3.3.1/TUIFIManager/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,37 +3,43 @@
 
 from     contextlib import contextmanager
 from     send2trash import send2trash
 from      functools import partial
 from        pathlib import Path
 from         typing import Optional, Final
 from           time import time
-from             os import sep
+from             os import sep, access, W_OK
 from           math import log10
 from       .TUIMenu import TUIMenu
 from       .TUIFile import TUIFile
 from   .TUItilities import Component, Cd, Label, END_MOUSE, BEGIN_MOUSE, BEGIN_MOUSE, END_MOUSE, IS_WINDOWS, HOME_DIR, IS_TERMUX   
 from  .TUIFIProfile import TUIFIProfiles, DEFAULT_PROFILE , DEFAULT_WITH, DEFAULT_OPENER
 import   subprocess
 import    unicurses
 import       shutil
 import       signal
+import         json
 import          ast
 import           re
 import           os
 
-__version__: Final[str] = "3.0.0"
+__version__: Final[str] = "3.3.1"
 
 PADDING_LEFT   = 2
 PADDING_RIGHT  = 2
 PADDING_TOP    = 1
 PADDING_BOTTOM = 0
 
-UP             = -1
-DOWN           =  1
+SCROLL_SENSITIVITY      = int(os.getenv('tuifi_scroll_sensitivity'     , 1))
+CTRL_SCROLL_SENSITIVITY = int(os.getenv('tuifi_ctrl_scroll_sensitivity', 7))
+
+UP             = -      SCROLL_SENSITIVITY
+DOWN           =        SCROLL_SENSITIVITY
+CTRL_UP        = - CTRL_SCROLL_SENSITIVITY
+CTRL_DOWN      =   CTRL_SCROLL_SENSITIVITY
 
 CONFIG_PATH    = os.getenv('tuifi_config_path',f'{HOME_DIR}{sep}.config{sep}tuifi')
 STTY_EXISTS    = shutil.which('stty')
 INIT_DIRECTORY = os.getcwd()
 
 
 def stty_a(key=None):  # whatever [...]
@@ -98,20 +104,24 @@
 
         if directory:
             self.directory = os.path.normpath(directory)
             self.load_files(directory, suffixes, sort_by)
             if draw_files:
                 self.draw()
 
+        self.load_markers       ()
         self.load_commands      ()
         self.__set_normal_events()
         if stty_a('^C') or unicurses.OPERATING_SYSTEM == 'Windows': signal.signal(signal.SIGINT,self.copy) # https://docs.microsoft.com/en-us/windows/console/ctrl-c-and-ctrl-break-signals
         if os.getenv('tuifi_vim_mode', str(vim_mode)) == 'True'   : self.toggle_vim_mode()
 
 
+    def __del__(self):
+        self.save_markers()
+
 
     def draw(self):
         unicurses.werase(self.pad)
         #self.refresh()
         if self.maxpLines < self.height:
             self.maxpLines = self.height
         unicurses.wresize(self.pad, self.maxpLines, self.width)
@@ -148,15 +158,15 @@
         self.__count = 0
         self.___y    = PADDING_TOP
         self.___x    = PADDING_LEFT
 
 
     def __set_coordinates(self, file, resize=False):
         tempX = (PADDING_LEFT + file.profile.width + PADDING_RIGHT)
-        if self.___x > self.width-tempX + PADDING_RIGHT - self.x :
+        if self.___x > self.width + self.x - tempX + PADDING_RIGHT - self.x :
             self.___x  = PADDING_LEFT
             self.___y += self.__max_h + PADDING_TOP + PADDING_BOTTOM  # ... +1 because the next has to be below :P
             self.__count = 0
             self.__max_h = 0
 
         file.y = self.___y
         file.x = self.___x
@@ -174,16 +184,19 @@
             if self.maxpLines < self.height:
                 self.maxpLines = self.height
             unicurses.wresize(self.pad, self.maxpLines, self.width)
 
 
     def __is_valid_file(self, name):
         if not self.show_hidden and name.startswith('.'): return False
-        if self.is_in_find_mode:
-            return self.__temp_find_filename in name
+        if self.is_in_find_mode or self.__keep_search_results:
+            if self.__temp_find_filename.islower():
+                return self.__temp_find_filename in name.lower()
+            else:
+                return self.__temp_find_filename in name
         if self.suffixes and os.path.isfile(self.directory + sep + name):
             for s in self.suffixes:
                 if name.endswith(s): return True
             return False
         return True
 
 
@@ -236,20 +249,29 @@
         #if self.height + self.position.iy > y:
         #    self.position.iy -= self.height + self.position.iy - y  # NOT SURE AT ALL BUT IT WORKS LOL, actually NOP ):(
         #self.draw()
         #self.select(self.__clicked_file) #  ??????????????
         return self.files
 
 
-    def reload(self,draw_files=True):
-        self.position.iy             = 0
-        self.__clicked_file          = None
-        self.__index_of_clicked_file = None
-        self.__pre_hov               = None           
+    __keep_search_results = False # really bad practice but whatever lol (and i can't take advantage of is_in_find_mode because of error when moving files that ...)
+    def reload(self,draw_files=True, keep_search_results=False):
+        if not keep_search_results:
+            self.__temp_find_filename = ''
+        else:
+            self.__keep_search_results = True
+        self.position.iy                = 0
+        self.__mouse_btn1_pressed_file  = None
+        self.__pre_clicked_file         = None
+        self.__clicked_file             = None
+        self.__index_of_clicked_file    = None
+        self.__pre_hov                  = None           
+        self.__count_selected           = 0
         self.load_files(self.directory)
+        self.__keep_search_results      = False
         if draw_files:
             self.draw()
 
 
     @contextmanager
     def suspend(self):
         """
@@ -285,32 +307,35 @@
             proc = subprocess.Popen([open_with, *dirs], shell=IS_WINDOWS)
             proc.wait()
         print(BEGIN_MOUSE, end='\r')
         self.__set_label_on_file_selection()
         return
 
 
+    def __open_multiple(self, directory, suffixes=[], sort_by=None, _with=None): # TODO: check if selected files are folders and open them in new tabs
+        prof = f'/{os.path.splitext(directory)[1][1:]}'
+        open_with = TUIFIProfiles.get(prof, DEFAULT_PROFILE).open_with
+        return self.__try_open_with(directory, open_with, True)
+
+
     def open(self, directory, suffixes=[], sort_by=None, _with=None):
         """
         `open()` is `load_files()` + `draw()`
         """
         if directory is None or not directory:
             return None
 
         if isinstance(directory, TUIFile):
             directory = self.directory + sep + directory.name
 
         if _with: 
             return self.__try_open_with(directory, _with)
 
-        multiple = self.__count_selected > 1
-        if not os.path.isdir(directory) or multiple:
-            prof = f'/{os.path.splitext(directory)[1][1:]}'
-            open_with = TUIFIProfiles.get(prof, DEFAULT_PROFILE).open_with
-            return self.__try_open_with(directory, open_with, multiple)
+        # if there is at least one file that it is not a directory OR multiple selected files that they are whatever, then: ... (Now it makes sense why `not isdir`)
+        if not os.path.isdir(directory) or self.__count_selected > 1 : return self.__open_multiple(directory, suffixes, sort_by, _with)
 
         if self.vim_mode and self.escape_event_consumed and not self.is_in_command_mode: # SuS SuS SuS SuS SuS damn that's so Sus lol
             self.find()
         else:
             self.is_in_find_mode       = False
             self.escape_event_consumed = False
         self.__change_escape_event_consumed = False
@@ -361,34 +386,41 @@
             tuifile = self.__clicked_file
         if not tuifile:
             for f in self.files:
                 if f.is_selected:
                     f.is_selected = False
                     f.draw(self.pad, color_pair_offset=self.color_pair_offset)
             self.__count_selected = 0 # i can just -= 1 and break it if 0 :P
-        else:
+        elif tuifile.is_selected:
             tuifile.is_selected = False
             tuifile.draw(self.pad, color_pair_offset=self.color_pair_offset)
             self.__count_selected -=1
 
 
     def select(self, tuifile):
+        if tuifile.is_selected:return
         self.__count_selected +=1
-        if not tuifile:
-            return
         #for y in range(tuifile.y, tuifile.y + tuifile.profile.height):
         #    mvwchgat(self.pad,y, tuifile.x, tuifile.profile.width,A_REVERSE,7)
         tuifile.is_selected = True
         tuifile.draw(self.pad, color_pair_offset=self.color_pair_offset)
 
 
+    def select_all_files(self):
+        for f in self.files[1:]:
+            self.select(f)
+        self.__set_label_text(f'[{self.__count_selected}] Files selected')
+
+
     def scroll_pad(self, y):
-        if self.position.iy == 0 and y < 0:
+        if self.position.iy <= 0 and y < 0:
+            self.position.iy = 0
             return
         if self.position.iy >= unicurses.getmaxy(self.pad) - self.height  and y > 0:
+            self.position.iy = unicurses.getmaxy(self.pad) - self.height
             return
         self.position.iy += y
 
 
     def exit_to_self_directory(self):
         if not IS_WINDOWS and not self.directory == INIT_DIRECTORY:
             self.cd(self.directory)
@@ -412,14 +444,15 @@
             unicurses.KEY_UP        : self.__perform_key_up             ,
             unicurses.KEY_DOWN      : self.__perform_key_down           ,
             unicurses.KEY_LEFT      : self.__perform_key_left           ,
             unicurses.KEY_RIGHT     : self.__perform_key_right          ,
             unicurses.KEY_BTAB      : self.__perform_key_btab           ,
             unicurses.KEY_DC        : self.delete                       ,
             unicurses.KEY_F(5)      : self.reload                       ,
+            unicurses.CTRL('A')     : self.select_all_files             ,
             unicurses.CTRL('T')     : self.toggle_hidden_files          ,
             unicurses.CTRL('R')     : self.rename                       ,
             unicurses.CTRL('C')     : self.copy                         ,
             unicurses.CTRL('K')     : self.copy                         ,
             unicurses.CTRL('X')     : self.cut                          ,
             unicurses.CTRL('V')     : self.paste                        ,
             unicurses.CTRL('W')     : partial(self.create_new, 'file'  ),
@@ -427,15 +460,15 @@
             unicurses.CTRL('F')     : self.find                         ,
             unicurses.CTRL('O')     : self.__open_DEFAULT_WITH          , # https://stackoverflow.com/a/33966657/11465149
             unicurses.CTRL('E')     : self.exit_to_self_directory       ,
             unicurses.KEY_HOME      : partial(self.open, HOME_DIR)      ,
             unicurses.KEY_ENTER     : self.__perform_key_enter          ,
             10                      : self.__perform_key_enter          ,
             unicurses.KEY_BACKSPACE : self.__open_previous_dir          ,
-            8                       : self.__open_previous_dir          ,
+            8                       : self.__open_previous_dir          , # https://superuser.com/questions/212874/why-is-backspace-often-represented-with-h | TODO: I might remove it 
             127                     : self.__open_previous_dir          ,
             263                     : self.__open_previous_dir          ,
             unicurses.KEY_RESIZE    : self.__handle_resize_event        ,
             32                      : self.command                      , # SPACEBAR
         }
 
     def toggle_vim_mode(self): # TODO: Use it in rename and find or something
@@ -502,19 +535,27 @@
             return
         temp_sum_of_Y__y_and_height_of_tuifile = self.y + tuifile.y + tuifile.profile.height + tuifile.name_height + PADDING_TOP
         temp_sum_of_visible_H_and_Y =  self.height + self.position.iy
         if temp_sum_of_Y__y_and_height_of_tuifile > temp_sum_of_visible_H_and_Y  :
             self.position.iy += temp_sum_of_Y__y_and_height_of_tuifile - (temp_sum_of_visible_H_and_Y )
 
 
+    def has_write_access(self, path):
+        if not access(path, W_OK):
+            self.__set_label_text('[ERROR] NO WRITE PERMISSION')
+            return False
+        return True
+
+
     __is_cut = False
     def cut(self):
         """
         Cut-copies the selected files | Not fully implemented yet
         """
+        if not self.has_write_access(self.directory): return
         self.__is_cut = True  # TODO: DON'T FORGET TO CHANGE TERMUX CUT WHEN NEW VERSION[...]
         self.__stack_files_for_action()
 
 
     def copy(self, signum=None, frame=None):
         """
         Copies the selected files (ignore signum=None, frame=None [...]) | Not fully implemented yet
@@ -579,52 +620,67 @@
                 else                : shutil.move    (source, destination)
 
 
     def paste(self):  # TODO: ask to check if overwrite on copy
         """
         Pastes the already selected and copied/cutted files.
         """
+        if not self.has_write_access(self.directory): return
         if len(self.__temp__copied_files) == 0 or not os.path.exists(self.__temp_dir_of_copied_files): return # u never no if the user deleted anything from other file manager this is also something i haven't consider for the rest of the things and [...]
         if self.__temp_dir_of_copied_files != self.directory: self.__copy_cut ()
         else                                                : self.__duplicate()
-        self.reload()
+        self.reload(keep_search_results=True)
 
 
     def delete(self):
         """
         Deletes the selected file(s). | Not fully implemented yet
         """
+        if not self.has_write_access(self.directory): return
         if self.__count_selected == 1 and self.__clicked_file :
             # checking under __delete_file too but nvm cause i have no time right now
             if self.__clicked_file.name != '..':
                 self.__delete_file(self.__clicked_file)
                 temp_i = self.__index_of_clicked_file - 1
-                self.reload()
+                self.reload(keep_search_results=True)
                 self.__index_of_clicked_file = temp_i
                 self.__clicked_file          = self.files[temp_i]
                 self.__pre_clicked_file      = None # hmm.. sus?
                 self.select(self.__clicked_file)
         else: # if self.__count_selected > 1:  # Why do i even > 1 very sus
             if self.__clicked_file:
                 temp_i = self.__index_of_clicked_file - self.__count_selected
             else:
                 temp_i = 0 # VERY SUS BUT NVM NOW
 
             for f in self.files:
                 if f.is_selected:
                     self.__delete_file(f)
                     if self.__count_selected == 0:
-                        self.reload()
+                        self.reload(keep_search_results=True)
                         self.__index_of_clicked_file = temp_i
                         self.__clicked_file          = self.files[temp_i]
                         self.__pre_clicked_file      = None # hmm.. sus
                         self.select(self.__clicked_file)
                         break
 
 
+    def load_markers(self, path=CONFIG_PATH):
+        path = path + sep + 'MARKERS'
+        if not os.path.isfile(path) : return
+        with open(path, 'r') as file:
+            self.markers = json.load(file)
+
+
+    def save_markers(self, path=CONFIG_PATH):
+        self.markers['`'] = self.directory
+        with open(path + sep + 'MARKERS','w') as fp:
+            fp.write(json.dumps(self.markers))
+
+
     def clear_find_results(self):
         self.is_in_find_mode                = False
         self.__change_escape_event_consumed = True
         self.__temp_findname                = ''
         self.__clicked_file                 = self.files[0] # https://github.com/GiorgosXou/TUIFIManager/issues/25
         self.__index_of_clicked_file        = 0
         self.load_files(self.directory)
@@ -656,15 +712,15 @@
         elif event in self.__arrow_keys or unicurses.CTRL(event) == event:
             i = 0 if len(self.files) == 1 else 1
             self.__change_escape_event_consumed = True
             self.is_in_find_mode                = False
             self.__index_of_clicked_file        = i
             self.__clicked_file                 = self.files[i]
             return False
-        elif event in (unicurses.KEY_ENTER,10,unicurses.KEY_RESIZE,unicurses.KEY_MOUSE,unicurses.KEY_HOME): # Ignore this shit :P
+        elif event in (unicurses.KEY_ENTER,10,unicurses.KEY_RESIZE,unicurses.KEY_MOUSE,unicurses.KEY_HOME , unicurses.KEY_DC) or unicurses.keyname(event) in ('kxOUT','kxIN'): # Ignore this shit :P
             return False
         else:
             self.__temp_findname += unicurses.RCCHAR(event)
 
         self.find_file(self.__temp_findname)
         self.__set_label_text(f'SEARCH: {self.__temp_findname}')
         i = 0 if len(self.files) == 1 else 1
@@ -682,27 +738,28 @@
         self.draw()
 
 
     def find(self):
         self.__set_label_text('[INPUT]')
         self.is_in_find_mode = True
         self.escape_event_consumed = True
-        self.__temp_findname = '' # just ot make sure although it might not be need it
+        self.__temp_findname = '' # just to make sure although it might not be need it
 
 
     def __refine_path(self, path):
         path = HOME_DIR       + path[1:] if path.startswith('~') else path
         path = self.directory + path[1:] if path.startswith('.') else path 
         path = os.path.realpath(os.path.normpath(path))
         return path
 
 
     def __cmd_open(self, **args):
         if args['directory']: 
             args['directory'] = self.__refine_path(args['directory'] )
+            if os.path.isdir(args['directory']): self.__count_selected = 0
         else:
             args['directory'] = self.__clicked_file
         self.open(**args)
 
 
     def __cmd_stack(self, pattern):
         self.__temp__copied_files = []
@@ -767,64 +824,69 @@
         f.close()
 
 
     def __execute_cmd(self, cmd):
         return subprocess.Popen(cmd.split(), shell=IS_WINDOWS, stdout=subprocess.PIPE)[0]
 
 
-    marker_stack = {}
+    markers = {}
     def __perform_static_cmd_events(self, event):
         if self.__temp_findname.startswith('m'):
             self.__set_label_text('[MARKER]')
             if len(self.__temp_findname) == 2:
                 marker = unicurses.RCCHAR(event)
                 self.__set_label_text(f'[MARKER] SET TO [{marker}]')
-                self.marker_stack[marker]           = self.directory
+                self.markers[marker]                = self.directory
                 self.__temp_findname                = ''
                 self.__change_escape_event_consumed = True
                 self.is_in_command_mode             = False
             return True
         elif self.__temp_findname.startswith(('`',';')):
             self.__set_label_text('[GOTO MARKER]')
             if len(self.__temp_findname) == 2:
                 marker = unicurses.RCCHAR(event)
-                dir    = self.marker_stack.get(marker) 
+                dir    = self.markers.get(marker) 
                 if dir: 
                     self.open(dir) # scroll to file maby too?
                 else: 
                     self.__set_label_text('[MARKER] NOT FOUND')
                     self.__change_escape_event_consumed = True
                     self.is_in_command_mode             = False
             return True
         # elif Z_EXISTS and self.__temp_findname.startswith('z'): # TODO: I've wanted to call z command but it says something about permissions and stopped trying
             
         return False
 
 
+    def call_command(self,command):
+        cmd = self.command_events.get(command)
+        if not cmd: return False
+        self.__change_escape_event_consumed = True # it has to be before cmd call
+        cmd[0](self, **cmd[1])
+        self.__temp_findname    = ''
+        self.is_in_command_mode = False
+        if cmd[2]: self.__set_label_text(cmd[2])
+        return True
+
+
     is_in_command_mode = False
     def handle_command_events(self, event):
         self.__set_label_text('[COMMAND]')
         if event == 27:
             self.__change_escape_event_consumed = True
             self.is_in_command_mode = False
             self.__temp_findname    = ''
             self.__set_label_text('[NORMAL]')
-        elif event == unicurses.KEY_MOUSE:
+        elif event == unicurses.KEY_MOUSE or unicurses.keyname(event) in ('kxOUT','kxIN'):
             return False
         else:
             self.__temp_findname += unicurses.RCCHAR(event)
             self.__set_label_text(f'[COMMAND] {self.__temp_findname}')
         if self.__perform_static_cmd_events(event): return True
-        cmd = self.command_events.get(self.__temp_findname)
-        if cmd:
-            self.__change_escape_event_consumed = True # it has to be before cmd call
-            cmd[0](self, **cmd[1])
-            self.__temp_findname    = ''
-            self.is_in_command_mode = False
-            if cmd[2]: self.__set_label_text(cmd[2])
+        self.call_command(self.__temp_findname)
         return True
 
 
     def command(self):
         self.__set_label_text('[COMMAND]')
         self.is_in_command_mode    = True
         self.escape_event_consumed = True
@@ -849,28 +911,28 @@
     __temp_i                       = 0
     __illegal_filename_characters  = ('<', '>', ':',  '/', '\\', '|', '?', '*', '"')
     def handle_rename_events(self, event):  # At this momment i don't even care about optimizing anything... just kidding, you get the point, no free time | TODO: change event == ... to self.events.get(...)
         if event == unicurses.KEY_LEFT:
             if self.__temp_i != 0: self.__temp_i -= 1
         elif event == unicurses.KEY_RIGHT:
             if self.__temp_i != len(self.__temp_name): self.__temp_i += 1
-        elif unicurses.RCCHAR(event) in self.__illegal_filename_characters or event == unicurses.KEY_MOUSE:
-            return
-        elif event in (27, unicurses.KEY_ENTER, 10):
+        elif event in (27, unicurses.KEY_ENTER, 10): # TODO: clicks to act as enter
             new_path_name                       = self.directory + sep + self.__temp_name
             self.__temp_i                       = 0
             self.__change_escape_event_consumed = True
             if  event != 27 and self.__temp_name.strip() != '' and not os.path.exists(new_path_name):
                 os.rename(self.directory + sep + self.__clicked_file.name, new_path_name)
                 self.__clicked_file.name    = self.__temp_name
                 self.__clicked_file.profile = self.get_profile(new_path_name)
                 self.resort()
                 self.scroll_to_file(self.__clicked_file, True, True)
             else:
                 self.__temp_name = self.__clicked_file.name
+        elif unicurses.RCCHAR(event) in self.__illegal_filename_characters or event == unicurses.KEY_MOUSE or unicurses.keyname(event) in ('kxOUT','kxIN'):
+            return
         elif event in (unicurses.KEY_BACKSPACE, 8, 127, 263):
             if self.__temp_i != 0:
                 self.__temp_i   -= 1
                 self.__temp_name = self.__temp_name[:self.__temp_i] + self.__temp_name[self.__temp_i+1:]
             elif self.__first_pass:
                 self.__temp_name = ''
         elif event == unicurses.KEY_HOME: self.__temp_i = 0
@@ -885,14 +947,15 @@
         self.__temp_pre_name = self.__temp_name
         self.__first_pass    = False
         #if event in (unicurses.KEY_BACKSPACE, 8, 127, 263):
         #    pass
 
 
     def create_new(self,_type='folder'): # temporary implementation but nvm
+        if not self.has_write_access(self.directory): return
         i, j = '', 0
         exists = os.path.isdir if _type == 'folder' else os.path.isfile
 
         while exists(self.directory + sep + 'New ' + _type + i):
             i = f' ({str(j)})'
             j += 1
         filename = f'New {_type}{i}'
@@ -980,60 +1043,77 @@
             self.__pre_hov = tmp_hov_file
         elif self.__pre_hov:
             self.__pre_hov.draw(self.pad, color_pair_offset=self.color_pair_offset)
             self.__pre_hov = None
 
 
 
-    def __handle_mouse_events(self, event):
+    __index_of_alt_clicked_file     = None
+    __index_of_pressed_file         = None
+    def __handle_mouse_events(self, event): # I know it's a messy code ... lol
         if event != unicurses.KEY_MOUSE: return False
         in_range, id, x, y, z, bstate = self.get_mouse()
         if not IS_WINDOWS and not in_range: return True # TODO: https://github.com/GiorgosXou/TUIFIManager/issues/49
         if self.__perform_menu_selected_action(self.menu.handle_mouse_events(id, x, y, z, bstate)): return True
         if self.__x != x or self.__y != y: self.hover_mode = True #hover mode
 
-        if   not self.hover_mode and (bstate & unicurses.BUTTON4_PRESSED): self.scroll_pad(UP  )
-        elif not self.hover_mode and (bstate & unicurses.BUTTON5_PRESSED): self.scroll_pad(DOWN)
+        if   not self.hover_mode and (bstate & unicurses.BUTTON4_PRESSED): self.scroll_pad(UP   if not bstate & unicurses.BUTTON_CTRL else CTRL_UP  )
+        elif not self.hover_mode and (bstate & unicurses.BUTTON5_PRESSED): self.scroll_pad(DOWN if not bstate & unicurses.BUTTON_CTRL else CTRL_DOWN)
         elif not IS_TERMUX or not self.termux_touch_only: # because there are some times that long like presses might be translated to BUTTON1_PRESSED instead of CLICK
             self.__handle_hover_mode(y,x)
             if (bstate & unicurses.BUTTON1_RELEASED) or (bstate & unicurses.BUTTON3_RELEASED) or (unicurses.OPERATING_SYSTEM == 'Windows' and bstate & unicurses.BUTTON1_DOUBLE_CLICKED): # unicurses.OPERATING_SYSTEM == 'Windows' because issues with ncurses
                 if self.hover_mode: return True
                 self.__index_of_clicked_file, self.__clicked_file = self.get_tuifile_by_coordinates(y, x, return_enumerator=True)
                 self.__delay1 = time() - self.__delay1
                 sumed_time    = time() - self.__start_time - self.__delay1 # yeah whatever
                 if self.__clicked_file: self.__set_label_on_file_selection() # Hell, pain on my eyes, lol
 
-                if self.__mouse_btn1_pressed_file == self.__clicked_file and not bstate & unicurses.BUTTON_CTRL:
+                if self.__count_selected == 1: # for BUTTON_ALT\BUTTON_SHIFT selection
+                    self.__index_of_alt_clicked_file = self.__index_of_clicked_file
+                elif self.__clicked_file and not self.__clicked_file.name == '..':
+                    self.__set_label_text(f'[{self.__count_selected}] Files selected')
+
+                if self.__mouse_btn1_pressed_file == self.__clicked_file and not (bstate & unicurses.BUTTON_CTRL or bstate & unicurses.BUTTON_ALT or bstate & unicurses.BUTTON_SHIFT):
                     if not ((bstate & unicurses.BUTTON3_RELEASED) and self.__count_selected > 1 and self.__clicked_file and self.__clicked_file.is_selected):
                         self.menu.delete()
                         self.deselect()
                     if bstate & unicurses.BUTTON3_RELEASED:
                         self.menu.create(y,x)
                     if self.__mouse_btn1_pressed_file and not self.__mouse_btn1_pressed_file.name == '..' and not self.__mouse_btn1_pressed_file.is_selected :
                         self.select(self.__mouse_btn1_pressed_file )
                     if (((sumed_time < self.double_click_DELAY) and (bstate & unicurses.BUTTON1_RELEASED)) or bstate & unicurses.BUTTON1_DOUBLE_CLICKED) and self.__clicked_file: #and count == 2  :
                         self.open(self.__clicked_file)
                 elif self.__clicked_file and self.__mouse_btn1_pressed_file and not self.__mouse_btn1_pressed_file == self.__clicked_file: #and not self.__clicked_file.is_selected:
-                    if os.path.isdir(self.directory + sep + self.__clicked_file.name):
+                    if os.path.isdir(self.directory + sep + self.__clicked_file.name) and self.has_write_access(self.directory) and  self.has_write_access(self.directory + sep + self.__clicked_file.name):
                         for f in self.files:
                             if f.is_selected:
                                 shutil.move(self.directory + sep + f.name, self.directory + sep + self.__clicked_file.name + sep + f.name)
                         self.__pre_clicked_file = None
-                        self.reload()
+                        self.reload(keep_search_results=True)
 
                 self.__start_time = time()
             elif (bstate & unicurses.BUTTON1_PRESSED) or (bstate & unicurses.BUTTON3_PRESSED):
                 self.__delay1 = time()
-                self.__mouse_btn1_pressed_file = self.get_tuifile_by_coordinates(y, x)
+                self.__index_of_pressed_file, self.__mouse_btn1_pressed_file = self.get_tuifile_by_coordinates(y, x, return_enumerator=True)
+
+                if not bstate & unicurses.BUTTON_CTRL and self.__pre_clicked_file and self.__pre_clicked_file.is_selected:#and summ > self.double_click_DELAY:
+                    if self.__count_selected == 1:
+                        self.deselect(self.__pre_clicked_file)
+                        self.menu.delete()
+                if bstate & unicurses.BUTTON_ALT or bstate & unicurses.BUTTON_SHIFT: 
+                        self.deselect()
 
-                if not bstate & unicurses.BUTTON_CTRL and self.__pre_clicked_file and self.__pre_clicked_file.is_selected and  self.__count_selected == 1:#and summ > self.double_click_DELAY:
-                    self.deselect(self.__pre_clicked_file)
-                    self.menu.delete()
                 if self.__mouse_btn1_pressed_file and self.__mouse_btn1_pressed_file.name != '..':
                     if not self.__mouse_btn1_pressed_file.is_selected and not (bstate & unicurses.BUTTON3_PRESSED):
+                        if (bstate & unicurses.BUTTON_ALT or bstate & unicurses.BUTTON_SHIFT) and self.__index_of_alt_clicked_file:
+                            start = min(self.__index_of_alt_clicked_file, self.__index_of_pressed_file)
+                            end   = max(self.__index_of_alt_clicked_file, self.__index_of_pressed_file)
+                            for f in self.files[start:end+1]: # __index_of_alt_clicked_file acts as the index of the pre-clicked file | that "+1" it's so weird....
+                                self.select(f)
+                            # self.select(self.files[end])
                         self.select(self.__mouse_btn1_pressed_file)
                     elif bstate & unicurses.BUTTON_CTRL :#and summ > self.double_click_DELAY:
                         self.deselect(self.__mouse_btn1_pressed_file)
 
                 self.__pre_clicked_file = self.__mouse_btn1_pressed_file
         else: self.__handle_termux_touch_events(bstate, y, x)
 
@@ -1151,16 +1231,16 @@
 
     def __perform_key_left(self):
         if self.__index_of_clicked_file == 0   : return
         if self.__reset_index_of_clicked_file(): return
         self.__change_index_of_clicked_file(self.__index_of_clicked_file - 1)
 
 
-    def __perform_key_btab(self):
-        if self.__clicked_file and self.__clicked_file.name != '..':
+    def __perform_key_btab(self): # TODO: Multiple files shifttab if needed
+        if self.__clicked_file and self.__clicked_file.name != '..' and self.has_write_access(self.directory) and self.has_write_access(self.directory + sep + '..'):
             shutil.move(self.directory + sep + self.__clicked_file.name, self.directory + sep + '..' + sep + self.__clicked_file.name)
             temp_i = self.__index_of_clicked_file - 1
             self.reload()
             self.__index_of_clicked_file = temp_i
             self.__clicked_file = self.files[temp_i]
             self.select(self.__clicked_file)
 
@@ -1172,14 +1252,15 @@
 
 
     def handle_events(self, event): # wtf, ok .. works acceptably :P, TODO: REMOVE rrrrepeating code but nvm for now >:( xD  | UPDATE: WHAT HAVE I DONE, WHY SO MANY IF AND NOT JSUT A DIRCT WITH FUNCTIONS
         if event == 0 or not self.is_focused                                           : return  # https://github.com/GiorgosXou/TUIFIManager/issues/24
         if self.__is_escape_consumed(event)                                            : return
         if self.__perform_menu_selected_action(self.menu.handle_keyboard_events(event)): return
 
+        if unicurses.keyname(event) in ('kxOUT','kxIN') :return # https://github.com/GiorgosXou/TUIFIManager/issues/81
         if self.events.get(event, self.__return)() != True : return # Is this too bad of a practice? let me know
         if self.__handle_mouse_events          (event) : return
         if self.__handle_alt_down              (event) : return
         if self.__handle_termux_keyboard_events(event) : return
         if self.auto_cmd_on_typing and event != 27:
             self.command()
             self.handle_events(event)
@@ -1189,10 +1270,11 @@
 
 
             #unicurses.waddstr(self.pad, unicurses.keyname(event))
         #TODO: return event\action or none if any performed
 
 
 """
+- 2023-07-29 03:09:22 AM TODO: ctrl+i or o for navigation to last edited or exited place | Icons | Tabs | Undo redo | Sort | click-drag select multiple | windows unicurses recompile dlls | prevent errors by checking permissions | zz midle word
 - 2022-12-19 01:15:32 AM REMINDER: THE REASON WHY I USED self.position.iy INSTEAD OF self.iy IS BECAUSE CHANGING IT THAT WAY DOESN'T REDRAW THE WINDOW
 - 2022-12-21 08:23:25 PM REMINDER: What if i rename .. folder?
 """
```

### Comparing `TUIFIManager-3.0.0/TUIFIManager/__main__.py` & `TUIFIManager-3.3.1/TUIFIManager/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Entry point for TUIFIManager."""
 from __future__ import annotations
 # import sys                                                          # TESTING: UNCOMMENT TO USE LOCAL PACKAGE (./__init__.py) | https://stackoverflow.com/a/25888670/11465149
 # from os.path import dirname, abspath                                # TESTING: UNCOMMENT TO USE LOCAL PACKAGE (./__init__.py) | https://stackoverflow.com/a/25888670/11465149
 # sys.path.insert(0, dirname(dirname(abspath(__file__))))             # TESTING: UNCOMMENT TO USE LOCAL PACKAGE (./__init__.py) | https://stackoverflow.com/a/25888670/11465149
 # sys.path.append('..')                                               # TESTING WITH DAP
-# sys.path.append('/home/xou/.local/lib/python3.10/site-packages/')   # TESTING WITH DAP
+# sys.path.append('/home/xou/.local/lib/python3.11/site-packages/')   # TESTING WITH DAP | REMINDER: python3.XX
 import argparse
 import unicurses as uc
 from TUIFIManager import TUIFIManager, BEGIN_MOUSE, END_MOUSE, __version__
 
 ESCAPE_KEY = 27
 
 
@@ -62,10 +62,9 @@
 # https://stackoverflow.com/questions/11753909/clean-up-ncurses-mess-in-terminal-after-a-crash
 # https://stackoverflow.com/questions/35336532/ncurses-subwin-or-subpad-of-a-pad
 # https://stackoverflow.com/questions/31488362/why-is-dict-faster-than-if-else-in-python
 # https://stackoverflow.com/questions/18166977/cd-to-dir-after-exiting-script-system-independent-way-purely-in-python
 
 # TODO:
 """
-- Scroll sensitivity
 - TERMUX start from bottom (because most mobile screens are too big)
 """
```

### Comparing `TUIFIManager-3.0.0/TUIFIManager.egg-info/PKG-INFO` & `TUIFIManager-3.3.1/TUIFIManager.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TUIFIManager
-Version: 3.0.0
+Version: 3.3.1
 Summary: A cross-platform terminal-based termux-oriented file manager.
 Home-page: https://github.com/GiorgosXou/TUIFIManager
 Author: George Chousos
 Author-email: gxousos@gmail.com
 License: General Public License v3.0
 Project-URL: Github, https://github.com/GiorgosXou/TUIFIManager
 Keywords: file-manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-platform
@@ -40,146 +40,155 @@
 	</a>
 </p>
 </div>
 
 A cross-platform terminal-based termux-oriented file manager *(and component)*, meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses) project or as is. This project is mainly an attempt to get more attention to the [Uni-Curses](https://github.com/unicurses/unicurses) project.
 
 
-## Installation
+# ⚙️ Installation
 ```terminal
 sudo pip3 install tuifimanager --upgrade
 ```
 ```terminal
 pip3 install TUIFIManager --upgrade
 ```
 or just ^^^ if it works for you. *(eg. on termux?)*
 
 
-## Usage
+# 💥 Usage
 Run `tuifi` in your terminal to use it as is or import it in one of your [Uni-Curses](https://github.com/unicurses/unicurses) project as a component like:
 ```python
 from TUIFIManager import *
 ```
 for more details look into the `__main__.py`
 
 <img src="./Peek.gif">
 <sub>FONT: Cartograph CF</sub>
 
-## Features & Shortcuts  
-### *Current:*
+# 📦 Features 
+### • 📌 *Current:*
 - Supports most of the common mouse events so far
 - It is somewhat fully customizable?
 - Can be used as a component
 - Uses only ~30MB of RAM
 - It is pretty snappy <!-- Kinda lol -->
 - Supports [Termux](https://github.com/termux) 
 - Cross Platform 
 - and more
 
-### *Desired:*
+### • 🔮 *Desired:*
 - Undo\Redo
 - tool-tips
 - Scroll bar
 - Sixel support
 - Multiple tabs
 - Better performance
 - Effect on cutted Files
 - [Drop files into GUI apps](https://github.com/GiorgosXou/TUIFIManager/issues/21)
 
-### *Common Shortcuts\Keybindings*
+# ⌨️ Keybindings
 In `vim_mode` both normal and vim shortcuts work 
 | Normal      | vim_mode | Action                                        |
 |----         | ---- |:----                                          |
 |`SHIFT + TAB`  |   |Moves selected file to the previous directory |
 |`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory          |
 |`ALT + DOWN`   |   |Opens\Closes the "right-click menu"           |
 |`KEY_HOME`     | `H`  |Navigates to the $HOME directory              |
 |`KEY_F5`       |   |Reload\Refresh current directory              |
 |`CTRL + V`     | `p` |Pastes the Copied or Cuted files              |
 |`DEL`          | `CTRL+d`  |Deletes the selected files                    |
 |`CTRL + F`     | `i`  |Find Files *(if not auto_find_on_typing)*     |
 |`CTRL + O`     | `O`  |Open whole directory in editor                |
+|`CTRL + A`     |  |Select all files in current folder|
 |`CTRL + C`     | `yy`  |Copies the selected files                     |
 |`CTRL + K`     |   |Copies the selected files                     |
 |`CTRL + X`     | `c`  |Cuts the selected files                       |
 |`CTRL + R`     | `r` |Rename selected file                          | 
+|`CTRL + T`     | | Toggle hidden files|
 |`CTRL + N`     | `W` |Create new folder                             |
 |`CTRL + W`     | `w` |Create new file                               |
 |`ARROW KEYS`   | `l` `k` `j` `h`  |Navigates files                               |
 |`KEY_ENTER`    | `K`|Opens files                                   |
 |`CTRL + E`     | `e` |Exit with `cd`                                  |
 |`ESCAPE`       |   |Exit                                          |
 
+**(*TIP:** 🐁 use `ALT + CLICK` for multiple mouse selection if `SHIFT` not working)*
 
-### *TERMUX only Shortcuts\Keybindings*
+***TERMUX only Shortcuts\Keybindings***
 | Shortcut    | Action                                                                         |
 |----         |:----                                                                           |
 |`CTRL + DOWN`| Goes in&out of select-mode while also automatically copies the selected file(s)|
 |`CTRL + LEFT`| Goes out of select-mode while also cuts the seleccted file(s)                  |
 |`CTRL + END` | Goes out of select-mode while also deleting the selected file(s)               |
 |`CTRL + UP`  | Same as `CTRL + V`, Pastes the Copied or Cuted files                           |
 |`END`        | Deletes selected files                                                         |
 
 
-### *Default & Custom - Commands*
-To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing`-env variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
+# 👨‍💻 Commands
+**(Default & Custom Comands)** - To perform a command under the normal-mode, you first have to press the space-bar and then type the command. Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can be found under the `~/.config/tuifi/cmds.conf` where you can add your custom ones too:**
 
 | Cmd | Type | Attributes | Label Comment|
 |---|---|---|---|
 |`gt` | open | 'directory':'~/.config/tuifi'           | - tuifi -|
 |`gh` | open | 'directory':'~/'                        | - Home -|
 |`owv` | open | 'directory':None,'\_with':'vim'         |Opened With Vim|
 |`yat` | copy | 'pattern':'.+\.txt'                     ||
 |`yy` | copy | 'pattern':None                          ||
 
 There are also some "static" ones like the `m`+character which marks the current directory into the character, so you can navigate back to it by using \` or `;`+that_character 
 
 
-# Documentation
+# 📜 Documentation
 <sub>Work in progress 🛠️🏗 ...</sub>
 
 
-## Customization 
-***How do I enable vim_mode?***
+# 💭 Customization 
+*How do I enable vim_mode?*
 > Set `tuifi_vim_mode` enviroment variable to `True`
 
-***How do I change the default keys (besides commands)?***
+*How do I change the default keys (besides commands)?*
 > This is not possible right now althought you could play around with the content of `toggle_vim_mode` function under `__init__.py`
 
-***How do I set the default editor?***
+*How do I set the default editor?*
 > Set `tuifi_default_editor` enviroment variable to `vim` or whatever you prefer
 
-***How do I disable the auto-find-mode?***
+*How do I disable the auto-find-mode?*
 > You can just set `tuifi_auto_find_on_typing` enviroment variable to `False`
 
-***How do I change the default configuration path?***
+*How do I change the scroll sensitivity?*
+> You can set either or both `tuifi_scroll_sensitivity`, `tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number of characters per scroll action *(they default to 1 and 7)*
+
+How do I change the number of visible lines of filenames that are visible?
+> You can set how mnay lines you want using `tuifi_visible_filename_lines` *(Defaults to 4)*
+
+*How do I change the default configuration path?*
 > Set `tuifi_config_path` enviroment variable to whatever you prefer most
 
-***How do I toggle hidden files/folders?***
+*How do I toggle hidden files/folders?*
 > You can either `CTRL + T` or set `tuifi_show_hidden` enviroment variable to `True`
 
-***How do I change the default colors?***
+*How do I change the default colors?*
 > [look here for more informations](https://github.com/GiorgosXou/TUIFIManager/issues/38)
 
 
-# Donation
+# 💗 Donation
 I do really need money to survive, I have no job, living in a basement, making things for free, because I love to.
 - [***Paypal Address***](https://www.paypal.com/donate/?hosted_button_id=QNQN23M55EJVS)
 - ***Monero Address:*** `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
 
 <div align="center">
 <img src='./TUIFI.png'>
 </div>
 
 
-# Special thanks to
+# 🫶 Special thanks to
 - [Bryan Lunduke for this article](https://lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the)
 - [Brodie Robertson for this video](https://youtu.be/9laxdMKTZLA)
 - [r/linux community for their comments](https://www.reddit.com/r/linux/comments/zzf5rx)
 - [r/cyberDeck community for their comments](https://www.reddit.com/r/cyberDeck/comments/zttur0)
 - [r/commandline community for their comments](https://www.reddit.com/r/commandline/comments/zt30v9)
 
-# Help
+# 🕳️ Help
 Any Idea with this issue https://github.com/unicurses/unicurses/issues/21 ?
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TUIFIManager Version: 3.0.0 Summary: A cross-
+Metadata-Version: 2.1 Name: TUIFIManager Version: 3.3.1 Summary: A cross-
 platform terminal-based termux-oriented file manager. Home-page: https://
 github.com/GiorgosXou/TUIFIManager Author: George Chousos Author-email:
 gxousos@gmail.com License: General Public License v3.0 Project-URL: Github,
 https://github.com/GiorgosXou/TUIFIManager Keywords: file-
 manager,terminal,tui,ncurses,pdcurses,uni-curses,termux,vim,vim-motions,cross-
 platform Platform: unix Platform: linux Platform: osx Platform: cygwin
 Platform: windows Classifier: Intended Audience :: Developers Classifier:
@@ -17,78 +17,86 @@
             [https://img.shields.io/github/last-commit/GiorgosXou/
 TUIFIManager?color=%4dc71f&label=Last%20Commit&logo=github&style=flat-square]
               [https://img.shields.io/github/license/GiorgosXou/
             TUIFIManager?label=License&logo=GNU&style=flat-square]
 A cross-platform terminal-based termux-oriented file manager *(and component)*,
 meant to be used with a [Uni-Curses](https://github.com/unicurses/unicurses)
 project or as is. This project is mainly an attempt to get more attention to
-the [Uni-Curses](https://github.com/unicurses/unicurses) project. ##
+the [Uni-Curses](https://github.com/unicurses/unicurses) project. # âï¸
 Installation ```terminal sudo pip3 install tuifimanager --upgrade ```
 ```terminal pip3 install TUIFIManager --upgrade ``` or just ^^^ if it works for
-you. *(eg. on termux?)* ## Usage Run `tuifi` in your terminal to use it as is
-or import it in one of your [Uni-Curses](https://github.com/unicurses/
+you. *(eg. on termux?)* # ð¥ Usage Run `tuifi` in your terminal to use it as
+is or import it in one of your [Uni-Curses](https://github.com/unicurses/
 unicurses) project as a component like: ```python from TUIFIManager import *
 ``` for more details look into the `__main__.py` [./Peek.gif] FONT: Cartograph
-CF ## Features & Shortcuts ### *Current:* - Supports most of the common mouse
+CF # ð¦ Features ### â¢ ð *Current:* - Supports most of the common mouse
 events so far - It is somewhat fully customizable? - Can be used as a component
 - Uses only ~30MB of RAM - It is pretty snappy  - Supports [Termux](https://
-github.com/termux) - Cross Platform - and more ### *Desired:* - Undo\Redo -
-tool-tips - Scroll bar - Sixel support - Multiple tabs - Better performance -
-Effect on cutted Files - [Drop files into GUI apps](https://github.com/
-GiorgosXou/TUIFIManager/issues/21) ### *Common Shortcuts\Keybindings* In
+github.com/termux) - Cross Platform - and more ### â¢ ð® *Desired:* -
+Undo\Redo - tool-tips - Scroll bar - Sixel support - Multiple tabs - Better
+performance - Effect on cutted Files - [Drop files into GUI apps](https://
+github.com/GiorgosXou/TUIFIManager/issues/21) # â¨ï¸ Keybindings In
 `vim_mode` both normal and vim shortcuts work | Normal | vim_mode | Action | |-
 --- | ---- |:---- | |`SHIFT + TAB` | |Moves selected file to the previous
 directory | |`KEY_BACKSPACE`| `J` |Opens\Goes to the previous directory | |`ALT
 + DOWN` | |Opens\Closes the "right-click menu" | |`KEY_HOME` | `H` |Navigates
 to the $HOME directory | |`KEY_F5` | |Reload\Refresh current directory | |`CTRL
 + V` | `p` |Pastes the Copied or Cuted files | |`DEL` | `CTRL+d` |Deletes the
 selected files | |`CTRL + F` | `i` |Find Files *(if not auto_find_on_typing)* |
-|`CTRL + O` | `O` |Open whole directory in editor | |`CTRL + C` | `yy` |Copies
-the selected files | |`CTRL + K` | |Copies the selected files | |`CTRL + X` |
-`c` |Cuts the selected files | |`CTRL + R` | `r` |Rename selected file | |`CTRL
-+ N` | `W` |Create new folder | |`CTRL + W` | `w` |Create new file | |`ARROW
-KEYS` | `l` `k` `j` `h` |Navigates files | |`KEY_ENTER` | `K`|Opens files |
-|`CTRL + E` | `e` |Exit with `cd` | |`ESCAPE` | |Exit | ### *TERMUX only
-Shortcuts\Keybindings* | Shortcut | Action | |---- |:---- | |`CTRL + DOWN`|
-Goes in&out of select-mode while also automatically copies the selected file
-(s)| |`CTRL + LEFT`| Goes out of select-mode while also cuts the seleccted file
-(s) | |`CTRL + END` | Goes out of select-mode while also deleting the selected
-file(s) | |`CTRL + UP` | Same as `CTRL + V`, Pastes the Copied or Cuted files |
-|`END` | Deletes selected files | ### *Default & Custom - Commands* To perform
-a command under the normal-mode, you first have to press the space-bar and then
-type the command. Alternatively, use `vim_mode` or enable the
-`tuifi_auto_command_on_typing`-env variable *(notice: it disables
-`tuifi_auto_find_on_typing`)*. **The default commands can be seen below and can
-be found under the `~/.config/tuifi/cmds.conf` where you can add your custom
-ones too:** | Cmd | Type | Attributes | Label Comment| |---|---|---|---| |`gt`
-| open | 'directory':'~/.config/tuifi' | - tuifi -| |`gh` | open | 'directory':
-'~/' | - Home -| |`owv` | open | 'directory':None,'\_with':'vim' |Opened With
-Vim| |`yat` | copy | 'pattern':'.+\.txt' || |`yy` | copy | 'pattern':None ||
-There are also some "static" ones like the `m`+character which marks the
-current directory into the character, so you can navigate back to it by using
-\` or `;`+that_character # Documentation Work in progress ð ï¸ð ... ##
-Customization ***How do I enable vim_mode?*** > Set `tuifi_vim_mode` enviroment
-variable to `True` ***How do I change the default keys (besides commands)?*** >
-This is not possible right now althought you could play around with the content
-of `toggle_vim_mode` function under `__init__.py` ***How do I set the default
-editor?*** > Set `tuifi_default_editor` enviroment variable to `vim` or
-whatever you prefer ***How do I disable the auto-find-mode?*** > You can just
-set `tuifi_auto_find_on_typing` enviroment variable to `False` ***How do I
-change the default configuration path?*** > Set `tuifi_config_path` enviroment
-variable to whatever you prefer most ***How do I toggle hidden files/
-folders?*** > You can either `CTRL + T` or set `tuifi_show_hidden` enviroment
-variable to `True` ***How do I change the default colors?*** > [look here for
-more informations](https://github.com/GiorgosXou/TUIFIManager/issues/38) #
+|`CTRL + O` | `O` |Open whole directory in editor | |`CTRL + A` | |Select all
+files in current folder| |`CTRL + C` | `yy` |Copies the selected files | |`CTRL
++ K` | |Copies the selected files | |`CTRL + X` | `c` |Cuts the selected files
+| |`CTRL + R` | `r` |Rename selected file | |`CTRL + T` | | Toggle hidden
+files| |`CTRL + N` | `W` |Create new folder | |`CTRL + W` | `w` |Create new
+file | |`ARROW KEYS` | `l` `k` `j` `h` |Navigates files | |`KEY_ENTER` |
+`K`|Opens files | |`CTRL + E` | `e` |Exit with `cd` | |`ESCAPE` | |Exit | **
+(*TIP:** ð use `ALT + CLICK` for multiple mouse selection if `SHIFT` not
+working)* ***TERMUX only Shortcuts\Keybindings*** | Shortcut | Action | |---
+- |:---- | |`CTRL + DOWN`| Goes in&out of select-mode while also automatically
+copies the selected file(s)| |`CTRL + LEFT`| Goes out of select-mode while also
+cuts the seleccted file(s) | |`CTRL + END` | Goes out of select-mode while also
+deleting the selected file(s) | |`CTRL + UP` | Same as `CTRL + V`, Pastes the
+Copied or Cuted files | |`END` | Deletes selected files | # ð¨âð»
+Commands **(Default & Custom Comands)** - To perform a command under the
+normal-mode, you first have to press the space-bar and then type the command.
+Alternatively, use `vim_mode` or enable the `tuifi_auto_command_on_typing` env-
+variable *(notice: it disables `tuifi_auto_find_on_typing`)*. **The default
+commands can be seen below and can be found under the `~/.config/tuifi/
+cmds.conf` where you can add your custom ones too:** | Cmd | Type | Attributes
+| Label Comment| |---|---|---|---| |`gt` | open | 'directory':'~/.config/tuifi'
+| - tuifi -| |`gh` | open | 'directory':'~/' | - Home -| |`owv` | open |
+'directory':None,'\_with':'vim' |Opened With Vim| |`yat` | copy | 'pattern':
+'.+\.txt' || |`yy` | copy | 'pattern':None || There are also some "static" ones
+like the `m`+character which marks the current directory into the character, so
+you can navigate back to it by using \` or `;`+that_character # ð
+Documentation Work in progress ð ï¸ð ... # ð­ Customization *How do I
+enable vim_mode?* > Set `tuifi_vim_mode` enviroment variable to `True` *How do
+I change the default keys (besides commands)?* > This is not possible right now
+althought you could play around with the content of `toggle_vim_mode` function
+under `__init__.py` *How do I set the default editor?* > Set
+`tuifi_default_editor` enviroment variable to `vim` or whatever you prefer *How
+do I disable the auto-find-mode?* > You can just set
+`tuifi_auto_find_on_typing` enviroment variable to `False` *How do I change the
+scroll sensitivity?* > You can set either or both `tuifi_scroll_sensitivity`,
+`tuifi_ctrl_scroll_sensitivity` enviromental variables, to the disered number
+of characters per scroll action *(they default to 1 and 7)* How do I change the
+number of visible lines of filenames that are visible? > You can set how mnay
+lines you want using `tuifi_visible_filename_lines` *(Defaults to 4)* *How do I
+change the default configuration path?* > Set `tuifi_config_path` enviroment
+variable to whatever you prefer most *How do I toggle hidden files/folders?* >
+You can either `CTRL + T` or set `tuifi_show_hidden` enviroment variable to
+`True` *How do I change the default colors?* > [look here for more
+informations](https://github.com/GiorgosXou/TUIFIManager/issues/38) # ð
 Donation I do really need money to survive, I have no job, living in a
 basement, making things for free, because I love to. - [***Paypal Address***]
 (https://www.paypal.com/donate/?hosted_button_id=QNQN23M55EJVS) - ***Monero
 Address:***
 `897ehhSQJQpGF7tYDhQM51jiX7nnHmzuYAW4q8JGwJxu8JKXvaK6AivCzatuJxnifjZ2qy98ks2g2PhmTaYCMMta2Ga2LJx`
                                  [./TUIFI.png]
-# Special thanks to - [Bryan Lunduke for this article](https://
+# ð«¶ Special thanks to - [Bryan Lunduke for this article](https://
 lunduke.substack.com/p/tuifi-manager-a-file-manager-in-the) - [Brodie Robertson
 for this video](https://youtu.be/9laxdMKTZLA) - [r/linux community for their
 comments](https://www.reddit.com/r/linux/comments/zzf5rx) - [r/cyberDeck
 community for their comments](https://www.reddit.com/r/cyberDeck/comments/
 zttur0) - [r/commandline community for their comments](https://www.reddit.com/
-r/commandline/comments/zt30v9) # Help Any Idea with this issue https://
+r/commandline/comments/zt30v9) # ð³ï¸ Help Any Idea with this issue https://
 github.com/unicurses/unicurses/issues/21 ?
```

### Comparing `TUIFIManager-3.0.0/pyproject.toml` & `TUIFIManager-3.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TUIFIManager"
-version = "3.0.0"
+version = "3.3.1"
 
 description = "A cross-platform terminal-based termux-oriented file manager."
 requires-python = ">=3.8"
 readme = "README.md"
 
 dependencies = [
     "uni-curses >= 2.1.3",
```

### Comparing `TUIFIManager-3.0.0/setup.cfg` & `TUIFIManager-3.3.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = TUIFIManager
-version = 3.0.0
+version = 3.3.1
 description = A cross-platform terminal-based termux-oriented file manager
 long_description = file: docs/README.md
 long_description_content_type = text/markdown
 author = George Chousos
 author_email = gxousos@gmail.com
 keywords = file-manager, terminal, tui, ncurses, pdcurses, uni-curses, termux, vim, vim-motions, cross-platform
 license = GPL-3.0
```

