.. _semanticframework-type:

SemanticFramework
=================

The details about a semantic framework or system. Used to describe other semantic frameworks to which resources in EDCI can be associated, tagged or aligned with

.. code-block:: xml

  <!-- SEQUENCE -->
  <identifier>...Identifier...</identifier> <!-- 0,n -->
  <title>...LanguageString...</title> <!-- 1,n -->
  <description>...Note...</description> <!-- 0,n -->
  <supplementaryDoc>...Document...</supplementaryDoc> <!-- 0,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``identifier``
      - :ref:`identifier-type`
      - An alternative identifier of the semantic framework or system.
    * - ``title``
      - :ref:`languagestring-type`
      - Maximum one value per language is allowed.
    * - ``description``
      - :ref:`note-type`
      - A free text describing the semantic framework. Maximum one value per language is allowed.
    * - ``supplementaryDoc``
      - :ref:`document-type`
      - A public web document containing additional documentation about the semantic framework. It can be any document containing further information about the the semantic framework. The document can be a web page that can be navigated or a downloadable file


.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``id``
      - ``required`` :ref:`id-type`
      - A portable identifier of the the semantic framework (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this semantic framework from other places within the credential document.
