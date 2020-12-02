.. _scoringschemereferences-element:

scoringSchemeReferences element
===============================

Container element to record all Scoring - or Grading Scheme entities that can be linked or refered to from other places in the xml document.

.. code-block:: xml

  <scoringSchemeReferences>
    <!-- SEQUENCE -->
    <scoringScheme>...</scoringScheme> <!-- 0,n -->
  </scoringSchemeReferences>

Elements
--------

``scoringScheme``: :ref:`scoringscheme-element`
	A scoring scheme. A numeric or text type of scoring methodology or convention. A grading system.


