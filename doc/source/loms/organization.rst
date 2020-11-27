.. _organization-type:

Organization
============

A legal organization (e.g. the credential issuer, an awarding body, an academic or training institution,...).

.. code-block:: xml

  <!-- SEQUENCE -->
  <registration>...LegalIdentifier...</registration> <!-- 0,1 -->
  <vatIdentifier>...LegalIdentifier...</vatIdentifier> <!-- 0,n -->
  <taxIdentifier>...LegalIdentifier...</taxIdentifier> <!-- 0,n -->
  <identifier>...Identifier...</identifier> <!-- 0,n -->
  <type>...EscoOrganizationType...</type> <!-- 0,n -->
  <prefLabel>...LanguageString...</prefLabel> <!-- 1,n -->
  <altLabel>...LanguageString...</altLabel> <!-- 0,n -->
  <homepage>...Document...</homepage> <!-- 0,n -->
  <additionalNote>...Note...</additionalNote> <!-- 0,n -->
  <hasLocation>...SpatialCodeLocation...</hasLocation> <!-- 1,n -->
  <contactPoint>...ContactPoint...</contactPoint> <!-- 0,n -->
  <hasUnit>...IdReference...</hasUnit> <!-- 0,n -->
  <unitOf>...IdReference...</unitOf> <!-- 0,1 -->
  <logo>...ImageObject...</logo> <!-- 0,1 -->
  <lastModificationDate>...xs:dateTime...</lastModificationDate> <!-- 0,1 -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``registration``
      - :ref:`legalidentifier-type`
      - The legal identifier of an organization. The identifier given to a registered organization by the authority with which it is registered. The legal status of a registered organization is conferred on it by an authority within a given jurisdiction. The Legal Identifier is therefore a fundamental relationship between an organization and the authority with which it is registered.
    * - ``vatIdentifier``
      - :ref:`legalidentifier-type`
      - The Value-added Tax ID.
    * - ``taxIdentifier``
      - :ref:`legalidentifier-type`
      - The Tax/Fiscal ID of the organization.
    * - ``identifier``
      - :ref:`identifier-type`
      - 
    * - ``type``
      - :ref:`escoorganizationtype-type`
      - The type of agent (i.e. the ESCO organization category).
    * - ``prefLabel``
      - :ref:`languagestring-type`
      - The primary name of the organization (e.g. legally recognized name). The name by which to refer to an organisation. In case of a registered organisation this is the legal name of the organization. Maximum one value per language is allowed.
    * - ``altLabel``
      - :ref:`languagestring-type`
      - An alternative name of the organization. An organization may have any number of alternative or informal names.
    * - ``homepage``
      - :ref:`document-type`
      - A homepage about the organization.
    * - ``additionalNote``
      - :ref:`note-type`
      - An additional free text note containing any further information about a organization.
    * - ``hasLocation``
      - :ref:`spatialcodelocation-type`
      - The legally registered site of the organisation. The country or region and eventually the address.
    * - ``contactPoint``
      - :ref:`contactpoint-type`
      - The contact information of the organization. This property links to any "channel" through which the organization can be contacted. It is a means of contacting the organization. It gives the details of how to contact the organization and is repeatable for each type of contact method.
    * - ``hasUnit``
      - :ref:`idreference-type`
      - Indicates a unit which is part of this Organization, e.g. a Department within a larger Organization. It MUST refer to an existing 'organization'-record in the 'agentReferences'-section within the xml document.
    * - ``unitOf``
      - :ref:`idreference-type`
      - Indicates an Organization of which this Unit is a part, e.g. a Department within a larger Organization. It MUST refer to an existing 'organization'-record in the 'agentReferences'-section within the xml document.
    * - ``logo``
      - :ref:`imageobject-type`
      - The logo of the organization.
    * - ``lastModificationDate``
      - `xs:dateTime <https://www.w3.org/TR/xmlschema11-2/#dateTime>`_
      - The date when the organization was last updated since it was published


.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``id``
      - ``required`` :ref:`id-type`
      - A portable identifier of the organization (i.e. a urn in the uuid namespace). It is this identifier that MUST be used to link or refer to this organization from other places within the credential document.
