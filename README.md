# ansible_guacamole_install
Ansible role installing Apache Guacamole on Ubuntu. 
(WARNING: THIS IS NOT WORKING PROPERLY YET = WORK IN PROGRESS)

### Tested on
* Ubuntu 22.04

### Tested with
* Ansible 2.10
  * community.mysql 1.2.0

### Requirements
* Local MySQL (optional, required if using DB auth)

### Features
* Deployed with Tomcat
* Authentication
  * default
  * MySQL
  * TOTP (requires MySQL, TODO)
* Session recording: TODO
* Optionally, install LXQt and xrdp

### Vars
TODO
