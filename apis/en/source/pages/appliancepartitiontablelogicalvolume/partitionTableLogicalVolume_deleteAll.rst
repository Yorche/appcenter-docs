.. Copyright 2016 FUJITSU LIMITED

.. _partitionTableLogicalVolume-deleteAll:

partitionTableLogicalVolume_deleteAll
-------------------------------------

.. function:: DELETE users/{uid}/appliances/{aid}/installProfile/{ipid}/pt/{ptid}/volumes

.. sidebar:: Summary

	* Method: ``DELETE``
	* Response Code: ``204 / 200``
	* Response Formats: 
	* Since: ``UForge 2.1``

Removes all the logical volumes from a partitioning table.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``appliance_create``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the user name (login name) of the :ref:`user-object` that has created the appliance
* ``ptid`` (required): the id of the :ref:`partitiontable-object`
* ``aid`` (required): the id of the :ref:`appliance-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "https://uforge.example.com/apiusers/{uid}/appliances/{aid}/installProfile/{ipid}/pt/{ptid}/volumes" -X DELETE \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`appliancepartitiontabledisk-api-resources`
	 * :ref:`appliancepartitiontablediskpartition-api-resources`
	 * :ref:`appliancepartitiontablelogicalgroup-api-resources`
	 * :ref:`partitiontable-object`
	 * :ref:`appliance-object`
	 * :ref:`logicalvolume-object`
	 * :ref:`partitionTableLogicalVolume-create`
	 * :ref:`partitionTableLogicalVolume-getAll`
	 * :ref:`partitionTableLogicalVolume-delete`
	 * :ref:`partitionTableLogicalVolume-get`
	 * :ref:`partitionTableLogicalVolume-update`
