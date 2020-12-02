.. _document-type:

Document type
=============

A public accessible web document.

.. code-block:: xml

  <... uri="...">
    <!-- SEQUENCE -->
    <title>...</title> <!-- 0,n -->
    <language>...</language> <!-- 0,n -->
    <subject>...</subject> <!-- 0,n -->
  </...>


Attributes
-----------

``uri``: ``required`` :ref:`documenturl-type`
	The URL of the web document. The URL to access or download the web document.


Elements
--------

``title``: :ref:`languagestring-type`
	Maximum one value per language is allowed.

``language``: :ref:`languagecode-type`
	The language of the document.

``subject``: :ref:`subjecttypecode-type`
	A subject or topic that is described in the document.


