Building on Linux
=================

Building Dune 3D on Linux is as simple as running meson after you’ve cloned
the repo.

Install dependencies
--------------------

Make sure you got these dependencies installed:


*  gtkmm-4.0
*  cairomm
*  opencascade
*  uuid
*  pkg-config (build-time only)
*  librsvg (build-time only)
*  glm (build-time only, since it's just headers)
*  python (build-time only)
*  cmake (build-time only)
*  meson (build-time only)
*  eigen (build-time only, since it's just headers)
*  range-v3 (build-time only, since it's just headers)
*  git (build-time only, required when building from a git repo)
*  python-gobject (build-time only)
*  python-cairo (build-time only)

And a C++ compiler that supports ``format``.


See the `the CI configuration <https://github.com/dune3d/dune3d/blob/main/.github/workflows/all.yml>`_ for the exact package names for debian-based distros and Arch Linux.


Build it
--------

::

   meson setup build
   meson compile -C build

If ``meson compile`` isn't available yet, invoke ninja directly:

::

   ninja -C build

Running
-------

The resulting binaries are self-contained and don’t require any external
data files like icons or so.
``dune3d`` is the main program executable. Run it from the build
directory:

::

   build/dune3d
