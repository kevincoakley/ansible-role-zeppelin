ansible-role-zeppelin
=====================

[![Build Status](https://travis-ci.org/kevincoakley/ansible-role-zeppelin.svg?branch=master)](https://travis-ci.org/kevincoakley/ansible-role-zeppelin)

Install Apache Zeppelin - https://zeppelin.apache.org . Tested with CentOS 7 and Ubuntu 16.04

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
