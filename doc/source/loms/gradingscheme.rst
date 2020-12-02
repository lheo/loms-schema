.. _gradingscheme-element:

gradingScheme element
=====================

Used grading scheme. It MUST refer to an existing record in the 'scoringSchemeReferences'-section of this document.

.. code-block:: xml

  <gradingScheme idref="...">
  </gradingScheme>

Attributes
-----------

``idref``: ``required`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	The id of the referenced entity (record).


