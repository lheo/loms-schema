.. _limitoccupation-element:

limitOccupation element
=======================

A link to an ESCO Occupcation or Occupational Category.

.. code-block:: xml

  <limitOccupation>
  </limitOccupation>

Restricts: :ref:`code-type`

Attributes
-----------

``uri``: ``prohibited`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
	

``targetID``: ``optional`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	The URI identifier of the related ESCO occupation.

``type``: ``prohibited`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``description``: ``optional`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	A string describing the semantics of the relation.

``targetNotation``: ``prohibited`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	

``targetFrameworkID``: ``prohibited`` :ref:`id-type`
	

``targetFrameworkUrl``: ``prohibited`` :ref:`documenturl-type`
	

``targetFrameworkSpatialID``: ``prohibited`` :ref:`locationcodecontent-type`
	


