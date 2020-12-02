.. _haslocation-element:

hasLocation element
===================

The legally registered site of the organisation. The country or region and eventually the address.

.. code-block:: xml

  <hasLocation>
  </hasLocation>

Restricts: :ref:`location-type`

.. code-block:: xml


    <!-- SEQUENCE -->
    <identifier>...</identifier> <!-- 0,n -->
    <name>...</name> <!-- 0,n -->
    <description>...</description> <!-- 0,n -->
    <hasAddress>...</hasAddress> <!-- 0,n -->
    <spatialCode>...</spatialCode> <!-- 1,n -->

Elements
--------

``identifier``: :ref:`identifier-type`
	

``name``: :ref:`languagestring-type`
	A proper noun applied to a spatial object. The place name. A simple (string) label or name for a location. Only one value per language allowed.

``description``: :ref:`note-type`
	A free text describing the location. Only one value per language allowed.

``hasAddress``: :ref:`address-type`
	An address associated with the location.

``spatialCode``: :ref:`locationcode-type`
	A code (i.e. location or region) identifying a spatial scope in which this physical location is located


