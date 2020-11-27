.. _document-type:

Document
========

A public accessible web document.

.. code-block:: xml

  <!-- SEQUENCE -->
  <title>...</title> <!-- 0,n -->
  <language>...</language> <!-- 0,n -->
  <subject>...</subject> <!-- 0,n -->

Elements
--------

``title``: :ref:`languagestring-type`
	Maximum one value per language is allowed.

``language``: :ref:`languagecode-type`
	The language of the document.

``subject``: :ref:`subjecttypecode-type`
	A subject or topic that is described in the document.


Attributes
-----------

``uri``: ``required`` :ref:`documenturl-type`
	The URL of the web document. The URL to access or download the web document.


