.. _relatedescoskill-element:

relatedEscoSkill element
========================

A link/alignment to an ESCO Skill.

.. code-block:: xml

  <relatedEscoSkill>
  </relatedEscoSkill>

Restricts: :ref:`code-type`

Attributes
-----------

``uri``: ``prohibited`` `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_
	

``targetID``: ``optional`` `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	The URI identifier of the related ESCO skill.

``type``: ``optional`` :ref:`skillalignmenttypeenum-type`
	A code indicating the semantics of the relation.

``description``: ``optional`` `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	A string describing the semantics of the relation.

``targetNotation``: ``prohibited`` `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	

``targetFrameworkID``: ``prohibited`` :ref:`id-type`
	

``targetFrameworkUrl``: ``prohibited`` :ref:`documenturl-type`
	

``targetFrameworkSpatialID``: ``prohibited`` :ref:`locationcodecontent-type`
	


