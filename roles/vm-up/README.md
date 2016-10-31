vm-up
=========

Deploy a compute instance in openstack.

Currently only supports boot from image.

Requirements
------------

Ansible 2.0+

Shade

cloud.yaml

	clouds:
	    mycloud:
	       auth:
		auth_url: http://openstack.com/v2.0/
		username: yvarbanov
		password: mypass
		project_name: demo

Place config file in /etc/ansible/openstack.yaml, /etc/openstack/clouds.yaml or ~/.config/openstack/clouds.yaml

Role Variables
--------------

Check defaults/main.yml

Dependencies
------------

None.

Configuration
-------------


Set with valid variables (*Must exists within your Openstack env):

	- instance_name
	- image_name*
	- key_name*
	- net_name*


Example Playbook
----------------

    - hosts: all
      roles:
         - { role: vm-up, cloud: mycloud }

License
-------

BSD

Author Information
------------------

yvarbanov
