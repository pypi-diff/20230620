# Comparing `tmp/rhdndat-2.6.7.tar.gz` & `tmp/rhdndat-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhdndat-2.6.7.tar", max compression
+gzip compressed data, was "rhdndat-2.6.8.tar", max compression
```

## Comparing `rhdndat-2.6.7.tar` & `rhdndat-2.6.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35150 2022-09-11 11:27:41.980306 rhdndat-2.6.7/LICENSE.txt
--rw-r--r--   0        0        0     7993 2022-09-11 11:27:41.980306 rhdndat-2.6.7/README.rst
--rw-r--r--   0        0        0      921 2022-09-11 11:27:41.980306 rhdndat-2.6.7/pyproject.toml
--rw-r--r--   0        0        0       22 2022-09-11 11:27:41.980306 rhdndat-2.6.7/rhdndat/__init__.py
--rw-r--r--   0        0        0    39211 2022-09-11 11:27:41.980306 rhdndat-2.6.7/rhdndat/__main__.py
--rw-r--r--   0        0        0     9152 2022-09-11 11:27:52.282227 rhdndat-2.6.7/setup.py
--rw-r--r--   0        0        0     9084 2022-09-11 11:27:52.283485 rhdndat-2.6.7/PKG-INFO
+-rw-r--r--   0        0        0    35150 2023-06-19 22:58:08.265606 rhdndat-2.6.8/LICENSE.txt
+-rw-r--r--   0        0        0     7909 2023-06-19 22:58:08.265606 rhdndat-2.6.8/README.rst
+-rw-r--r--   0        0        0      904 2023-06-19 22:58:08.265606 rhdndat-2.6.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-19 22:58:08.265606 rhdndat-2.6.8/rhdndat/__init__.py
+-rw-r--r--   0        0        0    39110 2023-06-19 22:58:08.265606 rhdndat-2.6.8/rhdndat/__main__.py
+-rw-r--r--   0        0        0     9054 2023-06-19 22:58:17.451535 rhdndat-2.6.8/setup.py
+-rw-r--r--   0        0        0     8975 2023-06-19 22:58:17.452594 rhdndat-2.6.8/PKG-INFO
```

### Comparing `rhdndat-2.6.7/LICENSE.txt` & `rhdndat-2.6.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rhdndat-2.6.7/README.rst` & `rhdndat-2.6.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 **rhdndat** finds ``rhdndat.ver`` files to check for romhacking.net updates
 
 A version file is named ``rhdndat.ver`` and has a version number line followed by a romhacking.net url line, repeated. These correspond to each hack or translation. To check for needed updates to version file, if any patch version in the file does not match the version on the romhacking.net patch page, it presents a warning.
 
 **rhdndat-rn** renames files and patches to new .DAT [1]_ [2]_ rom names if it can find the rom checksum in those .DAT files and memorizes the checksum of the 'original rom' as a extended attribute ``user.rhdndat.rom_sha1`` to speed up renaming in subsequent executions (in unix, not windows).
 
-To find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (i don't know of any emulator that supports softpatching for those, except those that support delta chd).
+To find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (since delta chd support is rare).
 
-rhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a name that is existing file in the rom directory.
+rhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a existing file in the rom directory.
 
 Besides bare rom files, files affected by renames are compressed wii/gamecube .rvz files, .cue/.toc/.gdi (treated especially to not ask for every track), the softpatch types .ips, .bps, .ups, including the new retroarch multiple softpatch convention (a number after the softpatch extension), .rxdelta, .pal NES color palettes, and sbi subchannel data files.
 
 ``nes fds lnx a78`` roms require headers and are hardcoded to ignore headers when calculating ``user.rhdndat.rom_sha1`` to match the no-intro dat checksums that checksum everything except the header. This is problematic for hacks, where you can 'verify' a file is the right rom, but the hack was created for a rom with another header. A solution that keeps the softpatch is tracking down the right rom, hardpatching it, and creating a softpatch from the current no-intro rom to the older patched rom. For sfc and pce ips hacks that target a headered rom I recommend ipsbehead to change the patch to target the no-header rom.
 
 Requires xdelta3 (to process rxdelta) and dolphin-tool (to operate on rvz files) on path or the same directory.
```

### Comparing `rhdndat-2.6.7/pyproject.toml` & `rhdndat-2.6.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 [tool.poetry]
 name = "rhdndat"
-version = "2.6.7"
+version = "2.6.8"
 description = "www.romhacking.net update checker"
 authors = ["i30817 <i30817@gmail.com>"]
 license = "GNU General Public License v3.0"
 readme = "README.rst"
 repository = "https://github.com/i30817/rhdndat"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 beautifulsoup4 = "^4.10.0"
 questionary = "^1.10.0"
 typer = "^0.5.0"
 colorama = "^0.4.4"
 lxml = "^4.9.1"
-chd-rs-py = "^*"
 xattr = [
     { version = "^0.9.9", markers = "sys_platform != 'win32'" },
 ]
 
 [tool.poetry.scripts]
 rhdndat = 'rhdndat.__main__:main'
 rhdndat-rn = 'rhdndat.__main__:rename'
```

### Comparing `rhdndat-2.6.7/rhdndat/__main__.py` & `rhdndat-2.6.8/rhdndat/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         if old != new and old.exists():
             if new.exists():
                 print_err(new)
             else:
                 torename_main.append((old, new))
     #if it has index text, it has tracks
     if index_txt:
-        roms_json = game.find_all('rom') #these invariants (first entry is indexfile) were already tested
+        roms_json = game.find_all('rom') #invariants were checked (first entry is indexfile and len(files) == len(roms_json))
         roms_json.pop(0)                 #remove the cue/gdi/toc since it was renamed above
         #check tracks
         for oldtrc, r_json in zip(files, roms_json):
             #oldtrc is absolute, so newtrc is too. Tracks do not use 'newrom' for the name but the dat entry
             newtrc = oldtrc.with_name(r_json.get('name'))
             for old, new in ( (oldtrc, newtrc), (oldtrc.with_suffix('.rxdelta'), newtrc.with_suffix('.rxdelta')) ):
                 if old != new and old.exists():
@@ -301,17 +301,17 @@
             verbose: bool = typer.Option(False, '--verbose', help='Print more information about skipped roms.')
             ):
     """
     rom renamer
     
     rhdndat-rn renames files and patches to new .DAT¹² rom names if it can find the rom checksum in those .DAT files and memorizes the checksum of the 'original rom' as a extended attribute user.rhdndat.rom_sha1 to speed up renaming in subsequent executions (in unix, not windows).
 
-    To find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (i don't know of any emulator that supports softpatching for those, except those that support delta chd).
+    To find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (since delta chd support is rare).
 
-    rhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a name that is existing file in the rom directory.
+    rhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a existing file in the rom directory.
 
     Besides bare rom files, files affected by renames are compressed wii/gamecube .rvz files, .cue/.toc/.gdi (treated especially to not ask for every track), the softpatch types .ips, .bps, .ups, including the new retroarch multiple softpatch convention (a number after the softpatch extension), .rxdelta, .pal NES color palettes, and sbi subchannel data files.
     
     'nes fds lnx a78' roms require headers and are hardcoded to ignore headers when calculating 'user.rhdndat.rom_sha1' to match the no-intro dat checksums that checksum everything except the header. This is problematic for hacks, where you can 'verify' a file is the right rom, but the hack was created for a rom with another header. A solution that keeps the softpatch is tracking down the right rom, hardpatching it, and creating a softpatch from the current no-intro rom to the older patched rom. For sfc and pce ips hacks that target a headered rom I recommend ipsbehead³ to change the patch to target the no-header rom.
 
     Requires xdelta3⁴ (to process rxdelta) and dolphin-tool⁵ (to operate on rvz files) on path or the same directory.
     
@@ -403,34 +403,38 @@
                     continue
                 #instead of considering just the 'rom' file, consider also all file referenced inside cue or gdi or toc
                 #since toc and cue can have a single 'file' but multiple 'tracks' this needs a ordered set
                 if rom.suffix == '.gdi':
                     regex = '"(.*)"'
                 else:
                     regex = 'FILE\s+"(.*)"'
+                class TrackAlreadyCheckedError(ValueError):
+                    '''already checked'''
                 def track_constructor(st):
                     tmp = Path(st)
-                    if tmp.is_absolute():
-                        return tmp.resolve()
-                    return Path(rom.parent, tmp).resolve()
-                files = list(map( track_constructor, OrderedDict.fromkeys(re.findall(regex, index_txt)).keys() ))
-                #set so that files that repeat the same filename don't show errors right away (make sure order does not matter in this loop)
-                for f in set(files):
-                    if not errors:
-                        if f in savedtracks:
-                            errors = True
-                            #if for instance, you have the redump dreamcast set and put in the cues and the gdi in the same directories
-                            error('error: track(s) were checked before, may be caused by multiple files using them '
-                                  f'{link(rom.as_uri(),"(open cue/toc/gdi)")} {link(rom.parent.as_uri(),"(open dir)")}')
-                        if not f.is_file():
-                            errors = True
-                            #can happen if 'multiple index files' happened and the user renamed but not only
-                            error('error: missing track(s), may be caused by corrupt file, or previous rename '
-                                  f'{link(rom.as_uri(),"(open cue/toc/gdi)")} {link(rom.parent.as_uri(),"(open dir)")}')
-                    savedtracks.add(f)
+                    if not tmp.is_absolute():
+                        tmp = Path(rom.parent, tmp)
+                    tmp = tmp.resolve()
+                    if not tmp.is_file():
+                        raise ValueError('track must be a file')
+                    if tmp in savedtracks:
+                        raise TrackAlreadyCheckedError()
+                    savedtracks.add(tmp)
+                    return tmp
+                #although a toc or a cue can point to the same file for different tracks, dats will only have '1' unique file
+                try:
+                    files = list(map( track_constructor, OrderedDict.fromkeys(re.findall(regex, index_txt)).keys() ))
+                except TrackAlreadyCheckedError:
+                    errors = True
+                    error('error: track(s) were checked before, may be caused by multiple files using them '
+                          f'{link(rom.as_uri(),"(open cue/toc/gdi)")} {link(rom.parent.as_uri(),"(open dir)")}')
+                except:
+                    errors = True
+                    error('error: missing track(s), may be caused by corrupt file, or previous rename '
+                          f'{link(rom.as_uri(),"(open cue/toc/gdi)")} {link(rom.parent.as_uri(),"(open dir)")}')
                 if errors:
                     continue
             
             if not files: #share the next loop
                 files = [ rom ]
             
             games = None
```

### Comparing `rhdndat-2.6.7/setup.py` & `rhdndat-2.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,32 +5,31 @@
 ['rhdndat']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['beautifulsoup4>=4.10.0,<5.0.0',
- 'chd-rs-py',
  'colorama>=0.4.4,<0.5.0',
  'lxml>=4.9.1,<5.0.0',
  'questionary>=1.10.0,<2.0.0',
  'typer>=0.5.0,<0.6.0']
 
 extras_require = \
 {':sys_platform != "win32"': ['xattr>=0.9.9,<0.10.0']}
 
 entry_points = \
 {'console_scripts': ['rhdndat = rhdndat.__main__:main',
                      'rhdndat-rn = rhdndat.__main__:rename']}
 
 setup_kwargs = {
     'name': 'rhdndat',
-    'version': '2.6.7',
+    'version': '2.6.8',
     'description': 'www.romhacking.net update checker',
-    'long_description': "romhacking.net_ update checker and rom renamer\n==============================================\n\n.. _romhacking.net: http://www.romhacking.net\n\n\n**rhdndat** finds ``rhdndat.ver`` files to check for romhacking.net updates\n\nA version file is named ``rhdndat.ver`` and has a version number line followed by a romhacking.net url line, repeated. These correspond to each hack or translation. To check for needed updates to version file, if any patch version in the file does not match the version on the romhacking.net patch page, it presents a warning.\n\n**rhdndat-rn** renames files and patches to new .DAT [1]_ [2]_ rom names if it can find the rom checksum in those .DAT files and memorizes the checksum of the 'original rom' as a extended attribute ``user.rhdndat.rom_sha1`` to speed up renaming in subsequent executions (in unix, not windows).\n\nTo find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (i don't know of any emulator that supports softpatching for those, except those that support delta chd).\n\nrhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a name that is existing file in the rom directory.\n\nBesides bare rom files, files affected by renames are compressed wii/gamecube .rvz files, .cue/.toc/.gdi (treated especially to not ask for every track), the softpatch types .ips, .bps, .ups, including the new retroarch multiple softpatch convention (a number after the softpatch extension), .rxdelta, .pal NES color palettes, and sbi subchannel data files.\n\n``nes fds lnx a78`` roms require headers and are hardcoded to ignore headers when calculating ``user.rhdndat.rom_sha1`` to match the no-intro dat checksums that checksum everything except the header. This is problematic for hacks, where you can 'verify' a file is the right rom, but the hack was created for a rom with another header. A solution that keeps the softpatch is tracking down the right rom, hardpatching it, and creating a softpatch from the current no-intro rom to the older patched rom. For sfc and pce ips hacks that target a headered rom I recommend ipsbehead to change the patch to target the no-header rom.\n\nRequires xdelta3 (to process rxdelta) and dolphin-tool (to operate on rvz files) on path or the same directory.\n\nTo check for updates if you have the version files:\n\n``rhdndat romdir``\n                        check if there are any updates\n\nTo rename files if you have the dat files:\n\n``rhdndat-rn [--force] [--ext a78 --ext nes ...] romdir xmlpath``\n                        the rom extensions should be all file extensions on the files you want to rename (see below for default)\n\nrhdndat [OPTIONS] ROMDIR\n  :ROMDIR:  Directory to search for versions to check.  [required]\n\n  --show                Show link to each checked directory.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\nrhdndat-rn [OPTIONS] ROMDIR XMLPATH\n  :ROMDIR:  Directory to search for roms to rename.  [required]\n  \n  :XMLPATH: Xml dat file or directory to search for xml dat files to use as source of new names.  [required]\n\n  --skip DIRECTORY      Directory to skip, can be repeated.\n  --ext TEXT            ROM extensions to find names of, can be\n                        repeated. Note that you can ommit this\n                        argument to get the predefined list.\n                        [default: a78, hdi, fdi, ngc, ws, wsc, pce,\n                        gb, gba, gbc, n64, v64, z64, 3ds, nds, nes,\n                        lnx, fds, sfc, smc, bs, nsp, 32x, gg, sms,\n                        md, iso, dim, adf, ipf, dsi, wad, cue, gdi,\n                        toc, rvz]\n  --force               Force a recalculation and store of checksum\n                        (on windows the calculation always happens).\n  --no-rename           Check and store checksums only.\n  --verbose             Print more information about skipped roms.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\n.. [1] `scroll down and click 'prepare' to get a collection of cartidge rom .DAT files <https://datomatic.no-intro.org/index.php?page=download&s=64&op=daily>`_.\n.. [2] `download cd/dvd roms .DAT files here <http://redump.org/downloads/>`_.\n\nInstall\n-------\n\nrhdndat requires python 3.8 or later.\n\nrhdndat may fail to execute in linux if the dir ``~/.local/bin`` to is not in the ``$PATH``.\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python. \n\nThe project can be installed with pip but you'll have to provide your own xdelta3 and dolphin-tool executables in the path (or current dir) for supporting rvz and rxdelta.\n\nIn linux just installing xdelta3 from the repositories is enough, in windows, placing a executable for xdelta3 named ``xdelta3.exe`` in the python install ``Scripts`` directory if you installed with the path option selected is enough.\n\nIn linux you'll have to build dolphin-tool (it's not built by dolphin-emu packages) and place it in ``~/.local/bin``, and in windows you can copy it from the dolphin install directory, rename it to ``dolphin-tool.exe`` and place it in the python install ``Scripts`` directory.\n\n\n+----------------+----------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall rhdndat``                                              |\n+----------------+----------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/rhdndat/archive/master.zip`` |\n+----------------+----------------------------------------------------------------------------------------+\n\nLinks\n-----\n\n.. class:: tablacreditos\n\n+-------------------------------------------------------+----------------------------------------------+\n| Alcaro for helpful comments and for flips             | https://github.com/Alcaro/Flips              |\n+-------------------------------------------------------+----------------------------------------------+\n| romhacking.net for being awesome                      | http://www.romhacking.net/                   |\n+-------------------------------------------------------+----------------------------------------------+\n| Turn sfc and pce ips header patches to no-header      | https://github.com/heuripedes/ipsbehead      |\n| patches                                               |                                              |\n+-------------------------------------------------------+----------------------------------------------+\n| Remember to rename to xdelta3 and place in path       | https://github.com/jmacd/xdelta-gpl/releases |\n+-------------------------------------------------------+----------------------------------------------+\n| Remember to rename to dolphin-tool and place in path, | https://dolphin-emu.org/download/            |\n| linux requires build                                  |                                              |\n+-------------------------------------------------------+----------------------------------------------+\n\n`The source for this project is available here\n<https://github.com/i30817/rhdndat>`_.\n",
+    'long_description': "romhacking.net_ update checker and rom renamer\n==============================================\n\n.. _romhacking.net: http://www.romhacking.net\n\n\n**rhdndat** finds ``rhdndat.ver`` files to check for romhacking.net updates\n\nA version file is named ``rhdndat.ver`` and has a version number line followed by a romhacking.net url line, repeated. These correspond to each hack or translation. To check for needed updates to version file, if any patch version in the file does not match the version on the romhacking.net patch page, it presents a warning.\n\n**rhdndat-rn** renames files and patches to new .DAT [1]_ [2]_ rom names if it can find the rom checksum in those .DAT files and memorizes the checksum of the 'original rom' as a extended attribute ``user.rhdndat.rom_sha1`` to speed up renaming in subsequent executions (in unix, not windows).\n\nTo find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (since delta chd support is rare).\n\nrhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a existing file in the rom directory.\n\nBesides bare rom files, files affected by renames are compressed wii/gamecube .rvz files, .cue/.toc/.gdi (treated especially to not ask for every track), the softpatch types .ips, .bps, .ups, including the new retroarch multiple softpatch convention (a number after the softpatch extension), .rxdelta, .pal NES color palettes, and sbi subchannel data files.\n\n``nes fds lnx a78`` roms require headers and are hardcoded to ignore headers when calculating ``user.rhdndat.rom_sha1`` to match the no-intro dat checksums that checksum everything except the header. This is problematic for hacks, where you can 'verify' a file is the right rom, but the hack was created for a rom with another header. A solution that keeps the softpatch is tracking down the right rom, hardpatching it, and creating a softpatch from the current no-intro rom to the older patched rom. For sfc and pce ips hacks that target a headered rom I recommend ipsbehead to change the patch to target the no-header rom.\n\nRequires xdelta3 (to process rxdelta) and dolphin-tool (to operate on rvz files) on path or the same directory.\n\nTo check for updates if you have the version files:\n\n``rhdndat romdir``\n                        check if there are any updates\n\nTo rename files if you have the dat files:\n\n``rhdndat-rn [--force] [--ext a78 --ext nes ...] romdir xmlpath``\n                        the rom extensions should be all file extensions on the files you want to rename (see below for default)\n\nrhdndat [OPTIONS] ROMDIR\n  :ROMDIR:  Directory to search for versions to check.  [required]\n\n  --show                Show link to each checked directory.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\nrhdndat-rn [OPTIONS] ROMDIR XMLPATH\n  :ROMDIR:  Directory to search for roms to rename.  [required]\n  \n  :XMLPATH: Xml dat file or directory to search for xml dat files to use as source of new names.  [required]\n\n  --skip DIRECTORY      Directory to skip, can be repeated.\n  --ext TEXT            ROM extensions to find names of, can be\n                        repeated. Note that you can ommit this\n                        argument to get the predefined list.\n                        [default: a78, hdi, fdi, ngc, ws, wsc, pce,\n                        gb, gba, gbc, n64, v64, z64, 3ds, nds, nes,\n                        lnx, fds, sfc, smc, bs, nsp, 32x, gg, sms,\n                        md, iso, dim, adf, ipf, dsi, wad, cue, gdi,\n                        toc, rvz]\n  --force               Force a recalculation and store of checksum\n                        (on windows the calculation always happens).\n  --no-rename           Check and store checksums only.\n  --verbose             Print more information about skipped roms.\n  --install-completion  Install completion for the current shell.\n  --show-completion     Show completion for the current shell, to copy it or\n                        customize the installation.\n  --help                Show this message and exit.\n\n\n.. [1] `scroll down and click 'prepare' to get a collection of cartidge rom .DAT files <https://datomatic.no-intro.org/index.php?page=download&s=64&op=daily>`_.\n.. [2] `download cd/dvd roms .DAT files here <http://redump.org/downloads/>`_.\n\nInstall\n-------\n\nrhdndat requires python 3.8 or later.\n\nrhdndat may fail to execute in linux if the dir ``~/.local/bin`` to is not in the ``$PATH``.\n\nIn windows, you'll want to check the option to “Add Python to PATH” when installing python. \n\nThe project can be installed with pip but you'll have to provide your own xdelta3 and dolphin-tool executables in the path (or current dir) for supporting rvz and rxdelta.\n\nIn linux just installing xdelta3 from the repositories is enough, in windows, placing a executable for xdelta3 named ``xdelta3.exe`` in the python install ``Scripts`` directory if you installed with the path option selected is enough.\n\nIn linux you'll have to build dolphin-tool (it's not built by dolphin-emu packages) and place it in ``~/.local/bin``, and in windows you can copy it from the dolphin install directory, rename it to ``dolphin-tool.exe`` and place it in the python install ``Scripts`` directory.\n\n\n+----------------+----------------------------------------------------------------------------------------+\n| Latest release | ``pip install --force-reinstall rhdndat``                                              |\n+----------------+----------------------------------------------------------------------------------------+\n| Current code   | ``pip install --force-reinstall https://github.com/i30817/rhdndat/archive/master.zip`` |\n+----------------+----------------------------------------------------------------------------------------+\n\nLinks\n-----\n\n.. class:: tablacreditos\n\n+-------------------------------------------------------+----------------------------------------------+\n| Alcaro for helpful comments and for flips             | https://github.com/Alcaro/Flips              |\n+-------------------------------------------------------+----------------------------------------------+\n| romhacking.net for being awesome                      | http://www.romhacking.net/                   |\n+-------------------------------------------------------+----------------------------------------------+\n| Turn sfc and pce ips header patches to no-header      | https://github.com/heuripedes/ipsbehead      |\n| patches                                               |                                              |\n+-------------------------------------------------------+----------------------------------------------+\n| Remember to rename to xdelta3 and place in path       | https://github.com/jmacd/xdelta-gpl/releases |\n+-------------------------------------------------------+----------------------------------------------+\n| Remember to rename to dolphin-tool and place in path, | https://dolphin-emu.org/download/            |\n| linux requires build                                  |                                              |\n+-------------------------------------------------------+----------------------------------------------+\n\n`The source for this project is available here\n<https://github.com/i30817/rhdndat>`_.\n",
     'author': 'i30817',
     'author_email': 'i30817@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/i30817/rhdndat',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `rhdndat-2.6.7/PKG-INFO` & `rhdndat-2.6.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: rhdndat
-Version: 2.6.7
+Version: 2.6.8
 Summary: www.romhacking.net update checker
 Home-page: https://github.com/i30817/rhdndat
 License: GNU General Public License v3.0
 Author: i30817
 Author-email: i30817@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
-Requires-Dist: chd-rs-py
 Requires-Dist: colorama (>=0.4.4,<0.5.0)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: questionary (>=1.10.0,<2.0.0)
 Requires-Dist: typer (>=0.5.0,<0.6.0)
 Requires-Dist: xattr (>=0.9.9,<0.10.0); sys_platform != "win32"
 Project-URL: Bug Tracker, https://github.com/i30817/rhdndat/issues
 Project-URL: Repository, https://github.com/i30817/rhdndat
@@ -33,17 +32,17 @@
 
 **rhdndat** finds ``rhdndat.ver`` files to check for romhacking.net updates
 
 A version file is named ``rhdndat.ver`` and has a version number line followed by a romhacking.net url line, repeated. These correspond to each hack or translation. To check for needed updates to version file, if any patch version in the file does not match the version on the romhacking.net patch page, it presents a warning.
 
 **rhdndat-rn** renames files and patches to new .DAT [1]_ [2]_ rom names if it can find the rom checksum in those .DAT files and memorizes the checksum of the 'original rom' as a extended attribute ``user.rhdndat.rom_sha1`` to speed up renaming in subsequent executions (in unix, not windows).
 
-To find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (i don't know of any emulator that supports softpatching for those, except those that support delta chd).
+To find the checksum of the original file for hardpatched roms, rhdndat-rn can support a custom convention for 'revert patches'. Revert patches are a patch that you apply to a hardpatched file to get the original. These have the same name as the file and extension '.rxdelta' and are done with xdelta3. I keep them for patch updates for cd images (since delta chd support is rare).
 
-rhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a name that is existing file in the rom directory.
+rhdndat-rn will read a xml dat file or every dat file from a directory given, and ask for renaming for every match where the rom filename is not equal to the dat name proposed. It will skip the question if all the names proposed already exist in the rom directory, and not allow a rename to a existing file in the rom directory.
 
 Besides bare rom files, files affected by renames are compressed wii/gamecube .rvz files, .cue/.toc/.gdi (treated especially to not ask for every track), the softpatch types .ips, .bps, .ups, including the new retroarch multiple softpatch convention (a number after the softpatch extension), .rxdelta, .pal NES color palettes, and sbi subchannel data files.
 
 ``nes fds lnx a78`` roms require headers and are hardcoded to ignore headers when calculating ``user.rhdndat.rom_sha1`` to match the no-intro dat checksums that checksum everything except the header. This is problematic for hacks, where you can 'verify' a file is the right rom, but the hack was created for a rom with another header. A solution that keeps the softpatch is tracking down the right rom, hardpatching it, and creating a softpatch from the current no-intro rom to the older patched rom. For sfc and pce ips hacks that target a headered rom I recommend ipsbehead to change the patch to target the no-header rom.
 
 Requires xdelta3 (to process rxdelta) and dolphin-tool (to operate on rvz files) on path or the same directory.
```

