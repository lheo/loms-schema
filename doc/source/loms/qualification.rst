.. _qualification-type:

Qualification
=============

The details of a qualification that can or has been awarded such as the (expected) learning outcomes. This can be a copy or a specialization of an existing qualification standard. A qualification can be part of a national qualification framework (NQF Qualification) which can be specified by the NQF level.

.. code-block:: xml

  <!-- SEQUENCE -->
  <!-- begin group LearningSpecificationElements -->
  <identifier>...</identifier> <!-- 0,n -->
  <type>...</type> <!-- 0,n -->
  <title>...</title> <!-- 1,n -->
  <altLabel>...</altLabel> <!-- 0,n -->
  <definition>...</definition> <!-- 0,n -->
  <description>...</description> <!-- 0,n -->
  <additionalNote>...</additionalNote> <!-- 0,n -->
  <homepage>...</homepage> <!-- 0,n -->
  <supplementaryDoc>...</supplementaryDoc> <!-- 0,n -->
  <hasISCED-FCode>...</hasISCED-FCode> <!-- 1,n -->
  <hasEducationSubject>...</hasEducationSubject> <!-- 0,n -->
  <volumeOfLearning>...</volumeOfLearning> <!-- 0,1 -->
  <hasECTSCreditPoints>...</hasECTSCreditPoints> <!-- 0,1 -->
  <hasCreditPoints>...</hasCreditPoints> <!-- 0,n -->
  <hasEducationLevel>...</hasEducationLevel> <!-- 0,n -->
  <language>...</language> <!-- 0,n -->
  <mode>...</mode> <!-- 0,n -->
  <learningSettingType>...</learningSettingType> <!-- 0,1 -->
  <duration>...</duration> <!-- 0,1 -->
  <targetGroup>...</targetGroup> <!-- 0,n -->
  <entryRequirementsNote>...</entryRequirementsNote> <!-- 0,n -->
  <learningOutcomes>...</learningOutcomes> <!-- 1,1 -->
  <learningActivitySpecification>...</learningActivitySpecification> <!-- 0,1 -->
  <assessmentSpecification>...</assessmentSpecification> <!-- 0,1 -->
  <entitlementSpecification>...</entitlementSpecification> <!-- 0,n -->
  <awardingOpportunities>...</awardingOpportunities> <!-- 0,1 -->
  <!-- end group LearningSpecificationElements -->
  <isPartialQualification>...</isPartialQualification> <!-- 0,1 -->
  <eqfLevel>...</eqfLevel> <!-- 1,1 -->
  <nqfLevel>...</nqfLevel> <!-- 1,n -->
  <qualificationCode>...</qualificationCode> <!-- 0,n -->
  <hasPart>...</hasPart> <!-- 0,n -->
  <specializationOf>...</specializationOf> <!-- 0,1 -->

Elements
--------

``identifier``: :ref:`identifier-type`
	

``type``: :ref:`learningopportunitytype-type`
	The type of learning opportunity that the learning specification/qualification is a part of. The form(at) or type of learning opportunity for which this learning specification/qualification (curricula) is designed. It needs to have some pedalogical relevance or some logical relevance in the structure of the curricula of the learning specification/qualification. In case of a tree of learning opportunities (cfr hasPart poperty), make sure that the proper structure is followed. All types can be put on the top level but the type of the descendant nodes is limited by the types of their ancestors. e.g. 'Degree programme' > 'Module' > 'Course' > 'Class'

``title``: :ref:`languagestring-type`
	The exact and official title of the learning specification/qualification. Maximum one value per language is allowed.

``altLabel``: :ref:`languagestring-type`
	

``definition``: :ref:`note-type`
	Short and abstract description about the learning specification/qualification. Maximum one value per language is allowed.

``description``: :ref:`note-type`
	The full learning outcome description of the learning specification/qualification. Maximum one value per language is allowed.

``additionalNote``: :ref:`note-type`
	An additional free text note containing any further information about a learning specification/qualification.

``homepage``: :ref:`document-type`
	The homepage (a public web document) of the learning specification/qualification. There can be only one learning specification/qualification that has a particular homepage.

``supplementaryDoc``: :ref:`document-type`
	A public web document containing additional documentation about the learning specification/qualification, such as a diploma or certificate supplement. It can be any document containing further information about the learning specification/qualification. The document can be a web page that can be navigated or a downloadable file.

``hasISCED-FCode``: :ref:`iscedfoetcode-type`
	The ISCED FoET 2013 classification code. It indicates the thematic area of the learning specification/qualification.

``hasEducationSubject``: :ref:`haseducationsubject-type`
	An associated field of education from another semantic framework than the ISCED classification.

``volumeOfLearning``: `xs:duration <https://www.w3.org/TR/xmlschema11-2/#duration>`_
	An indication of how many hours of learning efforts are needed, i.e. notional learning hours.

``hasECTSCreditPoints``: :ref:`ectscreditpoints-type`
	The credit points assigned to the learning specification/qualification, following the ECTS credit system.

``hasCreditPoints``: :ref:`creditpoints-type`
	The credit points assigned to the learning specification/qualification, following a given credit system other than ECTS.

``hasEducationLevel``: :ref:`haseducationlevel-type`
	An associated level of education within a semantic framework describing education levels.

``language``: :ref:`languagecode-type`
	The instruction and/or assessment language(s) used.

``mode``: :ref:`learningmode-type`
	The mode of learning and or assessment (i.e. online, blended, presential, work based)

``learningSettingType``: :ref:`learningsettingtype-type`
	The type of learning setting (i.e. formal learning, non-formal learning).

``duration``: `xs:duration <https://www.w3.org/TR/xmlschema11-2/#duration>`_
	The maximum duration of a learning opportunity for which this specification/qualification is designed. The maximum duration a learning opportunity that implements this specification/qualification should take.

``targetGroup``: :ref:`targetgroupcode-type`
	A specific target group or category for which this specification/qualification is designed.

``entryRequirementsNote``: :ref:`note-type`
	Specific entry requirements or prerequisites of individuals for which this specification/qualification is designed. Maximum one value per language is allowed.

``learningOutcomes``: :ref:`learningoutcomes-type`
	Learning outcomes of the learning specification or qualification.

``learningActivitySpecification``: :ref:`idreference-type`
	What will or can an individual do to acquire the expected learning outcomes. The learning activities. It MUST refer to an existing record in the 'learningActivitySpecificationReferences-section of this document.

``assessmentSpecification``: :ref:`idreference-type`
	How will a learner be assessed to proof the (expected) learning outcomes. The assessments. It MUST refer to an existing record in the 'assessmentSpecificationReferences-section of this document.

``entitlementSpecification``: :ref:`idreference-type`
	A specification of an entitlement to which this learning specification/qualification may give rise to. A specification of a right this learning specification/qualification may give access to. It MUST refer to an existing record in the 'entitlementSpecificationReferences-section of this document.

``awardingOpportunities``: :ref:`awardingopportunities-type`
	Refers to activities related to the awarding of the learning specification/qualification, such as the country or region where the learning specification/qualification is or was awarded, the awarding body and optionally the awarding period now or in the past.

``isPartialQualification``: `xs:boolean <https://www.w3.org/TR/xmlschema11-2/#boolean>`_
	Indicates whether a qualification is a full qualification or part of another qualification. In the latter, the qualification is only obtained as a formal outcome of a “broader” qualification of which it is part.

``eqfLevel``: :ref:`eqflevel-type`
	The qualification level as specified by the European Qualification Framework.

``nqfLevel``: :ref:`nqflevel-type`
	A qualification can be part of a national qualification framework (NQF Qualification) which can be specified by the NQF level. This the qualification level as specified by a National Qualifications Framework.

``qualificationCode``: :ref:`qualificationcode-type`
	An identifying code from a qualification based reference semantic asset. This property is used to classify the qualification information with a qualification from a known qualification framework. (e.g. the link to the accredidated NQF qualification)

``hasPart``: :ref:`idreference-type`
	A qualification can be part of another "broader" qualification. It MUST refer to an existing record in the 'learningSpecificationReferences'-section of this document.

``specializationOf``: :ref:`idreference-type`
	A qualification (e.g. a standard) of which this specification is a specialization. An opportunity can have its own specific curricula, based on or in addition to a given standard. In this case the qualification of the opportunity is a specialization of another LearningSpecification which is a standard. It MUST refer to an existing record in the 'learningSpecificationReferences'-section of this document.


Attributes
-----------

``id``: ``required`` :ref:`id-type`
	A portable identifier of the qualification. (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this qualification from other places within the document.


