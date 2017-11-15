Table of Contents

- [Requirements](#requirements)
  * [Operating systems](#operating-systems)
  * [Zabbix Versions](#zabbix-versions)
    + [Zabbix 3.4](#zabbix-34)
    + [Zabbix 3.2](#zabbix-32)
    + [Zabbix 3.0](#zabbix-30)
    + [Zabbix 2.4](#zabbix-24)
    + [Zabbix 2.2](#zabbix-22)
  * [Main variables](#main-variables)
    + [Overall Zabbix](#overall-zabbix)
    + [Zabbix Server](#zabbix-server)
  * [Database](#database)
- [Dependencies](#dependencies)
- [Example Playbook](#example-playbook)
- [Molecule](#molecule)
- [Contributors](#contributors)
- [License](#license)
- [Author Information](#author-information)

# Upgrades

## 1.0.0

With this 1.0.0 release, the following is changed:

* This repository will only contain all the actions that are needed for correct configuring a Zabbix Server. All tasks regarding the frontend/webui of Zabbix has been transferred to the `dj-wasabi.zabbix-web` role.
* All properties starts with `zabbix_` now. Example, property named `server_dbuser` is now `zabbix_server_dbuser`.

# Requirements

## Operating systems

This role will work on the following operating systems:

 * Red Hat
 * Debian
 * Ubuntu

So, you'll need one of those operating systems.. :-)
Please sent Pull Requests or suggestions when you want to use this role for other Operating systems.


