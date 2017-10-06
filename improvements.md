# Improvements 

Improvements can be done in [osm_zabbix](https://github.com/opstree-ansible/osm_zabbix) role

* Use Handlers when applying configuration changes instead of restarting service using service module.

* Write proper messages for task.

* There must be proper checks in tasks so that then can be run over and over in a same or different machine.

* Mysql playbook must be independent and generic and have all mysql task in it.

* Use command/shell module only when required.

* If become privilege is used at main site.yml then there is no need to include become at task level.  


