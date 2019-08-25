Description
==========

prettyping is a wrapper around the standard ping tool with the objective of making the output prettier, more colorful, more compact, 
and easier to read.

prettyping runs the standard ping in the background and parses its output, showing the ping responses in a graphical way at the terminal 
(by using colors and Unicode characters).

prettyping is written in bash and awk, and is reported to work on many different systems (Linux, Mac OS X, BSD…), 
as well as running on different versions of awk (gawk, mawk, nawk, busybox awk).

Read about the history of this project, as well as detailed information, screenshots, videos at: http://denilsonsa.github.io/prettyping/

Requirements
============

bash (tested on 4.20, should work on versions as old as 2008)

awk (either gawk, mawk, nawk or busybox awk; should work on gawk versions as old as 2008; should probably work on any other awk implementation)

ping (from iputils, or any other version that prints essentially the same output, like Mac OS X ping or oping)

Optional dependency on stty or tput to auto-detect the terminal size.

Installation
============

On any Linux Debian versions: 

$ sudo dpkg -i ./prettyping_1.1.1.deb

Testing
=======

$ lintian ./prettyping_1.1.1.deb 

E: prettyping: changelog-file-missing-in-native-package
E: prettyping: no-copyright-file
W: prettyping: description-synopsis-starts-with-article
W: prettyping: description-too-long
W: prettyping: extended-description-line-too-long
E: prettyping: depends-on-essential-package-without-using-version depends: bash
W: prettyping: virtual-package-depends-without-real-package-depends depends: awk
E: prettyping: needlessly-depends-on-awk depends
E: prettyping: usr/ 1000/1000
E: prettyping: usr/bin/ 1000/1000
E: prettyping: usr/bin/prettyping 1000/1000
E: prettyping: usr/share/ 1000/1000
E: prettyping: usr/share/doc/ 1000/1000
E: prettyping: usr/share/doc/Readme.md 1000/1000
E: prettyping: usr/share/doc/Readme.md 
E: prettyping: usr/share/doc/copyright 1000/1000
E: prettyping: usr/share/doc/copyright
E: prettyping: usr/share/doc/prettyping/ 1000/1000
E: prettyping: usr/share/doc/prettyping/ 
W: prettyping: binary-without-manpage usr/bin/prettyping

