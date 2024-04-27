Constraints
===========

Constraints are used to define the spatial relationship between 
entities or parameters of entities themselves. Some constraints such a 
distance or angle allow entering a value.

Some constraints can have a workplane. Unless otherwise noted, this 
means that the constraint applies in the workplane, that is all 
entities are projected onto the workplane.

In general, constraints are created by selecting the to be constrained 
entities and invoking the requisite tool.

Points coincident
-----------------

Constrains two points to be at the same position.

:Workplane: optional
:Selection: Two points
:Tool: Constrain coincident

Point on line
-------------

Constrains a point to be on a line. Keep in mind that lines are 
infinite from the constraint's point of view.

:Workplane: optional
:Selection: Line (2D or 3D), point
:Tool: Constrain coincident

Midpoint
--------

Constrains a point to be at the midpoint of a line.

:Workplane: optional
:Selection: Line (2D or 3D), point
:Tool: Constrain midpoint

Point/line distance
-------------------

Constrains the distance from a point to a line to be the entered value. 
The distance between a point and a line is the shortest path between 
the two, i.e. a line perpendicular to the line passing through the 
point.

:Workplane: optional
:Selection: Line (2D or 3D), point
:Tool: Constrain distance


Point on circle
---------------

Constrains a point to be on a circle or an arc. From the constraint's 
point of view, arcs are full circles.

:Workplane: none
:Selection: Arc/Circle (2D or 3D), point
:Tool: Constrain coincident


Point in plane
--------------

Constrains a point to be in a plane defined by two lines.

:Workplane: none
:Selection: Two lines, point
:Tool: Constrain coincident


Point in workplane
------------------

Constrains a point to be in a workplane

:Workplane: none
:Selection: Workplane, point
:Tool: Constrain point in workplane

Since version 1.1


Point/plane distance
--------------------

Constrains a point's distance from a plane defined by two lines to be the 
entered value.

:Workplane: none
:Selection: Two lines, point
:Tool: Constrain distance


Distance
--------

Constrains the (euclidean) distance between two points to the 
entered value. Selecting a line is equivalent to selecting its endpoints.

:Workplane: optional
:Selection: Two points or a line (2D or 3D)
:Tool: Constrain distance

Horizontal / Vertical distance
------------------------------

Constrains the horizontal/vertical distance between two points to the 
entered value. Selecting a line is equivalent to selecting its endpoints.

:Workplane: required
:Selection: Two points or a line (2D or 3D)
:Tool: Constrain horizontal distance, Constrain vertical distance


Horizontal / Vertical
---------------------

Constrains two points to be at the same X position (vertical) or to be 
at the same Y position (horizontal). Selecting a line is equivalent to selecting its endpoints.

:Workplane: required
:Selection: Two points or a line (2D or 3D)
:Tool: Constrain horizontal, Constrain vertical


Symmetric horizontal / vertical
-------------------------------

Constrains two points to be symmetric about the vertical sketch axis (horizontal) or to be 
at symmetric about the horizontal sketch axis (vertical). Selecting a line is equivalent to selecting its endpoints.

:Workplane: required
:Selection: Two points or a line (2D or 3D)
:Tool: Constrain symmetric horizontally / vertically

Since version 1.1

Symmetric about line
--------------------

Constrains two points to be symmetric about a line. Selecting a line is equivalent to selecting its endpoints.

:Workplane: required
:Selection: Two points or a line (2D or 3D)
:Tool: Constrain symmetric about line

Select the line the symmetry applies to in the tool.

Since version 1.1

Diameter / Radius
-----------------

Constrains the diameter or radius of a circle or an arc to the entered 
value.

:Workplane: none
:Selection: Arc or circle
:Tool: Constrain diameter, Constrain radius

Equal length
------------

Constrains two or more lines to have the same length.

:Workplane: optional
:Selection: Two or more lines (2D or 3D)
:Tool: Constrain equal length

Equal radius
------------

Constrains two or more arcs or circles to have the same radius.

:Workplane: optional
:Selection: Two or more arcs or circles
:Tool: Constrain equal radius


Workplane normal
----------------

Constrains workplane's orientation to a plane defined by two lines.

:Workplane: none
:Selection: The to-be constrained workplane
:Tool: Constrain workplane normal

The tool is special in the way that it's interactive. After invoking 
the tool, first click on the line that should define the workplane's X 
axis, then on another line with a shared point to define the plane. 
Both lines must be in a group before the workplane.


Perpendicular
-------------

Constrains two lines to be perpendicular with respect to each other.

:Workplane: optional
:Selection: Two lines (2D or 3D)
:Tool: Constrain perpendicular


Line/points perpendicular
-------------------------

Constrains a line to be perpendicular to the vector between two points.


:Workplane: none
:Selection: Line (3D only) and two points
:Tool: Constrain perpendicular

Angle
------

Constrains the angle between two lines to the entered value.

:Workplane: optional
:Selection: Two lines (2D or 3d)
:Tool: Constrain angle


Arc/Arc tangent
---------------

Constrains two arcs to be tangent at a shared point.

:Workplane: none
:Selection: Two arcs
:Tool: Constrain parallel


Arc/Line tangent
----------------

Constrains a line and an arc to be tangent at a shared point.

:Workplane: none
:Selection: Line (2D only) and arc
:Tool: Constrain parallel



Parallel
--------

This constraint can do two things:

1. Constrains two lines to be parallel.

:Workplane: none
:Selection: Two lines (2D or 3D)
:Tool: Constrain parallel

2. Constrains a line to be parallel to the normal vector of a workplane

:Workplane: none
:Selection: Line (3D only) and workplane
:Tool: Constrain parallel



Same orientation
----------------

Constrains two workplanes/STEP models to have the same orientation. 
There's still one hidden degree of freedom along the normal in 
increments of 90°. Use the Rotate tool to get the entity to the target 
orientation.


:Workplane: none
:Selection: Two workplanes, two step models, or one workplane and one step model
:Tool: Constrain same orientation

Lock rotation
-------------

Locks the STEP model/workplane to the rotation set in the "Rotate" tool.
Even with the constraint applied, the rotate tool can still be used.

:Workplane: none
:Selection: One workplane or STEP model
:Tool: Lock rotation 


