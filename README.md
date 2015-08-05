# JACoders "OpenJK" project #

[![License](https://img.shields.io/github/license/JACoders/OpenJK.svg)](https://github.com/JACoders/OpenJK/blob/master/LICENSE.txt)

[![GitHub tag](https://img.shields.io/github/tag/JACoders/OpenJK.svg)](https://github.com/JACoders/OpenJK/tags)
[![GitHub release](https://img.shields.io/github/release/JACoders/OpenJK.svg)](https://github.com/Unvanquished/JACoders/OpenJK/latest)
[![Github release](https://img.shields.io/github/downloads/JACoders/OpenJK/latest/total.svg)](https://github.com/JACoders/OpenJK/releases/latest)

[![IRC](https://img.shields.io/badge/irc-%23JACoders-brightgreen.svg)](http://unic0rn.github.io/tiramisu/jacoders/)
[![Forum](https://img.shields.io/badge/forum-JKHub.org%20OpenJK-brightgreen.svg)](http://jkhub.org/forum/51-discussion/)

[![Coverity Scan Build Status](https://scan.coverity.com/projects/1153/badge.svg)](https://scan.coverity.com/projects/1153)

### Build Status ###

| Windows | OSX | Linux x86 | Linux x64 |
|---------|-----|-----------|-----------|
| [![IRC](https://img.shields.io/badge/build-Windows-blue.svg)](http://jk.xd.cm/builders/windows) | [ ![IRC](https://img.shields.io/badge/build-OSX-blue.svg)](http://jk.xd.cm/builders/osx) | [ ![IRC](https://img.shields.io/badge/build-Linux%20x86-blue.svg)](http://jk.xd.cm/builders/linux) | [ ![IRC](https://img.shields.io/badge/build-Linux%20x64-blue.svg)](http://jk.xd.cm/builders/linux-64) |

The purpose of this project is to maintain and improve the Jedi Academy and Jedi Outcast games, developed by Raven Software. This project does not attempt to rebalance or otherwise modify core gameplay.

Major enhancement changes are very low priority at this time unless patches are made available and which do not alter the core functionality of gameplay or the stock renderer itself.

Please use discretion when making issue requests on GitHub. The [JKHub sub-forum](http://jkhub.org/forum/51-discussion/) is a better place for support queries, discussions, and feature requests.

## Jedi Outcast Support ##

_Do not make issues regarding Jedi Outcast problems at this time. It is considered mostly unfinished, broken, and to be used at your own risk!_

There is no Multiplayer code for JK2MP at all on our repository at this time. The Single-player support must be explicitly turned on in your own compile. The pre-built versions will not include this.

## 64-bit Support

64-bit is currently supported on non-Windows platforms.

## Installation ##

First, install Jedi Academy. If you don't already own the game you can buy it from online stores such as [Steam](http://store.steampowered.com/app/6020/), [Amazon](http://www.amazon.com/Star-Wars-Jedi-Knight-Academy-Pc/dp/B0000A2MCN) or [Play](http://www.play.com/Games/PC/4-/127805/Star-Wars-Jedi-Knight-Jedi-Academy/Product.html?searchstring=jedi+academy&searchsource=0&searchtype=allproducts&urlrefer=search). Then unpack the OpenJK zip file to your Jedi Academy GameData folder.

## Maintainers (in alphabetical order) ##

* eezstreet
* Ensiform
* Razish
* redsaurus
* Xycaleth

## Significant contributors (in alphabetical order) ##

* exidl
* ImperatorPrime
* mrwonko
* Scooper
* Sil

## Dependencies ##

* SDL2 (2.0.3+) (included on Windows)
* OpenGL
* OpenAL (included on Windows)
* libpng (included on Windows)
* libjpeg (included on Windows)
* zlib (included on Windows)

## Dedicated Server ##

In order to run a dedicated server, you must use the openjkded binary. Running dedicated from the main executable is currently not possible because it was broken with the addition of modular renderer.

## Developer Notes ##

OpenJK is licensed under GPLv2 as free software. You are free to use, modify and redistribute OpenJK following the terms in LICENSE.txt.

Please be aware of the implications of the GPLv2 licence. In short, be prepared to share your code under the same GPLv2 licence.

### If you wish to contribute to OpenJK, please do the following ###
* [Fork](https://github.com/JACoders/OpenJK/fork) the project on GitHub
* Create a new branch and make your changes
* Send a [pull request](https://help.github.com/articles/creating-a-pull-request) to upstream (JACoders/OpenJK)

### If you wish to base your work off OpenJK (mod or engine) ###
* [Fork](https://github.com/JACoders/OpenJK/fork) the project on GitHub
* Change the GAMEVERSION define in codemp/game/g_local.h from "OpenJK" to your project name
* If you make a nice change, please consider back-porting to upstream via pull request as described above. This is so everyone benefits without having to reinvent the wheel for every project.

### Reserved renderer names ###
* rd-vanilla (JA's original renderer)
* rd-dedicated (Stripped down renderer for use with dedicated server)
* rd-rend2 (Maintainer: Xycaleth)
* rd-es (OpenGL ES compliant renderer for use with Raspberry Pi, Ouya, etc - please contribute!)
* rd-strawberry (Maintainer: Xycaleth)
* rd-vader (Maintainer: mrwonko)
* rd-palpatine (Maintainer: mrwonko)
* rd-sidious (Maintainer: mrwonko)

### Engine hacks in existing mods ###
Mods which make use of runtime memory patches may fail to run under OpenJK, and in the worst case will cause the program to crash. Consider forking OpenJK and adding your engine modifications directly, or applying these patches only if you are running on the retail engine.

### Links of Interest ###
* [Buildbot](http://jk.xd.cm/)
* [Buildbot builds](http://builds.openjk.org/)
* [Compilation Guide](https://github.com/JACoders/OpenJK/wiki/Compilation-guide)
* [JKHub sub-forum](http://jkhub.org/forum/51-discussion/)
