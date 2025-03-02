DXF import
==========

Dune 3D supports importing DXF files into workplanes. The "Import DXF" 
tool therefore only is available if the current group has an active 
workplane.

If it looks like nothing has happened after import, zoom in or out as the 
imported geometry might be significantly larger than the current zoom 
level or may be at an unexpected offset.

Once imported, it's recommended to use the "create coincident 
constraints" tool to make near-coincident points actually coincident so 
that they can form closed paths as required for extrusion or other 
groups. In this tool, adjust the tolerance as required and confirm by 
right-clicking.

If the imported geometry is purely decorative and doesn't need to be 
modified other than scaled or rotated, put in a :doc:`Cluster<cluster>`.
