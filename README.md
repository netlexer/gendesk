我是光年实验室高级招聘经理。
我在github上访问了你的开源项目，你的代码超赞。你最近有没有在看工作机会，我们在招软件开发工程师，拉钩和BOSS等招聘网站也发布了相关岗位，有公司和职位的详细信息。
我们公司在杭州，业务主要做流量增长，是很多大型互联网公司的流量顾问。公司弹性工作制，福利齐全，发展潜力大，良好的办公环境和学习氛围。
公司官网是http://www.gnlab.com,公司地址是杭州市西湖区古墩路紫金广场B座，若你感兴趣，欢迎与我联系，
电话是0571-88839161，手机号：18668131388，微信号：echo 'bGhsaGxoMTEyNAo='|base64 -D ,静待佳音。如有打扰，还请见谅，祝生活愉快工作顺利。

Desktop File Generator
======================

[![Build Status](https://travis-ci.org/xyproto/gendesk.svg?branch=master)](https://travis-ci.org/xyproto/gendesk)

Generates .desktop files and downloads .png icons based on command line arguments.

See `gendesk --help` or the man page for more info.

Pull requests are welcome.

TODO
----
* Move kw/category mappings into a separate configuration file.

Changes from 0.6.5 to 0.7
-------------------------
* Updated vendored dependencies.
* Added support for [goreleaser](https://github.com/goreleaser/goreleaser).
* Improved handling of icons, if an icon is missing.
* Minor changes and refactoring.

Changes from 0.6.4 to 0.6.5
---------------------------
* Ignore the `-svn` suffix in package names (same as for `-git`, thanks @mstraube).
* Use `text/template` for generating the `.desktop` file contents.
* Minor changes to the command line output / documentation.
* Some refactoring.
* Tested with Go 1.9.

Changes from 0.6.3 to 0.6.4
---------------------------
* Fix bug where some flags could not be overridden.

Changes from 0.6.2 to 0.6.3
---------------------------
* Will ignore the "-git" suffix if it is part of a package name.

Changes from 0.6.1 to 0.6.2
---------------------------
* Added the possibility of having a configuration file for specifying a different URL for searching for missing icons.
* Removed the --iconurl parameter.
* Refactored out some code to an external package.

Changes from 0.6 to 0.6.1
-------------------------
* Support for StartupNotify=true/false
* Both --mimetype and --mimetypes are allowed
* Guesses more categories than before

Changes from 0.5.5 to 0.6
-------------------------
* Added an option for generating .desktop files for launching window managers

Changes from 0.5.4 to 0.5.5
---------------------------
* Bug fix when generating .desktop files from PKGBUILD files

Changes from 0.5.3 to 0.5.4
---------------------------
* Added a -f flag for overwriting files (will not overwrite without it)
* Some refactoring

Changes from 0.5.2 to 0.5.3
---------------------------
* Added a --terminal flag for specifying if the application should be run in a terminal
* Some refactoring

Changes from 0.5.1 to 0.5.2
---------------------------
* Support for additional environment variables

Changes from 0.5.0 to 0.5.1
---------------------------
* Support for $pkgname and $pkgdesc
* Updated the man page
* Will try to download icons specified with --iconurl

Changes from 0.4.4 to 0.5.0
---------------------------
* Command line options, no need to specify a PKGBUILD

Changes from 0.4.3 to 0.4.4
---------------------------
* Changed the URL for searching for icons from Fedora to Open Icon Library

Changes from 0.4.2 to 0.4.3
---------------------------
* Fixed minor bug where puzzle games were not placed in the right category
* Added \_categories=()


Changes from 0.4.1 to 0.4.2
---------------------------
* Added category "Graphics;3DGraphics;" for 3D modellers
* Added category "System;" for sensor monitors
* Added category "Game;BoardGame;" for kw "board", "chess", "goban" or "chessboard"
* Added category "Office" for kw "e-book" and "ebook"
* Doesn't use ".png" by default when specifying an icon


Changes from 0.4 to 0.4.1
-------------------------
* Fixed a bug where \_name=() and \_comment=() didn't work as they should


Changes from 0.3 to 0.4
-----------------------
* Added \_genericname=()
* Added \_comment=()
* Added \_mimetype=()
* Added Type=Application
* Added category "Game;LogicGame" for keyword "puzzle"
* Added category "Game;ArcadeGame" for keyword "fighting"
* Fixed weird formatting in --help output
* Added \_custom=() for adding custom fields at the end of the .desktop file
* Glob for existing .svg icons too
* Shorter lines
* Moved functions and settings related to terminal output to a separate file


Changes from 0.2 to 0.3
-----------------------
* New flag: -q for quiet
* New flag: --nocolor for no color
* New flag: -n for not downloading anything (only generate a .desktop file)
* New flag: -q for quiet (no stdout output)
* Added \_name=('Name') to be able to specify a name that isn't only lowercase (like "ZynAddSubFX" or "jEdit")
* kw "synthesizer" is now category AudioVideo
* kw "editor" is now category TextEditor and/or Development;TextEditor
* kw "emulator" is now category "Game"
* kw "game" is now category "Game"
* kw "combat" is now be category "Game;ArcadeGame"
* kw "GPS" or "inspecting" is now category "Application;Science"
* kw "player" is now category "Application;Game;"
* kw "shooter" is now "Application;Game;ActionGame;"
* kw "roguelike" is now "Application;Game;AdventureGame;"
* kw "git" is now category Development;RevisionControl


General information
-------------------

* License: MIT
* Author: Alexander Rødseth

