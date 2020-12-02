.. _status-element:

status element
==============

The status of the entitlement. A concept indicating the status of the entitlement. Whether the entitlement is prospective, i.e. awarding the right to apply for the entitlement; or actual, i.e. granting the entitlement

.. code-block:: xml

  <status uri="...">
  </status>

Restricts: :ref:`uribasedcode-type`

Attributes
-----------

``uri``: ``required`` :ref:`entitlementstatusenum-type`
	The URI identifier of a known code that indicates/specifies the status of the entitlement.


