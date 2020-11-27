.. _uribasedcode-type:

URIBasedCode
============

A code (i.e a code from a controlled vocabulary) that can be fully identified by a URI

Restricts: :ref:`code-type`

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``uri``
      - ``required`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
      - A URI identifier of the code
    * - ``targetID``
      - ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - 
    * - ``type``
      - ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - 
    * - ``description``
      - ``prohibited`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
      - 
    * - ``targetNotation``
      - ``prohibited`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
      - 
    * - ``targetFrameworkID``
      - ``prohibited`` :ref:`id-type`
      - 
    * - ``targetFrameworkName``
      - ``prohibited`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
      - 
    * - ``targetFrameworkUrl``
      - ``prohibited`` :ref:`documenturl-type`
      - 
    * - ``targetFrameworkSpatialID``
      - ``prohibited`` :ref:`locationcodecontent-type`
      - 

