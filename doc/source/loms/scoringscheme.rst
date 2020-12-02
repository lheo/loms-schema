.. _scoringscheme-element:

scoringScheme element
=====================

A scoring scheme. A numeric or text type of scoring methodology or convention. A grading system.

.. code-block:: xml

  <scoringScheme id="...">
    <!-- SEQUENCE -->
    <identifier>...</identifier> <!-- 0,n -->
    <title>...</title> <!-- 1,n -->
    <description>...</description> <!-- 0,n -->
    <supplementaryDoc>...</supplementaryDoc> <!-- 0,n -->
  </scoringScheme>

Attributes
-----------

``id``: ``required`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	A portable identifier of the grading system (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this grading system from other places within the credential document.


Elements
--------

``identifier``: :ref:`identifier-type`
	A scoring scheme identifier.

``title``: :ref:`languagestring-type`
	Maximum one value per language is allowed.

``description``: :ref:`note-type`
	A free text describing the scoring methodology or convention. Maximum one value per language is allowed.

``supplementaryDoc``: :ref:`document-type`
	A public web document containing additional documentation about the scoring/grading system. It can be any document containing further information about the scoring system. The document can be a web page that can be navigated or a downloadable file


