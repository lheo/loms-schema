.. _qualificationcode-element:

qualificationCode element
=========================

An identifying code from a qualification based reference semantic asset. This property is used to classify the qualification information with a qualification from a known qualification framework. (e.g. the link to the accredidated NQF qualification)

.. code-block:: xml

  <qualificationCode>
  </qualificationCode>

Restricts: :ref:`code-type`

.. code-block:: xml


    <!-- SEQUENCE -->
    <targetFrameworkName>...</targetFrameworkName> <!-- 0,n -->

Elements
--------

``targetFrameworkName``: :ref:`languagestring-type`
	The name of the framework or system used to describe qualifications.


Attributes
-----------

``uri``: ``prohibited`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
	

``targetID``: ``optional`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	The URI identifier of the associated qualification in the targeted framework.

``type``: ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``description``: ``prohibited`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	

``targetNotation``: ``optional`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	A notation or code of the associated qualification in the targeted framework.

``targetFrameworkID``: ``optional`` :ref:`id-type`
	The ID of the framework or system used to describe qualifications.

``targetFrameworkUrl``: ``optional`` :ref:`documenturl-type`
	The URL of the framework or system used to describe qualifications.

``targetFrameworkSpatialID``: ``optional`` :ref:`locationcodecontent-type`
	The spatial coverage (country or region) of the framework or system used to describe qualifications.


