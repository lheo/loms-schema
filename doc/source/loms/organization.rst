.. _organization-type:

Organization type
=================

A legal organization (e.g. the credential issuer, an awarding body, an academic or training institution,...).

.. code-block:: xml

  <... id="...">
    <!-- SEQUENCE -->
    <registration>...</registration> <!-- 0,1 -->
    <vatIdentifier>...</vatIdentifier> <!-- 0,n -->
    <taxIdentifier>...</taxIdentifier> <!-- 0,n -->
    <identifier>...</identifier> <!-- 0,n -->
    <type>...</type> <!-- 0,n -->
    <prefLabel>...</prefLabel> <!-- 1,n -->
    <altLabel>...</altLabel> <!-- 0,n -->
    <homepage>...</homepage> <!-- 0,n -->
    <additionalNote>...</additionalNote> <!-- 0,n -->
    <hasLocation>...</hasLocation> <!-- 1,n -->
    <contactPoint>...</contactPoint> <!-- 0,n -->
    <hasUnit>...</hasUnit> <!-- 0,n -->
    <unitOf>...</unitOf> <!-- 0,1 -->
    <logo>...</logo> <!-- 0,1 -->
    <lastModificationDate>...</lastModificationDate> <!-- 0,1 -->
  </...>


Attributes
-----------

``id``: ``required`` :ref:`id-type`
	A portable identifier of the organization (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this organization from other places within the credential document.


Elements
--------

``registration``: :ref:`legalidentifier-type`
	The legal identifier of an organization. The identifier given to a registered organization by the authority with which it is registered. The legal status of a registered organization is conferred on it by an authority within a given jurisdiction. The Legal Identifier is therefore a fundamental relationship between an organization and the authority with which it is registered.

``vatIdentifier``: :ref:`legalidentifier-type`
	The Value-added Tax ID.

``taxIdentifier``: :ref:`legalidentifier-type`
	The Tax/Fiscal ID of the organization.

``identifier``: :ref:`identifier-type`
	

``type``: :ref:`escoorganizationtype-type`
	The type of agent (i.e. the ESCO organization category).

``prefLabel``: :ref:`languagestring-type`
	The primary name of the organization (e.g. legally recognized name). The name by which to refer to an organisation. In case of a registered organisation this is the legal name of the organization. Maximum one value per language is allowed.

``altLabel``: :ref:`languagestring-type`
	An alternative name of the organization. An organization may have any number of alternative or informal names.

``homepage``: :ref:`document-type`
	A homepage about the organization.

``additionalNote``: :ref:`note-type`
	An additional free text note containing any further information about a organization.

``hasLocation``: :ref:`haslocation-element`
	The legally registered site of the organisation. The country or region and eventually the address.

``contactPoint``: :ref:`contactpoint-element`
	The contact information of the organization. This property links to any "channel" through which the organization can be contacted. It is a means of contacting the organization. It gives the details of how to contact the organization and is repeatable for each type of contact method.

``hasUnit``: :ref:`idreference-type`
	Indicates a unit which is part of this Organization, e.g. a Department within a larger Organization. It MUST refer to an existing 'organization'-record in the 'agentReferences'-section within the xml document.

``unitOf``: :ref:`idreference-type`
	Indicates an Organization of which this Unit is a part, e.g. a Department within a larger Organization. It MUST refer to an existing 'organization'-record in the 'agentReferences'-section within the xml document.

``logo``: :ref:`logo-element`
	The logo of the organization.

``lastModificationDate``: `xs:dateTime <https://www.w3.org/TR/xmlschema11-2/#dateTime>`_
	The date when the organization was last updated since it was published


