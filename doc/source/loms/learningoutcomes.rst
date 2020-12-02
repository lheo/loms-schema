.. _learningoutcomes-element:

learningOutcomes element
========================

Learning outcomes of the learning specification or qualification.

.. code-block:: xml

  <learningOutcomes>
    <!-- SEQUENCE -->
    <learningOutcome>...</learningOutcome> <!-- 1,n -->
  </learningOutcomes>

Elements
--------

``learningOutcome``: :ref:`idreference-type`
	An individual (expected) learning outcome of the learning specification/qualification. It MUST refer to an existing :ref:`learningoutcome-type` in the :ref:`learningoutcomereferences-element` of this document.


