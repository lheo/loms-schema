.. _nqflevel-element:

nqfLevel element
================

A qualification can be part of a national qualification framework (NQF Qualification) which can be specified by the NQF level. This the qualification level as specified by a National Qualifications Framework.

.. code-block:: xml

  <nqfLevel>
  </nqfLevel>

Restricts: :ref:`code-type`

Attributes
-----------

``uri``: ``prohibited`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
	

``targetID``: ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``type``: ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``description``: ``prohibited`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	

``targetNotation``: ``optional`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	A notation or code of the qualification framework level within the national framework.

``targetFrameworkID``: ``optional`` :ref:`qualificationframeworkenum-type`
	The ID (URI) of the national qualification framework.

``targetFrameworkUrl``: ``prohibited`` :ref:`documenturl-type`
	

``targetFrameworkSpatialID``: ``prohibited`` :ref:`locationcodecontent-type`
	


