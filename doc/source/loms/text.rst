.. _text-type:

Text
====

A formatted character string (i.e. a finite set of characters) in the form of words of a language.

Extends: `xs:string <https://www.w3.org/TR/xmlschema11-2/#string>`_

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``lang``
      - ``required`` :ref:`languagecharcodeenum-type`
      - The language used in the text
    * - ``content-type``
      - ``required`` :ref:`textcontenttypecodeenum-type`
      - The text format specified by the corresponding mimetype (text/plain, text/html)

