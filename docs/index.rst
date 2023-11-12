.. Flowify documentation master file, created by
   sphinx-quickstart on Sat Nov 11 17:11:53 2023.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Flowify
===================================

---------------------------------
What is Flowify?
---------------------------------

Flowify is a Blender add-on for 3D modelers enabling them to map an object to any quad surface with four corners.  This allows for the creation of interesting shapes that can be challenging to model otherwise.


.. |Flowify| raw:: html

   <a href="https://blendermarket.com/products/flowify">Conform Object</a>

For Flowify to work in Blender you will need:

#. The **Source Object** that you wish to deform
#. The flat rectangular **Source Grid** to use as a reference for the surface.
#. The **Target Surface** consisting of quad faces with 4 distinct corners.

In the viewport, right-click in object mode and select 'Flowify'. By default, the viewport will change to face orientation mode to make sure the faces of the **Source Grid** and **Target Grid** are pointing in the same direction (ie the same blue colour). Then:

#. Select the **Source Object**.
#. Select a corner on the **Source Grid**.
#. Select the equivalent corner on the **Target Grid**.

Then, the **Source Object** should be copied onto the Target Surface.

.. note::
    If you're having any trouble and it is not answered here, don't hesitate to :ref:`contact us<Contact>`.


-----------------
Features:
-----------------

* A quick interactive workflow allows for the quick creation once the objects are set up.
* Simple right-click menu option starts.
* Any changes to the original object are automatically updated.


.. toctree::
   :maxdepth: 2
   :caption: Contents:
   
   contact



Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
