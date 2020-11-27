.. _learningoutcome-type:

LearningOutcome
===============

A learning outcome (i.e. knowledge, skill, autonomy-responsibility). The details, such as the description, of a learning outcome.

.. code-block:: xml

  <!-- SEQUENCE -->
  <identifier>...Identifier...</identifier> <!-- 0,n -->
  <prefLabel>...LanguageString...</prefLabel> <!-- 1,n -->
  <description>...Note...</description> <!-- 0,n -->
  <learningOutcomeType>...LearningOutcomeType...</learningOutcomeType> <!-- 0,1 -->
  <reusabilityLevel>...ReusabilityLevel...</reusabilityLevel> <!-- 0,1 -->
  <relatedEscoSkill>...RelatedEscoSkill...</relatedEscoSkill> <!-- 0,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``identifier``
      - :ref:`identifier-type`
      - 
    * - ``prefLabel``
      - :ref:`languagestring-type`
      - A legible, descriptive name for the learning outcome. Maximum cardinality of one per language.
    * - ``description``
      - :ref:`note-type`
      - A free text describing the learning outcome. Maximum cardinality of one per language.
    * - ``learningOutcomeType``
      - :ref:`learningoutcometype-type`
      - The learning outcome type (i.e. knowledge, skill, ...).
    * - ``reusabilityLevel``
      - :ref:`reusabilitylevel-type`
      - The reusability level.
    * - ``relatedEscoSkill``
      - :ref:`relatedescoskill-type`
      - A link/alignment to an ESCO Skill.


.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``id``
      - ``optional`` :ref:`id-type`
      - A portable identifier of the learning outcome (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this learning outcome from other places within the document document.

