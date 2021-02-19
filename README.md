<p align="center">
  <img src="https://libevent.org/libevent3.png" alt="libevent logo"/>
</p>


# ubuntu  build
```
(base) heidsoft@dev01:~/libevent$ lsb_release -a
No LSB modules are available.
Distributor ID:	Ubuntu
Description:	Ubuntu 18.04.5 LTS
Release:	18.04
Codename:	bionic
(base) heidsoft@dev01:~/libevent$ 

(base) heidsoft@dev01:~/libevent-2.1.12-stable$ ./configure 
checking for a BSD-compatible install... /usr/bin/install -c
checking whether build environment is sane... yes
checking for a thread-safe mkdir -p... /bin/mkdir -p
checking for gawk... no
checking for mawk... mawk
checking whether make sets $(MAKE)... yes
checking whether make supports nested variables... yes
checking whether make supports nested variables... (cached) yes
checking whether make supports the include directive... yes (GNU style)
checking for gcc... gcc
checking whether the C compiler works... yes
checking for C compiler default output file name... a.out
checking for suffix of executables... 
checking whether we are cross compiling... no
checking for suffix of object files... o
checking whether we are using the GNU C compiler... yes
checking whether gcc accepts -g... yes
checking for gcc option to accept ISO C89... none needed
checking whether gcc understands -c and -o together... yes
checking dependency style of gcc... gcc3
checking how to run the C preprocessor... gcc -E
checking for grep that handles long lines and -e... /bin/grep
checking for egrep... /bin/grep -E
checking for ANSI C header files... yes
checking for sys/types.h... yes
checking for sys/stat.h... yes
checking for stdlib.h... yes
checking for string.h... yes
checking for memory.h... yes
checking for strings.h... yes
checking for inttypes.h... yes
checking for stdint.h... yes
checking for unistd.h... yes
checking minix/config.h usability... no
checking minix/config.h presence... no
checking for minix/config.h... no
checking whether it is safe to define __EXTENSIONS__... yes
checking build system type... x86_64-pc-linux-gnu
checking host system type... x86_64-pc-linux-gnu
checking whether ln -s works... yes
checking for a sed that does not truncate output... /bin/sed
checking whether gcc needs -traditional... no
checking how to print strings... printf
checking for a sed that does not truncate output... (cached) /bin/sed
checking for fgrep... /bin/grep -F
checking for ld used by gcc... /usr/bin/ld
checking if the linker (/usr/bin/ld) is GNU ld... yes
checking for BSD- or MS-compatible name lister (nm)... /usr/bin/nm -B
checking the name lister (/usr/bin/nm -B) interface... BSD nm
checking the maximum length of command line arguments... 1572864
checking how to convert x86_64-pc-linux-gnu file names to x86_64-pc-linux-gnu format... func_convert_file_noop
checking how to convert x86_64-pc-linux-gnu file names to toolchain format... func_convert_file_noop
checking for /usr/bin/ld option to reload object files... -r
checking for objdump... objdump
checking how to recognize dependent libraries... pass_all
checking for dlltool... no
checking how to associate runtime and link libraries... printf %s\n
checking for ar... ar
checking for archiver @FILE support... @
checking for strip... strip
checking for ranlib... ranlib
checking command to parse /usr/bin/nm -B output from gcc object... ok
checking for sysroot... no
checking for a working dd... /bin/dd
checking how to truncate binary pipes... /bin/dd bs=4096 count=1
checking for mt... mt
checking if mt is a manifest tool... no
checking for dlfcn.h... yes
checking for objdir... .libs
checking if gcc supports -fno-rtti -fno-exceptions... no
checking for gcc option to produce PIC... -fPIC -DPIC
checking if gcc PIC flag -fPIC -DPIC works... yes
checking if gcc static flag -static works... yes
checking if gcc supports -c -o file.o... yes
checking if gcc supports -c -o file.o... (cached) yes
checking whether the gcc linker (/usr/bin/ld -m elf_x86_64) supports shared libraries... yes
checking whether -lc should be explicitly linked in... no
checking dynamic linker characteristics... GNU/Linux ld.so
checking how to hardcode library paths into programs... immediate
checking whether stripping libraries is possible... yes
checking if libtool supports shared libraries... yes
checking whether to build shared libraries... yes
checking whether to build static libraries... yes
checking for library containing inet_ntoa... none required
checking for library containing socket... none required
checking for library containing inet_aton... none required
checking for library containing clock_gettime... none required
checking for clock_gettime... yes
checking for library containing sendfile... none required
checking for WIN32... no
checking for MIDIPIX... no
checking for CYGWIN... no
checking zlib.h usability... no
checking zlib.h presence... no
checking for zlib.h... no
checking for special C compiler options needed for large files... no
checking for _FILE_OFFSET_BITS value needed for large files... no
checking for pkg-config... /usr/bin/pkg-config
checking if pkg-config is at least version 0.15.0... yes
checking for library containing SSL_new... no
checking for library containing SSL_new... no
checking openssl/ssl.h usability... no
checking openssl/ssl.h presence... no
checking for openssl/ssl.h... no
configure: error: openssl is a must but can not be found. You should add the directory containing `openssl.pc' to the `PKG_CONFIG_PATH' environment variable, or set `CFLAGS' and `LDFLAGS' directly for openssl, or use `--disable-openssl' to disable support for openssl encryption
(base) heidsoft@dev01:~/libevent-2.1.12-stable$ sudo apt-get install openssl openssl-devl
[sudo] password for heidsoft: 
(base) heidsoft@dev01:~/libevent-2.1.12-stable$ sudo apt-get install openssl openssl-devel
[sudo] password for heidsoft: 
Reading package lists... Done
Building dependency tree       
Reading state information... Done
E: Unable to locate package openssl-devel
(base) heidsoft@dev01:~/libevent-2.1.12-stable$ sudo apt-get install openssl
Reading package lists... Done
Building dependency tree       
Reading state information... Done
openssl is already the newest version (1.1.1-1ubuntu2.1~18.04.8).
0 upgraded, 0 newly installed, 0 to remove and 43 not upgraded.
(base) heidsoft@dev01:~/libevent-2.1.12-stable$ 
(base) heidsoft@dev01:~/libevent-2.1.12-stable$ sudo apt-get install openssl openssl-dev
Reading package lists... Done
Building dependency tree       
Reading state information... Done
E: Unable to locate package openssl-dev
(base) heidsoft@dev01:~/libevent-2.1.12-stable$ ./configure 
checking for a BSD-compatible install... /usr/bin/install -c
checking whether build environment is sane... yes
checking for a thread-safe mkdir -p... /bin/mkdir -p
checking for gawk... no
checking for mawk... mawk
checking whether make sets $(MAKE)... yes
checking whether make supports nested variables... yes
checking whether make supports nested variables... (cached) yes
checking whether make supports the include directive... yes (GNU style)
checking for gcc... gcc
checking whether the C compiler works... yes
checking for C compiler default output file name... a.out
checking for suffix of executables... 
checking whether we are cross compiling... no
checking for suffix of object files... o
checking whether we are using the GNU C compiler... yes
checking whether gcc accepts -g... yes
checking for gcc option to accept ISO C89... none needed
checking whether gcc understands -c and -o together... yes
checking dependency style of gcc... gcc3
checking how to run the C preprocessor... gcc -E
checking for grep that handles long lines and -e... /bin/grep
checking for egrep... /bin/grep -E
checking for ANSI C header files... yes
checking for sys/types.h... yes
checking for sys/stat.h... yes
checking for stdlib.h... yes
checking for string.h... yes
checking for memory.h... yes
checking for strings.h... yes
checking for inttypes.h... yes
checking for stdint.h... yes
checking for unistd.h... yes
checking minix/config.h usability... no
checking minix/config.h presence... no
checking for minix/config.h... no
checking whether it is safe to define __EXTENSIONS__... yes
checking build system type... x86_64-pc-linux-gnu
checking host system type... x86_64-pc-linux-gnu
checking whether ln -s works... yes
checking for a sed that does not truncate output... /bin/sed
checking whether gcc needs -traditional... no
checking how to print strings... printf
checking for a sed that does not truncate output... (cached) /bin/sed
checking for fgrep... /bin/grep -F
checking for ld used by gcc... /usr/bin/ld
checking if the linker (/usr/bin/ld) is GNU ld... yes
checking for BSD- or MS-compatible name lister (nm)... /usr/bin/nm -B
checking the name lister (/usr/bin/nm -B) interface... BSD nm
checking the maximum length of command line arguments... 1572864
checking how to convert x86_64-pc-linux-gnu file names to x86_64-pc-linux-gnu format... func_convert_file_noop
checking how to convert x86_64-pc-linux-gnu file names to toolchain format... func_convert_file_noop
checking for /usr/bin/ld option to reload object files... -r
checking for objdump... objdump
checking how to recognize dependent libraries... pass_all
checking for dlltool... no
checking how to associate runtime and link libraries... printf %s\n
checking for ar... ar
checking for archiver @FILE support... @
checking for strip... strip
checking for ranlib... ranlib
checking command to parse /usr/bin/nm -B output from gcc object... ok
checking for sysroot... no
checking for a working dd... /bin/dd
checking how to truncate binary pipes... /bin/dd bs=4096 count=1
checking for mt... mt
checking if mt is a manifest tool... no
checking for dlfcn.h... yes
checking for objdir... .libs
checking if gcc supports -fno-rtti -fno-exceptions... no
checking for gcc option to produce PIC... -fPIC -DPIC
checking if gcc PIC flag -fPIC -DPIC works... yes
checking if gcc static flag -static works... yes
checking if gcc supports -c -o file.o... yes
checking if gcc supports -c -o file.o... (cached) yes
checking whether the gcc linker (/usr/bin/ld -m elf_x86_64) supports shared libraries... yes
checking whether -lc should be explicitly linked in... no
checking dynamic linker characteristics... GNU/Linux ld.so
checking how to hardcode library paths into programs... immediate
checking whether stripping libraries is possible... yes
checking if libtool supports shared libraries... yes
checking whether to build shared libraries... yes
checking whether to build static libraries... yes
checking for library containing inet_ntoa... none required
checking for library containing socket... none required
checking for library containing inet_aton... none required
checking for library containing clock_gettime... none required
checking for clock_gettime... yes
checking for library containing sendfile... none required
checking for WIN32... no
checking for MIDIPIX... no
checking for CYGWIN... no
checking zlib.h usability... no
checking zlib.h presence... no
checking for zlib.h... no
checking for special C compiler options needed for large files... no
checking for _FILE_OFFSET_BITS value needed for large files... no
checking for pkg-config... /usr/bin/pkg-config
checking if pkg-config is at least version 0.15.0... yes
checking for library containing SSL_new... no
checking for library containing SSL_new... no
checking openssl/ssl.h usability... no
checking openssl/ssl.h presence... no
checking for openssl/ssl.h... no
configure: error: openssl is a must but can not be found. You should add the directory containing `openssl.pc' to the `PKG_CONFIG_PATH' environment variable, or set `CFLAGS' and `LDFLAGS' directly for openssl, or use `--disable-openssl' to disable support for openssl encryption
(base) heidsoft@dev01:~/libevent-2.1.12-stable$ sudo apt-get install libssl-dev
Reading package lists... Done
Building dependency tree       
Reading state information... Done
Suggested packages:
  libssl-doc
The following NEW packages will be installed:
  libssl-dev
0 upgraded, 1 newly installed, 0 to remove and 43 not upgraded.
Need to get 1,566 kB of archives.
After this operation, 7,849 kB of additional disk space will be used.
Get:1 http://mirrors.aliyun.com/ubuntu bionic-security/main amd64 libssl-dev amd64 1.1.1-1ubuntu2.1~18.04.8 [1,566 kB]
Fetched 1,566 kB in 0s (6,623 kB/s)
Selecting previously unselected package libssl-dev:amd64.
(Reading database ... 188066 files and directories currently installed.)
Preparing to unpack .../libssl-dev_1.1.1-1ubuntu2.1~18.04.8_amd64.deb ...
Unpacking libssl-dev:amd64 (1.1.1-1ubuntu2.1~18.04.8) ...
Setting up libssl-dev:amd64 (1.1.1-1ubuntu2.1~18.04.8) ...
(base) heidsoft@dev01:~/libevent-2.1.12-stable$ 

```


[![CI linux](https://github.com/libevent/libevent/workflows/linux/badge.svg)](https://github.com/libevent/libevent/actions?query=workflow%3Alinux)
[![CI windows](https://github.com/libevent/libevent/workflows/windows/badge.svg)](https://github.com/libevent/libevent/actions?query=workflow%3Awindows)
[![CI mingw](https://github.com/libevent/libevent/workflows/mingw/badge.svg)](https://github.com/libevent/libevent/actions?query=workflow%3Amingw)
[![CI macos](https://github.com/libevent/libevent/workflows/macos/badge.svg)](https://github.com/libevent/libevent/actions?query=workflow%3Amacos)

[![Coverage Status](https://coveralls.io/repos/github/libevent/libevent/badge.svg)](https://coveralls.io/github/libevent/libevent)
[![Join the chat at https://gitter.im/libevent/libevent](https://badges.gitter.im/libevent/libevent.svg)](https://gitter.im/libevent/libevent?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)
[![doxygen](https://img.shields.io/badge/doxygen-documentation-blue.svg)](https://libevent.org/doc)



# 1. BUILDING AND INSTALLATION

## Autoconf

```
$ ./configure
$ make
$ make verify   # (optional)
$ sudo make install
```

See [Documentation/Building#Autoconf](/Documentation/Building.md#autoconf) for more information

## CMake (Windows)

Install CMake: <https://www.cmake.org>

```
$ md build && cd build
$ cmake -G "Visual Studio 10" ..   # Or use any generator you want to use. Run cmake --help for a list
$ cmake --build . --config Release # Or "start libevent.sln" and build with menu in Visual Studio.
```

See [Documentation/Building#Building on Windows](/Documentation/Building.md#building-on-windows) for more information

## CMake (Unix)

```
$ mkdir build && cd build
$ cmake ..     # Default to Unix Makefiles.
$ make
$ make verify  # (optional)
```

See [Documentation/Building#Building on Unix (With CMake)](/Documentation/Building.md#building-on-unix-cmake) for more information

## Package Managers

You can download and install libevent using the [vcpkg](https://github.com/Microsoft/vcpkg) dependency manager:

    git clone https://github.com/Microsoft/vcpkg.git
    cd vcpkg
    ./bootstrap-vcpkg.sh
    ./vcpkg integrate install
    ./vcpkg install libevent

The libevent port in vcpkg is kept up to date by Microsoft team members and community contributors. If the version is out of date, please [create an issue or pull request](https://github.com/Microsoft/vcpkg) on the vcpkg repository.

# 2. USEFUL LINKS:

For the latest released version of Libevent, see the official website at
<http://libevent.org/> .

There's a pretty good work-in-progress manual up at
   <http://www.wangafu.net/~nickm/libevent-book/> .

For the latest development versions of Libevent, access our Git repository
via

```
$ git clone https://github.com/libevent/libevent.git
```

You can browse the git repository online at:

<https://github.com/libevent/libevent>

To report bugs, issues, or ask for new features:

__Patches__: https://github.com/libevent/libevent/pulls
> OK, those are not really _patches_. You fork, modify, and hit the "Create Pull Request" button.
> You can still submit normal git patches via the mailing list.

__Bugs, Features [RFC], and Issues__: https://github.com/libevent/libevent/issues
> Or you can do it via the mailing list.

There's also a libevent-users mailing list for talking about Libevent
use and development: 

<http://archives.seul.org/libevent/users/>

# 3. ACKNOWLEDGMENTS

The [following people](/CONTRIBUTORS.md) have helped with suggestions, ideas,
code or fixing bugs.
