.. _qmslearningopportunities-element:

qmsLearningOpportunities element
================================

An opportunity to learn. An opportunity to realize a given set of learning outcomes via a learning activity and/or assessment. For example a training, a degree programme or a course, provided by a given institution at a given time, to obtain a certain learning award such as a qualification, this is a learning opportunity. A 'learning opportunity' is the opportunity for an individual to do a set of 'learning activities' where he can acquire knowledge, skills or responsibility and autonomy as proven by an assessment.

.. code-block:: xml

  <qmsLearningOpportunities>
    <!-- SEQUENCE -->
    <learningOpportunities>...</learningOpportunities> <!-- 1,1 -->
    <learningSpecificationReferences>...</learningSpecificationReferences> <!-- 0,1 -->
    <learningOutcomeReferences>...</learningOutcomeReferences> <!-- 0,1 -->
    <learningActivitySpecificationReferences>...</learningActivitySpecificationReferences> <!-- 0,1 -->
    <assessmentSpecificationReferences>...</assessmentSpecificationReferences> <!-- 0,1 -->
    <entitlementSpecificationReferences>...</entitlementSpecificationReferences> <!-- 0,1 -->
    <agentReferences>...</agentReferences> <!-- 0,1 -->
    <scoringSchemeReferences>...</scoringSchemeReferences> <!-- 0,1 -->
    <semanticFrameworkReferences>...</semanticFrameworkReferences> <!-- 0,1 -->
  </qmsLearningOpportunities>

Attributes
-----------

``xsdVersion``: ``optional`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
	used xsd version


Elements
--------

``learningOpportunities``: :ref:`learningopportunities-element`
	LearningOpportunities that are/will be published

``learningSpecificationReferences``: :ref:`learningspecificationreferences-element`
	Container element to record all LearningSpecification entities that can be linked or refered to from other places in the xml document.

``learningOutcomeReferences``: :ref:`learningoutcomereferences-element`
	Container element to record all LearningOutcome entities that can be linked or refered to from other places in the xml document.

``learningActivitySpecificationReferences``: :ref:`learningactivityspecificationreferences-element`
	Container element to record all LearningActivitySpecification entities that can be linked or refered to from other places in the xml document.

``assessmentSpecificationReferences``: :ref:`assessmentspecificationreferences-element`
	Container element to record all AssessmentSpecification entities that can be linked or refered to from other places in the xml document.

``entitlementSpecificationReferences``: :ref:`entitlementspecificationreferences-element`
	Container element to record all EntitlementSpecification entities that can be linked or refered to from other places in the xml document.

``agentReferences``: :ref:`agentreferences-element`
	Container element to record all Organization entities that can be linked or refered to from other places in the xml document.

``scoringSchemeReferences``: :ref:`scoringschemereferences-element`
	Container element to record all Scoring - or Grading Scheme entities that can be linked or refered to from other places in the xml document.

``semanticFrameworkReferences``: :ref:`semanticframeworkreferences-element`
	Container element to record semantic frameworks to which resources in this xml document can be associated, tagged or aligned with


