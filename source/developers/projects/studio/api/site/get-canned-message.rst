.. _crafter-studio-api-site-get-canned-message:

==================
Get Canned Message
==================

Get rejection reason.

--------------------
Resource Information
--------------------

+----------------------------+-------------------------------------------------------------------+
|| HTTP Verb                 || GET                                                              |
+----------------------------+-------------------------------------------------------------------+
|| URL                       || ``/api/1/services/api/1/site/get-canned-message.json``           |
+----------------------------+-------------------------------------------------------------------+
|| Response Formats          || ``JSON``                                                         |
+----------------------------+-------------------------------------------------------------------+
|| Required Role             || N/A                                                              |
+----------------------------+-------------------------------------------------------------------+

----------
Parameters
----------

+---------------+-------------+---------------+--------------------------------------------------+
|| Name         || Type       || Required     || Description                                     |
+===============+=============+===============+==================================================+
|| site_id      || String     || |checkmark|  || Site to use                                     |
+---------------+-------------+---------------+--------------------------------------------------+
|| locale       || String     || |checkmark|  || Locale of message                               |
+---------------+-------------+---------------+--------------------------------------------------+
|| type         || String     || |checkmark|  || Message type                                    |
+---------------+-------------+---------------+--------------------------------------------------+

-------
Example
-------

^^^^^^^
Request
^^^^^^^

.. code-block:: guess

    GET .../api/1/services/api/1/site/get-canned-message.json?site_id=mysite&locale=en&type=NotApproved

^^^^^^^^
Response
^^^^^^^^

``Status 200 OK``

.. code-block:: json

    "Please make the following revisions and resubmit."


---------
Responses
---------

+---------+-------------------------------------------+---------------------------------------------------+
|| Status || Location                                 || Response Body                                    |
+=========+===========================================+===================================================+
|| 200    ||                                          || See example above.                               |
+---------+-------------------------------------------+---------------------------------------------------+
