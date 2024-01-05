Usage
====

Navigation
----------

Move around the 3D viewport either with mouse, touchpad, trackpoint or 
touchscreen.

Mouse
^^^^^

:Dragging middle mouse button:  Pan
:Dragging right mouse button + Shift:  Pan
:Dragging right mouse button:  Rotate
:Dragging middle mouse button + Shift:  Rotate
:Dragging right mouse button + Ctrl:  Tilt
:Double middle click:  Reset tilt
:Scrolling:  Zoom


Trackpoint
^^^^^^^^^^

:Scrolling:  Pan
:Scrolling + Shift:  Rotate
:Scrolling + Ctrl:  Zoom


Touchpad / Touchscreen
^^^^^^^^^^^^^^^^^^^^^^

Use two-finger gestures for pan and zoom.

Actions
^^^^^^^

Double-click a workplane to center and align the view to it. Also see 
further actions available from the context and spacebar menu in the 
"View" group.

Solid model
-----------

Show or hide the current body's solid model by clicking on the cube 
next to it in the workspace browser in the left side of the window.

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
pressing keys will d1o in this particular tool.


Selection
---------

The selection in Dune 3D has two distinct modes. In hover select mode, 
the item under the cursor is selected automatically and can be used in 
tools. So you only need to hover over an item before deleting it by 
pressing :kbd:`Del`.

Clicking on an item switches to click select mode. In click select 
mode, the current selection is retained until it's explicitly modified. 
Clicking on an item adds or removes it from the current selection.

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
