File versions
===================

To protect against loss of fidelity when opening documents in an older 
version of Dune 3D than they were created with, documents include a 
version level.

This version level is distinct from the application version and is only 
incremented for changes that are incompatible with older versions.

Forward compatibility, as in being able to open 
files that were crated in an earlier version, is always given.

By Application version
----------------------

.. csv-table::
   :header: "Type", "1.0.0", "1.1.0"

   Document, 10, 12


Changelog
---------

  - 1: Add angle/perpendicular constraints
  - 2: Add linear array group
  - 3: Add Point2D entity
  - 4: Add polar array group
  - 5: save entity names
  - 6: Add point in plane constraint
  - 7: Add point/line distance constraint
  - 8: Add point/plane distance constraint
  - 9: Add lock rotation constraint
  - 10: Add intersection solid model operation
  - 11: Add point in workplane constraint
  - 12: Add symmetry constraints
