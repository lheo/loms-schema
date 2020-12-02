.. _mediaobject-type:

MediaObject type
================

A media object, such as a pdf, image, video, or audio object embedded in another resource or published on the web.

.. code-block:: xml

  <...>
    <!-- SEQUENCE -->
    <contentType>...</contentType> <!-- 1,1 -->
    <contentEncoding>...</contentEncoding> <!-- 1,1 -->
    <contentSize>...</contentSize> <!-- 0,1 -->
    <contentUrl>...</contentUrl> <!-- 0,1 -->
    <content>...</content> <!-- 1,1 -->
  </...>


Attributes
-----------

``id``: ``optional`` :ref:`id-type`
	A portable identifier of the media object. It is this identifier that MUST be used to link or refer to this media object from other places within the credential document.


Elements
--------

``contentType``: :ref:`mediatype-type`
	The media-type, the format, of the media resource (e.g. application/pdf, image/png, image/jpeg, image/gif).

``contentEncoding``: :ref:`contentencoding-type`
	The encoding used to encode the binary data contents of the media resource. MUST be Base64.

``contentSize``: `xs:integer <https://www.w3.org/TR/xmlschema11-2/#integer>`_
	The Content-Length indicates the size of the content, in bytes

``contentUrl``: `xs:anyURI <https://www.w3.org/TR/xmlschema11-2/#anyURI>`_
	

``content``: `xs:base64Binary <https://www.w3.org/TR/xmlschema11-2/#base64Binary>`_
	The binary data encoded using Base64. The actual (encoded) binary data in the media type specified by the mediatype property. The actual bytes of the media resource (e.g the image file).


