# Comparing `tmp/arch_github_package-0.0.3.tar.gz` & `tmp/arch_github_package-0.0.4.tar.gz`

## Comparing `arch_github_package-0.0.3.tar` & `arch_github_package-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/arch_github_package/__init__.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/arch_github_package/gh.py
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/arch_github_package/main.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/arch_github_package/pm.py
--rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/arch_github_package/state.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/LICENSE
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/README.md
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 arch_github_package-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/__init__.py
+-rw-r--r--   0        0        0     2550 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/gh.py
+-rw-r--r--   0        0        0     3317 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/main.py
+-rw-r--r--   0        0        0     4296 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/pm.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/arch_github_package/state.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/README.md
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 arch_github_package-0.0.4/PKG-INFO
```

### Comparing `arch_github_package-0.0.3/arch_github_package/main.py` & `arch_github_package-0.0.4/arch_github_package/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from .gh import Releases
 from .pm import Pkgbuild
-from .state import State, Package
+from .state import State
 
 from typing import Optional, Annotated
 import typer
 from tabulate import tabulate
 import subprocess
 
 
 app = typer.Typer()
 
 
 def install_or_upgrade(releases: Releases, pkgbuild: Pkgbuild):
-    print('Downloading tarball...')
     tarball_name = releases.download_tarball(pkgbuild.get_build_dir())
-
-    print('Installing...')
-    pkgbuild.create_pkgbuild(tarball_name, 'SKIP')
+    pkgbuild.create_pkgbuild(tarball_name, "SKIP")
     pkgbuild.build_and_install()
     pkgbuild.cleanup()
 
 
 @app.command()
 def list():
     with State() as state:
@@ -28,18 +25,19 @@
         table = [[pkg.package_name, pkg.repo, pkg.version, pkg.publish_date] for pkg in packages]
         print(tabulate(table, headers=["Package","Repo", "Version", "Date"]))
 
 
 @app.command()
 def install(repo: str):
     with State() as state:
+        print(f"Fetching releases from {repo}...")
         releases = Releases(repo)
         pkgbuild = Pkgbuild(releases.get_repo_name(), releases.get_project_name(), releases.get_project_description(), releases.get_latest_version())
 
-        print(f'Installing {repo} {releases.get_latest_version()} as {pkgbuild.get_pkgname()}')
+        print(f"Installing {repo} {releases.get_latest_version()} as {pkgbuild.get_pkgname()}\n")
         install_or_upgrade(releases, pkgbuild)
 
         state.new_package(pkgbuild.get_pkgname(), repo, releases.get_latest_version(), releases.get_publish_date())
 
 
 @app.command()
 def upgrade(package: Annotated[Optional[str], typer.Argument()] = None):
@@ -66,32 +64,31 @@
                          releases and releases.get_latest_version(), releases and releases.get_publish_date()] for pkg, releases in packages],
                        headers=["Package", "Repo", "Old Version", "Date", "New Version", "Date"]))
         
         if num_updates == 0:
             print("\nNo updates available")
             return
         
-        if not typer.confirm(f"\nUpgrade {num_updates} packages?", default=True):
-            return
-
+        typer.confirm(f"\nUpgrade {num_updates} packages?", default=True, abort=True)
+            
         for pkg, releases in packages:
             if releases is None:
                 continue
             
-            print(f'Upgrading {pkg.package_name} from {pkg.version} to {releases.get_latest_version()}')
+            print(f"Upgrading {pkg.package_name} from {pkg.version} to {releases.get_latest_version()}")
             pkgbuild = Pkgbuild(releases.get_repo_name(), releases.get_project_name(), releases.get_project_description(), releases.get_latest_version())
             install_or_upgrade(releases, pkgbuild)
             state.update_package(pkg.package_name, releases.get_latest_version(), releases.get_publish_date())
 
 
 @app.command()
 def uninstall(package: str):
     with State() as state:
         p = state.get_package(package)
-        ret = subprocess.call(['sudo', 'pacman', '-R', package])
+        ret = subprocess.call(["sudo", "pacman", "-R", package])
         if ret != 0:
             raise Exception("Failed to uninstall package")
         state.remove_package(package)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `arch_github_package-0.0.3/arch_github_package/pm.py` & `arch_github_package-0.0.4/arch_github_package/pm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,103 +1,120 @@
+import typer
 from pathlib import Path
 import tempfile
 import tarfile
 import zipfile
+import gzip
 import shutil
 import subprocess
-import filetype
+import re
+import shutil
 
 
 class Pkgbuild:
     def __init__(self, repo, project_name, project_description, version):
         self.repo = repo
-        self.pkgname = project_name + '-github'
+        self.pkgname = project_name + "-github"
         self.pkgdesc = project_description
         self.pkgver = version
-        self.build_dir = Path(tempfile.mkdtemp(prefix='pkgbuild-'+self.pkgname+"-"))
-        self.maintainer = 'arch-github-package <https://github.com/jinliu/arch-github-package>'
+        self.build_dir = Path(tempfile.mkdtemp(prefix="pkgbuild-"+self.pkgname+"-"))
+        self.maintainer = "arch-github-package <https://github.com/jinliu/arch-github-package>"
 
     def get_build_dir(self):
         return self.build_dir
     
     def create_pkgbuild(self, tarball_name, sha256sum):
         pkgbuild = \
-f'''# Maintainer: {self.maintainer}
+f"""# Maintainer: {self.maintainer}
 pkgname={self.pkgname}
 pkgver={self.pkgver}
 pkgrel=1
-pkgdesc='{self.pkgdesc}'
+pkgdesc='{re.escape(self.pkgdesc)}'
 arch=('x86_64')
 url="https://github.com/{self.repo}"
 license=('custom')
 source=({tarball_name})
 sha256sums=('{sha256sum}')
 package() {{
-'''
+"""
 
-        p = Path(self.build_dir/'inspect')
+        print("\nInspecting tarball...\n")
+        p = Path(self.build_dir/"inspect")
         p.mkdir()
-        if tarball_name.endswith('.zip'):
+        if tarball_name.endswith(".zip"):
             zipfile.ZipFile(self.build_dir/tarball_name).extractall(p)
         else:
-            tarfile.open(self.build_dir/tarball_name).extractall(p)
+            try:
+                tarfile.open(self.build_dir/tarball_name).extractall(p)
+            except:
+                if tarball_name.endswith(".gz"):
+                    with gzip.open(self.build_dir/tarball_name, "rb") as f_in:
+                        (p/tarball_name.removesuffix(".gz")).write_bytes(f_in.read())
+                else:
+                    shutil.copy(self.build_dir/tarball_name, p)
 
         # descent into single directory
         d = list(p.iterdir())
         while len(d) == 1 and d[0].is_dir():
             d = list(d[0].iterdir())
 
         for f in d:
             if not f.is_dir():
                 mod = f.stat().st_mode
-                mime = None
-                t = filetype.guess(f)
-                if t is not None:
-                    mime = t.mime
+                mime = ""
+                ret = subprocess.run(["file", "-b", "--mime-type", f], capture_output=True)
+                if ret:
+                    mime = ret.stdout.decode("utf-8").strip()
 
                 # executable?
-                if mod & 0o111 or mime == 'application/x-executable':
+                if mod & 0o111 or "executable" in mime or "shellscript" in mime:
                     pkgbuild += f"    install -Dm755 {f} -t \"$pkgdir/usr/bin/\"\n"
+                    print(f"{f.name} -> /usr/bin/{f.name}")
                     continue
 
-                if f.name == 'LICENSE':
+                if f.name.startswith("LICENSE"):
                     pkgbuild += f"    install -Dm644 {f} -t \"$pkgdir/usr/share/licenses/$pkgname\"\n"
+                    print(f"{f.name} -> /usr/share/licences/{self.pkgname}/{f.name}")
                     continue
 
-                if f.name.startswith('README'):
+                if f.name.endswith(".md") or f.name.startswith("README") or f.name.startswith("CHANGELOG"):
                     pkgbuild += f"    install -Dm644 {f} -t \"$pkgdir/usr/share/doc/$pkgname\"\n"
+                    print(f"{f.name} -> /usr/share/doc/{self.pkgname}/{f.name}")
                     continue
 
                 # manpage?
                 matched = False
                 for section in range(1, 10):
                     if f.name.endswith(f".{section}.gz"):
                         pkgbuild += f"    install -Dm644 {f} -t \"$pkgdir/usr/share/man/man{section}/$pkgname\"\n"
+                        print(f"{f.name} -> /usr/share/man/man{section}/{f.name}")
                         matched = True
                         break
                 if matched:
                     continue
 
-                print(f"Unknown file type, skipped: {f}")
+                print(f"{f.name} -> Unknown file type {mime}, skipped.")
         
         pkgbuild += "}\n"
 
-        (self.build_dir/'PKGBUILD').write_text(pkgbuild)
+        typer.confirm("\nIs this OK?", default=True, abort=True)
+
+        (self.build_dir/"PKGBUILD").write_text(pkgbuild)
 
     def get_pkgname(self):
         return self.pkgname
 
     def build_and_install(self):
-        if subprocess.call(['makepkg', '-si'], cwd=self.build_dir, env={'PACKAGER': self.maintainer}) != 0:
+        if subprocess.call(["makepkg", "-si"], cwd=self.build_dir, env={"PACKAGER": self.maintainer}) != 0:
             raise Exception("Failed to build package")
 
     def cleanup(self):
         shutil.rmtree(self.get_build_dir())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     import gh
-    r = gh.Releases('zix99/rare')
+    r = gh.Releases("zix99/rare")
     p = Pkgbuild(r.get_repo_name(), r.get_project_name(), r.get_project_description(), r.get_latest_version())
     tarball_name = r.download_tarball(p.get_build_dir())
-    p.create_pkgbuild(tarball_name, 'SKIP')
+    p.create_pkgbuild(tarball_name, "SKIP")
     print(p.get_build_dir())
```

### Comparing `arch_github_package-0.0.3/arch_github_package/state.py` & `arch_github_package-0.0.4/arch_github_package/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,36 +5,36 @@
 
 
 class Package:
     @staticmethod
     def load(state_dir, package_name):
         config = configparser.ConfigParser()
         config.read(Path(state_dir)/package_name)
-        c = config['DEFAULT']
-        return Package(package_name, c['repo'], c['version'], c['publish_date'])
+        c = config["DEFAULT"]
+        return Package(package_name, c["repo"], c["version"], c["publish_date"])
         
     def __init__(self, package_name, repo, version, publish_date):
         self.package_name = package_name
         self.repo = repo
         self.version = version
         self.publish_date = publish_date
 
     def save(self, state_dir):
         config = configparser.ConfigParser()
-        c = config['DEFAULT']
-        c['repo'] = self.repo
-        c['version'] = self.version
-        c['publish_date'] = self.publish_date
-        with open(state_dir/self.package_name, 'w') as f:
+        c = config["DEFAULT"]
+        c["repo"] = self.repo
+        c["version"] = self.version
+        c["publish_date"] = self.publish_date
+        with open(state_dir/self.package_name, "w") as f:
             config.write(f)
 
 
 class State:
     def __init__(self):
-        self.state_dir = Path.home()/'.local/share/arch-github-package'
+        self.state_dir = Path.home()/".local/share/arch-github-package"
         self.state_dir.mkdir(parents=True, exist_ok=True)
 
     def __enter__(self):
         self.state_dir_fd = os.open(self.state_dir, os.O_RDONLY)
         fcntl.flock(self.state_dir_fd, fcntl.LOCK_EX)
         return self
```

### Comparing `arch_github_package-0.0.3/.gitignore` & `arch_github_package-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.3/LICENSE` & `arch_github_package-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `arch_github_package-0.0.3/README.md` & `arch_github_package-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,17 +19,19 @@
 ```
 
 pipx installs the package in a virtualenv, so it doesn't pollute your system.
 
 You can also use pip:
 
 ```bash
-pip install --user arch-github-package
+pip install --user --break-system-packages arch-github-package
 ```
 
+(This will install the package in your user site-packages, not really breaking system packages.)
+
 ## Usage
 
 ### Install a package
 
 ```bash
 agp install <github-repo>
 ```
@@ -48,15 +50,16 @@
    for keywords like "linux", "x86-64", "x86_64", "amd64", "gnu" in
    the release assets.
 
 1. It downloads the tarball, extracts it, and tries to dertermine which
    file goes where. E.g.:
    * If a file is ELF, or its x modbit is set, it goes to `/usr/bin`.
    * Files like *.1.gz go to `/usr/share/man`.
-   * LICENSE and README.* go to `/usr/share/doc/<package-name>`.
+   * README.* go to `/usr/share/doc/<package-name>`.
+   * LICENSE goes to `/usr/share/licenses/<package-name>`.
 
 1. It creates a PKGBUILD file, and runs `makepkg -si` to build and install it.
    The package name is `<github-project-name>-github`. E.g., `ortesi/devd` becomes
    `devd-github`.
 
 ### List installed packages
 
@@ -68,14 +71,17 @@
 
 ```bash
 agp upgrade
 ```
 
 You can also use `agp upgrade <package-name>` to upgrade a single package.
 
+Note: if you run this command repeatively in quick succession, it will hit
+GitHub's rate limit for anonymous API access.
+
 ### Uninstall a package
 
 ```bash
 agp uninstall <package-name>
 ```
 
 If you uninstall an -github package with `pacman`, it will still be listed by `agp list`.
```

### Comparing `arch_github_package-0.0.3/pyproject.toml` & `arch_github_package-0.0.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "arch-github-package"
-version = "0.0.3"
+version = "0.0.4"
 description = "Convert GitHub project releases to Archlinux package, with autoupdate."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   { name="Jin Liu", email="m.liu.jin@gmail.com" },
 ]
 keywords = ["arch", "archlinux", "AUR", "github", "package", "package-manager"]
@@ -16,15 +16,14 @@
     "Operating System :: POSIX :: Linux",
     "Topic :: System"
 ]
 dependencies = [
   "typer==0.9.*",
   "PyGithub==1.58.*",
   "tabulate==0.9.*",
-  "filetype==1.2.*",
 ]
 
 [project.urls]
 "Repository" = "https://github.com/jinliu/arch-github-package"
 "Bug Tracker" = "https://github.com/jinliu/arch-github-package/issues"
 
 [project.scripts]
```

### Comparing `arch_github_package-0.0.3/PKG-INFO` & `arch_github_package-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: arch-github-package
-Version: 0.0.3
+Version: 0.0.4
 Summary: Convert GitHub project releases to Archlinux package, with autoupdate.
 Project-URL: Repository, https://github.com/jinliu/arch-github-package
 Project-URL: Bug Tracker, https://github.com/jinliu/arch-github-package/issues
 Author-email: Jin Liu <m.liu.jin@gmail.com>
 License-File: LICENSE
 Keywords: AUR,arch,archlinux,github,package,package-manager
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System
 Requires-Python: >=3.7
-Requires-Dist: filetype==1.2.*
 Requires-Dist: pygithub==1.58.*
 Requires-Dist: tabulate==0.9.*
 Requires-Dist: typer==0.9.*
 Description-Content-Type: text/markdown
 
 # arch-github-package
 
@@ -41,17 +40,19 @@
 ```
 
 pipx installs the package in a virtualenv, so it doesn't pollute your system.
 
 You can also use pip:
 
 ```bash
-pip install --user arch-github-package
+pip install --user --break-system-packages arch-github-package
 ```
 
+(This will install the package in your user site-packages, not really breaking system packages.)
+
 ## Usage
 
 ### Install a package
 
 ```bash
 agp install <github-repo>
 ```
@@ -70,15 +71,16 @@
    for keywords like "linux", "x86-64", "x86_64", "amd64", "gnu" in
    the release assets.
 
 1. It downloads the tarball, extracts it, and tries to dertermine which
    file goes where. E.g.:
    * If a file is ELF, or its x modbit is set, it goes to `/usr/bin`.
    * Files like *.1.gz go to `/usr/share/man`.
-   * LICENSE and README.* go to `/usr/share/doc/<package-name>`.
+   * README.* go to `/usr/share/doc/<package-name>`.
+   * LICENSE goes to `/usr/share/licenses/<package-name>`.
 
 1. It creates a PKGBUILD file, and runs `makepkg -si` to build and install it.
    The package name is `<github-project-name>-github`. E.g., `ortesi/devd` becomes
    `devd-github`.
 
 ### List installed packages
 
@@ -90,14 +92,17 @@
 
 ```bash
 agp upgrade
 ```
 
 You can also use `agp upgrade <package-name>` to upgrade a single package.
 
+Note: if you run this command repeatively in quick succession, it will hit
+GitHub's rate limit for anonymous API access.
+
 ### Uninstall a package
 
 ```bash
 agp uninstall <package-name>
 ```
 
 If you uninstall an -github package with `pacman`, it will still be listed by `agp list`.
```

