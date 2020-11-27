.. _imageobject-type:

ImageObject
===========

A static visual representation. An image file as a media object embedded in another resource or published on the web.

Restricts: :ref:`mediaobject-type`

.. code-block:: xml

  <!-- SEQUENCE -->
  <contentType>...</contentType> <!-- 1,1 -->
  <contentEncoding>...</contentEncoding> <!-- 1,1 -->
  <contentSize>...</contentSize> <!-- 0,1 -->
  <contentUrl>...</contentUrl> <!-- 0,1 -->
  <content>...</content> <!-- 1,1 -->

Elements
--------

``contentType``: :ref:`imagemediatype-type`
	The media-type, the format, of the image resource (image/png, image/jpeg, image/gif).

``contentEncoding``: :ref:`contentencoding-type`
	The encoding used to encode the binary data contents of the image type resource. MUST be Base64.

``contentSize``: `xs:integer <https://www.w3.org/TR/xmlschema11-2/#integer>`_
	The Content-Length indicates the size of the content, in bytes

``contentUrl``: `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``content``: `xs:base64Binary <https://www.w3.org/TR/xmlschema11-2/#base64Binary>`_
	The binary data encoded using Base64.


