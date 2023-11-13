
.. _howto:

#####################################
How To Use
#####################################

.. note::
    If you're having any trouble, don't hesitate to :ref:`contact us<Contact>`.

Pre-Requisites
------------------------

.. image:: images/source_target_objects.jpg

Once :ref:`installed<installation>`, for Flowify to work in Blender you will need the following objects arranged as above:

#. The **Source Object** that you wish to deform.

    .. note::
        The deformation will only be as good as an object’s mesh topology.

#. A flat rectangular **Source Grid** to use as a reference for the target surface.

    .. note::
        .. image:: images/source_grid.jpg
        
        Flowify understands a source grid to consist of 4 sided faces with 4 distinct corners and to be entirely flat.  Its face direction (or |normals|) should also match the Target Surface.

#. An irregularly shaped **Target Surface** consisting of **evenly spaced** 4 sided faces with 4 distinct corners.


    .. note::
        .. image:: images/target_grid.jpg
        
        The vertices of the grid must be evenly spaced for Flowify to work well.  Blender's built in |Loop Tools| add-on's *Space* operation should help with this.
        
        The target surface should also consist of 4 sided faces with 4 distinct corners.  Its face direction (or |normals|) should also match the Source Grid. 

.. |Loop Tools| raw:: html

   <a href="https://docs.blender.org/manual/en/latest/addons/mesh/looptools.html" target="_blank">Loop Tools</a>

.. |normals| raw:: html

    <a href="https://docs.blender.org/manual/en/2.79/modeling/meshes/editing/normals.html" target="_blank">Normals</a>

Step by Step
---------------------

.. figure:: images/flowify_stepbystep.gif

    The Flowify workflow in Blender

The workflow is as follows:

#. In object mode, **select the Source Object(s)** and right-click in the viewport.  Select 'Flowify' from the menu that appears. 

    .. image:: images/right_click_menu.jpg

    .. note:: 
        You can select multiple source objects at once.


#. By default, the viewport will change to :ref:`face orientation<face_orientation>` mode so you can make sure the face directions (or |normals|) of the **Source Grid** and **Target Surface** are pointing in the same way (ie the same blue colour).

    .. image:: images/face_orientation_mode.jpg

    .. note:: 
        .. figure:: images/face_orientation_good_bad.jpg
        
        Good and bad face orientations. Both matching sides of the source and the target surface objects should be blue for the add-on to work correctly.  Red faces denote faces with their directions (or |Normals|) pointing in the opposite direction.

#. Hover the mouse over the **Source Grid** to detect a corner on the grid.  When a corner is detected, a circle will appear on the corner.  Click the left mouse button to select this corner and continue.

    .. image:: images/source_grid_corner_circle.jpg

#. Hover the mouse over the **Target Surface** and click the matching corner.  A line should appear between the Source Grid and the Target Surface, indicating how the mapping will be applied.

    .. image:: images/target_grid_corner_circle.jpg

    .. note:: 
        It is important that the corner of the **Source Grid** is aligned to the same representative corner on the **Target Surface** to match the correct orientation.

#. The **Source Object** should be mapped onto the Target Surface in a new object called *Source Object* + *Flowify*. 
    
   In this object, there is a :ref:`Flowify Modifier<modifier_settings>` which has :ref:`additional settings<modifier_settings>`:

   .. image:: images/flowify_complete.jpg


.. note::
    Check out the :ref:`Tips and Troubleshooting<troubleshooting>` section and don't hesitate to :ref:`contact us<Contact>` if you are having issues.