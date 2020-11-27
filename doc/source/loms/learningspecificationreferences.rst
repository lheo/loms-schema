.. _learningspecificationreferences-type:

LearningSpecificationReferences
===============================



.. code-block:: xml

  <!-- CHOICE 0,n -->
  <learningSpecification>...LearningSpecification...</learningSpecification>
  <qualification>...Qualification...</qualification>
  <qualificationRef>...References...</qualificationRef>

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``learningSpecification``
      - :ref:`learningspecification-type`
      - A specification of learning. A specification or package of learning that is expressed in 1 or more learning outcomes. It is used to specify what a person did learn OR what a person can learn (e.g. by a given learning opportunity).
    * - ``qualification``
      - :ref:`qualification-type`
      - The details of a qualification that can or has been awarded such as the (expected) learning outcomes. This can be a copy or a specialization of an existing qualification standard.
    * - ``qualificationRef``
      - :ref:`references-type`
      - Reference for a qualification from another dataset that can or has been awarded such as the (expected) learning outcomes.

