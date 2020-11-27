.. _address-type:

Address
=======

An adress. Properties specifying an entity’s physical location.

.. code-block:: xml

  <!-- SEQUENCE -->
  <identifier>...</identifier> <!-- 0,n -->
  <fullAddress>...</fullAddress> <!-- 0,n -->
  <country>...</country> <!-- 0,1 -->

Elements
--------

``identifier``: :ref:`identifier-type`
	An adress identifier.

``fullAddress``: :ref:`note-type`
	The complete address with or without formatting. Use of this property is recommended as it will not suffer any misunderstandings that might arise through the breaking up of an address into its component parts. Maximum one value per language is allowed.

``country``: :ref:`countrycode-type`
	The address country Code. The uppermost administrative unit for the address.


