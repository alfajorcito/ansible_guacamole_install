# ansible_guacamole_install
Ansible role installing Apache Guacamole on Ubuntu. 

### Tested on
* Ubuntu 20.04
* Ubuntu 22.04

### Tested with
* Ansible 2.10
  * community.mysql 1.2.0
* MySQL 8.0.30

### Requirements
* Local MySQL (optional, required if using DB authentication)

### Features
* Deploy with Tomcat 
* Install xrdp, LXQt
* Authentication
  * default
  * MySQL
  * TOTP (requires MySQL, WIP)
* ~~Manage groups and users: TODO~~ (will not implement, check out [this repo](https://github.com/scicore-unibas-ch/ansible-modules-guacamole) instead!)
* ~~Manage connections: TODO~~ (same as above)

### Vars
TODO
