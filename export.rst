Export
======

Dune 3D supports exporting both 2D and 3D formats.

3D: STL / STEP
--------------

To export the current group's solid model use the "Export STL" or "Export STEP" action available from the spacebar menu.
The export only includes the solid model and omits imported STEP models.

2D: Paths
---------

The "Export Paths" action exports all closed paths in current group's 
active workplane to an SVG document. It also includes closed paths in 
workplanes from other groups, projecting them onto the current group's
workplane.

2D: Projection
--------------

The "Export Projection" action exports the projection of the current 
group's solid model from the camera's perspective.

If a workplane is selected, it's projected through it instead.
