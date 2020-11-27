.. _document-type:

Document
========

A public accessible web document.

.. code-block:: xml

  <!-- SEQUENCE -->
  <title>...LanguageString...</title> <!-- 0,n -->
  <language>...LanguageCode...</language> <!-- 0,n -->
  <subject>...SubjectTypeCode...</subject> <!-- 0,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``title``
      - :ref:`languagestring-type`
      - Maximum one value per language is allowed.
    * - ``language``
      - :ref:`languagecode-type`
      - The language of the document.
    * - ``subject``
      - :ref:`subjecttypecode-type`
      - A subject or topic that is described in the document.


.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Attribute
      - Type
      - Description
    * - ``uri``
      - ``required`` :ref:`documenturl-type`
      - The URL of the web document. The URL to access or download the web document.

