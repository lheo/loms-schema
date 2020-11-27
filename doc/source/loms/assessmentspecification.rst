.. _assessmentspecification-type:

AssessmentSpecification
=======================

An AssessmentSpecification is a specification of a process establishing the extent to which a learner has attained particular knowledge, skills and competences against criteria such as learning outcomes or standards of competence.

.. code-block:: xml

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
  <language>...</language> <!-- 0,n -->
  <mode>...</mode> <!-- 0,n -->
  <gradingScheme>...</gradingScheme> <!-- 0,n -->
  <proves>...</proves> <!-- 0,n -->
  <hasPart>...</hasPart> <!-- 0,n -->
  <specializationOf>...</specializationOf> <!-- 0,n -->

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

``type``: :ref:`assessmenttype-type`
	The type of assessment. A concept indicating the type of assessment.

``language``: :ref:`languagecode-type`
	The language(s) of assessment used.

``mode``: :ref:`learningmode-type`
	The mode of learning and or assessment (i.e. online, blended, presential, work based)

``gradingScheme``: :ref:`gradingscheme-type`
	Used grading scheme. It MUST refer to an existing record in the 'scoringSchemeReferences'-section of this document.

``proves``: :ref:`idreference-type`
	Which learning outcomes are or have been prooved. It MUST refer to an existing record in the 'learningSpecificationReferences'-section of this document.

``hasPart``: :ref:`idreference-type`
	An assessment specification (a "package") can be part of another "broader" assessment specification. It MUST refer to an existing record in the 'assessmentSpecificationReferences'-section of this document.

``specializationOf``: :ref:`idreference-type`
	An assessment specification (a "package") can be a specialization of another assessment specification. It MUST refer to an existing record in the 'assessmentSpecificationReferences'-section of this document.


Attributes
-----------

``id``: ``required`` :ref:`id-type`
	A portable identifier of the assessment specification. (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this assessment specification from other places within the document.


