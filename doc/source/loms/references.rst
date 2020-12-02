.. _qualificationref-element:

qualificationRef element
========================

Reference for a qualification from another dataset that can or has been awarded such as the (expected) learning outcomes.

.. code-block:: xml

  <qualificationRef id="...">
    <!-- SEQUENCE -->
    <identifier>...</identifier> <!-- 1,1 -->
  </qualificationRef>

Attributes
-----------

``id``: ``required`` :ref:`id-type`
	A portable identifier of the qualification. (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this qualification from other places within the credential document.


Elements
--------

``identifier``: :ref:`identifier-type`
	


