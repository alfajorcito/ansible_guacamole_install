# ansible_guacamole_install
Ansible role installing Apache Guacamole on Ubuntu. 

### Tested on
* Ubuntu 20.04
* Ubuntu 22.04

### Tested with
* Ansible 2.10
  * community.mysql 1.2.0
* Guacamole 1.4.0
* MySQL 8.0.30
* Tomcat 9.0.31

### Requirements
* Local MySQL (optional, required if using DB authentication)

### Features
* Deploy with Tomcat 9
* Install xrdp, LXQt
* Authentication
  * default (XML-based)
  * MySQL
  * TOTP (requires MySQL)
* ~~Manage groups and users: TODO~~ (will not implement, check out [this repo](https://github.com/scicore-unibas-ch/ansible-modules-guacamole) instead!)
* ~~Manage connections: TODO~~ (same as above)

### Vars (including default values)
```
guacamole__guacd_port: "4822"
guacamole__version: "1.4.0"
guacamole__tomcat_install: "yes"
guacamole__xrdp_install: "yes"
guacamole__lxqt_install: "yes"
guacamole__username: "guacadmin" # value fixed @ MySQL auth, can be changed if using XML auth
guacamole__password: "guacadmin" # same as above
guacamole__mysql_auth: "yes" # change this to any other value in order to use XML auth instead
guacamole__mysql_host: "localhost"
guacamole__mysql_db: "guacd"
guacamole__mysql_root_user: "root"
guacamole__mysql_root_password: "root"
guacamole__mysql_user: "guacadmin"
guacamole__mysql_password: "guacadmin"
guacamole__mysql_connector_java_ver: "8.0.30"
guacamole__totp_auth: "yes"
```
