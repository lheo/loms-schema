.. _qualificationcode-type:

QualificationCode
=================

An identifying code from a qualification based reference semantic asset. This property is used to classify the qualification information with a qualification from a known qualification framework. (e.g. the link to the accredidated NQF qualification)

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
      - ``optional`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - The URI identifier of the associated qualification in the targeted framework.
    * - ``type``
      - ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - 
    * - ``description``
      - ``prohibited`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
      - 
    * - ``targetNotation``
      - ``optional`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
      - A notation or code of the associated qualification in the targeted framework.
    * - ``targetFrameworkID``
      - ``optional`` :ref:`id-type`
      - The ID of the framework or system used to describe qualifications.
    * - ``targetFrameworkUrl``
      - ``optional`` :ref:`documenturl-type`
      - The URL of the framework or system used to describe qualifications.
    * - ``targetFrameworkSpatialID``
      - ``optional`` :ref:`locationcodecontent-type`
      - The spatial coverage (country or region) of the framework or system used to describe qualifications.

