.. _limitnationaloccupation-type:

LimitNationalOccupation
=======================

A link to a National Occupation.

Restricts: :ref:`code-type`

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``uri``
      - ``prohibited`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
      - 
    * - ``targetID``
      - ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - 
    * - ``type``
      - ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - 
    * - ``description``
      - ``optional`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
      - A string describing the semantics of the relation.
    * - ``targetNotation``
      - ``optional`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
      - A notation or code of the associated occupation in the targeted framework.
    * - ``targetFrameworkID``
      - ``optional`` :ref:`id-type`
      - The ID of the framework or system used to describe occupations.
    * - ``targetFrameworkUrl``
      - ``optional`` :ref:`documenturl-type`
      - The URL of the framework or system used to describe occupations.
    * - ``targetFrameworkSpatialID``
      - ``optional`` :ref:`locationcodecontent-type`
      - The spatial coverage (country or region) of the framework or system used to describe occupations.

