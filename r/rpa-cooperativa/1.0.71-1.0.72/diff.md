# Comparing `tmp/rpa_cooperativa-1.0.71.tar.gz` & `tmp/rpa_cooperativa-1.0.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_cooperativa-1.0.71.tar", last modified: Tue Jul 25 11:34:03 2023, max compression
+gzip compressed data, was "rpa_cooperativa-1.0.72.tar", last modified: Tue Aug  8 18:13:59 2023, max compression
```

## Comparing `rpa_cooperativa-1.0.71.tar` & `rpa_cooperativa-1.0.72.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 11:34:03.391317 rpa_cooperativa-1.0.71/
--rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.71/LICENSE
--rw-rw-rw-   0        0        0     6969 2023-07-25 11:34:03.388395 rpa_cooperativa-1.0.71/PKG-INFO
--rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.71/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 11:34:03.271074 rpa_cooperativa-1.0.71/rpa_coop/
--rw-rw-rw-   0        0        0      613 2023-07-21 18:26:52.000000 rpa_cooperativa-1.0.71/rpa_coop/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-25 11:34:03.353936 rpa_cooperativa-1.0.71/rpa_coop/img/
--rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.71/rpa_coop/img/hash
--rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.71/rpa_coop/img/relatorios_azul.PNG
--rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.71/rpa_coop/img/relatorios_verde.PNG
--rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.71/rpa_coop/img/sacg_branco.PNG
--rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.71/rpa_coop/img/sagc_verde.PNG
--rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.71/rpa_coop/img/siac_amarelo.PNG
--rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.71/rpa_coop/img/siac_branco.PNG
--rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.71/rpa_coop/img/siat_amarelo.PNG
--rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.71/rpa_coop/img/siat_branco.PNG
--rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.71/rpa_coop/img/transacional_azul.PNG
--rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.71/rpa_coop/img/transacional_verde.PNG
--rw-rw-rw-   0        0        0   104249 2023-07-25 11:32:18.000000 rpa_cooperativa-1.0.71/rpa_coop/rpa_coop.py
-drwxrwxrwx   0        0        0        0 2023-07-25 11:34:03.383319 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/
--rw-rw-rw-   0        0        0     6969 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      631 2023-07-25 11:34:03.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      581 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-25 11:34:02.000000 rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 11:34:03.391317 rpa_cooperativa-1.0.71/setup.cfg
--rw-rw-rw-   0        0        0     2350 2023-07-25 11:33:12.000000 rpa_cooperativa-1.0.71/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:13:59.140333 rpa_cooperativa-1.0.72/
+-rw-rw-rw-   0        0        0     1115 2023-03-09 01:05:15.000000 rpa_cooperativa-1.0.72/LICENSE
+-rw-rw-rw-   0        0        0     6969 2023-08-08 18:13:59.136774 rpa_cooperativa-1.0.72/PKG-INFO
+-rw-rw-rw-   0        0        0     5824 2023-07-13 15:55:54.000000 rpa_cooperativa-1.0.72/README.md
+drwxrwxrwx   0        0        0        0 2023-08-08 18:13:58.989992 rpa_cooperativa-1.0.72/rpa_coop/
+-rw-rw-rw-   0        0        0      613 2023-07-21 18:26:52.000000 rpa_cooperativa-1.0.72/rpa_coop/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:13:59.081748 rpa_cooperativa-1.0.72/rpa_coop/img/
+-rw-rw-rw-   0        0        0      140 2023-03-16 01:30:18.000000 rpa_cooperativa-1.0.72/rpa_coop/img/hash
+-rw-rw-rw-   0        0        0     2980 2023-03-09 16:48:20.000000 rpa_cooperativa-1.0.72/rpa_coop/img/relatorios_azul.PNG
+-rw-rw-rw-   0        0        0     3576 2023-03-09 16:47:53.000000 rpa_cooperativa-1.0.72/rpa_coop/img/relatorios_verde.PNG
+-rw-rw-rw-   0        0        0      379 2023-05-19 19:03:26.000000 rpa_cooperativa-1.0.72/rpa_coop/img/sacg_branco.PNG
+-rw-rw-rw-   0        0        0      463 2023-06-01 13:04:34.000000 rpa_cooperativa-1.0.72/rpa_coop/img/sagc_verde.PNG
+-rw-rw-rw-   0        0        0      384 2023-02-28 19:53:19.000000 rpa_cooperativa-1.0.72/rpa_coop/img/siac_amarelo.PNG
+-rw-rw-rw-   0        0        0      370 2023-04-17 14:08:47.000000 rpa_cooperativa-1.0.72/rpa_coop/img/siac_branco.PNG
+-rw-rw-rw-   0        0        0      364 2023-04-17 14:10:18.000000 rpa_cooperativa-1.0.72/rpa_coop/img/siat_amarelo.PNG
+-rw-rw-rw-   0        0        0      349 2023-02-28 19:53:39.000000 rpa_cooperativa-1.0.72/rpa_coop/img/siat_branco.PNG
+-rw-rw-rw-   0        0        0     6079 2023-03-09 16:47:31.000000 rpa_cooperativa-1.0.72/rpa_coop/img/transacional_azul.PNG
+-rw-rw-rw-   0        0        0     6652 2023-03-09 16:46:38.000000 rpa_cooperativa-1.0.72/rpa_coop/img/transacional_verde.PNG
+-rw-rw-rw-   0        0        0   100759 2023-08-08 18:07:56.000000 rpa_cooperativa-1.0.72/rpa_coop/rpa_coop.py
+drwxrwxrwx   0        0        0        0 2023-08-08 18:13:59.128323 rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/
+-rw-rw-rw-   0        0        0     6969 2023-08-08 18:13:58.000000 rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      631 2023-08-08 18:13:58.000000 rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-08 18:13:58.000000 rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-08 18:13:58.000000 rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      576 2023-08-08 18:13:58.000000 rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-08 18:13:58.000000 rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-08 18:13:59.141331 rpa_cooperativa-1.0.72/setup.cfg
+-rw-rw-rw-   0        0        0     2346 2023-08-08 18:13:46.000000 rpa_cooperativa-1.0.72/setup.py
```

### Comparing `rpa_cooperativa-1.0.71/LICENSE` & `rpa_cooperativa-1.0.72/LICENSE`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.71/PKG-INFO` & `rpa_cooperativa-1.0.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa_cooperativa
-Version: 1.0.71
+Version: 1.0.72
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.71/README.md` & `rpa_cooperativa-1.0.72/README.md`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.71/rpa_coop/__init__.py` & `rpa_cooperativa-1.0.72/rpa_coop/__init__.py`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.71/rpa_coop/img/relatorios_azul.PNG` & `rpa_cooperativa-1.0.72/rpa_coop/img/relatorios_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.71/rpa_coop/img/relatorios_verde.PNG` & `rpa_cooperativa-1.0.72/rpa_coop/img/relatorios_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.71/rpa_coop/img/transacional_azul.PNG` & `rpa_cooperativa-1.0.72/rpa_coop/img/transacional_azul.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.71/rpa_coop/img/transacional_verde.PNG` & `rpa_cooperativa-1.0.72/rpa_coop/img/transacional_verde.PNG`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.71/rpa_coop/rpa_coop.py` & `rpa_cooperativa-1.0.72/rpa_coop/rpa_coop.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 import pandas as pd
 from sqlalchemy import create_engine
 from urllib.request import urlretrieve
 import urllib.parse
 import site
 import ssl
 ssl._create_default_https_context = ssl._create_unverified_context
+from ahk import AHK
+# ahk = AHK(executable_path='C:\\Program Files\\AutoHotkey\\AutoHotkey.exe')
+ahk = AHK()
+
 
 user_site_packages = site.getusersitepackages()
 user_site_packages = user_site_packages.replace('Roaming', 'Local\\Programs').replace('site-packages','Lib\\site-packages')
 
 
 def gerador_pwd(palavra_chave:str, select_atributo='usuario', retorna_atributo=True, retorna_dicionario=False ,print_atributo=False, mostrar_todas_credenciais=False, return_conex_fluid = False):
     '''
@@ -1195,269 +1199,152 @@
     def __init__(self):
         self.usuario_acc = str(gerador_pwd('acc', 'usuario'))
         self.senha_acc = str(gerador_pwd('acc', 'senha'))
         self.janela_sacg = 'janela'
         self.janela_siat = 'janela'
         self.janela_siac = 'janela'
 
-    
-    def open_acclient_old(self, siat_siac_sacg, transacional=True):
-        # Open AC Client
-        try:
-            self.p.sleep(1)
-            os.system('taskkill /F /FI "WindowTitle eq C:\\ProgramData\\ac\\teoff-exe*" /T')
-        except Exception:
-            pass
-        
-        try:
-            os.system('taskkill /F /IM javaw_ac.exe')
-            self.p.sleep(1)
-        except Exception:
-            pass
-        
-        user_acc = self.usuario_acc
-        pw_acclient = self.senha_acc
-         
-        self.subprocess.Popen("C:\\Users\\Public\\Desktop\\AC Client.lnk",shell=True)
-        self.p.sleep(15)
-        
-
-        # pegar retangulo da janela pelo titulo parcial
-        janela = self.p.getWindowsWithTitle('Aplicações Core - Login')[0]
-        janela.activate()
-
-        self.p.press('tab')
-        self.p.press('tab')
-        # digitar usuario
-        self.p.typewrite(user_acc)
-        self.p.press('tab')
-        self.p.typewrite(pw_acclient)
-        self.p.press('tab')
-        self.p.press('enter')
-        print('passou do login')
-
-        self.p.sleep(12)
-        # pegar retangulo da janela pelo titulo parcial
-        janela = self.p.getWindowsWithTitle('AC Client')[0]
-        janela.activate()
-        janela.left
-        self.p.sleep(1)
-        self.p.press('pgdn')
-
-        # Selecionar o MENU SIAT
-        posicao = 0
-        pasta_imagens = user_site_packages +  '\\rpa_coop\\img\\'
-                   
-        
-        if 'SACG' in str(siat_siac_sacg).upper():
-            try:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, grayscale=True)
-            except:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png', confidence=0.9, grayscale=True)
-        elif 'SIAT' in str(siat_siac_sacg).upper():
-            try:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png', confidence=0.9, grayscale=True)
-            except:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png', confidence=0.9, grayscale=True)
-        elif 'SIAC' in str(siat_siac_sacg).upper():
-            try:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png', confidence=0.9, grayscale=True)
-            except:
-                posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png', confidence=0.9, grayscale=True)
-        time.sleep(1)
-        self.p.click(posicao)
-        print('selecionou o menu: siat, siac, sacg')
-        time.sleep(3)
-        
-        if transacional:
-            self.p.moveTo(janela.left + 48, janela.top + 165)
-            time.sleep(1)
-            self.p.doubleClick()
-        else:
-            self.p.moveTo(janela.left + 48, janela.top + 245)
-            self.p.doubleClick()
-        time.sleep(7)
-        
-           
+               
     def open_acclient(self, siat_siac_sacg: str | list, transacional=True):
         ''' acc.open_acclient('siac') \n
-         acc.open_acclient(['siat', 'sacg'])'''
+        acc.open_acclient(['siat', 'sacg'])'''
+
         opcoes = []
-        if isinstance(siat_siac_sacg, str):
-            opcoes.append(siat_siac_sacg)
-        else:
-            opcoes = siat_siac_sacg
+        if isinstance(siat_siac_sacg, str): opcoes.append(siat_siac_sacg)
+        else: opcoes = siat_siac_sacg
             
-        # Open AC Client
-        try:
-            self.p.sleep(1)
-            os.system('taskkill /F /FI "WindowTitle eq C:\\ProgramData\\ac\\teoff-exe*" /T')
-        except Exception:
-            pass
+        try: os.system('taskkill /F /FI "WindowTitle eq C:\\ProgramData\\ac\\teoff-exe*" /T')
+        except Exception: pass
         
-        try:
-            os.system('taskkill /F /IM javaw_ac.exe')
-            self.p.sleep(1)
-        except Exception:
-            pass
+        try: os.system('taskkill /F /IM javaw_ac.exe')
+        except Exception: pass
         
         user_acc = self.usuario_acc
         pw_acclient = self.senha_acc
          
         self.subprocess.Popen("C:\\Users\\Public\\Desktop\\AC Client.lnk",shell=True)
-        time.sleep(5)
         
-
-        # pegar retangulo da janela pelo titulo parcial
-        espera = 0
-        while espera < 26:
-            if espera == 25:
-                raise Exception('Nao conseguiu clicar na janela, Login ACC')
-            try:
-                self.janela_login = self.p.getWindowsWithTitle('Aplicações Core - Login')[0]
-                self.janela_login.activate()
-                espera = 0
-                break
-            except:
-                time.sleep(2)
-                espera = espera + 1
-           
-                
-        self.p.press('tab')
+        # esperar janela de login
+        win_login = ahk.win_wait(title=r'Aplicações Core - Login', timeout=20, title_match_mode=2)
+        win_login.activate()
+        win_login.to_top() 
+        self.p.hotkey('shift','tab')
+        ahk.type(user_acc)
         self.p.press('tab')
-        # digitar usuario
-        self.p.typewrite(user_acc)
-        self.p.press('tab')
-        self.p.typewrite(pw_acclient)
+        ahk.type(pw_acclient)
         self.p.press('tab')
         self.p.press('enter')
         print('passou do login')
 
-        time.sleep(3)
-        # pegar retangulo da janela pelo titulo parcial
-        espera = 0
-        while espera < 26:
-            if espera == 25:
-                raise Exception('Nao conseguiu clicar na janela, Menu ACC')
-            try:
-                self.janela = self.p.getWindowsWithTitle('AC Client')[0]
-                self.janela.activate()
-                espera = 0
-                break
-            except:
-                time.sleep(2)
-                espera = espera + 1
-
+        # esperar janela de menu, após o login
+        self.win_menu = ahk.win_wait(title=r'AC Client', timeout=20, title_match_mode=2)
+        self.win_menu.set_title('MENU_ACC')
+        self.win_menu.activate()
+        self.win_menu.to_top() 
         self.p.sleep(1)
         self.p.press('pgdn')
+        self.janela_menu_acc = self.win_menu.get_position()
+        
+        self.win_sacg = None
+        self.win_siat = None
+        self.win_siac = None
 
         # Selecionar o MENU SIAT
         posicao = 0
         pasta_imagens = user_site_packages +  '\\rpa_coop\\img\\'
         
-                   
-        
+        # clica no botao transacional ou relatório
         if transacional:
-            self.p.moveTo(self.janela.left + 48, self.janela.top + 165)
+            self.p.moveTo(self.janela_menu_acc.x + 48, self.janela_menu_acc.y + 165)
             time.sleep(1)
             self.p.click()
-            # self.p.doubleClick()
         else:
-            self.p.moveTo(self.janela.left + 48, self.janela.top + 245)
+            self.p.moveTo(self.janela_menu_acc.x + 48, self.janela_menu_acc.y + 245)
             self.p.click()
-            # self.p.doubleClick()
         time.sleep(3)
             
-   
-
-        num_menu = 0
         self.janelas = []
-        # self.janela_sacg = self.janela
-        # self.janela_siat = self.janela
-        # self.janela_siac = self.janela
-        
         opcoes = [x.upper() for x in opcoes]
+        controle = 1
+        self.win_principal = None
         
         for menu in opcoes:
-            time.sleep(2)
-            # espera = 0
-            # while espera < 26:
-            #     if espera == 25:
-            #         raise Exception('Nao conseguiu clicar na janela, Menu ACC')
-            #     try:
-            #         self.janela = self.p.getWindowsWithTitle('AC Client')[0]
-            #         self.janela.activate()
-            #         espera = 0
-            #         break
-            #     except:
-            #         time.sleep(2)
-            #         espera = espera + 1
-                
+            time.sleep(2)   
             self.p.press('pgdn')
             time.sleep(1)
             
             if menu == 'SACG':
-                # Abrir SACG
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_branco.png', confidence=0.9, minSearchTime=2.0)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'sacg_verde.png', confidence=0.9, minSearchTime=2.0)
                 print('posicao do click sacg', posicao)
                 self.p.doubleClick(posicao)
-                time.sleep(7)
-                self.janela_sacg = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
-                self.janelas.append(self.janela_sacg)
+                self.win_sacg = ahk.win_wait(title=r'teoff', timeout=20, title_match_mode=2)
+                self.win_sacg.set_title('SACG')
+                self.win_sacg.activate()
+                self.win_sacg.to_top() 
+                if controle == 1: self.win_principal = self.win_sacg
                 print('clicou no menu: sacg')
-                time.sleep(3)
-                # self.janela_sacg.activate()
+                self.win_menu.activate()
+                self.win_menu.to_top()
             elif menu == 'SIAT':
-                # Abrir SIAT
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siat_amarelo.png', confidence=0.9, minSearchTime=2.0)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siat_branco.png', confidence=0.9, minSearchTime=2.0)
                 print('posicao do click siat', posicao)
                 self.p.doubleClick(posicao)
-                time.sleep(7)
-                self.janela_siat = self.p.getWindowsWithTitle('teoff-exe')[num_menu] 
-                self.janelas.append(self.janela_siat)
+                self.win_siat = ahk.win_wait(title=r'teoff', timeout=20, title_match_mode=2)
+                self.win_siat.set_title('SIAT')
+                self.win_siat.activate()
+                self.win_siat.to_top() 
+                if controle == 1: self.win_principal = self.win_siat
                 print('clicou no menu: siat')
-                time.sleep(3)
-                # self.janela_siat.activate()
+                self.win_menu.activate()
+                self.win_menu.to_top()
             elif menu == 'SIAC':
                 try:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siac_branco.png', confidence=0.9, minSearchTime=2.0)
                 except:
                     posicao = self.p.locateOnScreen(pasta_imagens + 'siac_amarelo.png', confidence=0.9, minSearchTime=2.0)
                 print('posicao do click siac', posicao)
                 self.p.doubleClick(posicao)
-                time.sleep(7)
-                self.janela_siac = self.p.getWindowsWithTitle('teoff-exe')[num_menu]
-                self.janelas.append(self.janela_siac)
+                self.win_siac = ahk.win_wait(title=r'teoff', timeout=20, title_match_mode=2)
+                self.win_siac.set_title('SIAC')
+                self.win_siac.activate()
+                self.win_siac.to_top() 
+                if controle == 1: self.win_principal = self.win_siac
                 print('clicou no menu: siac')
-                time.sleep(3)
-                # self.janela_siac.activate()
+                self.win_menu.activate()
+                self.win_menu.to_top()
             time.sleep(1)
-        return self.janelas
+            controle = controle + 1
+        self.win_principal.activate()
+        self.win_principal.to_top() 
+        time.sleep(1)
+        return self.win_menu, self.win_siat, self.win_siac, self.win_sacg
 
-             
+               
     def select_menu_letras(self, letras, nome_janela=None):
         '''acc.select_menu_letras(letras) \n
          acc.select_menu_letras(letras, nome_janela='sacg')'''
         self.p.sleep(1)
         nome_janela = str(nome_janela).upper()
         if nome_janela == 'SIAT':
-            janela = self.janela_siat
+            janela = self.win_siat
         elif nome_janela == 'SIAC':
-            janela = self.janela_siac
+            janela = self.win_siac
         elif nome_janela == 'SACG':
-            janela = self.janela_sacg
+            janela = self.win_sacg
         else:
-            janela = self.p.getWindowsWithTitle('teoff-exe')[0]
+            janela = ahk.get_active_window()
+        renomear_janela = janela.get_title()
         janela.activate()
+        
         # Selecionar o Menu de opções
         self.p.sleep(1)
         if len(letras) == 2:
             self.p.typewrite(letras[0])
             self.p.sleep(1)
             self.p.typewrite(letras[1])
             self.p.sleep(1)
@@ -1514,58 +1401,59 @@
             self.p.sleep(1)
             self.p.typewrite(letras[5])
             self.p.sleep(1)
             self.p.typewrite(letras[6])
             self.p.sleep(1)
         else:
             print('ops funcao entende apenas 2, 3, 4, 5, 6 ou 7 letras')
-            
-                  
-    def get_text(self, ini_linha: int=22, fim_linha: int=632, topo1: int=410, topo2: int=415, tempo_arrastar_soltar: float=1.5, nome_janela: str | None=None, index_janela: int=-1):
+        janela.set_title(renomear_janela)
+        
+                            
+    def get_text(self, ini_linha: int=22, fim_linha: int=632, topo1: int=410, topo2: int=415, tempo_arrastar_soltar: float=1.5, nome_janela: str | None=None):
         ''' acc.get_text('Retorna ao Sistema')\n
          acc.get_text('Retorna ao Sistema', nome_janela = 'sacg')'''
         time.sleep(1)
         nome_janela = str(nome_janela).upper()
-        if index_janela >= 0:
-            janela = self.janelas[index_janela] 
+        if nome_janela == 'SIAT':
+            janela = self.win_siat
+        elif nome_janela == 'SIAC':
+            janela = self.win_siac
+        elif nome_janela == 'SACG':
+            janela = self.win_sacg
         else:
-            if nome_janela == 'SIAT':
-                janela = self.janela_siat
-            elif nome_janela == 'SIAC':
-                janela = self.janela_siac
-            elif nome_janela == 'SACG':
-                janela = self.janela_sacg
-            else:
-                janela = self.p.getWindowsWithTitle('teoff-exe')[0]
+            janela = ahk.get_active_window()
+        posicao_janela = janela.get_position()
+        renomear_janela = janela.get_title()
+        janela.activate()
   
         time.sleep(1)
-        janela.activate()
-        self.p.moveTo(janela.left + ini_linha, janela.top + topo1)
+        self.p.moveTo(posicao_janela.x + ini_linha, posicao_janela.y + topo1)
         self.p.sleep(1)
-        self.p.dragTo(janela.left + fim_linha, janela.top + topo2, tempo_arrastar_soltar, button='left')
-        self.p.moveTo(janela.left + ini_linha, janela.top + topo2)
+        self.p.dragTo(posicao_janela.x + fim_linha, posicao_janela.y + topo2, tempo_arrastar_soltar, button='left')
+        self.p.moveTo(posicao_janela.x + ini_linha, posicao_janela.y + topo2)
         self.p.rightClick()
         capturado = self.pyperclip.paste()
         print(f'texto capturado:{capturado}')
+        janela.set_title(renomear_janela)
         return capturado            
             
               
-    def exist_text(self, texto_esperado: str, max_tentativas: int=7, segundos_entre_tentativas: int=3, ini_linha: int=22, fim_linha: int=632, topo1: int=412, topo2: int=412, tempo_arrastar_soltar: float=1.5, continua_seerro: bool=False, nome_janela: str |None=None, index_janela: int=-1):
+    def exist_text(self, texto_esperado: str, max_tentativas: int=7, segundos_entre_tentativas: int=3, ini_linha: int=22, fim_linha: int=632, topo1: int=412, topo2: int=412, tempo_arrastar_soltar: float=1.5, continua_seerro: bool=False, nome_janela: str |None=None):
         ''' acc.exist_text('Retorna ao Sistema')\n
          acc.exist_text('Retorna ao Sistema', nome_janela = 'sacg')'''
         time.sleep(1)
         self.pyperclip.copy('')
         tentativas = 0
         time.sleep(1)
-        captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela, index_janela=index_janela)
+        captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela)
         resultado = True
         while not texto_esperado in captura and tentativas < max_tentativas:
             print('esperando texto: ', texto_esperado)
             self.p.sleep(segundos_entre_tentativas)
-            captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela, index_janela=index_janela)
+            captura = self.get_text(ini_linha, fim_linha, topo1, topo2, tempo_arrastar_soltar, nome_janela = nome_janela)
             tentativas += 1
             if tentativas == max_tentativas:
                 resultado = False
         print(resultado)
         if resultado == False and continua_seerro == False:
             raise Exception(f'Execução pausada. O texto: "{texto_esperado}" não foi localizado durante a execução do robô.')
         return resultado
@@ -1782,20 +1670,24 @@
         return C 
 
 
     def taxa_por_extenso(self, taxa: float | str, nome_separador: str = 'virgula') -> str:
         '''taxa_texto = taxa_por_extenso(128.09)\n
             cento e vinte e oito virgula zero nove por cento
         ''' 
+        
         if isinstance(taxa, float):
             taxa = str(taxa).replace('.', ',')
             if taxa[-2] == ',': taxa = taxa + '0'
         else:
             taxa = str(taxa).replace('.', ',').replace(' ', '')
-            if taxa[-2] == ',': taxa = taxa + '0'
+            if ',' not in taxa: 
+                taxa = taxa + ',00'
+            elif taxa[-2] == ',': 
+                taxa = taxa + '0'
             
         if ',' in taxa:
             valor_aux = taxa.split(',')
             valor_dir = valor_aux[0]
             valor_esq = valor_aux[1]
         else:
             valor_dir = taxa
@@ -2275,14 +2167,15 @@
             msg_log = f'{dica1} --> {str(list_traceback[2]).strip()} \n{dica2} --> {erro}'
         except:
             try:
                 list_traceback = str_traceback.splitlines()
                 msg_log = f'{dica1} --> {str(list_traceback[2]).strip()} \n{dica2}'
             except:      
                 msg_log = f'{dica1} \n{dica2}'
+        msg_log = msg_log.replace('.','_')
         msg_log = msg_log[:490]
         return msg_log
```

### Comparing `rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/PKG-INFO` & `rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-cooperativa
-Version: 1.0.71
+Version: 1.0.72
 Summary: Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc
 Home-page: https://github.com/edenilsonsantos/rpa_cooperativa
 Author: Edenilson Fernandes dos Santos
 Author-email: santoeen@gmail.com
 License: MIT License
 Project-URL: repository, https://github.com/edenilsonsantos/rpa_cooperativa
 Keywords: rpa cooperativa fluid api automação sql sqlalchemy
```

### Comparing `rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/SOURCES.txt` & `rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_cooperativa-1.0.71/rpa_cooperativa.egg-info/requires.txt` & `rpa_cooperativa-1.0.72/rpa_cooperativa.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -28,21 +28,21 @@
 pyrect
 pyscreeze
 pytz
 graypy
 reportlab
 psutil
 requests-html
-paramiko
 opencv-python
 pytesseract
 xmltodict
 pywin32
 pywinauto
 beautifulsoup4
 mechanize
 matplotlib
 Unidecode
 WMI
 tabulate
 python-dateutil>=2.8.2
 secure-smtplib
+ahk
```

### Comparing `rpa_cooperativa-1.0.71/setup.py` & `rpa_cooperativa-1.0.72/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as arq:
     readme = arq.read()
 
 
 setup(
     name="rpa_cooperativa",
-    version="1.0.71",
+    version="1.0.72",
     license='MIT License',
     author="Edenilson Fernandes dos Santos",
     author_email='santoeen@gmail.com',
     description="Classes referente automação com python para... api fluid, api whatsapp, api sms, sql, acc",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords='rpa cooperativa fluid api automação sql sqlalchemy',
@@ -36,11 +36,11 @@
         "Operating System :: Microsoft :: Windows",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
     python_requires='>=3.8',
     install_requires=['wheel', 'pandas<=2.0.1', 'openpyxl', 'cryptography', 'xlsxwriter', 'xlrd', 'openpyxl','selenium==4.9.1', 'webdriver_manager', 'easygui', 'pyperclip', 'mysql-connector-python>=8.0.28',
                       'pymysql', 'pyodbc', 'sqlalchemy==1.4.37', 'psycopg2', 'psycopg2-binary', 'denodo-sqlalchemy', 'pymssql', 'pillow', 'requests>=2.28.1', 'urllib3>=1.26.9', 
                       'certifi>=2022.5.18.1', 'pyopenssl>=22.0.0', 'idna>=3.3', 'charset-normalizer>=2.0.12', 'pyautogui',
-                      'pyrect', 'pyscreeze', 'pytz', 'graypy', 'reportlab', 'psutil', 'requests-html', 'paramiko','opencv-python',
+                      'pyrect', 'pyscreeze', 'pytz', 'graypy', 'reportlab', 'psutil', 'requests-html', 'opencv-python',
                       'pytesseract', 'xmltodict', 'pywin32', 'pywinauto', 'beautifulsoup4', 'mechanize', 'matplotlib', 
-                      'Unidecode', 'WMI', 'tabulate', 'python-dateutil>=2.8.2', 'secure-smtplib']
+                      'Unidecode', 'WMI', 'tabulate', 'python-dateutil>=2.8.2', 'secure-smtplib', 'ahk']
 )
```

