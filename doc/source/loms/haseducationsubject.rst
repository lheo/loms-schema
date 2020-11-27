.. _haseducationsubject-type:

HasEducationSubject
===================

An associated field of education from another semantic framework than the ISCED classification.

Restricts: :ref:`code-type`

.. code-block:: xml

  <!-- SEQUENCE -->
  <targetName>...</targetName> <!-- 0,n -->
  <targetDescription>...</targetDescription> <!-- 0,n -->
  <targetFrameworkName>...</targetFrameworkName> <!-- 0,n -->

Elements
--------

``targetName``: :ref:`languagestring-type`
	A name or label of the associated field of education in the targeted framework.

``targetDescription``: :ref:`note-type`
	A description of the associated field of education in the targeted framework.

``targetFrameworkName``: :ref:`languagestring-type`
	he name of the framework or system used to describe fields of education.


Attributes
-----------

``uri``: ``prohibited`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
	

``targetID``: ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``type``: ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``description``: ``prohibited`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	

``targetNotation``: ``optional`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	A notation or code of the associated field of education in the targeted framework.

``targetFrameworkID``: ``optional`` :ref:`id-type`
	The ID of the framework or system used to describe fields of education.

``targetFrameworkUrl``: ``optional`` :ref:`documenturl-type`
	The URL of the framework or system used to describe fields of education.

``targetFrameworkSpatialID``: ``optional`` :ref:`locationcodecontent-type`
	The spatial coverage (country or region) of the framework or system used to describe fields of education.


