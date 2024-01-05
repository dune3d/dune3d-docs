Building on Windows
===================

Install MSYS2
-------------

Download and run the msys2 installer from http://msys2.github.io/ I’ve
only tested with the 64bit version, 32bit should work as well (but come
on, it’s 2017…) Make sure that the path you select for installation
doesn’t contain any spaces. (Don’t blame me for that one)

Start MSYS console
------------------

Launch the Start Menu item “MSYS2 mingw 64 bit” you should be greeted
with a console window. All steps below refer to what you should type
into that window.

Install updates
---------------

Type

::

   pacman -Syu

if it tells you to close restart msys, close the console window and
start it again. Then run ``pacman -Syu`` again.

Install dependencies
--------------------

Type/paste

::

   pacman -S \
   mingw-w64-x86_64-gcc \
   mingw-w64-x86_64-pkgconf \
   mingw-w64-x86_64-gtkmm4 \
   mingw-w64-x86_64-glm \
   mingw-w64-x86_64-opencascade \
   mingw-w64-x86_64-eigen3 \
   mingw-w64-x86_64-meson \
   mingw-w64-x86_64-cmake \
   mingw-w64-x86_64-python \
   mingw-w64-x86_64-python-cairo \
   mingw-w64-x86_64-python-gobject \
   mingw-w64-x86_64-range-v3 \
   zip \
   unzip \
   git \
   dos2unix \
   --needed

When prompted, just hit return. Sit back and wait for it to install
what’s almost a complete linux environment.

Before continuing you may change to another directory. It easiest to
type ``cd`` followed by a space and drop the folder you want to change
to on the window.

Clone Dune 3D
-------------

::

   git clone https://github.com/dune3d/dune3d
   cd dune3d

Build it
--------

::

   meson setup build
   meson compile -C build

.. note::
  If you get the error meson: command not found, you are probably using the MSYS console (rather than the MINGW64 console). You can run the command export PATH=/bin/mingw64:$PATH to tell the console where to find meson (and the rest of mingw64).

Running
-------

You won’t be able to double-click the resulting executables since all
the required DLLs are in a directory unknown to windows. You’ll have to
launch them from the mingw shell using ``build/dune3d`` for example.

Packaging
---------

To create the zip archive as it’s available from the CI, run
``./make_bindist.sh``.
