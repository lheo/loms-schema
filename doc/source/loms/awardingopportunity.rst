.. _awardingopportunity-type:

AwardingOpportunity
===================



.. code-block:: xml

  <!-- SEQUENCE -->
  <organization>...IdReference...</organization> <!-- 0,n -->
  <location>...LocationCode...</location> <!-- 0,1 -->
  <startedAtTime>...xs:dateTime...</startedAtTime> <!-- 0,1 -->
  <endedAtTime>...xs:dateTime...</endedAtTime> <!-- 0,1 -->

.. list-table::
    :widths: 25 25 50
    :header-rows: 1

    * - Element
      - Type
      - Description
    * - ``organization``
      - :ref:`idreference-type`
      - The awarding body. The organization that awards or issues the Learning Specification (i.e a qualification). It MUST refer to an existing 'organization'-record in the 'agentReferences'-section. Only in cases of co-awarding/co-graduation, where a qualification is issued to an individual by two or more organisations the cardinality is greater than 1
    * - ``location``
      - :ref:`locationcode-type`
      - The location where the awarding activities take/took place (country/region where the qualification is awarded)
    * - ``startedAtTime``
      - `xs:dateTime <https://www.w3.org/TR/xmlschema11-2/#dateTime>`_
      - The date since when the awarding activities take place. If not specified it is undefined (“not known”)
    * - ``endedAtTime``
      - `xs:dateTime <https://www.w3.org/TR/xmlschema11-2/#dateTime>`_
      - The date until when the awarding activities take/took place

