Workspace views
===============

To quickly switch between different viewing angles and group/body 
visibility settings, Dune 3D supports workspace views. A workspace view 
stores

* Camera position (pan)
* Camera angle (rotation)
* Zoom
* Projection (perspective / orthographic)
* For each opened document

  * Visibility
  * Visibility of construction entities from previous groups
  * Current group
  * Groups visibility
  * For each body

    * Visibility
    * Solid model visibility
 
Workspace views can be created by clicking the plus icon in the 
bottom-right corner of the window or from the context menu of an 
existing workspace view.

While a single workspace view can contain information relating to 
multiple documents, workspace views are stored per-document alongside 
the document itself with the extension ``.d3dwrk`` if it is visible in 
the workspace view. When opening 
multiple documents, their workspace views will get merged.

By default, workspace views don't have a name and are shown with the 
name of the visible documents. To rename a workspace view, double-click 
its tab or choose rename from the tab's context menu.

