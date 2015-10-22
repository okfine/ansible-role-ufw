ansible-role-ufw [![Build Status](https://travis-ci.org/okfine/ansible-role-ufw.svg?branch=master)](https://travis-ci.org/okfine/ansible-role-ufw)
=========

Ansible role to install and configure ufw on Debian/Ubuntu systems.

Requirements
------------

This role is designed for use on the Operating Systems listed below.

* Debian/Ubuntu

Role Variables
--------------

The ```allow_list``` variable is a list of hashes which include ports/protocols to allow through the firewall.

	allow_list:
	  - { port: "22", protocol: 'tcp' }

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: ansible-role-ufw }

License
-------

BSD / MIT

Author Information
------------------

[okfine](https://github.com/okfine)
