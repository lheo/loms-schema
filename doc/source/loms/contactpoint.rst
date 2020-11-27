.. _contactpoint-type:

ContactPoint
============



.. code-block:: xml

  <!-- SEQUENCE -->
  <note>...Note...</note> <!-- 0,n -->
  <description>...Note...</description> <!-- 0,n -->
  <address>...Address...</address> <!-- 0,n -->
  <phone>...Phone...</phone> <!-- 0,n -->
  <mailBox>...MBox...</mailBox> <!-- 0,n -->
  <webresource>...InteractiveWebResource...</webresource> <!-- 0,n -->
  <wallet>...MBox...</wallet> <!-- 0,n -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``note``
      - :ref:`note-type`
      - A note about the contactpoint. E.g. a note about the usage and availibility about this contactpoint.
    * - ``description``
      - :ref:`note-type`
      - A free text describing the contact details.
    * - ``address``
      - :ref:`address-type`
      - A postal address used for contacting the agent.
    * - ``phone``
      - :ref:`phone-type`
      - A phone number used for contacting the agent.
    * - ``mailBox``
      - :ref:`mbox-type`
      - An email address used for contacting the agent.
    * - ``webresource``
      - :ref:`interactivewebresource-type`
      - A contact form used for contacting the agent.
    * - ``wallet``
      - :ref:`mbox-type`
      - The address of an electronic wallet where credentials may be deposited.

