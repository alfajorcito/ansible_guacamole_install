# ansible_guacamole_install
Ansible role installing Apache Guacamole on Ubuntu.

### Tested on
* Ubuntu 22.04

### Tested with
* Ansible 2.10
  * community.mysql 1.2.0

### Requirements
* MySQL (optional, required if using DB auth)

### Features
* Deployed with Tomcat
* Authentication
  * default
  * MySQL (TODO)
  * TOTP (requires MySQL, TODO)
* Session recording: TODO
* Install LXQt and xrdp

### Vars
TODO
