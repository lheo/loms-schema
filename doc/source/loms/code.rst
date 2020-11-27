.. _code-type:

Code
====

A term from a controlled vocabulary. A code is a character string of letters, numbers, special characters (except escape sequences), and symbols. It represents a definitive value, a method, or a property description in an abbreviated or language-independent form that is part of a finite list of allowed values. The CodeType is used for all elements that are used to enable a common coded value representation. Typical example of code types are: Country Code and Language Code. The CodeType should be used in case of a finite list of allowed values. The IdentifierType should be used in case of an infinite set of objects. This CodeType is a generic data type which is also used to represent association objects.

.. code-block:: xml

  <!-- SEQUENCE -->
  <targetName>...LanguageString...</targetName> <!-- 0,n -->
  <targetDescription>...Note...</targetDescription> <!-- 0,n -->
  <targetFrameworkName>...LanguageString...</targetFrameworkName> <!-- 0,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``targetName``
      - :ref:`languagestring-type`
      - A name or label of the associated object in the targeted framework.
    * - ``targetDescription``
      - :ref:`note-type`
      - A description of the associated object in the targeted framework.
    * - ``targetFrameworkName``
      - :ref:`languagestring-type`
      - The name of the framework or system used to describe the associated object.


.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``uri``
      - ``optional`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
      - A URI identifier of the code. For URI identifier of an associated object, USE targetID attribute instead of this.
    * - ``targetID``
      - ``optional`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - The URI identifier of the associated object in the targeted framework. For URI identifier of the code, USE uri attribute instead of this.
    * - ``type``
      - ``optional`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - A code indicating the semantics of the relation.
    * - ``description``
      - ``optional`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
      - A string describing the semantics of the relation.
    * - ``targetNotation``
      - ``optional`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
      - A notation or code of the associated object in the targeted framework.
    * - ``targetFrameworkID``
      - ``optional`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
      - The ID of the framework or system used to describe the assoicated object.
    * - ``targetFrameworkUrl``
      - ``optional`` :ref:`documenturl-type`
      - The URL of the framework or system used to describe the assoicated object..
    * - ``targetFrameworkSpatialID``
      - ``optional`` :ref:`locationcodecontent-type`
      - The spatial coverage (country or region) of the framework or system used to describe the assoicated object..

