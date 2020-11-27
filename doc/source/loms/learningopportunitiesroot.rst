.. _learningopportunitiesroot-type:

LearningOpportunitiesRoot
=========================

This is root element of the document.

.. code-block:: xml

  <!-- SEQUENCE -->
  <learningOpportunities>...LearningOpportunityReferences...</learningOpportunities> <!-- 1,1 -->
  <learningSpecificationReferences>...LearningSpecificationReferences...</learningSpecificationReferences> <!-- 0,1 -->
  <learningOutcomeReferences>...LearningOutcomeReferences...</learningOutcomeReferences> <!-- 0,1 -->
  <learningActivitySpecificationReferences>...LearningActivitySpecificationReferences...</learningActivitySpecificationReferences> <!-- 0,1 -->
  <assessmentSpecificationReferences>...AssessmentSpecificationReferences...</assessmentSpecificationReferences> <!-- 0,1 -->
  <entitlementSpecificationReferences>...EntitlementSpecificationReferences...</entitlementSpecificationReferences> <!-- 0,1 -->
  <agentReferences>...AgentReferences...</agentReferences> <!-- 0,1 -->
  <scoringSchemeReferences>...ScoringSchemeReferences...</scoringSchemeReferences> <!-- 0,1 -->
  <semanticFrameworkReferences>...FrameworkReferences...</semanticFrameworkReferences> <!-- 0,1 -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``learningOpportunities``
      - :ref:`learningopportunityreferences-type`
      - LearningOpportunities that are/will be published
    * - ``learningSpecificationReferences``
      - :ref:`learningspecificationreferences-type`
      - Container element to record all LearningSpecification entities that can be linked or refered to from other places in the xml document.
    * - ``learningOutcomeReferences``
      - :ref:`learningoutcomereferences-type`
      - Container element to record all LearningOutcome entities that can be linked or refered to from other places in the xml document.
    * - ``learningActivitySpecificationReferences``
      - :ref:`learningactivityspecificationreferences-type`
      - Container element to record all LearningActivitySpecification entities that can be linked or refered to from other places in the xml document.
    * - ``assessmentSpecificationReferences``
      - :ref:`assessmentspecificationreferences-type`
      - Container element to record all AssessmentSpecification entities that can be linked or refered to from other places in the xml document.
    * - ``entitlementSpecificationReferences``
      - :ref:`entitlementspecificationreferences-type`
      - Container element to record all EntitlementSpecification entities that can be linked or refered to from other places in the xml document.
    * - ``agentReferences``
      - :ref:`agentreferences-type`
      - Container element to record all Organization entities that can be linked or refered to from other places in the xml document.
    * - ``scoringSchemeReferences``
      - :ref:`scoringschemereferences-type`
      - Container element to record all Scoring - or Grading Scheme entities that can be linked or refered to from other places in the xml document.
    * - ``semanticFrameworkReferences``
      - :ref:`frameworkreferences-type`
      - Container element to record semantic frameworks to which resources in this xml document can be associated, tagged or aligned with


.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``xsdVersion``
      - ``optional`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
      - used xsd version

