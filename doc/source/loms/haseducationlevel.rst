.. _haseducationlevel-type:

HasEducationLevel
=================

An level of education within a semantic framework describing education levels.

Restricts: :ref:`code-type`

.. code-block:: xml

  <!-- SEQUENCE -->
  <targetName>...</targetName> <!-- 0,n -->
  <targetDescription>...</targetDescription> <!-- 0,n -->
  <targetFrameworkName>...</targetFrameworkName> <!-- 0,n -->

Elements
--------

``targetName``: :ref:`languagestring-type`
	A name or label of the associated education level in the targeted framework.

``targetDescription``: :ref:`note-type`
	A description of the associated education level in the targeted framework.

``targetFrameworkName``: :ref:`languagestring-type`
	The name of the framework or system used to education levels.


Attributes
-----------

``uri``: ``prohibited`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
	

``targetID``: ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``type``: ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``description``: ``prohibited`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	

``targetNotation``: ``optional`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	A notation or code of the associated edcuation level in the targeted framework.

``targetFrameworkID``: ``optional`` :ref:`id-type`
	The ID of the framework or system used to education levels.

``targetFrameworkUrl``: ``optional`` :ref:`documenturl-type`
	The URL of the framework or system used to education levels.

``targetFrameworkSpatialID``: ``optional`` :ref:`locationcodecontent-type`
	The spatial coverage (country or region) of the framework or system used to describe education levels.


