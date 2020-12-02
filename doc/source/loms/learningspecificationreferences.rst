.. _learningspecificationreferences-element:

learningSpecificationReferences element
=======================================

Container element to record all LearningSpecification entities that can be linked or refered to from other places in the xml document.

.. code-block:: xml

  <learningSpecificationReferences>
    <!-- CHOICE 0,n -->
    <learningSpecification>...</learningSpecification>
    <qualification>...</qualification>
    <qualificationRef>...</qualificationRef>
  </learningSpecificationReferences>

Elements
--------

``learningSpecification``: :ref:`learningspecification-element`
	A specification of learning. A specification or package of learning that is expressed in 1 or more learning outcomes. It is used to specify what a person did learn OR what a person can learn (e.g. by a given learning opportunity).

``qualification``: :ref:`qualification-element`
	The details of a qualification that can or has been awarded such as the (expected) learning outcomes. This can be a copy or a specialization of an existing qualification standard.

``qualificationRef``: :ref:`qualificationref-element`
	Reference for a qualification from another dataset that can or has been awarded such as the (expected) learning outcomes.


