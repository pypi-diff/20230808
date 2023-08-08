# Comparing `tmp/viv-23.8a1.tar.gz` & `tmp/viv-23.8a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viv-23.8a1.tar", last modified: Fri Aug  4 19:35:57 2023, max compression
+gzip compressed data, was "viv-23.8a3.tar", last modified: Tue Aug  8 21:29:26 2023, max compression
```

## Comparing `viv-23.8a1.tar` & `viv-23.8a3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1074 2023-06-02 13:44:22.530182 viv-23.8a1/LICENSE
--rw-r--r--   0        0        0     4163 2023-08-03 23:16:31.419220 viv-23.8a1/README.md
--rw-r--r--   0        0        0      821 2023-06-02 21:56:40.027575 viv-23.8a1/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-02 13:44:22.533515 viv-23.8a1/src/viv/__init__.py
--rw-r--r--   0        0        0       61 2023-06-02 13:44:22.536848 viv-23.8a1/src/viv/__main__.py
--rwxr-xr-x   0        0        0    58045 2023-08-04 19:35:35.537376 viv-23.8a1/src/viv/viv.py
--rw-r--r--   0        0        0     4487 1970-01-01 00:00:00.000000 viv-23.8a1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-02 13:44:22.530182 viv-23.8a3/LICENSE
+-rw-r--r--   0        0        0     4169 2023-08-08 21:12:49.153273 viv-23.8a3/README.md
+-rw-r--r--   0        0        0      814 2023-08-08 21:29:26.949054 viv-23.8a3/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-02 13:44:22.533515 viv-23.8a3/src/viv/__init__.py
+-rw-r--r--   0        0        0       61 2023-06-02 13:44:22.536848 viv-23.8a3/src/viv/__main__.py
+-rwxr-xr-x   0        0        0    64642 2023-08-08 21:29:21.459017 viv-23.8a3/src/viv/viv.py
+-rw-r--r--   0        0        0     4538 1970-01-01 00:00:00.000000 viv-23.8a3/PKG-INFO
```

### Comparing `viv-23.8a1/LICENSE` & `viv-23.8a3/LICENSE`

 * *Files identical despite different names*

### Comparing `viv-23.8a1/README.md` & `viv-23.8a3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 ```python
 __import__("viv").use("click")
 ```
 
 To remove all `vivenvs` you can use the below command:
 
 ```sh
-viv remove $(viv list -q)
+viv cache remove $(viv list -q)
 ```
 
 To remove `viv` all together you can use the included `purge` command:
 
 ```sh
 python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge
 ```
```

#### html2text {}

```diff
@@ -20,26 +20,26 @@
 customize this with `--src`. ```sh export PYTHONPATH="$PYTHONPATH:$HOME/.local/
 share/viv" ``` ### Pypi (Not Recommended) ```sh pip install viv ``` Why is this
 *not recommended*? Mainly, because `viv` is all about hacking your `sys.path`.
 Placing it in it's own virtual environment or installing in a user site
 directory may complicate this endeavor. ## Usage In any python script with
 external dependencies you can add this line, to automate `vivenv` creation and
 installation of dependencies. ```python __import__("viv").use("click") ``` To
-remove all `vivenvs` you can use the below command: ```sh viv remove $(viv list
--q) ``` To remove `viv` all together you can use the included `purge` command:
-```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge ``` ## Additional
-Features An experimental feature of `viv` is generating shim's that leverage
-the principles of `viv`. These shims would operate similar to `pipx` in which
-you can specify a command line app to "install". *Note* that `--standalone`
-will auto-generate a mini function version of `viv` to accomplish the same
-basic task as using a local copy of `viv`. After generating this standalone
-`shim` you can freely use this script across unix machines which have
-`python>3.8`. See [examples/black](https://github.com/daylinmorgan/viv/blob/
-dev/examples/black) for output of below command. ```sh python3 <(curl -fsSL
-viv.dayl.in/viv.py) shim black -o ./black --standalone --freeze ``` ##
+remove all `vivenvs` you can use the below command: ```sh viv cache remove $
+(viv list -q) ``` To remove `viv` all together you can use the included `purge`
+command: ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge ``` ##
+Additional Features An experimental feature of `viv` is generating shim's that
+leverage the principles of `viv`. These shims would operate similar to `pipx`
+in which you can specify a command line app to "install". *Note* that `--
+standalone` will auto-generate a mini function version of `viv` to accomplish
+the same basic task as using a local copy of `viv`. After generating this
+standalone `shim` you can freely use this script across unix machines which
+have `python>3.8`. See [examples/black](https://github.com/daylinmorgan/viv/
+blob/dev/examples/black) for output of below command. ```sh python3 <(curl -
+fsSL viv.dayl.in/viv.py) shim black -o ./black --standalone --freeze ``` ##
 Alternatives ### [pip-run](https://github.com/jaraco/pip-run) ```sh pip-run
 (10.0.5) âââ autocommand (2.2.2) âââ jaraco-context (4.3.0)
 âââ jaraco-functools (3.6.0) â âââ more-itertools (9.1.0)
 âââ jaraco-text (3.11.1) â âââ autocommand (2.2.2) â âââ
 inflect (6.0.2) â â âââ pydantic>=1.9.1 (1.10.5) â â âââ
 typing-extensions>=4.2.0 (4.5.0) â âââ jaraco-context>=4.1 (4.3.0) â
 âââ jaraco-functools (3.6.0) â â âââ more-itertools (9.1.0) â
```

### Comparing `viv-23.8a1/pyproject.toml` & `viv-23.8a3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = [
-    "pdm-pep517>=1.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [project]
 name = "viv"
 description = "viv isn't venv"
 authors = [
     { name = "Daylin Morgan", email = "daylinmorgan@gmail.com" },
 ]
 dependencies = []
 requires-python = ">= 3.8"
 readme = "README.md"
 dynamic = []
-version = "23.8a1"
+version = "23.8a3"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://github.com/daylinmorgan/viv"
 repository = "https://github.com/daylinmorgan/viv"
```

### Comparing `viv-23.8a1/src/viv/viv.py` & `viv-23.8a3/src/viv/viv.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,26 +37,29 @@
 from logging.handlers import RotatingFileHandler
 from pathlib import Path
 from textwrap import dedent, fill
 from types import TracebackType
 from typing import (
     Any,
     Dict,
+    Generator,
     List,
     NoReturn,
     Optional,
     Sequence,
+    Set,
     TextIO,
     Tuple,
     Type,
+    Union,
 )
 from urllib.error import HTTPError
 from urllib.request import urlopen
 
-__version__ = "23.8a1"
+__version__ = "23.8a3"
 
 
 class Spinner:
     """spinner modified from:
     https://raw.githubusercontent.com/Tagar/stuff/master/spinner.py
     """
 
@@ -141,33 +144,32 @@
         return [i for i in os.getenv("VIV_SPEC", "").split(" ") if i]
 
     @property
     def _viv_log_path(self) -> Path:
         return _path_ok(Path(self.xdg_data_home) / "viv") / "viv.log"
 
 
-class Cache:
-    def __init__(self) -> None:
-        self.base = Env().viv_cache
-
+class Cfg:
     @property
     def src(self) -> Path:
-        return _path_ok(self.base / "src")
+        p = Path(Env().xdg_data_home) / "viv" / "viv.py"
+        p.parent.mkdir(exist_ok=True, parents=True)
+        return p
 
     @property
-    def venv(self) -> Path:
-        return _path_ok(self.base / "venvs")
+    def cache_base(self) -> Path:
+        return Env().viv_cache
 
+    @property
+    def cache_src(self) -> Path:
+        return _path_ok(self.cache_base / "src")
 
-class Cfg:
     @property
-    def src(self) -> Path:
-        p = Path(Env().xdg_data_home) / "viv" / "viv.py"
-        p.parent.mkdir(exist_ok=True, parents=True)
-        return p
+    def cache_venv(self) -> Path:
+        return _path_ok(self.cache_base / "venvs")
 
 
 class Ansi:
     """control ouptut of ansi(VT100) control codes"""
 
     def __init__(self) -> None:
         self.bold: str = "\033[1m"
@@ -318,15 +320,15 @@
         logger.addHandler(fh)
     return logger
 
 
 log = gen_logger()
 
 
-def err_quit(*msg: str, code: int = 1) -> None:
+def err_quit(*msg: str, code: int = 1) -> NoReturn:
     log.error("\n".join(msg))
     sys.exit(code)
 
 
 class Template:
     _standalone_func = r"""def _viv_use(*pkgs, track_exe=False, name=""):
     import hashlib, json, os, site, shutil, sys, venv  # noqa
@@ -335,29 +337,27 @@
     from subprocess import run  # noqa
 
     if not {*map(type, pkgs)} == {str}:
         raise ValueError(f"spec: {pkgs} is invalid")
 
     meta = dict.fromkeys(("created", "accessed"), (t := str(datetime.today())))
     runner = str(Path(__file__).absolute().resolve())
-    env = lambda x: os.getenv(f"VIV_{x}") # noqa
-    F, V, no_st = map(env, ("FORCE", "VERBOSE", "NO_SETUPTOOLS"))
-    xdg = os.getenv("XDG_CACHE_HOME")
-    cache = (Path(xdg) if xdg else Path.home() / ".cache") / "viv" / "venvs"
-    cache.mkdir(parents=True, exist_ok=True)
+    envvar = lambda x: os.getenv(f"VIV_{x}")  # noqa
+    F, V, no_st = map(envvar, ("FORCE", "VERBOSE", "NO_SETUPTOOLS"))
+    base = Path(xdg) if (xdg := os.getenv("XDG_CACHE_HOME")) else Path.home() / ".cache"
+    (cache := (base) / "viv/venvs").mkdir(parents=True, exist_ok=True)
     exe = str(Path(sys.executable).resolve()) if track_exe else "N/A"
-    (sha256 := hashlib.sha256()).update((str(spec := [*pkgs]) + exe).encode())
-    _id = sha256.hexdigest()
+    _id = hashlib.sha256((str(spec := [*pkgs]) + exe).encode()).hexdigest()
     if (env := cache / (name if name else _id)) not in cache.glob("*/") or F:
         sys.stderr.write(f"generating new vivenv -> {env.name}\n")
         venv.create(env, prompt=f"viv-{name}", symlinks=True, clear=True)
         kw = dict(zip(("stdout", "stderr"), ((None,) * 2 if V else (-1, 2))))
-        if (not no_st) and (not [x for x in spec if x.startswith("setuptools")]):
-            spec.append("setuptools")
         cmd = ["pip", "--python", str(env / "bin" / "python"), "install", *spec]
+        if (not no_st) and (not [x for x in spec if x.startswith("setuptools")]):
+            cmd.append("setuptools")
         p = run(cmd, **kw)
         if (rc := p.returncode) != 0:
             if env.is_dir():
                 shutil.rmtree(env)
             sys.stderr.write(f"pip had non zero exit ({rc})\n{p.stdout.decode()}\n")
             sys.exit(rc)
         meta.update(dict(id=_id, spec=spec, exe=exe, name=name, files=[runner]))
@@ -371,15 +371,15 @@
 """
 
     @staticmethod
     def description(name: str) -> str:
         return f"""
 
 {a.tagline()}
-command line: `{a.bold}{name} --help{a.end}`
+command line: `{a.bold}viv run typer rich-click -s ./script.py{a.end}`
 python api: {a.style('__import__("viv").use("typer", "rich-click")','bold')}
 """
 
     @staticmethod
     def noqa(txt: str) -> str:
         max_length = max(map(len, txt.splitlines()))
         return "\n".join((f"{line:{max_length}} # noqa" for line in txt.splitlines()))
@@ -500,15 +500,15 @@
             "\n".join(
                 f"  {a.bold}{k}{a.end}: {v}"
                 for k, v in (
                     ("Version", __version__),
                     ("CLI", cli),
                     ("Running Source", running),
                     ("Local Source", local),
-                    ("Cache", Cache().base),
+                    ("Cache", Cfg().cache_base),
                 )
             )
             + "\n"
         )
 
 
 # TODO: convert the below functions into a proper file/stream logging interface
@@ -665,45 +665,84 @@
             action_length = invocation_length + self._current_indent
             self._action_max_length = max(self._action_max_length, action_length)
 
             # add the item to the list
             self._add_item(self._format_action, [action])
 
 
+class KVAppendAction(Action):
+    def __init__(self, *args: Any, keys: List[str], **kwargs: Any) -> None:
+        self._keys = keys
+        super(KVAppendAction, self).__init__(*args, **kwargs)
+
+    def __call__(
+        self,
+        parser: StdArgParser,
+        namespace: Namespace,
+        values: Union[str, Sequence[Any], None],
+        option_string: str | None = None,
+    ) -> None:
+        if not isinstance(values, str):
+            raise TypeError("expected string for `values`")
+        try:
+            (k, v) = values.split(":")
+            if k not in self._keys:
+                err_quit(
+                    "".join(
+                        (
+                            f"unexpected key: {a.yellow}{k}{a.end} for {self.dest},",
+                            " must be one of: ",
+                            ", ".join((a.style(k, "bold") for k in self._keys)),
+                        )
+                    )
+                )
+            d = {k: v}
+        except ValueError:
+            err_quit(
+                f"failed to parse key-value for {self.dest} "
+                f'"{a.bold}{values}{a.end}" as k:v'
+            )
+        items = getattr(namespace, self.dest)
+        if not items:
+            items = {}
+
+        items.update(d)
+        setattr(namespace, self.dest, items)
+
+
 class ArgumentParser(StdArgParser):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
         super().__init__(*args, **kwargs)
 
         self.formatter_class = lambda prog: CustomHelpFormatter(
             prog,
             max_help_position=35,
         )
 
     def error(self, message: str) -> NoReturn:
-        error(message, f"see `{self.prog} --help` for more info")
+        error(message, f"see `{a.bold}{self.prog} --help{a.end}` for more info")
         sys.exit(2)
 
 
-def run(
+def subprocess_run(
     command: List[str],
     spinmsg: str = "",
     clean_up_path: Optional[Path] = None,
     verbose: bool = False,
     ignore_error: bool = False,
     check_output: bool = False,
 ) -> str:
     """run a subcommand
 
     Args:
         command: Subcommand to be run in subprocess.
         verbose: If true, print subcommand output.
     """
 
-    # TODO: remove 'verbose' and rely on log level?
-    log.debug("executing subcmd\n\t" + " ".join(command))
+    log.debug("executing subcmd:\n  " + " ".join(command))
 
     if spinmsg and not verbose:
         with Spinner(spinmsg):
             p = subprocess.run(
                 command,
                 stdout=None if verbose else subprocess.PIPE,
                 stderr=None if verbose else subprocess.STDOUT,
@@ -713,34 +752,39 @@
         p = subprocess.run(
             command,
             stdout=None if verbose else subprocess.PIPE,
             stderr=None if verbose else subprocess.STDOUT,
             universal_newlines=True,
         )
 
-    if not verbose:
-        log.debug(
-            "output:\n" + "\n".join(f"-> {line}" for line in p.stdout.splitlines())
-        )
-
     if p.returncode != 0 and not ignore_error:
         a.subprocess(command, p.stdout)
 
         if clean_up_path and clean_up_path.is_dir():
             shutil.rmtree(str(clean_up_path))
 
         sys.exit(p.returncode)
 
-    elif check_output:
+    if not verbose:
+        log.debug(
+            "output:\n" + "\n".join(f"-> {line}" for line in p.stdout.splitlines())
+        )
+
+    if check_output:
         return p.stdout
 
     else:
         return ""
 
 
+def subprocess_run_quit(command: List[str | Path], **kwargs: Any) -> None:
+    log.debug("executing subcmd:\n  " + " ".join(map(str, command)))
+    sys.exit(subprocess.run(command, **kwargs).returncode)
+
+
 def get_hash(spec: Tuple[str, ...] | List[str], track_exe: bool = False) -> str:
     """generate a hash of package specifications
 
     Args:
         spec: sequence of package specifications
         track_exe: if true add python executable to hash
     Returns:
@@ -765,26 +809,26 @@
     files: List[str]
     exe: str
     created: str = ""
     accessed: str = ""
 
     @classmethod
     def load(cls, name: str) -> "Meta":
-        if not (Cache().venv / name / "vivmeta.json").exists():
+        if not (Cfg().cache_venv / name / "vivmeta.json").exists():
             log.warning(f"possibly corrupted vivenv: {name}")
             # add empty values for corrupted vivenvs so it will still load
             return cls(name=name, spec=[""], files=[""], exe="", id="")
         else:
-            meta = json.loads((Cache().venv / name / "vivmeta.json").read_text())
+            meta = json.loads((Cfg().cache_venv / name / "vivmeta.json").read_text())
 
         return cls(**meta)
 
     def write(self, p: Path | None = None) -> None:
         if not p:
-            p = (Cache().venv) / self.name / "vivmeta.json"
+            p = (Cfg().cache_venv) / self.name / "vivmeta.json"
 
         p.write_text(json.dumps(self.__dict__))
 
     def addfile(self, f: Path) -> None:
         log.debug(f"associating {f} with {self.name}")
         self.accessed = str(datetime.today())
         self.files = sorted({*self.files, str(f.absolute().resolve())})
@@ -807,15 +851,15 @@
             spec = self._validate_spec(spec)
         id = id if id else get_hash(spec, track_exe)
 
         self.name = name if name else id[:8]
         self.set_path(path)
 
         if not metadata:
-            if self.name in (d.name for d in Cache().venv.iterdir()):
+            if self.name in (d.name for d in Cfg().cache_venv.iterdir()):
                 self.loaded = True
                 self.meta = Meta.load(self.name)
             else:
                 self.meta = Meta(
                     spec=spec,
                     name=self.name,
                     id=id,
@@ -832,15 +876,15 @@
             name: used as lookup in the vivenv cache
         """
         vivenv = cls(name=name, metadata=Meta.load(name))
 
         return vivenv
 
     def set_path(self, path: Path | None = None) -> None:
-        self.path = path if path else Cache().venv / self.name
+        self.path = path if path else Cfg().cache_venv / self.name
         self.python = str((self.path / "bin" / "python").absolute())
         self.pip = ("pip", "--python", self.python)
 
     def _validate_spec(self, spec: List[str]) -> List[str]:
         """ensure spec is at least of sequence of strings
 
         Args:
@@ -886,15 +930,15 @@
             "install",
             "--force-reinstall",
         ] + self.meta.spec
 
         if not Env().viv_no_setuptools and "setuptools" not in self.meta.spec:
             cmd.append("setuptools")
 
-        run(
+        subprocess_run(
             cmd,
             spinmsg="installing packages in vivenv",
             clean_up_path=self.path,
             verbose=bool(Env().viv_verbose),
         )
 
     def touch(self) -> None:
@@ -903,14 +947,17 @@
     def activate(self) -> None:
         # also add sys.path here so that it comes first
         log.debug(f"activating {self.name}")
         path_to_add = str(*(self.path / "lib").glob("python*/site-packages"))
         sys.path = [p for p in (path_to_add, *sys.path) if p != site.USER_SITE]
         site.addsitedir(path_to_add)
 
+    def files_exist(self) -> bool:
+        return len([f for f in self.meta.files if Path(f).is_file()]) == 0
+
     def show(self) -> None:
         _id = (
             self.meta.id[:8]
             if self.meta.id == self.name
             else (self.name[:5] + "..." if len(self.name) > 8 else self.name)
         )
 
@@ -975,15 +1022,15 @@
     vivenv.activate()
 
     return vivenv.path
 
 
 def get_venvs() -> Dict[str, ViVenv]:
     vivenvs = {}
-    for p in Cache().venv.iterdir():
+    for p in Cfg().cache_venv.iterdir():
         vivenv = ViVenv.load(p.name)
         vivenvs[vivenv.name] = vivenv
     return vivenvs
 
 
 def combined_spec(reqs: List[str], requirements: Path) -> List[str]:
     if requirements:
@@ -1001,15 +1048,17 @@
         "--dry-run",
         "--quiet",
         "--ignore-installed",
         "--report",
         "-",
     ] + spec
 
-    report = json.loads(run(cmd, check_output=True, spinmsg="resolving depedencies"))
+    report = json.loads(
+        subprocess_run(cmd, check_output=True, spinmsg="resolving depedencies")
+    )
     resolved_spec = [
         f"{pkg['metadata']['name']}=={pkg['metadata']['version']}"
         for pkg in report["install"]
     ]
 
     return resolved_spec
 
@@ -1033,15 +1082,15 @@
         + reference
         + "/src/viv/viv.py"
     )
 
     (hash := hashlib.sha256()).update(src.encode())
     sha256 = hash.hexdigest()
 
-    cached_src_file = Cache().src / f"{sha256}.py"
+    cached_src_file = Cfg().cache_src / f"{sha256}.py"
 
     if not cached_src_file.is_file():
         cached_src_file.write_text(src)
 
     return sha256
 
 
@@ -1065,15 +1114,15 @@
         """,
             txt,
             re.VERBOSE | re.MULTILINE,
         )
     )
 
 
-def _read_metadata_block(txt: str) -> None:
+def _read_metadata_block(txt: str) -> Generator[Tuple[str, str, List[str]], None, None]:
     """check for pep722 style metadata block and parse"""
 
     lines = iter(txt.splitlines())
     for line in lines:
         if line.startswith("##"):
             block_type, sep, extra = line[2:].strip().partition(":")
             if not sep:
@@ -1085,29 +1134,145 @@
                 line = line[2:].strip()
                 if not line:
                     continue
                 block_data.append(line)
             yield block_type, extra, block_data
 
 
-def deps_block(txt: str):
-    return list(
-        (
-            req
-            for block_type, extra, block_data in _read_metadata_block(txt)
-            for req in block_data
-            if block_type == "Script Dependencies"
+DEPENDENCY_BLOCK_MARKER = r"(?i)^#\s+script\s+dependencies:\s*$"
+
+
+def read_dependency_block(txt: str) -> List[str]:
+    lines = iter(txt.splitlines())
+    for line in lines:
+        if re.match(DEPENDENCY_BLOCK_MARKER, line):
+            for line in lines:
+                if not line.startswith("#"):
+                    break
+                # Remove comments. An inline comment is introduced by
+                # a hash, which must be preceded and followed by a
+                # space. The initial hash will be skipped as it has
+                # no space before it.
+                line = line.split(" # ", maxsplit=1)[0]
+                line = line[1:].strip()
+                if not line:
+                    continue
+                # let pip handle the requirement errors
+                yield line
+            break
+
+
+def _parse_date(txt: str) -> datetime:
+    """attempt to parse datetime string
+
+    acceptable formats `%Y-%m-%d` & `%Y-%m-%dT%H:%M`
+    """
+
+    try:
+        date = datetime.strptime(
+            txt,
+            "%Y-%m-%d",
         )
+        return date
+    except ValueError:
+        pass
+
+    try:
+        datetime.strptime(txt, "%Y-%m-%dT%H:%M")
+        return date
+    except ValueError:
+        pass
+
+    err_quit(
+        f"failed to parse {a.yellow}{txt}{a.end} as datetime\n"
+        "acceptable formats `%Y-%m-%d` & `%Y-%m-%dT%H:%M`"
     )
 
 
+class Cache:
+    def __init__(self) -> None:
+        self.vivenvs = self._get_venvs()
+
+    def _get_venvs(self) -> Dict[str, ViVenv]:
+        vivenvs = {}
+        for p in Cfg().cache_venv.iterdir():
+            vivenv = ViVenv.load(p.name)
+            vivenvs[vivenv.name] = vivenv
+        return vivenvs
+
+    @staticmethod
+    def _compare_dates(
+        vivenv: ViVenv, date_name: str, when: str, date: datetime
+    ) -> bool:
+        vivenv_date = datetime.strptime(
+            getattr(vivenv.meta, date_name), "%Y-%m-%d %H:%M:%S.%f"
+        )
+        if when == "before":
+            return vivenv_date < date
+        else:
+            return vivenv_date > date
+
+    def _filter_date(self, date_name: str, when: str, date: datetime) -> Set[ViVenv]:
+        return {
+            vivenv
+            for _, vivenv in self.vivenvs.items()
+            if self._compare_dates(
+                vivenv,
+                date_name,
+                when,
+                date,
+            )
+        }
+
+    def _filter_file(self, file: str) -> Set[ViVenv]:
+        if file == "None":
+            return {
+                vivenv for _, vivenv in self.vivenvs.items() if vivenv.files_exist()
+            }
+        else:
+            p = Path(file).absolute().resolve()
+            if not p.is_file():
+                err_quit(f"Unable to find local file: {file}")
+            return {
+                vivenv
+                for _, vivenv in self.vivenvs.items()
+                if str(p) in vivenv.meta.files
+            }
+
+    def _filter_spec(self, spec: str) -> Set[ViVenv]:
+        return {
+            vivenv
+            for _, vivenv in self.vivenvs.items()
+            if spec in ", ".join(vivenv.meta.spec)
+        }
+
+    def filter(self, filters: Dict[str, str]) -> Dict[str, ViVenv]:
+        vivenv_sets = []
+
+        for k, v in filters.items():
+            if "-" in k:  # date-based filters all have hyphen
+                (date_name, when) = k.split("-")
+                vivenv_sets.append(self._filter_date(date_name, when, _parse_date(v)))
+            elif k == "files":
+                vivenv_sets.append(self._filter_file(v))
+
+            elif k == "spec":
+                vivenv_sets.append(self._filter_spec(v))
+        if vivenv_sets:
+            return {vivenv.name: vivenv for vivenv in set.union(*vivenv_sets)}
+        else:
+            return {}
+
+
 class Viv:
     def __init__(self) -> None:
         self.t = Template()
-        self.vivenvs = get_venvs()
+        self._cache = Cache()
+        # compat layer
+        self.vivenvs = self._cache.vivenvs
         self._get_sources()
         self.name = "viv" if self.local else "python3 <(curl -fsSL viv.dayl.in/viv.py)"
 
     def _get_sources(self) -> None:
         self.local_source: Optional[Path] = None
         self.running_source = Path(__file__).resolve()
         self.local = not str(self.running_source).startswith("/proc/")
@@ -1129,15 +1294,17 @@
             self.git = (self.local_source.parent.parent.parent / ".git").is_dir()
         else:
             self.git = False
 
     def _match_vivenv(self, name_id: str) -> ViVenv:  # type: ignore[return]
         matches: List[ViVenv] = []
         for k, v in self.vivenvs.items():
-            if name_id == k or v.name == name_id:
+            if name_id == v.meta.id:
+                matches.append(v)
+            elif name_id == k or v.name == name_id:
                 matches.append(v)
             elif k.startswith(name_id) or (
                 v.meta.id.startswith(name_id) and v.meta.id == v.name
             ):
                 matches.append(v)
             elif v.name.startswith(name_id):
                 matches.append(v)
@@ -1148,33 +1315,36 @@
             err_quit(
                 "matches: " + ",".join((match.name for match in matches)),
                 "too many matches maybe try a longer name?",
             )
         else:
             err_quit(f"no matches found for {name_id}")
 
-    def remove(self, vivenvs: List[str]) -> None:
+    def cmd_cache(self) -> None:
+        """manage the viv vivenv cache"""
+
+    def cmd_cache_remove(self, vivenvs: List[str]) -> None:
         """\
         remove a vivenv
 
         To remove all viv venvs:
-        `viv rm $(viv l -q)`
+        `viv cache remove $(viv l -q)`
         """
 
         for name in vivenvs:
             vivenv = self._match_vivenv(name)
             if vivenv.path.is_dir():
                 log.info(f"removing {vivenv.name}")
                 shutil.rmtree(vivenv.path)
             else:
                 err_quit(
                     f"cowardly exiting because I didn't find vivenv: {name}",
                 )
 
-    def freeze(
+    def cmd_freeze(
         self,
         reqs: List[str],
         requirements: Path,
         keep: bool,
         standalone: bool,
         path: str,
     ) -> None:
@@ -1202,51 +1372,77 @@
             return
 
         if path and not self.local_source:
             err_quit("No local viv found to import from")
 
         sys.stdout.write(self.t.frozen_import(path, self.local_source, spec))
 
-    def list(self, quiet: bool, full: bool, use_json: bool) -> None:
-        """list all vivenvs"""
+    def cmd_list(
+        self,
+        quiet: bool,
+        verbose: bool,
+        use_json: bool,
+        filter: Dict[str, str],
+    ) -> None:
+        """\
+        list vivenvs
+
+        examples:
+          `viv list \\
+              --filter "accessed-after:2023-08-01"`
+          `viv list -q --filter \\
+            "created-before:$(date -d '2 weeks ago' +'%Y-%m-%d')"`
+          `viv list --filter "files:./script.py"`
+          `viv list --filter "files:None"`
+        """
+
+        if filter:
+            vivenvs = self._cache.filter(filter)
+        else:
+            vivenvs = self._cache.vivenvs
 
         if quiet:
-            sys.stdout.write("\n".join(self.vivenvs) + "\n")
-        elif len(self.vivenvs) == 0:
+            sys.stdout.write(
+                "\n".join((vivenv.meta.id for _, vivenv in vivenvs.items())) + "\n"
+            )
+        elif len(self._cache.vivenvs) == 0:
             log.info("no vivenvs setup")
-        elif full:
-            for _, vivenv in self.vivenvs.items():
+        elif len(vivenvs) == 0 and filter:
+            log.info("no vivenvs match filter")
+        elif verbose:
+            for _, vivenv in vivenvs.items():
                 vivenv.tree()
         elif use_json:
             sys.stdout.write(
-                json.dumps({k: v.meta.__dict__ for k, v in self.vivenvs.items()})
+                json.dumps({k: v.meta.__dict__ for k, v in vivenvs.items()})
             )
         else:
-            for _, vivenv in self.vivenvs.items():
+            for _, vivenv in vivenvs.items():
                 vivenv.show()
 
-    def exe(self, vivenv_id: str, cmd: str, rest: List[str]) -> None:
+    def cmd_exe(self, vivenv_id: str, cmd: str, rest: List[str]) -> None:
         """\
         run binary/script in existing vivenv
 
         examples:
             viv exe <vivenv> python -- script.py
             viv exe <vivenv> python -- -m http.server
         """
 
         vivenv = self._match_vivenv(vivenv_id)
         bin = vivenv.path / "bin" / cmd
 
-        vivenv.bin_exists(bin)
+        vivenv.bin_exists(bin.name)
 
         full_cmd = [str(bin), *rest]
 
-        run(full_cmd, verbose=True)
+        # TODO: use subprocess_run_quit
+        subprocess_run(full_cmd, verbose=True)
 
-    def info(self, vivenv_id: str, path: bool, use_json: bool) -> None:
+    def cmd_cache_info(self, vivenv_id: str, path: bool, use_json: bool) -> None:
         """get metadata about a vivenv"""
         vivenv = self._match_vivenv(vivenv_id)
         metadata_file = vivenv.path / "vivmeta.json"
 
         if not metadata_file.is_file():
             err_quit(f"Unable to find metadata for vivenv: {vivenv_id}")
 
@@ -1255,40 +1451,41 @@
         elif path:
             sys.stdout.write(f"{vivenv.path.absolute()}\n")
         else:
             vivenv.tree()
 
     def _install_local_src(self, sha256: str, src: Path, cli: Path, yes: bool) -> None:
         log.info("updating local source copy of viv")
-        shutil.copy(Cache().src / f"{sha256}.py", src)
+        shutil.copy(Cfg().cache_src / f"{sha256}.py", src)
         make_executable(src)
         log.info("symlinking cli")
 
         if cli.is_file():
             log.info(f"Existing file at {a.style(str(cli),'bold')}")
             if confirm("Would you like to overwrite it?", yes=yes):
                 cli.unlink()
                 cli.symlink_to(src)
         else:
+            cli.parent.mkdir(exist_ok=True, parents=True)
             cli.symlink_to(src)
 
         log.info("Remember to include the following line in your shell rc file:")
         sys.stderr.write(
             '  export PYTHONPATH="$PYTHONPATH:$HOME/'
             f'{src.relative_to(Path.home()).parent}"\n'
         )
 
     def _get_new_version(self, ref: str) -> Tuple[str, str]:
-        sys.path.append(str(Cache().src))
+        sys.path.append(str(Cfg().cache_src))
         return (sha256 := fetch_source(ref)), __import__(sha256).__version__
 
-    def manage(self) -> None:
+    def cmd_manage(self) -> None:
         """manage viv itself"""
 
-    def manage_show(
+    def cmd_manage_show(
         self,
         pythonpath: bool = False,
     ) -> None:
         """manage viv itself"""
         if pythonpath:
             if self.local and self.local_source:
                 sys.stdout.write(str(self.local_source.parent) + "\n")
@@ -1300,15 +1497,15 @@
                 self.t.show(
                     cli=shutil.which("viv"),
                     running=self.running_source,
                     local=self.local_source,
                 )
             )
 
-    def manage_update(
+    def cmd_manage_update(
         self,
         ref: str,
         src: Path,
         cli: Path,
         yes: bool,
     ) -> None:
         sha256, next_version = self._get_new_version(ref)
@@ -1327,15 +1524,15 @@
                 Path(
                     src if not self.local_source else self.local_source,
                 ),
                 cli,
                 yes,
             )
 
-    def manage_install(
+    def cmd_manage_install(
         self,
         ref: str,
         src: Path,
         cli: Path,
         yes: bool,
     ) -> None:
         sha256, downloaded_version = self._get_new_version(ref)
@@ -1348,24 +1545,24 @@
         if confirm(
             "Would you like to perform the above installation steps?",
             self.t.install(src, cli),
             yes=yes,
         ):
             self._install_local_src(sha256, src, cli, yes)
 
-    def manage_purge(
+    def cmd_manage_purge(
         self,
         ref: str,
         src: Path,
         cli: Path,
         yes: bool,
     ) -> None:
         to_remove = []
-        if Cache().base.is_dir():
-            to_remove.append(Cache().base)
+        if Cfg().cache_base.is_dir():
+            to_remove.append(Cfg().cache_base)
         if src.is_file():
             to_remove.append(src.parent if src == (Cfg().src) else src)
         if self.local_source and self.local_source.is_file():
             if self.local_source.parent.name == "viv":
                 to_remove.append(self.local_source.parent)
             else:
                 to_remove.append(self.local_source)
@@ -1390,15 +1587,15 @@
                 "`python3 <(curl -fsSL viv.dayl.in/viv.py) manage install`"
             )
 
     def _pick_bin(self, reqs: List[str], bin: str) -> Tuple[str, str]:
         default = re.split(r"[=><~!*]+", reqs[0])[0]
         return default, (default if not bin else bin)
 
-    def shim(
+    def cmd_shim(
         self,
         reqs: List[str],
         requirements: Path,
         bin: str,
         output: Path,
         freeze: bool,
         yes: bool,
@@ -1452,48 +1649,44 @@
 
             if Path(script).is_file():
                 script_text = Path(script).read_text()
             else:
                 script_text = fetch_script(script)
 
             viv_used = uses_viv(script_text)
-            deps = deps_block(script_text)
+            deps = list(read_dependency_block(script_text))
 
-            if viv_used and deps_block:
+            if viv_used and deps:
                 error(
                     "Script Dependencies block and "
                     "`viv` API can't be used in the same script"
                 )
 
             scriptpath.write_text(script_text)
 
             if not keep:
                 env.update({"VIV_CACHE": tmpdir})
                 os.environ["VIV_CACHE"] = tmpdir
 
             if viv_used:
                 env.update({"VIV_SPEC": " ".join(f"'{req}'" for req in spec)})
 
-                sys.exit(
-                    subprocess.run(
-                        [sys.executable, scriptpath, *rest], env=env
-                    ).returncode
-                )
+                subprocess_run_quit([sys.executable, scriptpath, *rest], env=env)
             else:
                 vivenv = ViVenv(spec + deps)
                 if not vivenv.loaded or Env().viv_force:
                     vivenv.create()
                     vivenv.install_pkgs()
 
                 vivenv.touch()
                 vivenv.meta.write()
 
-                sys.exit(subprocess.run([vivenv.python, scriptpath, *rest]).returncode)
+                subprocess_run_quit([vivenv.python, scriptpath, *rest])
 
-    def run(
+    def cmd_run(
         self,
         reqs: List[str],
         requirements: Path,
         script: str,
         keep: bool,
         rest: List[str],
         bin: str,
@@ -1522,192 +1715,198 @@
             if not vivenv.loaded or Env().viv_force:
                 if not keep:
                     with tempfile.TemporaryDirectory(prefix="viv-") as tmpdir:
                         vivenv.set_path(Path(tmpdir))
                         vivenv.create()
                         vivenv.install_pkgs()
                         vivenv.bin_exists(bin)
-                        sys.exit(
-                            subprocess.run(
-                                [vivenv.path / "bin" / bin, *rest]
-                            ).returncode
-                        )
+                        subprocess_run_quit([vivenv.path / "bin" / bin, *rest])
                 else:
                     vivenv.create()
                     vivenv.install_pkgs()
 
             vivenv.touch()
             vivenv.meta.write()
             vivenv.bin_exists(bin)
-            sys.exit(subprocess.run([vivenv.path / "bin" / bin, *rest]).returncode)
+            subprocess_run_quit([vivenv.path / "bin" / bin, *rest])
 
 
 class Arg:
-    def __init__(self, *args: str, **kwargs: Any) -> None:
-        self.args = args
+    def __init__(self, *args: Any, flag: str | None = None, **kwargs: Any) -> None:
+        if flag:
+            self.args: Tuple[Any, ...] = (f"-{flag[0]}", f"--{flag}")
+        else:
+            self.args = args
         self.kwargs = kwargs
 
 
+class BoolArg(Arg):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super(BoolArg, self).__init__(*args, action="store_true", **kwargs)
+
+
+class PathArg(Arg):
+    def __init__(self, *args: Any, **kwargs: Any) -> None:
+        super(PathArg, self).__init__(*args, metavar="<path>", type=Path, **kwargs)
+
+
 class Cli:
-    args = {
+    args: Dict[Tuple[str, ...], List[Arg]] = {
         ("list",): [
-            Arg(
-                "-f",
-                "--full",
-                help="show full metadata for vivenvs",
-                action="store_true",
+            BoolArg(
+                flag="verbose",
+                help="pretty print full metadata for vivenvs",
+            ),
+            BoolArg(
+                flag="quiet",
+                help="show only ids",
             ),
             Arg(
-                "-q",
-                "--quiet",
-                help="suppress non-essential output",
-                action="store_true",
+                flag="filter",
+                help="filter vivenvs based on key:val",
+                metavar="<key:value>",
+                action=KVAppendAction,
+                keys=[
+                    "created-before",
+                    "created-after",
+                    "accessed-before",
+                    "accessed-after",
+                    "files",
+                    "spec",
+                ],
             ),
         ],
         ("shim",): [
-            Arg(
-                "-f",
-                "--freeze",
+            BoolArg(
+                flag="freeze",
                 help="freeze/resolve all dependencies",
-                action="store_true",
             ),
-            Arg(
-                "-o",
-                "--output",
+            PathArg(
+                flag="output",
                 help="path/to/output file",
-                type=Path,
-                metavar="<path>",
             ),
         ],
-        ("info",): [
-            Arg(
-                "-p",
-                "--path",
+        ("cache_info",): [
+            BoolArg(
+                flag="path",
                 help="print the absolute path to the vivenv",
-                action="store_true",
             ),
         ],
-        ("remove",): [
-            Arg("vivenvs", help="name/hash of vivenv", nargs="*", metavar="vivenv")
-        ],
-        ("run",): [
-            Arg("-s", "--script", help="remote script to run", metavar="<script>")
-        ],
-        ("exe", "info"): [
+        ("run",): [Arg(flag="script", help="script to execute", metavar="<path/url>")],
+        ("exe", "cache_info"): [
             Arg("vivenv_id", help="name/hash of vivenv", metavar="vivenv")
         ],
-        ("list", "info"): [
-            Arg(
+        ("list", "cache_info"): [
+            BoolArg(
                 "--json",
                 help="name:metadata json for vivenvs ",
-                action="store_true",
                 default=False,
                 dest="use_json",
             )
         ],
         ("freeze", "shim"): [
             Arg(
-                "-p",
-                "--path",
+                flag="path",
                 help="generate line to add viv to sys.path",
                 choices=["abs", "rel"],
             ),
-            Arg(
-                "-s",
-                "--standalone",
+            BoolArg(
+                flag="standalone",
                 help="generate standalone activation function",
-                action="store_true",
             ),
         ],
         ("run", "freeze", "shim"): [
             Arg("reqs", help="requirements specifiers", nargs="*"),
-            Arg(
-                "-r",
-                "--requirements",
+            PathArg(
+                flag="requirements",
                 help="path/to/requirements.txt file",
-                metavar="<path>",
-                type=Path,
             ),
         ],
         ("run", "freeze"): [
-            Arg(
-                "-k",
-                "--keep",
+            BoolArg(
+                flag="keep",
                 help="preserve environment",
-                action="store_true",
             ),
         ],
         ("run", "shim"): [
-            Arg("-b", "--bin", help="console_script/script to invoke", metavar="<bin>"),
+            Arg(flag="bin", help="console_script/script to invoke", metavar="<bin>"),
         ],
-        ("manage|purge", "manage|update", "manage|install"): [
+        ("manage_purge", "manage_update", "manage_install"): [
             Arg(
-                "-r",
-                "--ref",
+                flag="ref",
                 help="git reference (branch/tag/commit)",
                 default="latest",
                 metavar="<ref>",
             ),
-            Arg(
-                "-s",
-                "--src",
+            PathArg(
+                flag="src",
                 help="path/to/source_file",
                 default=Cfg().src,
-                metavar="<src>",
             ),
-            Arg(
-                "-c",
-                "--cli",
+            PathArg(
+                flag="cli",
                 help="path/to/cli (symlink to src)",
                 default=Path.home() / ".local" / "bin" / "viv",
-                metavar="<cli>",
             ),
         ],
-        ("shim", "manage|purge", "manage|update", "manage|install"): [
-            Arg("-y", "--yes", help="respond yes to all prompts", action="store_true")
+        ("shim", "manage_purge", "manage_update", "manage_install"): [
+            BoolArg(flag="yes", help="respond yes to all prompts")
         ],
-        ("manage|show",): [
-            Arg(
-                "-p",
-                "--pythonpath",
+        ("manage_show",): [
+            BoolArg(
+                flag="pythonpath",
                 help="show the path/to/install",
-                action="store_true",
             )
         ],
         ("exe",): [
             Arg(
                 "cmd",
                 help="command to to execute",
             )
         ],
+        ("cache_remove",): [
+            Arg("vivenvs", help="name/hash of vivenv", nargs="*", metavar="vivenv")
+        ],
     }
     (
         cmds := dict.fromkeys(
             (
                 "list",
                 "shim",
                 "run",
                 "exe",
-                "remove",
+                "cache",
                 "freeze",
-                "info",
                 "manage",
             )
         )
     ).update(
         {
-            "manage": {
+            cmd: {
                 subcmd: {"help": help, "aliases": [subcmd[0]]}
-                for subcmd, help in (
-                    ("show", "show current installation"),
-                    ("install", "install fresh viv"),
-                    ("update", "update viv version"),
-                    ("purge", "remove traces of viv"),
-                )
+                for subcmd, help in subcmd_help
             }
+            for cmd, subcmd_help in (
+                (
+                    "cache",
+                    (
+                        ("info", "get metadata about a vivenv"),
+                        ("remove", "remove a vivenv"),
+                    ),
+                ),
+                (
+                    "manage",
+                    (
+                        ("show", "show current installation"),
+                        ("install", "install fresh viv"),
+                        ("update", "update viv version"),
+                        ("purge", "remove traces of viv"),
+                    ),
+                ),
+            )
         }
     )
 
     def __init__(self, viv: Viv) -> None:
         self.viv = viv
         self.parser = ArgumentParser(
             prog=viv.name, description=viv.t.description(viv.name)
@@ -1774,32 +1973,29 @@
                     + " shouldn't be used with a git-based installation",
                 )
 
         if name == "run":
             if not (args.reqs or args.script):
                 error("must specify a requirement or --script")
 
-        if name == "info":
+        if name == "cache_info":
             if args.use_json and args.path:
                 error("--json and -p/--path are mutually exclusive")
 
     def _get_subcmd_parser(
         self,
         subparsers: _SubParsersAction[ArgumentParser],
         name: str,
         attr: Optional[str] = None,
         **kwargs: Any,
     ) -> ArgumentParser:
-        # override for remove
-        if name == "remove":
-            aliases = ["rm"]
-        else:
-            aliases = kwargs.pop("aliases", [name[0]])
+        aliases = kwargs.pop("aliases", [name[0]])
+
+        cmd = getattr(self.viv, attr if attr else f"cmd_{name}")
 
-        cmd = getattr(self.viv, attr if attr else name)
         parser: ArgumentParser = subparsers.add_parser(
             name,
             help=cmd.__doc__.splitlines()[0],
             description=dedent(cmd.__doc__),
             aliases=aliases,
             **kwargs,
         )
@@ -1826,33 +2022,33 @@
                     title="subcommand", metavar="<sub-cmd>", required=True
                 )
                 for subcmd, kwargs in subcmds.items():
                     subcmd_cmd_p.add_parser(
                         subcmd,
                         parents=[
                             self.parsers[k]
-                            for k in self.cmd_arg_group_map[f"{cmd}|{subcmd}"]
+                            for k in self.cmd_arg_group_map[f"{cmd}_{subcmd}"]
                         ],
                         **kwargs,
-                    ).set_defaults(func=getattr(self.viv, f"{cmd}_{subcmd}"))
+                    ).set_defaults(func=getattr(self.viv, f"cmd_{cmd}_{subcmd}"))
 
             else:
                 self._get_subcmd_parser(
                     cmd_p,
                     cmd,
                     parents=[self.parsers.get(k) for k in self.cmd_arg_group_map[cmd]],
                 )
 
         if "--" in sys.argv:
             i = sys.argv.index("--")
             args = self.parser.parse_args(sys.argv[1:i])
             args.rest = sys.argv[i + 1 :]
         else:
             args = self.parser.parse_args()
-            if args.func.__name__ in ("run", "exe"):
+            if args.func.__name__ in ("cmd_run", "cmd_exe"):
                 args.rest = []
 
         self._validate_args(args)
         func = args.__dict__.pop("func")
         func(
             **vars(args),
         )
```

### Comparing `viv-23.8a1/PKG-INFO` & `viv-23.8a3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: viv
-Version: 23.8a1
+Version: 23.8a3
 Summary: viv isn't venv
+Home-page: https://github.com/daylinmorgan/viv
+Author-Email: Daylin Morgan <daylinmorgan@gmail.com>
 License: MIT
-Author-email: Daylin Morgan <daylinmorgan@gmail.com>
-Requires-Python: >= 3.8
-Project-URL: homepage, https://github.com/daylinmorgan/viv
-Project-URL: repository, https://github.com/daylinmorgan/viv
+Project-URL: Homepage, https://github.com/daylinmorgan/viv
+Project-URL: Repository, https://github.com/daylinmorgan/viv
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
   <a href="https://github.com/daylinmorgan/viv">
     <img src="https://raw.githubusercontent.com/daylinmorgan/viv/main/assets/logo.svg" alt="Logo" width=500 >
   </a>
   <p align="center">
@@ -80,15 +81,15 @@
 ```python
 __import__("viv").use("click")
 ```
 
 To remove all `vivenvs` you can use the below command:
 
 ```sh
-viv remove $(viv list -q)
+viv cache remove $(viv list -q)
 ```
 
 To remove `viv` all together you can use the included `purge` command:
 
 ```sh
 python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge
 ```
@@ -139,8 +140,7 @@
 ├── argcomplete>=1.9.4 (2.1.1)
 ├── packaging>=20.0 (23.0)
 └── userpath>=1.6.0 (1.8.0)
     └── click (8.1.3)
 ```
 
 [^1]: You do need to have `pip` but surely you have `pip` already.
-
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: viv Version: 23.8a1 Summary: viv isn't venv
-License: MIT Author-email: Daylin Morgan
-gmail.com> Requires-Python: >= 3.8 Project-URL: homepage, https://github.com/
-daylinmorgan/viv Project-URL: repository, https://github.com/daylinmorgan/viv
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: viv Version: 23.8a3 Summary: viv isn't venv Home-
+page: https://github.com/daylinmorgan/viv Author-Email: Daylin Morgan
+gmail.com> License: MIT Project-URL: Homepage, https://github.com/daylinmorgan/
+viv Project-URL: Repository, https://github.com/daylinmorgan/viv Requires-
+Python: >=3.8 Description-Content-Type: text/markdown
                                     [Logo]
                          ****** viv isn't venv ******
                                [cli screenshot]
                                  Documentation
 Try before you buy! ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) run pycowsay
 -- "viv isn't venv\!" ``` --- `Viv` is a standalone dependency-free `venv`
 creator [^1]. `Viv` helps you ignore silly things like managing temporary or
@@ -25,26 +25,26 @@
 customize this with `--src`. ```sh export PYTHONPATH="$PYTHONPATH:$HOME/.local/
 share/viv" ``` ### Pypi (Not Recommended) ```sh pip install viv ``` Why is this
 *not recommended*? Mainly, because `viv` is all about hacking your `sys.path`.
 Placing it in it's own virtual environment or installing in a user site
 directory may complicate this endeavor. ## Usage In any python script with
 external dependencies you can add this line, to automate `vivenv` creation and
 installation of dependencies. ```python __import__("viv").use("click") ``` To
-remove all `vivenvs` you can use the below command: ```sh viv remove $(viv list
--q) ``` To remove `viv` all together you can use the included `purge` command:
-```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge ``` ## Additional
-Features An experimental feature of `viv` is generating shim's that leverage
-the principles of `viv`. These shims would operate similar to `pipx` in which
-you can specify a command line app to "install". *Note* that `--standalone`
-will auto-generate a mini function version of `viv` to accomplish the same
-basic task as using a local copy of `viv`. After generating this standalone
-`shim` you can freely use this script across unix machines which have
-`python>3.8`. See [examples/black](https://github.com/daylinmorgan/viv/blob/
-dev/examples/black) for output of below command. ```sh python3 <(curl -fsSL
-viv.dayl.in/viv.py) shim black -o ./black --standalone --freeze ``` ##
+remove all `vivenvs` you can use the below command: ```sh viv cache remove $
+(viv list -q) ``` To remove `viv` all together you can use the included `purge`
+command: ```sh python3 <(curl -fsSL viv.dayl.in/viv.py) manage purge ``` ##
+Additional Features An experimental feature of `viv` is generating shim's that
+leverage the principles of `viv`. These shims would operate similar to `pipx`
+in which you can specify a command line app to "install". *Note* that `--
+standalone` will auto-generate a mini function version of `viv` to accomplish
+the same basic task as using a local copy of `viv`. After generating this
+standalone `shim` you can freely use this script across unix machines which
+have `python>3.8`. See [examples/black](https://github.com/daylinmorgan/viv/
+blob/dev/examples/black) for output of below command. ```sh python3 <(curl -
+fsSL viv.dayl.in/viv.py) shim black -o ./black --standalone --freeze ``` ##
 Alternatives ### [pip-run](https://github.com/jaraco/pip-run) ```sh pip-run
 (10.0.5) âââ autocommand (2.2.2) âââ jaraco-context (4.3.0)
 âââ jaraco-functools (3.6.0) â âââ more-itertools (9.1.0)
 âââ jaraco-text (3.11.1) â âââ autocommand (2.2.2) â âââ
 inflect (6.0.2) â â âââ pydantic>=1.9.1 (1.10.5) â â âââ
 typing-extensions>=4.2.0 (4.5.0) â âââ jaraco-context>=4.1 (4.3.0) â
 âââ jaraco-functools (3.6.0) â â âââ more-itertools (9.1.0) â
```

