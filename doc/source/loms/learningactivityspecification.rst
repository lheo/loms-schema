.. _learningactivityspecification-type:

LearningActivitySpecification type
==================================

A LearningActivitySpecification is a specification of a process which leads to the acquisition of knowdledge, skills or responsibilty and autonomy.

.. code-block:: xml

  <... id="...">
    <!-- SEQUENCE -->
    <!-- begin group CommonSpecificationElements -->
    <identifier>...</identifier> <!-- 0,n -->
    <title>...</title> <!-- 0,n -->
    <altLabel>...</altLabel> <!-- 0,n -->
    <description>...</description> <!-- 0,n -->
    <additionalNote>...</additionalNote> <!-- 0,n -->
    <homepage>...</homepage> <!-- 0,n -->
    <supplementaryDoc>...</supplementaryDoc> <!-- 0,n -->
    <!-- end group CommonSpecificationElements -->
    <type>...</type> <!-- 0,n -->
    <workload>...</workload> <!-- 0,1 -->
    <language>...</language> <!-- 0,n -->
    <mode>...</mode> <!-- 0,n -->
    <teaches>...</teaches> <!-- 0,n -->
    <hasPart>...</hasPart> <!-- 0,n -->
    <specializationOf>...</specializationOf> <!-- 0,n -->
  </...>


Attributes
-----------

``id``: ``required`` :ref:`id-type`
	A portable identifier of the learning activity specification. (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this learning activity specification from other places within the document.


Elements
--------

``identifier``: :ref:`identifier-type`
	An alternative identifier of the specification.

``title``: :ref:`languagestring-type`
	The title of the specification. Maximum one value per language is allowed.

``altLabel``: :ref:`languagestring-type`
	An alternative name of the specification.

``description``: :ref:`note-type`
	A free text description of the specification. Maximum one value per language is allowed.

``additionalNote``: :ref:`note-type`
	An additional free text note containing any further information about the specification.

``homepage``: :ref:`document-type`
	The homepage (a public web document) of the specification. There can be only one specification that has a particular homepage.

``supplementaryDoc``: :ref:`document-type`
	A public web document containing additional documentation about the specification. It can be any document containing further information about the specification. The document can be a web page that can be navigated or a downloadable file.

``type``: :ref:`activitytype-type`
	The type of activity. A concept indicating the type of activity.

``workload``: `xs:duration <https://www.w3.org/TR/xmlschema11-2/#duration>`_
	The expected workload. The expected workload in time. The expected amount of time the learner (will) spent undergoing the learning activity. The expected duration or volume of learning measured in years, days or hours of learning activity. The expected number of learning years, days or hours. This can be an indicative number (i.e. an estimated or notional number).

``language``: :ref:`languagecode-type`
	The language(s) of instruction.

``mode``: :ref:`learningmode-type`
	The mode of learning and or assessment (i.e. online, blended, presential, work based)

``teaches``: :ref:`idreference-type`
	The expected learning outcomes to which this learning activity specification contributes to. This is given by a LearningSpecification. A learning activity can lead to or contribute to the acquisition of a set of skills, knowdledge, autonomy and or responsibilty. It MUST refer to an existing record in the 'learningSpecificationReferences-section of this document.

``hasPart``: :ref:`idreference-type`
	An assessment specification (a "package") can be part of another "broader" assessment specification. It MUST refer to an existing record in the 'learningActivitySpecificationReferences'-section of this document.

``specializationOf``: :ref:`idreference-type`
	An activity specification can be a specialization of another activity specification. It MUST refer to an existing record in the 'learningActivitySpecificationReferences'-section of this document.


