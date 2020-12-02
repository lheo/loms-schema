.. _learningoutcome-type:

LearningOutcome type
====================

A learning outcome (i.e. knowledge, skill, autonomy-responsibility). The details, such as the description, of a learning outcome.

.. code-block:: xml

  <... id="...">
    <!-- SEQUENCE -->
    <identifier>...</identifier> <!-- 0,n -->
    <prefLabel>...</prefLabel> <!-- 1,n -->
    <description>...</description> <!-- 0,n -->
    <learningOutcomeType>...</learningOutcomeType> <!-- 0,1 -->
    <reusabilityLevel>...</reusabilityLevel> <!-- 0,1 -->
    <relatedEscoSkill>...</relatedEscoSkill> <!-- 0,n -->
  </...>


Attributes
-----------

``id``: ``optional`` :ref:`id-type`
	A portable identifier of the learning outcome (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this learning outcome from other places within the document document.


Elements
--------

``identifier``: :ref:`identifier-type`
	

``prefLabel``: :ref:`languagestring-type`
	A legible, descriptive name for the learning outcome. Maximum cardinality of one per language.

``description``: :ref:`note-type`
	A free text describing the learning outcome. Maximum cardinality of one per language.

``learningOutcomeType``: :ref:`learningoutcometype-element`
	The learning outcome type (i.e. knowledge, skill, ...).

``reusabilityLevel``: :ref:`reusabilitylevel-element`
	The reusability level.

``relatedEscoSkill``: :ref:`relatedescoskill-element`
	A link/alignment to an ESCO Skill.


