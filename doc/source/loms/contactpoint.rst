.. _contactpoint-element:

contactPoint element
====================

The contact information of the organization. This property links to any "channel" through which the organization can be contacted. It is a means of contacting the organization. It gives the details of how to contact the organization and is repeatable for each type of contact method.

.. code-block:: xml

  <contactPoint>
    <!-- SEQUENCE -->
    <note>...</note> <!-- 0,n -->
    <description>...</description> <!-- 0,n -->
    <address>...</address> <!-- 0,n -->
    <phone>...</phone> <!-- 0,n -->
    <mailBox>...</mailBox> <!-- 0,n -->
    <webresource>...</webresource> <!-- 0,n -->
    <wallet>...</wallet> <!-- 0,n -->
  </contactPoint>

Elements
--------

``note``: :ref:`note-type`
	A note about the contactpoint. E.g. a note about the usage and availibility about this contactpoint.

``description``: :ref:`note-type`
	A free text describing the contact details.

``address``: :ref:`address-type`
	A postal address used for contacting the agent.

``phone``: :ref:`phone-element`
	A phone number used for contacting the agent.

``mailBox``: :ref:`mbox-type`
	An email address used for contacting the agent.

``webresource``: :ref:`webresource-element`
	A contact form used for contacting the agent.

``wallet``: :ref:`mbox-type`
	The address of an electronic wallet where credentials may be deposited.


