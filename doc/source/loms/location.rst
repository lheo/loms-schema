.. _location-type:

Location
========

An identifiable geographic place. A physical location.

.. code-block:: xml

  <!-- SEQUENCE -->
  <identifier>...Identifier...</identifier> <!-- 0,n -->
  <name>...LanguageString...</name> <!-- 0,n -->
  <description>...Note...</description> <!-- 0,n -->
  <hasAddress>...Address...</hasAddress> <!-- 0,n -->
  <spatialCode>...LocationCode...</spatialCode> <!-- 0,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``identifier``
      - :ref:`identifier-type`
      - 
    * - ``name``
      - :ref:`languagestring-type`
      - A proper noun applied to a spatial object. The place name. A simple (string) label or name for a location. Only one value per language allowed.
    * - ``description``
      - :ref:`note-type`
      - A free text describing the location. Only one value per language allowed.
    * - ``hasAddress``
      - :ref:`address-type`
      - An address associated with the location.
    * - ``spatialCode``
      - :ref:`locationcode-type`
      - A code (i.e. location or region) identifying a spatial scope in which this physical location is located

