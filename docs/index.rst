.. Flowify documentation master file, created by
   sphinx-quickstart on Sat Nov 11 17:11:53 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Flowify
===================================


.. image:: images/flowify_in_action.gif
  :alt: Perspective Plotter at work

---------------------------------
What is Flowify?
---------------------------------

.. image:: images/source_target_objects.jpg

|Flowify| is a Blender add-on for 3D modelers that bends an object, called the **Source Object**, to a surface object with evenly spaced four sided faces and four corners, called the **Target Surface**. A flat reference grid object called the **Source Grid** is used to guide the add-on.  All these objects are created by the modeler themselves as regular objects, and the add-on uses these objects to generate the result.

This enables the creation of interesting objects that could be challenging to model otherwise.

.. note::

    It is based on the |Flowify Sketchup plugin| of the same name, which is in turn based on the |MoveAlongSurf| command in Rhino.

.. |Flowify| raw:: html

   <a href="https://blendermarket.com/products/flowify">Flowify</a>

.. |Flowify Sketchup plugin| raw:: html

   <a href="https://sketchucation.com/pluginstore?pln=flowify" target="_blank">Flowify Sketchup plugin</a>


.. |MoveAlongSurf| raw:: html

   <a href="https://docs.mcneel.com/rhino/5/help/en-us/commands/flowalongsrf.htm" target="_blank">MoveAlongSurf</a>



-----------------
Features:
-----------------

.. image:: images/move_demo.gif

* Change the Source Object and the result will be automatically updated.
* Change the Target Surface and the result will automatically update as well.
* Use on regular objects, instanced objects and text (:ref:`As long as they have deformable topology<troubleshooting>`).
* Materials will be copied over to as well.
* See the :ref:`Step By Step<howto>` guide for how to use.
* Configure a Flowify :ref:`modifier<modifier_settings>` with additional options afterwards.
* Use optionally in Blender's |Quad View| mode:

   .. image:: images/quad_view.png

.. |Quad View| raw:: html

   <a href="https://docs.blender.org/manual/en/latest/editors/3dview/navigate/views.html#quad-view" target="_blank">Quad View</a>

-----------------
Please Note!
-----------------

The deformation will only be as good as a Source Object's mesh topology.

--------------------------------------------------------------------
Differences to the |Conform Object| add-on:
--------------------------------------------------------------------

Workflow Approach:
^^^^^^^^^^^^^^^^^^^^^

* |Conform Object|: Offers a one-click workflow designed for efficiency and minimal setup time, making it more useful for quick tasks.
* |Flowify|: Requires some initial setup but offers a more detailed workflow. Tailored for users who need more control and customization in their projects.

Projection Capabilities:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* |Conform Object|: Suited for projecting objects in a single direction onto any surface. Ideal for simple, straightforward surface projections.
* |Flowify|: Specializes in wrapping objects onto a custom-designed target surface with exactly four corners of quad faces. This feature allows Flowify to handle a wider variety of objects and directions for more complex wrapping tasks.

Suitability for Surface Types:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* |Conform Object|: Projects smaller objects to the existing surfaces of larger objects, making it ideal for simpler, more direct projections.
* |Flowify|: Able to wrap objects around complex surface shapes, offering more flexibility for advanced modeling requirements.

Preset System:
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

* |Conform Object|: Includes a presets system for saving and applying settings for repeated tasks.
* |Flowify|: Currently does not have a presets system, catering to users who prefer manual control over each project's unique requirements.

If you are undecided about which add-on suits your needs, don't hesitate to :ref:`Contact Us<contact>`

.. |Conform Object| raw:: html

   <a href="https://blendermarket.com/products/conform-object">Conform Object</a>


.. toctree::
   :maxdepth: 2
   :caption: Contents:
   
   installation
   use
   settings
   preferences
   troubleshooting
   how_does_it_work
   contact



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
