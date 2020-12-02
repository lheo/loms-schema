.. _framework-element:

framework element
=================

The details about a semantic framework or system. Used to describe other semantic frameworks to which resources in EDCI can be associated, tagged or aligned with

.. code-block:: xml

  <framework id="...">
    <!-- SEQUENCE -->
    <identifier>...</identifier> <!-- 0,n -->
    <title>...</title> <!-- 1,n -->
    <description>...</description> <!-- 0,n -->
    <supplementaryDoc>...</supplementaryDoc> <!-- 0,n -->
  </framework>

Attributes
-----------

``id``: ``required`` :ref:`id-type`
	A portable identifier of the the semantic framework (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this semantic framework from other places within the credential document.


Elements
--------

``identifier``: :ref:`identifier-type`
	An alternative identifier of the semantic framework or system.

``title``: :ref:`languagestring-type`
	Maximum one value per language is allowed.

``description``: :ref:`note-type`
	A free text describing the semantic framework. Maximum one value per language is allowed.

``supplementaryDoc``: :ref:`document-type`
	A public web document containing additional documentation about the semantic framework. It can be any document containing further information about the the semantic framework. The document can be a web page that can be navigated or a downloadable file


