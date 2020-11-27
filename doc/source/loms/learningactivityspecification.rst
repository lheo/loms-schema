.. _learningactivityspecification-type:

LearningActivitySpecification
=============================

A LearningActivitySpecification is a specification of a process which leads to the acquisition of knowdledge, skills or responsibilty and autonomy.

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
  <type>...ActivityType...</type> <!-- 0,n -->
  <workload>...xs:duration...</workload> <!-- 0,1 -->
  <language>...LanguageCode...</language> <!-- 0,n -->
  <mode>...LearningMode...</mode> <!-- 0,n -->
  <teaches>...IdReference...</teaches> <!-- 0,n -->
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
      - :ref:`activitytype-type`
      - The type of activity. A concept indicating the type of activity.
    * - ``workload``
      - `xs:duration <https://www.w3.org/TR/xmlschema11-2/#duration>`_
      - The expected workload. The expected workload in time. The expected amount of time the learner (will) spent undergoing the learning activity. The expected duration or volume of learning measured in years, days or hours of learning activity. The expected number of learning years, days or hours. This can be an indicative number (i.e. an estimated or notional number).
    * - ``language``
      - :ref:`languagecode-type`
      - The language(s) of instruction.
    * - ``mode``
      - :ref:`learningmode-type`
      - The mode of learning and or assessment (i.e. online, blended, presential, work based)
    * - ``teaches``
      - :ref:`idreference-type`
      - The expected learning outcomes to which this learning activity specification contributes to. This is given by a LearningSpecification. A learning activity can lead to or contribute to the acquisition of a set of skills, knowdledge, autonomy and or responsibilty. It MUST refer to an existing record in the 'learningSpecificationReferences-section of this document.
    * - ``hasPart``
      - :ref:`idreference-type`
      - An assessment specification (a "package") can be part of another "broader" assessment specification. It MUST refer to an existing record in the 'learningActivitySpecificationReferences'-section of this document.
    * - ``specializationOf``
      - :ref:`idreference-type`
      - An activity specification can be a specialization of another activity specification. It MUST refer to an existing record in the 'learningActivitySpecificationReferences'-section of this document.


.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``id``
      - ``required`` :ref:`id-type`
      - A portable identifier of the learning activity specification. (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this learning activity specification from other places within the document.

