Building on macOS
=================

On macOS, homebrew, and LLVM from homebrew are needed to compile dune3d.


Install dependencies
--------------------

`Homebrew: <https://brew.sh>`_

::

   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"


Follow the instructions, now you should be able to install the remaining dependencies:

::

   brew install \
     python@3 \
     llvm \
     eigen \
     opencascade \
     pkg-config \
     gtk4 \
     gtkmm4 \
     glm \
     pygobject3 \
     librsvg \
     meson

Now you can build the project using the ``./scripts/build_macos.sh`` script.

You should now have the ``dune3d`` executable in the ``build/`` folder.


.. note::
  Building on macOS is still experimental. You might find workarounds for building/linking issues in this project's issues. Also be aware that selection in macOS is broken for now.
