Poly-memb
=====================================

poly-memb is a Python library implementing a 2D simulator of dynamics of membranes subject to electric fields.
The module 'mesh_manager' provides functions to generate polytopal meshes by cutting and agglomerating
background meshes intersected by moving interfaces.
The module 'solvers' provides functions to implement polygonal numerical schemes.
The simulator is based on a Hybrid High Order scheme :cite:`Di-Pietro.Droniou:20` to solve flow variables
and a Discrete De Rham :cite:`Di-Pietro.Droniou:23` scheme to solve for electric variables.

Gallery
=======

.. figure:: /images/agglomeration_demo.png
   :width: 800px
   :alt: Output 1
   :figclass: align-center

   Example of supported mesh, before and after agglomeration. The polygonal interface cuts
   originally simplicial elements to originate conformal polygonal subelements.
   The cut procedure is reiterated after movement of the membrane.

.. figure:: /images/electric_solver_demo.png
   :width: 800px
   :alt: Output 2
   :figclass: align-center

   Electrostatic potential and electric field resulting from the DDR method.
   The conformal setting allows for seamless treatment of interface conditions.

.. figure:: /images/solver_flow_demo.png
   :width: 800px
   :alt: Output 3
   :figclass: align-center

   A HHO solver is used to determine the membrane velocity. Interface edges are embedded as mesh edges.


.. toctree::
   :maxdepth: 2
   :caption: Contents:

Modules
=======


Module: mesh_manager
--------------------

.. automodule:: mesh_manager
   :members:
   :undoc-members:
   :show-inheritance:
   :imported-members:

Module: HHO_stokes
------------------

.. automodule:: HHO_stokes
   :members:
   :undoc-members:
   :show-inheritance:

Module: DDR_intface
-------------------

.. automodule:: DDR_intface
   :members:
   :undoc-members:
   :show-inheritance:


Bibliography
============

.. bibliography:: main.bib
   :cited:
   :style: plain

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
