ansible-role-pytest-rpc
=======================

This role will prepare RPC-O deployments for testing via Molecule. This
role is meant to be used in conjunction with the "[pytest-rpc](https://github.com/rcbops/pytest-rpc)"
plug-in.

Requirements
------------

This role requires an existing rpc-openstack deployment and a JSON file
containing the ansible dynamic inventory for that infrastructure. This role is
assumed to be executed from the "Deployment Host" for said OpenStack
deployment.

How to Use Role
---------------

Top level role:

    - hosts: hosts
      roles:
        - role: ansible-role-pytest-rpc
        
Including the role in the "main.yml" tasks file:

    - import_role:
        name: ansible-role-pytest-rpc

License
-------

Apache 2.0
