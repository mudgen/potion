
~ building potion ~

Normally,

  $ make

To build with debugging symbols,

  $ make DEBUG=1

To build with the JIT off,

  $ make JIT=0

Lastly, to verify your build,

  $ make test


~ the latest potion ~

To build the bleeding edge, you will need
make, binutils and gcc.

  $ git clone git://github.com/why/potion.git
  $ cd potion
  $ make


~ installing ~

Since Potion is only a single binary right now
and there's no additional libs, I haven't written
an installation step yet.


~ building on windows ~

Potion's win32 binaries are built using MinGW.
<http://mingw.org/>

It's a bit hard to setup mingw and make on Windows.
I usually run a shell under Cygwin and add MinGW
to my $PATH.

Once that's all done,

  $ make

The easiest way to do this, actually, is on Linux.

On Ubuntu, if you have MinGW installed,

  $ make CC=i586-mingw32msvc-gcc

You may then rename `potion` to `potion.exe` and
donate that binary to the needy.
