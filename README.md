correcthorse.kibana
=========

An ansible role for installing kibana 4.

Role Variables
--------------

| Variable			| Default						| Notes				|
| :---				| :---							| :---				|
| kibana_version		| '4.0.0'						|				|
| kibana_arch			| 'linux-x64'						|				|
| kibana_download_base		| 'https://download.elasticsearch.org/kibana/kibana/'	|				|
| kibana_home			| /opt/kibana						|				|
| kibana_base_name		| 'kibana-{{ kibana_version }}-{{ kibana_arch }}'	|				|
| kibana_archive		| '{{ kibana_base_name }}.tar.gz' 	      		|				|
| kibana_download_url		| '{{ kibana_download_base }}{{ kibana_archive}}'	|				|

Dependencies
------------

- correcthorse.common

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: correcthorse.kibana }

License
-------

MIT

Author Information
------------------

* [Joshua Rusch](https://correct.horse/)