.. _phone-type:

Phone
=====

A phone number.

.. code-block:: xml

  <!-- SEQUENCE -->
  <phoneNumber>...</phoneNumber> <!-- 0,1 -->
  <countryDialing>...</countryDialing> <!-- 0,1 -->
  <areaDialing>...</areaDialing> <!-- 0,1 -->
  <dialNumber>...</dialNumber> <!-- 0,1 -->

Elements
--------

``phoneNumber``: `xs:normalizedString <https://www.w3.org/TR/xmlschema11-2/#normalizedString>`_
	The full phone number as a string.

``countryDialing``: `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	The country dialling code for a contact number. (e.g. “0032”, “0034”, etc.)

``areaDialing``: `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	The area dialling code for a contact number.(e.g. “2”, “71, “93”, etc.)

``dialNumber``: `xs:token <https://www.w3.org/TR/xmlschema11-2/#token>`_
	The contact number, not including country dialling or area dialling codes. (e.g. “3445654”, “1234567”, etc.)


