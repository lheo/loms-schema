.. _learningopportunity-type:

LearningOpportunity
===================

An opportunity to learn. An opportunity to realize a given set of learning outcomes via a learning activity and/or assessment. For example a training, a degree programme or a course, provided by a given institution at a given time, to obtain a certain learning award such as a qualification, this is a learning opportunity. A *learning opportunity* is the opportunity for an individual to do a set of *learning activities* where he can acquire knowledge, skills or responsibility and autonomy as proven by an assessment.


.. code-block:: xml

  <!-- SEQUENCE -->
  <identifier>...</identifier> <!-- 1,n -->
  <title>...</title> <!-- 1,n -->
  <altLabel>...</altLabel> <!-- 0,n -->
  <description>...</description> <!-- 0,n -->
  <additionalNote>...</additionalNote> <!-- 0,n -->
  <homepage>...</homepage> <!-- 0,n -->
  <supplementaryDoc>...</supplementaryDoc> <!-- 0,n -->
  <startedAtDate>...</startedAtDate> <!-- 0,1 -->
  <endedAtDate>...</endedAtDate> <!-- 0,1 -->
  <duration>...</duration> <!-- 0,1 -->
  <learningSchedule>...</learningSchedule> <!-- 0,1 -->
  <scheduleInformation>...</scheduleInformation> <!-- 0,n -->
  <admissionProcedure>...</admissionProcedure> <!-- 0,n -->
  <priceDetails>...</priceDetails> <!-- 0,n -->
  <providedBy>...</providedBy> <!-- 1,n -->
  <providedAt>...</providedAt> <!-- 0,n -->
  <specifiedBy>...</specifiedBy> <!-- 1,1 -->
  <hasPart>...</hasPart> <!-- 0,n -->
  <referenceLanguage>...</referenceLanguage> <!-- 0,1 -->

Elements
--------

``identifier``: :ref:`identifier-type`
	An alternative identifier of the learning opportunity.

``title``: :ref:`languagestring-type`
	The title of the learning opportunity (e.g. name of a course offered at a given institution). Maximum cardinality of one per language.

``altLabel``: :ref:`languagestring-type`
	An alternative name of the learning opportunity.

``description``: :ref:`note-type`
	A free text description of the learning opportunity. Maximum cardinality of one per language.

``additionalNote``: :ref:`note-type`
	An additional free text note (e.g. a comment, a remark, …) containing any further information about the learning opportunity.

``homepage``: :ref:`document-type`
	The homepage (a public web document) of the learning opportunity. There can be only one learning opportunity that has a particular homepage.

``supplementaryDoc``: :ref:`document-type`
	A public web document containing additional documentation about the learning opportunity. It can be any document containing further information about the learning opportunity. The document can be a web page that can be navigated or a downloadable file.

``startedAtDate``: `xs:date <https://www.w3.org/TR/xmlschema11-2/#date>`_
	The start date when the learning opportunity will take place.

``endedAtDate``: `xs:date <https://www.w3.org/TR/xmlschema11-2/#date>`_
	The end date until when the learning opportunity will take or took place.

``duration``: `xs:duration <https://www.w3.org/TR/xmlschema11-2/#duration>`_
	The nominal duration of the learning opportunity. The duration for which the learning opportunity will continue to be offered.

``learningSchedule``: :ref:`learningscheduletype-type`
	The learning schedule. How often you need to go (i.e full time (more than 30 hours), PT intensive (8-30 hoours), PT light (less than 8 hours)).

``scheduleInformation``: :ref:`note-type`
	A free text note about the time schedule. More detailed information about the actual timetable (e.g twice a week, mondays at 4 pm,...). Maximum one value per language is allowed.

``admissionProcedure``: :ref:`note-type`
	A free text note about the admission procedure. Maximum one value per language is allowed.

``priceDetails``: :ref:`pricedetails-type`
	The price details.

``providedBy``: :ref:`idreference-type`
	The providing or directing agent. The cardinality can be more than one in case the learning opportunity is provided/organized by a collaboration of different agents, (e.g. co-awarding). It MUST refer to an existing 'organization'-record in the 'agentReferences'-section.

``providedAt``: :ref:`location-type`
	The location where the learning opportunity will take place (e.g. course location).

``specifiedBy``: :ref:`idreference-type`
	The learning specification, including the curricula, of this learning opportunity. It MUST refer to an existing 'learningSpecification'- or 'quailification'- record in the 'learningSpecificationReferences'-section of the xml document.

``hasPart``: :ref:`idreference-type`
	A learning opportunity can be composed of other learning opportunities. It MUST refer to an existing 'learningOpportunity'-record in the 'learningOpportunityReferences'-section of the xml document.

``referenceLanguage``: :ref:`languagecode-type`
	The language in which information about the learning opportunity is available in the NDS.


Attributes
-----------

``id``: ``required`` :ref:`id-type`
	A portable identifier of the learning opportunity (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this learning opportunity from other places within the document.


