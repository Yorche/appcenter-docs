.. Copyright 2016 FUJITSU LIMITED

.. _userTargetPlatformFormat-getAll:

userTargetPlatformFormat_getAll
-------------------------------

.. function:: GET /users/{uid}/targetplatforms/{tpid}/targetformats

.. sidebar:: Summary

	* Method: ``GET``
	* Response Code: ``200 / 304``
	* Response Formats: ``application/xml`` ``application/json``
	* Since: ``UForge 3.6``

Retrieves all the target formats in a target platform that the user has access to. 

A list of :ref:`targetformat-object` objects are returned. 

You can use a ``search criteria`` to retrieve a subset of these target platforms.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``appliance_create``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the user name (login name) of the :ref:`user-object`
* ``tpid`` (required): the id of the :ref:`targetplatform-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "https://uforge.example.com/api/users/{uid}/targetplatforms/{tpid}/targetformats" -X GET \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`targetformat-api-resources`
	 * :ref:`targetplatform-api-resources`
	 * :ref:`imageformat-object`
	 * :ref:`targetformat-object`
	 * :ref:`targetplatform-object`
	 * :ref:`userFormats-getAll`
	 * :ref:`userFormats-update`
	 * :ref:`userTargetFormat-getAll`
	 * :ref:`userTargetFormat-update`
	 * :ref:`userTargetPlatforms-getAll`
	 * :ref:`userTargetPlatforms-update`
