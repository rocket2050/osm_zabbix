Table of Contents

- [Requirements](#requirements)
  * [Operating systems](#operating-systems)
  * [Zabbix Versions](#zabbix-versions)
    + [Zabbix 3.4](#zabbix-34)
    + [Zabbix 3.2](#zabbix-32)
    + [Zabbix 3.0](#zabbix-30)
- [Dependencies](#dependencies)
- [Example Playbook](#example-playbook)

# Upgrades

## 1.0

With this 1.1 release, the following is changed:

* Ansible install different version of zabbix-Server and Zabbix-agent.
 

# Requirements
Python must be installed on the node machine.

## Operating systems

This role will work on the following operating systems:

 * Centos
 * Ubuntu

So, you'll need one of those operating systems.. :-)
Please sent Pull Requests or suggestions when you want to use this role for other Operating systems.

## Zabbix Versions

See the following list of supported Operating systems with the Zabbix releases.

### Zabbix 3.4

  * CentOS 7.2
  * Centos 6.8
  * Centos 7.0
  * Ubuntu 14.04


### Zabbix 3.2

  * CentOS 7.2
  * Centos 7.0
  * Ubuntu 14.04
  * Ubuntu 16.04

### Zabbix 3.0

  * CentOS 7.2
  * Centos 7.0
  * Ubuntu 14.04
  * Ubuntu 16.04

# Example Playbook
Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
```
   - hosts: zabbix
     roles:
        - osm_zabbix
```
## Role Variables

Available variables are listed below, along with default values:

    # The defaults provided by this role are specific to each distribution
       mysql_root_password: "root@123"
       zabbix_db_password: "password"
       zabbix_server_ip: "192.168.33.52"
       zabbix_db_name: "zabbixdb"
       zabbix_db_user_name: "zabbix"

Set these defaults according to your infrastructure.


# How to run the Playbook
ansible-playbook -i hosts(your host file) site.yml --extra-vars version=3.0/3.2/3.4


