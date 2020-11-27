.. _learningoutcomes-type:

LearningOutcomes
================

A list of learning outcomes.

.. code-block:: xml

  <!-- SEQUENCE -->
  <learningOutcome>...IdReference...</learningOutcome> <!-- 1,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``learningOutcome``
      - :ref:`idreference-type`
      - An individual (expected) learning outcome of the learning specification/qualification. It MUST refer to an existing :ref:`learningoutcome-type` in the :ref:`learningoutcomes-type` of this document.

