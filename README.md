Role Name
=========

The Elastic Stack, aka ELK.

Requirements
------------

TODO

Role Variables
--------------

* elastic_elasticsearch_install: true
* elastic_elasticsearch_cluster_name: development
* elastic_elasticsearch_node_name: development
* elastic_kibana_install: true
* elastic_logstash_install: true
* elastic_logstash_syslog_port: 5514
* elastic_logstash_gelf_port: 12201
* elastic_packetbeat_install: true
* elastic_metricbeat_install: true
* elastic_filebeat_install: true
* elastic_x_pack_install: false
* elastic_stack_version: 5.x

Dependencies
------------

* kurron.base

Example Playbook
----------------

```
- hosts: servers
  roles:
      - { role: kurron.elastic-stack, elastic_logstash_syslog_port: 514 }
```

License
-------

This project is licensed under the [Apache License Version 2.0, January 2004](http://www.apache.org/licenses/).

Author Information
------------------

[Author's website](http://jvmguy.com/).
