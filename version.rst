File versions
===================

To protect against loss of fidelity when opening documents in an older 
version of Dune 3D than they were created with, documents include a 
version level.

This version level is distinct from the application version and is only 
incremented for changes that are incompatible with older versions.

Forward compatibility, as in being able to open 
files that were created in an earlier version, is always given.

By Application version
----------------------

.. csv-table::
   :header: "Type", "1.0.0", "1.1.0", "1.2.0", "1.3.0", "1.4.0"

   Document, 10, 12, 23, 30, 35


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
  - 13: Add document entities
  - 14: Add measurements
  - 15: Add aligned distance constraint
  - 16: Add revolve group
  - 17: Add loft group
  - 18: Add bezier curves
  - 19: Add cluster entities
  - 20: Add point on bezier constraint
  - 21: Add text entities
  - 22: Add option to use STEP entities in solid model
  - 23: Add body colors
  - 24: Add h/v mirror groups
  - 25: Add solid model operation group
  - 26: Support constraining workplanes/STEP entities to circles
  - 27: Fix direction for aligned distance with workplanes
  - 28: Add clone group
  - 29: Add pipe group
  - 30: Add picture entities
  - 31: save solid model operation in sketch groups 
  - 32: support constraining points to 3D beziers
  - 33: add bezier/bezier same curvature constraint
  - 34: support multiple source groups on array and mirror groups
  - 35: add bezier/arc same curvature constraint
