ansible-role-zeppelin
=====================

[![Molecule Test](https://github.com/kevincoakley/ansible-role-zeppelin/actions/workflows/molecule-test.yml/badge.svg)](https://github.com/kevincoakley/ansible-role-zeppelin/actions/workflows/molecule-test.yml)

Install Apache Zeppelin - https://zeppelin.apache.org . Tested with Zeppelin 0.9.0 with CentOS 7 & 8 and Ubuntu 18.04 & 20.04.

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml

Dependencies
------------

None

Example Playbook
----------------

    - name: Zeppelin role for CentOS and Ubuntu systems
      hosts: zeppelin
      become: yes
      become_method: sudo
    
      vars:
        - zeppelin_notebook_dir: /mnt/notebooks
    
      roles:
        - ansible-role-zeppelin
    
      tags:
        - zeppelin
    
License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)
