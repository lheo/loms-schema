.. _entitlementspecification-type:

EntitlementSpecification type
=============================

The specification of a right a person has access to, typically as a result of a learning achievement. A specification may take the form of the right to be a member of an organisation, to follow a certain learning opportunity specification, or to follow a certain career. An entitlment may be prospective, i.e. awarding the right to apply for the entitlement, or actual, i.e. granting the entitlement

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
    <type>...</type> <!-- 1,1 -->
    <status>...</status> <!-- 1,1 -->
    <limitOrganization>...</limitOrganization> <!-- 0,n -->
    <limitJurisdiction>...</limitJurisdiction> <!-- 0,n -->
    <limitOccupation>...</limitOccupation> <!-- 0,n -->
    <limitNationalOccupation>...</limitNationalOccupation> <!-- 0,n -->
    <mayResultFrom>...</mayResultFrom> <!-- 0,n -->
    <hasPart>...</hasPart> <!-- 0,n -->
    <specializationOf>...</specializationOf> <!-- 0,n -->
  </...>


Attributes
-----------

``id``: ``required`` :ref:`id-type`
	A portable identifier of the entitlement specification. (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this entitlement specification from other places within the document.


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

``type``: :ref:`entitlementtype-type`
	The type of entitlement. A concept indicating the type of entitlement.

``status``: :ref:`status-element`
	The status of the entitlement. A concept indicating the status of the entitlement. Whether the entitlement is prospective, i.e. awarding the right to apply for the entitlement; or actual, i.e. granting the entitlement

``limitOrganization``: :ref:`idreference-type`
	It MUST refer to an existing 'organization'-record in the 'agentReferences'-section.

``limitJurisdiction``: :ref:`limitjurisdiction-element`
	The jurisdiction for which the entitlement is valid.

``limitOccupation``: :ref:`limitoccupation-element`
	A link to an ESCO Occupcation or Occupational Category.

``limitNationalOccupation``: :ref:`limitnationaloccupation-element`
	A link to a National Occupation.

``mayResultFrom``: :ref:`idreference-type`
	A LearningSpecification that may give rise to an entitlement with this specification. It MUST refer to an existing record in the 'learningSpecificationReferences'-section of this document.

``hasPart``: :ref:`idreference-type`
	A sub specification. An entitlement specification can be part of another "broader" entitlement specification. It MUST refer to an existing record in the 'entitlementSpecificationReferences'-section of this document.

``specializationOf``: :ref:`idreference-type`
	An entitlement specification can be a specialization of another entitlement specification. It MUST refer to an existing record in the 'entitlementSpecificationReferences'-section of this document.


