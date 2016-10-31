vm-rm
=========

Remove a compute instance.

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

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: vm-rm, cloud: mycloud }

License
-------

BSD

Author Information
------------------

yvarbanov
