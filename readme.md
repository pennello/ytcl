`ytcl` watches the clipboard for YouTube video URLs, and automatically
downloads them to the current working directory.

Dependencies
------------
`ytcl` makes use of the excellent program [`youtube-dl`][1] to do the
actual heavy lifting of downloading YouTube videos.  It's launched as a
subprocess, and needs to be in your path.

Installation
------------
Simply run `make && sudo make install`.  The `Makefile` takes advantage
of GNU extensions; therefore, you will want to use `gmake` on FreeBSD.
The `Makefile` supports `DESTDIR`.

Documentation
-------------
Run `ytcl --help` to get started.  In addition, most of the classes and
methods have Pydoc documentation.

Cross-Platform Support
----------------------
Cross-platform support for clipboard interaction and GUI notifications
is managed by the `ytcl.clipboard` and `ytcl.notify` modules,
respectively.  OS X is currently the only supported platform, but the
modules are written in such a way so as to make adding support for
platforms straight-forward.

[1]: http://rg3.github.io/youtube-dl/
