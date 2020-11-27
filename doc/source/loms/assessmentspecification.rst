.. _assessmentspecification-type:

AssessmentSpecification
=======================

An AssessmentSpecification is a specification of a process establishing the extent to which a learner has attained particular knowledge, skills and competences against criteria such as learning outcomes or standards of competence.

.. code-block:: xml

  <!-- SEQUENCE -->
  <!-- begin group CommonSpecificationElements -->
  <identifier>...Identifier...</identifier> <!-- 0,n -->
  <title>...LanguageString...</title> <!-- 0,n -->
  <altLabel>...LanguageString...</altLabel> <!-- 0,n -->
  <description>...Note...</description> <!-- 0,n -->
  <additionalNote>...Note...</additionalNote> <!-- 0,n -->
  <homepage>...Document...</homepage> <!-- 0,n -->
  <supplementaryDoc>...Document...</supplementaryDoc> <!-- 0,n -->
  <!-- end group CommonSpecificationElements -->
  <type>...AssessmentType...</type> <!-- 0,n -->
  <language>...LanguageCode...</language> <!-- 0,n -->
  <mode>...LearningMode...</mode> <!-- 0,n -->
  <gradingScheme>...GradingScheme...</gradingScheme> <!-- 0,n -->
  <proves>...IdReference...</proves> <!-- 0,n -->
  <hasPart>...IdReference...</hasPart> <!-- 0,n -->
  <specializationOf>...IdReference...</specializationOf> <!-- 0,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``identifier``
      - :ref:`identifier-type`
      - An alternative identifier of the specification.
    * - ``title``
      - :ref:`languagestring-type`
      - The title of the specification. Maximum one value per language is allowed.
    * - ``altLabel``
      - :ref:`languagestring-type`
      - An alternative name of the specification.
    * - ``description``
      - :ref:`note-type`
      - A free text description of the specification. Maximum one value per language is allowed.
    * - ``additionalNote``
      - :ref:`note-type`
      - An additional free text note containing any further information about the specification.
    * - ``homepage``
      - :ref:`document-type`
      - The homepage (a public web document) of the specification. There can be only one specification that has a particular homepage.
    * - ``supplementaryDoc``
      - :ref:`document-type`
      - A public web document containing additional documentation about the specification. It can be any document containing further information about the specification. The document can be a web page that can be navigated or a downloadable file.
    * - ``type``
      - :ref:`assessmenttype-type`
      - The type of assessment. A concept indicating the type of assessment.
    * - ``language``
      - :ref:`languagecode-type`
      - The language(s) of assessment used.
    * - ``mode``
      - :ref:`learningmode-type`
      - The mode of learning and or assessment (i.e. online, blended, presential, work based)
    * - ``gradingScheme``
      - :ref:`gradingscheme-type`
      - Used grading scheme. It MUST refer to an existing record in the 'scoringSchemeReferences'-section of this document.
    * - ``proves``
      - :ref:`idreference-type`
      - Which learning outcomes are or have been prooved. It MUST refer to an existing record in the 'learningSpecificationReferences'-section of this document.
    * - ``hasPart``
      - :ref:`idreference-type`
      - An assessment specification (a "package") can be part of another "broader" assessment specification. It MUST refer to an existing record in the 'assessmentSpecificationReferences'-section of this document.
    * - ``specializationOf``
      - :ref:`idreference-type`
      - An assessment specification (a "package") can be a specialization of another assessment specification. It MUST refer to an existing record in the 'assessmentSpecificationReferences'-section of this document.


.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``id``
      - ``required`` :ref:`id-type`
      - A portable identifier of the assessment specification. (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this assessment specification from other places within the document.

