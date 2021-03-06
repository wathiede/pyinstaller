=============
PyInstaller
=============

Requirements
============

Python:
    2.3 - 2.7 (Python 3 is not supported)

Windows (32bit/64bit):
  * Windows XP or newer.
  * pywin32 when using Python 2.6+
    http://sourceforge.net/projects/pywin32/

Linux (32bit/64bit)
  * ldd
    - Console application to print the shared libraries required 
      by each program or shared library.
  * objdump
    - Console application to display information from object files.

Mac OS X (32/64bit):
  * Mac OS X 10.4 (Tiger) or newer (Leopard, Snow Leopard, Lion).

Solaris (experimental)
  * ldd
  * objdump

AIX (experimental)
  * AIX 6.1 or newer.
    Python executables created using PyInstaller on AIX 6.1 should
    work on AIX 5.2/5.3. PyInstaller will not work with statically
    linked Python libraries which has been encountered in Python 2.2
    installations on AIX 5.x.
  * ldd
  * objdump

FreeBSD (experimental)
  * ldd
  * objdump
  * Build your own loader:
    $ cd source; python waf configure build install

Usage
=========

    python pyinstaller.py /path/to/yourscript.py

For more details see doc/Manual.html


Installation in brief
=====================

1) Unpack the archive on you path of choice.

2) For Windows (32/64bit), Linux (32/64bit) and Mac OS X (32/64bit)
   precompiled boot-loaders are available. So the installation is
   complete.

   For other platforms, users should first try to build the
   boot-loader:

     cd source
     python ./waf configure build install


Major changes in this release
=============================

See doc/CHANGES.txt
