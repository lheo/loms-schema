.. _learningopportunitiesroot-type:

LearningOpportunitiesRoot
=========================

This is root element of the document.

.. code-block:: xml

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

Elements
--------

``learningOpportunities``: :ref:`learningopportunityreferences-type`
	LearningOpportunities that are/will be published

``learningSpecificationReferences``: :ref:`learningspecificationreferences-type`
	Container element to record all LearningSpecification entities that can be linked or refered to from other places in the xml document.

``learningOutcomeReferences``: :ref:`learningoutcomereferences-type`
	Container element to record all LearningOutcome entities that can be linked or refered to from other places in the xml document.

``learningActivitySpecificationReferences``: :ref:`learningactivityspecificationreferences-type`
	Container element to record all LearningActivitySpecification entities that can be linked or refered to from other places in the xml document.

``assessmentSpecificationReferences``: :ref:`assessmentspecificationreferences-type`
	Container element to record all AssessmentSpecification entities that can be linked or refered to from other places in the xml document.

``entitlementSpecificationReferences``: :ref:`entitlementspecificationreferences-type`
	Container element to record all EntitlementSpecification entities that can be linked or refered to from other places in the xml document.

``agentReferences``: :ref:`agentreferences-type`
	Container element to record all Organization entities that can be linked or refered to from other places in the xml document.

``scoringSchemeReferences``: :ref:`scoringschemereferences-type`
	Container element to record all Scoring - or Grading Scheme entities that can be linked or refered to from other places in the xml document.

``semanticFrameworkReferences``: :ref:`frameworkreferences-type`
	Container element to record semantic frameworks to which resources in this xml document can be associated, tagged or aligned with


Attributes
-----------

``xsdVersion``: ``optional`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
	used xsd version


