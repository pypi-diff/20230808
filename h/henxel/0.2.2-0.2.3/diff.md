# Comparing `tmp/henxel-0.2.2.tar.gz` & `tmp/henxel-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "henxel-0.2.2.tar", last modified: Fri Jul 28 16:40:58 2023, max compression
+gzip compressed data, was "henxel-0.2.3.tar", last modified: Tue Aug  8 12:42:36 2023, max compression
```

## Comparing `henxel-0.2.2.tar` & `henxel-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-07-28 16:40:58.664128 henxel-0.2.2/
--rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2023-02-23 18:22:17.000000 henxel-0.2.2/LICENSE
--rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2023-07-28 16:17:56.000000 henxel-0.2.2/MANIFEST.in
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5074 2023-07-28 16:40:58.664128 henxel-0.2.2/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)     4429 2023-06-27 17:10:08.000000 henxel-0.2.2/README.md
--rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2023-07-28 16:17:28.000000 henxel-0.2.2/pyproject.toml
--rw-r--r--   0 samuel    (1000) samuel    (1000)      765 2023-07-28 16:40:58.664128 henxel-0.2.2/setup.cfg
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-07-28 16:40:58.660128 henxel-0.2.2/src/
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-07-28 16:40:58.664128 henxel-0.2.2/src/henxel/
--rw-r--r--   0 samuel    (1000) samuel    (1000)   116136 2023-07-28 16:17:05.000000 henxel-0.2.2/src/henxel/__init__.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     6358 2023-05-24 09:37:41.000000 henxel-0.2.2/src/henxel/changefont.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2022-12-03 19:17:18.000000 henxel-0.2.2/src/henxel/editor.png
--rw-r--r--   0 samuel    (1000) samuel    (1000)     7223 2023-07-18 15:40:28.000000 henxel-0.2.2/src/henxel/fdialog.py
--rw-r--r--   0 samuel    (1000) samuel    (1000)     8662 2023-07-28 16:13:32.000000 henxel-0.2.2/src/henxel/help.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)     2775 2023-06-27 16:42:55.000000 henxel-0.2.2/src/henxel/wordexpand.py
-drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-07-28 16:40:58.664128 henxel-0.2.2/src/henxel.egg-info/
--rw-r--r--   0 samuel    (1000) samuel    (1000)     5074 2023-07-28 16:40:58.000000 henxel-0.2.2/src/henxel.egg-info/PKG-INFO
--rw-r--r--   0 samuel    (1000) samuel    (1000)      327 2023-07-28 16:40:58.000000 henxel-0.2.2/src/henxel.egg-info/SOURCES.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-07-28 16:40:58.000000 henxel-0.2.2/src/henxel.egg-info/dependency_links.txt
--rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2023-07-28 16:40:58.000000 henxel-0.2.2/src/henxel.egg-info/top_level.txt
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-08-08 12:42:36.968872 henxel-0.2.3/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)    34801 2023-08-04 19:06:00.000000 henxel-0.2.3/LICENSE
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       50 2023-08-04 19:06:00.000000 henxel-0.2.3/MANIFEST.in
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6870 2023-08-08 12:42:36.968872 henxel-0.2.3/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6225 2023-08-08 12:35:51.000000 henxel-0.2.3/README.md
+-rw-r--r--   0 samuel    (1000) samuel    (1000)       98 2023-08-08 12:05:02.000000 henxel-0.2.3/pyproject.toml
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      765 2023-08-08 12:42:36.968872 henxel-0.2.3/setup.cfg
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-08-08 12:42:36.956650 henxel-0.2.3/src/
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-08-08 12:42:36.968872 henxel-0.2.3/src/henxel/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)   119572 2023-08-08 12:03:39.000000 henxel-0.2.3/src/henxel/__init__.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6358 2023-08-05 10:42:30.000000 henxel-0.2.3/src/henxel/changefont.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      359 2023-08-04 19:06:00.000000 henxel-0.2.3/src/henxel/editor.png
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     7223 2023-08-04 19:06:00.000000 henxel-0.2.3/src/henxel/fdialog.py
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     8475 2023-08-08 12:03:39.000000 henxel-0.2.3/src/henxel/help.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     2775 2023-08-04 19:06:00.000000 henxel-0.2.3/src/henxel/wordexpand.py
+drwxr-xr-x   0 samuel    (1000) samuel    (1000)        0 2023-08-08 12:42:36.968872 henxel-0.2.3/src/henxel.egg-info/
+-rw-r--r--   0 samuel    (1000) samuel    (1000)     6870 2023-08-08 12:42:36.000000 henxel-0.2.3/src/henxel.egg-info/PKG-INFO
+-rw-r--r--   0 samuel    (1000) samuel    (1000)      327 2023-08-08 12:42:36.000000 henxel-0.2.3/src/henxel.egg-info/SOURCES.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        1 2023-08-08 12:42:36.000000 henxel-0.2.3/src/henxel.egg-info/dependency_links.txt
+-rw-r--r--   0 samuel    (1000) samuel    (1000)        7 2023-08-08 12:42:36.000000 henxel-0.2.3/src/henxel.egg-info/top_level.txt
```

### Comparing `henxel-0.2.2/LICENSE` & `henxel-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `henxel-0.2.2/setup.cfg` & `henxel-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = henxel
-version = 0.2.2
+version = 0.2.3
 author = SamuelKos
 author_email = koskinens371@gmail.com
 description = GUI-editor for Python development.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SamuelKos/henxel
 project_urls =
```

### Comparing `henxel-0.2.2/src/henxel/__init__.py` & `henxel-0.2.3/src/henxel/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,43 +114,101 @@
 
 GOODFONTS = [
 			'Noto Mono',
 			'Bitstream Vera Sans Mono',
 			'Liberation Mono',
 			'DejaVu Sans Mono',
 			'Inconsolata',
-			'Courier 10 Pitch'
+			'Courier 10 Pitch',
+			'Courier'
 			]
 			
 ############ Constants End
 			
 class Editor(tkinter.Toplevel):
 
 	alive = False
 	
+	pkg_contents = None
+	no_icon = True
+	pic = None
+	helptxt = None
+	
+	root = None
 	
 	def __new__(cls):
 	
+		if not cls.root:
+			# Was earlier v.0.2.2 in init:
+			
+			# self.root = tkinter.Tk().withdraw()
+			
+			# wich worked in Debian 11, but not in Debian 12,
+			# resulted error msg like: class str has no some attribute etc.
+			# After changing this line in init to:
+			
+			# self.root = tkinter.Tk()
+			# self.root.withdraw()
+			
+			# Editor would launch, but after closing and reopening in the same python-console-instance,
+			# there would be same kind of messages but about icon, and also fonts would change.
+			# This is why that stuff is now here to keep those references.
+			
+			cls.root = tkinter.Tk()
+			cls.root.withdraw()
+		
+		if not cls.pkg_contents:
+			cls.pkg_contents = importlib.resources.files(__name__)
+		
+		if cls.pkg_contents:
+			
+			if cls.no_icon:
+				for item in cls.pkg_contents.iterdir():
+					
+					if item.name == ICONPATH:
+						try:
+							cls.pic = tkinter.Image("photo", file=item)
+							cls.no_icon = False
+							break
+							
+						except tkinter.TclError as e:
+							print(e)
+			
+			if not cls.helptxt:
+				for item in cls.pkg_contents.iterdir():
+				
+					if item.name == HELPPATH:
+						try:
+							cls.helptxt = item.read_text()
+							break
+							
+						except Exception as e:
+							print(e.__str__())
+						
+		if cls.no_icon: print('Could not load icon-file.')
+		
+		
 		if not cls.alive:
 			return super(Editor, cls).__new__(cls)
 			
 		else:
 			print('Instance of ', cls, ' already running!\n')
 			
 			# By raising error the object creation is totally aborted.
 			raise ValueError()
 			
 			
 
 	def __init__(self):
-	
-		self.root = tkinter.Tk().withdraw()
+		
+		self.root = self.__class__.root
 		super().__init__(self.root, class_='Henxel', bd=4)
 		self.protocol("WM_DELETE_WINDOW", self.quit_me)
 		
+		
 		# other widgets
 		self.to_be_closed = list()
 		
 		self.ln_string = ''
 		self.want_ln = True
 		self.syntax = True
 		self.oldconf = None
@@ -198,15 +256,15 @@
 		
 		self.waitvar = tkinter.IntVar()
 		self.state = 'normal'
 		
 		
 		# IMPORTANT:
 		# 1: Event is triggered in the widget that has focus but it has no binding for that event.
-		# 2: Widget is subclassed from such widget-class that has default bindging for this event.
+		# 2: Widget is from such widget-class that has default bindging for this event.
 		# 3: The desired binding is in the nearest parent-widget.
 		
 		# https://stackoverflow.com/questions/54185434/python-tkinter-override-default-ctrl-h-binding
 		# https://anzeljg.github.io/rin2/book2/2405/docs/tkinter/binding-levels.html
 		
 		# Example, print bindtag-order of two widgets in python-console,
 		# first widget is Text-widget and then Editor-widget
@@ -262,36 +320,24 @@
 		self.bind( "<Alt-t>", self.toggle_color)
 		self.bind( "<Alt-n>", self.new_tab)
 		self.bind( "<Alt-w>", self.walk_tabs)
 		
 		
 		self.bind( "<Alt-q>", lambda event: self.walk_tabs(event, **{'back':True}) )
 		
-		pkg_contents = importlib.resources.files(__name__)
-		
 		self.helptxt = 'Could not load help-file. Press ESC to return.'
-		no_icon = True
 		
-		for item in pkg_contents.iterdir():
-			if item.name == HELPPATH:
-				try:
-					self.helptxt = item.read_text()
-				except Exception as e:
-					print(e.__str__())
-			
-			elif item.name == ICONPATH:
-				try:
-					self.pic = tkinter.Image("photo", file=item)
-					self.tk.call('wm','iconphoto', self._w, self.pic)
-					no_icon = False
-				except tkinter.TclError as e:
-					print(e)
+		if self.__class__.helptxt:
+			self.helptxt = self.__class__.helptxt
 					
-		if no_icon: print('Could not load icon-file.')
-			
+		try:
+			self.tk.call('wm','iconphoto', self._w, self.__class__.pic)
+		except tkinter.TclError as e:
+			print(e)
+		
 		
 		# Initiate widgets
 		####################################
 		self.btn_git=tkinter.Button(self, takefocus=0)
 		
 		if self.branch:
 			branch = self.branch[:5]
@@ -365,45 +411,61 @@
 		
 		self.contents.bind( "<Alt-Return>", lambda event: self.btn_open.invoke())
 		
 		self.contents.bind( "<Alt-l>", self.toggle_ln)
 		self.contents.bind( "<Control-f>", self.search)
 		
 		self.contents.bind( "<Control-a>", self.goto_linestart)
+		self.contents.bind( "<Control-e>", self.goto_lineend)
+		
+		
+		# If started from Windows, is handled in tab_override
+		self.windows = False
+		try:
+			self.contents.bind( "<ISO_Left_Tab>", self.unindent)
+		except tkinter.TclError:
+			self.windows = True
+		
+		
 		self.contents.bind( "<Control-i>", self.move_right)
-		self.contents.bind( "<Control-j>", self.center_view)
+		self.contents.bind( "<Control-b>", self.move_left)
+		self.contents.bind( "<Control-n>", self.move_down)
+		self.contents.bind( "<Control-p>", self.move_up)
 		
+		self.contents.bind( "<Control-j>", self.center_view)
 		self.contents.bind( "<Alt-f>", self.font_choose)
 		self.contents.bind( "<Alt-x>", self.toggle_syntax)
 		self.contents.bind( "<Return>", self.return_override)
 		
 		self.contents.bind( "<Control-d>", self.del_tab)
 		self.contents.bind( "<Control-q>", lambda event: self.del_tab(event, **{'save':False}) )
 		
-		
 		self.contents.bind( "<Shift-Return>", self.comment)
 		self.contents.bind( "<Shift-BackSpace>", self.uncomment)
 		self.contents.bind( "<Tab>", self.tab_override)
-		self.contents.bind( "<ISO_Left_Tab>", self.unindent)
+		
 		self.contents.bind( "<Control-t>", self.tabify_lines)
 		self.contents.bind( "<Control-z>", self.undo_override)
 		self.contents.bind( "<Control-Z>", self.redo_override)
 		self.contents.bind( "<Control-v>", self.paste)
-		
 		self.contents.bind( "<Control-BackSpace>", self.search_next)
 		self.contents.bind( "<BackSpace>", self.backspace_override)
+		
 		self.contents.bind("<Left>", lambda event: self.move_line(event, **{'direction':'left'} ))
 		self.contents.bind("<Right>", lambda event: self.move_line(event, **{'direction':'right'} ))
 		
+		self.contents.bind("<Up>", lambda event: self.updown_override(event, **{'direction':'up'} ))
+		self.contents.bind("<Down>", lambda event: self.updown_override(event, **{'direction':'down'} ))
+		
 		# Unbind some default bindings
 		self.contents.unbind_class('Text', '<<NextPara>>')
 		self.contents.unbind_class('Text', '<<PrevPara>>')
 		self.contents.unbind_class('Text', '<<SelectNextPara>>')
 		self.contents.unbind_class('Text', '<<SelectPrevPara>>')
-		
+			
 	
 		# Needed in leave() taglink in: Run file Related
 		self.name_of_cursor_in_text_widget = self.contents['cursor']
 		
 		self.popup = tkinter.Menu(self.contents, tearoff=0, bd=0, activeborderwidth=0)
 		self.popup.bind("<FocusOut>", self.popup_focusOut) # to remove popup when clicked outside
 		self.popup.add_command(label="         run", command=self.run)
@@ -1147,16 +1209,19 @@
 		return res
 		
 		
 	def get_config(self):
 		dictionary = dict()
 		dictionary['curtheme'] = self.curtheme
 		dictionary['lastdir'] = self.lastdir.__str__()
-		dictionary['font'] = self.font.config()
-		dictionary['menufont'] = self.menufont.config()
+		
+		# replace possible Tkdefaulfont as family with real name
+		dictionary['font'] = self.font.actual()
+		dictionary['menufont'] = self.menufont.actual()
+		
 		dictionary['scrollbar_width'] = self.scrollbar_width
 		dictionary['elementborderwidth'] = self.elementborderwidth
 		dictionary['want_ln'] = self.want_ln
 		dictionary['syntax'] = self.syntax
 		dictionary['ind_depth'] = self.ind_depth
 		dictionary['themes'] = self.themes
 		
@@ -1806,77 +1871,27 @@
 		
 	def enter2(self, args, event=None):
 		''' When mousecursor enters hyperlink tagname in colorchooser.
 		'''
 		wid = args[0]
 		tagname = args[1]
 		
-		syntags = [
-		'normal_text',
-		'keywords',
-		'numbers',
-		'bools',
-		'strings',
-		'comments',
-		'breaks',
-		'calls',
-		'selfs',
-		'match',
-		'focus',
-		'replaced',
-		'mismatch',
-		'selected'
-		]
-		
-		
 		t = wid.textwid
-	
-		if tagname in syntags:
-			r = t.tag_nextrange(tagname, 1.0)
-			
-			t.delete(r[0], r[1])
-			t.insert(r[0], '%s\n' % tagname, tagname)
-		
 		
 		t.config(cursor="hand2")
 		t.tag_config(tagname, underline=1, font=self.boldfont)
 		
 		
 	def leave2(self, args, event=None):
 		''' When mousecursor leaves hyperlink tagname in colorchooser.
 		'''
 		wid = args[0]
 		tagname = args[1]
 		
-		syntags = [
-		'normal_text',
-		'keywords',
-		'numbers',
-		'bools',
-		'strings',
-		'comments',
-		'breaks',
-		'calls',
-		'selfs',
-		'match',
-		'focus',
-		'replaced',
-		'mismatch',
-		'selected'
-		]
-		
-		
 		t = wid.textwid
-	
-		if tagname in syntags:
-			r = t.tag_nextrange(tagname, 1.0)
-			
-			t.delete(r[0], r[1])
-			t.insert(r[0], '%s\n' % tagname, tagname)
-		
 		
 		t.config(cursor=self.name_of_cursor_in_text_widget)
 		t.tag_config(tagname, underline=0, font=self.menufont)
 		
 		
 	def lclick2(self, args, event=None):
 		'''	When clicked hyperlink in colorchooser.
@@ -2035,15 +2050,15 @@
 		elif tagname in savetags:
 			
 			if tagname == 'Save_TMP':
 				wid.tmp_theme = copy.deepcopy(self.themes)
 				wid.flag_tmp = True
 				self.flash_tag(wid, tagname)
 				
-			elif tagname == 'TMP' and flag_tmp:
+			elif tagname == 'TMP' and wid.flag_tmp:
 				self.themes = copy.deepcopy(wid.tmp_theme)
 				self.flash_tag(wid, tagname)
 				
 			elif tagname == 'Start':
 				self.themes = copy.deepcopy(wid.start_theme)
 				self.flash_tag(wid, tagname)
 				
@@ -2184,15 +2199,15 @@
 			t.insert(i, '[ ] Background color\n', 'Background')
 			
 			c.frontback_mode = 'foreground'
 			
 		
 		
 		t.insert(i, '\nSelect tag you want to modify\n', 'title')
-		t.insert(i, 'normal_text\n', 'normal_text')
+		t.insert(i, 'normal text\n', 'normal_text')
 		
 		
 		t.insert(i, '\nSyntax highlight tags\n', 'title')
 		t.insert(i, 'keywords\n', 'keywords')
 		t.insert(i, 'numbers\n', 'numbers')
 		t.insert(i, 'bools\n', 'bools')
 		t.insert(i, 'strings\n', 'strings')
@@ -2569,32 +2584,130 @@
 		''' move cursor right with
 			ctrl-i
 		'''
 		
 		if self.state not in  [ 'normal', 'error' ]:
 			self.bell()
 			return "break"
+			
+		self.contents.event_generate('<<NextChar>>')
 		
-		pos = self.contents.index( '%s + 1c' % tkinter.INSERT)
-		self.contents.see(pos)
-		self.contents.mark_set('insert', pos)
+		return "break"
+		
+		
+	def move_left(self, event=None):
+		''' move cursor right with
+			ctrl-b
+		'''
+		
+		if self.state not in  [ 'normal', 'error' ]:
+			self.bell()
+			return "break"
+			
+		self.contents.event_generate('<<PrevChar>>')
+		
+		return "break"
+		
+		
+	def move_up(self, event=None):
+		''' move cursor right with
+			ctrl-p
+		'''
+		
+		if self.state not in  [ 'normal', 'error' ]:
+			self.bell()
+			return "break"
+			
+		self.contents.event_generate('<<PrevLine>>')
+		
+		return "break"
+		
+		
+	def move_down(self, event=None):
+		''' move cursor right with
+			ctrl-n
+		'''
+		
+		if self.state not in  [ 'normal', 'error' ]:
+			self.bell()
+			return "break"
+			
+		self.contents.event_generate('<<NextLine>>')
 		
 		return "break"
 		
 	
+	def updown_override(self, event=None, direction=None):
+		''' up-down override, to expand possibly incorrect indentation
+		'''
+		
+		if self.state != 'normal':
+			return "continue"
+			
+		oldpos = self.contents.index(tkinter.INSERT)
+		
+		
+		if direction == 'down':
+			newpos = self.contents.index( '%s + 1lines' % tkinter.INSERT)
+			
+		# direction == 'up'
+		else:
+			newpos = self.contents.index( '%s - 1lines' % tkinter.INSERT)
+			
+		
+		oldline = self.contents.get( '%s linestart' % oldpos, '%s lineend' % oldpos)
+		newline = self.contents.get( '%s linestart' % newpos, '%s lineend' % newpos)
+		
+		
+		if newline.isspace() or newline == '':
+			
+			if oldline == '':
+				return 'continue'
+			
+			if not oldline.isspace():
+			
+				tmp = oldline.lstrip()
+				oldindent = oldline.index(tmp)
+				
+				if oldindent == 0:
+					return 'continue'
+			
+				self.contents.delete('%s linestart' % newpos,'%s lineend' % newpos)
+				self.contents.insert('%s linestart' % newpos, oldindent * '\t')
+				return 'continue'
+			
+			# coming from empty line:
+			else:
+				self.contents.delete('%s linestart' % newpos,'%s lineend' % newpos)
+				self.contents.insert('%s linestart' % newpos, len(oldline) * '\t')
+				return 'continue'
+			
+		else:
+			return 'continue'
+		
+		
 	def center_view(self, event=None):
 		''' Raise insertion-line
 		'''
 		if self.state != 'normal':
 			self.bell()
 			return "break"
 			
 			
 		self.contents.yview_scroll(12, 'units')
 		return "break"
+	
+	
+	def goto_lineend(self, event=None):
+		if self.state != 'normal':
+			self.bell()
+			return "break"
+			
+		self.contents.event_generate('<<LineEnd>>')
+		return "break"
 		
 		
 	def goto_linestart(self, event=None):
 		if self.state != 'normal':
 			self.bell()
 			return "break"
 		
@@ -2623,16 +2736,16 @@
 					pos = self.contents.index( '%i.%i' % (l2, indent) )
 		
 		
 		self.contents.see(pos)
 		self.contents.mark_set('insert', pos)
 		
 		return "break"
-	
-	
+		
+		
 	def raise_popup(self, event=None):
 		if self.state != 'normal':
 			self.bell()
 			return "break"
 		
 		self.popup.post(event.x_root, event.y_root)
 		self.popup.focus_set() # Needed to remove popup when clicked outside.
@@ -2675,15 +2788,15 @@
 			if i == s:
 				insert_at_selstart = True
 
 			# else: insert at selend
 
 			line_s = s.split('.')[0]
 			line_e = e.split('.')[0]
-
+			
 			# One line only:
 			if line_s == line_e: 	return 'continue'
 
 			# cursor line is empty:
 			if len(t.strip()) == 0: return 'continue'
 
 
@@ -2818,19 +2931,32 @@
 	
 	def tab_override(self, event):
 		'''	Used to bind Tab-key with indent()
 		'''
 		
 		if self.state in [ 'search', 'replace', 'replace_all' ]:
 			return 'break'
-				
-		# dont know if this is needed
-		if hasattr(event, 'state') and event.state != 0:
-			return
 		
+		# In Windows, Tab-key-event has state 8 and shift+Tab has state 9,
+		# so because shift-tab is unbinded if in Windows, we check that here
+		# and unindent if it is the state.
+		if hasattr(event, 'state'):
+			
+			if self.windows:
+				
+				if event.state == 9:
+					self.unindent()
+					return 'break'
+					
+				if event.state not in [8, 0]:
+					return
+			
+			elif event.state != 0:
+				return
+				
 		# Fix for tab-key not working sometimes.
 		# This happens because os-clipboard content is (automatically)
 		# added to selection content of a Text widget, and since there is no
 		# actual selection (clipboard-text is outside from Text-widget),
 		# tab_override() gets quite broken.
 		if len(self.contents.tag_ranges('sel')) == 0:
 			return
@@ -3585,41 +3711,43 @@
 				print(f'\n Could not save file: {self.tabs[self.tabindex].filepath}')
 				return
 				
 		############# Save End #######################################
 	
 ########## Save and Load End
 ########## Gotoline and Help Begin
-
+	
 	def do_gotoline(self, event=None):
 		try:
 			tmp = self.entry.get().strip()
-	
+			
 			if tmp in ['-1', '']:
 				line = tkinter.END
 			else:
 				line = tmp + '.0'
-			
+				
 			self.contents.focus_set()
 			self.contents.mark_set('insert', line)
 			self.ensure_idx_visibility(line)
 			
 			
 			try:
 				pos = self.contents.index(tkinter.INSERT)
 			except tkinter.TclError:
 				pos = '1.0'
-		
+				
 			self.tabs[self.tabindex].position = pos
 			self.stop_gotoline()
-		
+			
 		except tkinter.TclError as e:
 			print(e)
 			self.stop_gotoline()
-	
+			
+		return "break"
+		
 	
 	def stop_gotoline(self, event=None):
 		self.bind("<Escape>", self.do_nothing)
 		self.entry.bind("<Return>", self.load)
 		self.entry.delete(0, tkinter.END)
 		if self.tabs[self.tabindex].filepath:
 			self.entry.insert(0, self.tabs[self.tabindex].filepath)
@@ -3627,18 +3755,20 @@
 		
 		# set cursor pos
 		try:
 			line = self.tabs[self.tabindex].position
 			self.contents.focus_set()
 			self.contents.mark_set('insert', line)
 			self.ensure_idx_visibility(line)
-			
+		
 		except tkinter.TclError:
 			self.tabs[self.tabindex].position = '1.0'
 		
+		return "break"
+		
 	
 	def gotoline(self, event=None):
 		if self.state != 'normal':
 			self.bell()
 			return "break"
 			
 		try:
@@ -4497,38 +4627,40 @@
 		self.stop_search()
 		
 		
 	def start_replace(self, event=None):
 		self.new_word = self.entry.get()
 		
 		if self.old_word == self.new_word:
-			return
-		else:
-			self.bind("<Control-n>", self.show_next)
-			self.bind("<Control-p>", self.show_prev)
-			
-			# prevent focus messing
-			self.entry.bind("<Return>", self.do_nothing)
-			self.entry.config(state='disabled')
-			self.focus_set()
+			return 'break'
+				
+		self.bind("<Control-n>", self.show_next)
+		self.bind("<Control-p>", self.show_prev)
+		
+		# prevent focus messing
+		self.entry.bind("<Return>", self.do_nothing)
+		self.entry.config(state='disabled')
+		self.focus_set()
+		
+		self.contents.tag_remove('replaced', '1.0', tkinter.END)
+		
+		
+		if self.state == 'replace':
+		
+			self.replace_overlap_index = None
 			
-			self.contents.tag_remove('replaced', '1.0', tkinter.END)
-	
+			if self.old_word in self.new_word:
+				self.replace_overlap_index = self.new_word.index(self.old_word)
+				
+			self.title( f'Replace: 1/{self.search_matches}' )
+			self.bind( "<Return>", self.do_single_replace)
 			
-			if self.state == 'replace':
+		elif self.state == 'replace_all':
+			self.bind( "<Return>", self.do_replace_all)
+			self.title('Replacing ALL %s matches of %s with: %s' % (str(self.search_matches), self.old_word, self.new_word) )
 			
-				self.replace_overlap_index = None
-				
-				if self.old_word in self.new_word:
-					self.replace_overlap_index = self.new_word.index(self.old_word)
-				
-				self.title( f'Replace: 1/{self.search_matches}' )
-				self.bind( "<Return>", self.do_single_replace)
-				
-			elif self.state == 'replace_all':
-				self.bind( "<Return>", self.do_replace_all)
-				self.title('Replacing ALL %s matches of %s with: %s' % (str(self.search_matches), self.old_word, self.new_word) )
-
-
+		return 'break'
+		
+		
 ################ Replace End
 ########### Class Editor End
```

### Comparing `henxel-0.2.2/src/henxel/changefont.py` & `henxel-0.2.3/src/henxel/changefont.py`

 * *Files identical despite different names*

### Comparing `henxel-0.2.2/src/henxel/fdialog.py` & `henxel-0.2.3/src/henxel/fdialog.py`

 * *Files identical despite different names*

### Comparing `henxel-0.2.2/src/henxel/help.txt` & `henxel-0.2.3/src/henxel/help.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-		Keyboard shortcuts (* marks often needed):
+		Keyboard shortcuts:
 		
 		If key-sequence is like: Ctrl-c
 		It means: while holding ctrl-key down, press and release c-key.
 		
 		If key-sequence is like: Ctrl-c-f
 		It means: while holding ctrl-key down, press and release first
 		c-key then f-key.
 		 
-*		Alt-Return		Open file
+		Alt-Return		Open file
 		Ctrl-BackSpace  Show and select next occurence of last search.
 						If got too far, press arrowleft to go to last
 						cursor position.
-*		Ctrl-f  Search
+		Ctrl-f  Search
 		Ctrl-r  Replace
 		Ctrl-R  Replace all
-*		Ctrl-g  Gotoline:	-1 and empty goes to file-end
-				
-*		Shift-Tab  Unindent
-*		Tab        Indent
-		
-*		Shift-Return	Comment
-*		Shift-BackSpace	Uncomment
-				
+		Ctrl-g  Gotoline:	-1 and empty goes to file-end
+		
+		Shift-Tab  Unindent
+		Tab        Indent
+		
+		Shift-Return	Comment
+		Shift-BackSpace	Uncomment
+		
 		# Super means search-key.
-(*)		Ctrl-Super-Return	run file
+		Ctrl-Super-Return	run file
 		
-*		Ctrl-c  Copy		Try this: Ctrl-c-f
-*		Ctrl-v  Paste
-*		Ctrl-x  Cut
-*		Ctrl-z  Undo
+		Ctrl-c  Copy		Try this: Ctrl-c-f
+		Ctrl-v  Paste
+		Ctrl-x  Cut
+		Ctrl-z  Undo
 		Ctrl-Z  Redo
 		
 		Alt-f   Font setting
 		Alt-s   Color setting
 		Alt-t   Toggle color setting
 		Alt-l   Toggle linenumbers
 		Alt-x   Toggle syntax highlight
 		Alt-e   expand word
-*		Alt-n   Open new tab			Try this: Alt-n-Return
+		Alt-n   Open new tab			Try this: Alt-n-Return
 		
-*		Ctrl-d  Close current tab and save it
+		Ctrl-d  Close current tab and save it
 		Ctrl-q  Close current tab without saving it
-*		Alt-w   Walk tabs forward
-*		Alt-q   Walk tabs backwards
+		Alt-w   Walk tabs forward
+		Alt-q   Walk tabs backwards
 		
-		Ctrl-o  Insert linebreak at cursor
 		Ctrl-i  Move cursor right
 		Ctrl-b  Move cursor left
 		Ctrl-n  Move cursor down
 		Ctrl-p  Move cursor up
-*		Ctrl-e  Move cursor to lineend
-*		Ctrl-a  Move cursor to linestart
+		Ctrl-e  Move cursor to lineend
+		Ctrl-a  Move cursor to linestart
 		Ctrl-j  Scroll down 12 lines without moving cursor (center view)
 		Ctrl-k  Remove from cursor to lineend
+		Ctrl-o  Insert linebreak at cursor
 		
-*		Shift-up	Select one more line up
-*		Shift-down	Select one more line down
+		Shift-up	Select one more line up
+		Shift-down	Select one more line down
 		
-*		Ctrl-left  		Move cursor one word left
-*		Ctrl-right 		Move cursor one word right
-*		Ctrl-shift-left 	Select one more word to left
-*		Ctrl-shift-right	Select one more word to right
+		Ctrl-left  		Move cursor one word left
+		Ctrl-right 		Move cursor one word right
+		Ctrl-shift-left 	Select one more word to left
+		Ctrl-shift-right	Select one more word to right
 		
 		Ctrl-plus 	Increase scrollbar-width
 		Ctrl-minus	Decrease scrollbar-width
 		
 		Ctrl-t  	Change indentation of selected lines to current setting
 
 
@@ -197,23 +197,17 @@
 	  - If you copied something to your editor that has different indentation
 		than rest of the file:
 		(Note that you don't have to do anything if it is indented with normal
 		4 spaces and you have indent-depth the normal 4 )
 		1: Make sure you copied the block starting with one empty line.
 		2: Click cursor to start of empty line and paste.
 		
-  def myfunc(foo):
-	print(foo)
-	
-	return foo + 1
-
 		Then select that code and press Control-t, and
 		it should then be indented as you wanted and you can then continue
-		indenting the pasted code to the right place. You can try all this
-		by copying the code example above and then trying to fix it.
+		indenting the pasted code to the right place.
 		
 		(Note that you don't have to do anything if you open a file that has
 		different indentation than your setting, it is changed automatically
 		and saved with tabbed indentation after you for example close it.)
 	
 	
 	Running file
```

### Comparing `henxel-0.2.2/src/henxel/wordexpand.py` & `henxel-0.2.3/src/henxel/wordexpand.py`

 * *Files identical despite different names*

