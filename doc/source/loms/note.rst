.. _note-type:

Note
====

A formatted and annotated text fragment.

.. code-block:: xml

  <!-- SEQUENCE -->
  <text>...Text...</text> <!-- 1,1 -->
  <subject>...SubjectTypeCode...</subject> <!-- 0,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``text``
      - :ref:`text-type`
      - A formatted character string (i.e. a finite set of characters) generally in the form of words of a language.
    * - ``subject``
      - :ref:`subjecttypecode-type`
      - A subject or topic that is described in the text.

