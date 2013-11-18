tq2440-madplayer
================

##madplayer and libriries: zlib libmad libid3tag
###Build order
- zlib
- libmad
- libit3tag
- madplay

###Other necessary libs
Using the `readelf -d XXX.so.0.Y.Z | grep Shared` to get the dynamic libs.
Using the arm-linux-gcc -print-file-name=libXXX.so.Y.Z to locate the libs.
Copy the libs get from upon operations to the direcotry /lib of embedded system rootfs.
Set the LDLIBRARY in the embedded system shell if need.

## For the alsa-lib and alsa-utils
If you don't want to corss compile the ncurses library, dissable it. See the ReadmeFirst.txt in directory.
Whithout the ncurses, we should disable the alsamixer too.
