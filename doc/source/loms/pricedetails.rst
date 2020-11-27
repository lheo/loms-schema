.. _pricedetails-type:

PriceDetails
============

The details about a price or price category.

.. code-block:: xml

  <!-- SEQUENCE -->
  <amount>...</amount> <!-- 0,1 -->
  <name>...</name> <!-- 0,n -->
  <description>...</description> <!-- 0,n -->
  <additionalNote>...</additionalNote> <!-- 0,n -->

Elements
--------

``amount``: :ref:`amount-type`
	The amount.

``name``: :ref:`languagestring-type`
	A proper noun applied to a price. The price name. A simple (string) label or name for a price category.

``description``: :ref:`note-type`
	A free tex describing the price. Maximum one value per language is allowed.

``additionalNote``: :ref:`note-type`
	An additional free text note containing any further information about the price (e.g. conditions, reductions, ….).


