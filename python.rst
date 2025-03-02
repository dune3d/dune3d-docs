Python module
=============

Parts of Dune 3D are available as a python module for use in scripts.

Installation
~~~~~~~~~~~~

The python module isn't included in the :code:`all` target.  To build it, run :code:`meson compile -C build dune3d_py`.
This requires the python 3 headers and pybind11 to be installed.
You can then place it in python's :code:`sys.path` and import it using :code:`import dune3d_py as dune3d`.

Usage
~~~~~

See the `example script <https://github.com/dune3d/dune3d/blob/main/src/python_module/example.py>`_ for how to use it.
So far, the python module is mostly a proof-of-concept, but exposing more features already present in Dune 3D is expected to be easy.
Happy hacking!
