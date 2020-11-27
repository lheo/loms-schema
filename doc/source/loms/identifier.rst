.. _identifier-type:

Identifier
==========

Identifiers are needed to identify and link resources in a unique and persistent way. A resource identifier must be unique and persistent, meaning the identifier will always refer to the same resource and cannot be reused to identify other resources. A resource identifier consists of:

- a string identifier, unique and persistent within the scope of the issuing system.
- a unique identifier of the publishing system that issued the string identifier for that particular resource.

The combination of both, the string identifier and the unique identifier of the issuing system, makes the resource identifier globally unique. The *Identifier* type is used to describe a full (alternative) identifier of an entity or resource.

- The text content of an element of the *Identifier* type contains the character string to identify and distinguish uniquely the resource within the scope of the identification scheme
- The ``schemeID`` attribute is used to specify the identifier scheme. The identifier schema (or identifier register) refers to the agent/system that issued the identifier, it specifies where the identifier originates from. It is the namespace in which the identifier is unique and persistent.

The other attributes of the *Identifier* type provide supplementary information such as the identifier of the used code list and the agency that maintains this list


Extends: `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``schemeID``
      - ``optional`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
      - Identification of the identifier scheme or the identifier register (~ the managing/originating system of the identifier). This can be seen as the namespace in which the assigned identifier is unique.
    * - ``schemeAgencyID``
      - ``optional`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
      - Identification of the agent that manages the identifier scheme. The agent that issued the identifier.
    * - ``schemeAgencyName``
      - ``optional`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
      - The name of the agent that manages the identifier scheme. The agent that issued the identifier.
    * - ``issuedDate``
      - ``optional`` `xs:dateTime <https://www.w3.org/TR/xmlschema11-2/#dateTime>`_
      - The date on which the identifier was issued.
    * - ``type``
      - ``optional`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
      - A code used to classify the type of identifier
    * - ``spatialID``
      - ``optional`` :ref:`locationcodecontent-type`
      - The related country or region code (jurisdiction) of a legal identifier. A legal identifier is a formally issued identifier by a given authorithy within a given jurisdiction. The identifier has a spatial context.

