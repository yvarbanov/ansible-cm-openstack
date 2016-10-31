# ansible-cm-openstack
Ansible roles using cloud modules for Openstack administration.

Requirements
------------

Ansible 2.0+

Shade

cloud.yaml

Check roles readme for additional information.

Global Vars
--------------

You can modify clouds.yml to your needs.

Place config file in /etc/ansible/openstack.yaml, /etc/openstack/clouds.yaml or ~/.config/openstack/clouds.yaml

Edit all.yml:

* to boot an instance edit:

	- instance_name
	- image_name*
	- key_name*
	- net_name*

*Set with valid (existing) variables:

* to delete instance:

	- instance_name

Usage
-------

Create hosts file.

Check site.yml.sample for example playbook.


Author Information
------------------

yvarbanov
