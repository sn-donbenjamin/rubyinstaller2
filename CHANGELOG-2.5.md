## RubyInstaller-2.5.3-1 - 2018-10-21

### Changed
- Installer files are signed with a Microsoft trusted certificate now.
- Strip debug information from compiled extensions.
  This significantly decreases install size of C based gems. #130
- Fix RubyInstaller update mechanism, so that it no longer removes the PATH setting. #125
- Update to OpenSSL-1.1.1 and libgdbm-1.18.
- Update of the SSL CA certificate list.


## RubyInstaller-2.5.1-2 - 2018-06-24

### Changed
- Update `ridk install` to download msys2 installer version 20180531. #115
- Fix MSYS2 detection in `ridk install`. This broke download of MSYS2 installer. #114
- Don't crash when the mingw directory within MSYS2 isn't present.
- Update of the SSL CA certificate list.


## RubyInstaller-2.5.1-1 - 2018-03-29

### Added
- New installer for Ruby with builtin MSYS2 Devkit toolchain. #42

### Changed
- Update to ruby-2.5.1, see [release notes](https://www.ruby-lang.org/en/news/2018/03/28/ruby-2-5-1-released/).
- Update to OpenSSL-1.1.0h .
- Make installers with/without Devkit compatible, so that both can be mixed like:
  - Install RubyInstaller-Devkit first and update with smaller RubyInstaller later
  - Install RubyInstaller first and update by RubyInstaller-Devkit


## RubyInstaller-2.5.0-2 - 2018-02-27

### Changed
- Don't abort but fix pacman conflicts while 'ridk install'. #101


## RubyInstaller-2.5.0-1 - 2017-12-25

### Added
- Add ruby-2.5.0, see [release notes](https://www.ruby-lang.org/en/news/2017/12/25/ruby-2-5-0-released/).

### Changed
- RubyInstaller-2.5 bundles OpenSSL-1.1.0 (instead of 1.0.2 of RubyInstaller-2.4).
  This has some [implications to the Ruby API to OpenSSL](https://bugs.ruby-lang.org/issues/12324).
