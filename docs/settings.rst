.. _settings:

#####################################
Settings
#####################################

.. _modifier_settings:

======================================================
Modifer settings
======================================================

If the resulting Flowify object is selected, there is a Flowify *Geometry Nodes* Modifier that has additional settings for the add-on:

.. image:: images/flowify_modifier.jpg

Source Object
--------------------

The Source Object the add-on will map to the Target Surface.

Source Grid
--------------------

The reference grid used to map the Source Object to the Target Surface.

Target Surface
--------------------

The Target Surface grid used to deform the Source Object.

UV Map
-----------

The name of the grid like UV Map on the Target Surface

In Bounds
-----------------

By default, the modifier will try to keep all the vertices of the Source Objects within the bounds of the Target Surface.  When the vertices hit the edge of the Target Surface, they will be bunched up on that edge:

.. image:: images/bunch_up.jpg

If you wish the object's vertices and edges to be deleted if they cross an edge, you can uncheck this setting:

.. image:: images/bunch_up_not.jpg

Translation/Rotation/Scale
--------------------------------

These settings offset the transformation of the resulting deformed object in world space.

.. image:: images/offset_controls.jpg

