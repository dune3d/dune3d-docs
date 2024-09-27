Usage
=====

Navigation
----------

Move around the 3D viewport either with mouse, touchpad, trackpoint, 
touchscreen or keyboard.

Mouse
^^^^^

:Dragging middle mouse button:  Pan
:Dragging right mouse button + Shift:  Pan
:Dragging right mouse button:  Rotate
:Dragging middle mouse button + Shift:  Rotate
:Dragging right mouse button + Ctrl:  Tilt
:Double middle click:  Reset tilt
:Scrolling:  Zoom

Several rotation schemes for translating 2D motion to 3D rotation are 
available in the settings dialog.

Trackpoint
^^^^^^^^^^

:Scrolling:  Pan
:Scrolling + Shift:  Rotate
:Scrolling + Ctrl:  Zoom


Touchpad / Touchscreen
^^^^^^^^^^^^^^^^^^^^^^

Use two-finger gestures for pan, zoom and rotation.

Keyboard
^^^^^^^^

:Arrow keys:  Pan
:Arrow keys + Shift: Rotate
:Left/right + Shift + Ctrl: Tilt

These key bindings can be configured in the preferences dialog.

Actions
^^^^^^^

Double-click a workplane to center and align the view to it. Also see 
further actions available from the context and spacebar menu in the 
"View" group.

Help, I'm stuck!
^^^^^^^^^^^^^^^^

In some cases, such as looking at the ZX plane, the rotation axis coincide,
leaving only one rotational degree of freedom when using the turntable 
rotation scheme. In this case, hold 
:kbd:`Ctrl` to change the tilt axis or reset the tilt axis to go back 
to normal rotation.

If you're totally lost, use the "Reset view" action to look at the XY 
plane.

Solid model
-----------

Show or hide the current body's solid model by clicking on the cube 
next to it in the workspace browser in the left side of the window. 
Right-clicking on a body row in the workspace browser opens a context 
menu for renaming the body or changing its solid model color.

Use clipping planes to hide parts of the solid model.


Where to find things
--------------------

All tools and actions are available from the spacebar menu. Open it by 
by pressing :kbd:`Space` anywhere in the 3D viewport.

Tools and actions specific to the selection are also available from the 
context menu that can be invoked by the right mouse button.

For some tools and actions, there are predefined keyboard shortcuts 
that are listed in the spacebar menu. All keyboard shortcuts can be 
customized in the preferences window.

Tools
-----

After having started a tool, it receives all keyboard and mouse input, 
until the tool is finished or you end it by pressing :kbd:`Esc`.
Look at the bar that appeared at the bottom of the viewport to see what
pressing keys will do in this particular tool.


Points
------

Points are rendered as different icons depending on their type:

:■ Square: End points of lines, arcs, and bezier curves
:◆ Diamond: Origins of workplanes, STEP models, document entities, clusters and texts
:▼ Down-pointing triangle: Anchors of STEP models, clusters and texts
:● Circle: Bezier control points
:✖ Cross: Centers of circles and arcs

Selection
---------

The selection in Dune 3D has two distinct modes. In hover select mode, 
the item under the cursor is selected automatically and can be used in 
tools. So you only need to hover over an item before deleting it by 
pressing :kbd:`Del`.

Clicking on an item switches to click select mode. In click select 
mode, the current selection is retained until it's explicitly modified. 
Clicking on an item adds or removes it from the current selection. 

Clicking on an item multiple times brings up the selection menu to 
accurately select overlapping items. This menu can be invoked directly
by holding down :kbd:`Shift` when clicking on an item.

Pressing :kbd:`Esc` clears the current selection and returns to hover 
select mode.

The current selection mode is shown in the bottom left corner of the 
window.

Hovering over a constraint highlights the constrained entities.


Groups
------

Click on a group in the workspace browser on the left side of the 
window to make it the current group. The current group is shown in 
boldface. All groups after the current group are hidden automatically. 
Individual groups and bodies before the current group can be hidden by 
clicking on the checkbox. The number at the right side indicates the 
degrees of freedom for the group.

You can also switch groups with the :kbd:`PgUp`/:kbd:`PgDn` keys or the 
back/forward buttons on your mouse.

See :doc:`groups` for more details on them.

Workplanes
----------

The current group's workplane is shown in the status bar. Clear the 
checkbox to temporarily turn off the group's workplane for constraining 
in 3D. The active workplane is rendered with a double border.

Multiple documents
------------------

From version 1.2 onward, multiple documents can be opened in one 
window simultaneously, though just one document can be active at a 
time. The active document is shown in boldface in the workspace browser.
Only the active document can be interacted with. To switch the active 
document, select one of its groups in the workspace browser or 
double-click on one of its entities. Workplanes from inactive documents 
are hidden to reduce clutter.

This feature closely interacts with Document entities. Linking another 
document as an entity also opens it in the current window. Changes to 
the document are automatically reflected in all of its instances 
(document entities).
