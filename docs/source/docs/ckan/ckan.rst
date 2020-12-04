**********
CKAN
**********

Useful ckan commands
---------------------

Ŝhow implemented schema for datasets
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: bash

    ckanapi action scheming_dataset_schema_list -c /var/www/ckan/development.ini
    ckanapi action scheming_dataset_schema_show type=dataset -c /var/www/ckan/development.ini
    ckanapi action scheming_group_schema_list -c /var/www/ckan/development.ini
    ckanapi action scheming_organization_schema_list -c /var/www/ckan/development.ini
    ckanapi action scheming_group_schema_show type=dataset -c /var/www/ckan/development.ini
    ckanapi action scheming_organization_schema_show type=dataset -c /var/www/ckan/development.ini


Show datasets
^^^^^^^^^^^^^

.. code-block:: bash

    ckanapi action package_show id='fahrplan-2016-gtfs' -c /var/www/ckan/development.ini
    ckanapi action dataset_purge id='fahrplan-2016-gtfs' -c /var/www/ckan/development.ini
    paster --plugin=ckan dataset delete fahrplan-2016-gtfs -c /var/www/ckan/development.ini
    paster --plugin=ckan dataset show fahrplan-2016-gtfs -c /var/www/ckan/development.ini


Useful links
============

- `ckan api documentation <https://docs.ckan.org/en/2.8/api/>`__
