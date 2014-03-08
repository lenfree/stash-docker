Role Name: atlassian-stash-container
========

This role is to build atlassian-stash container, start and link with its data container.

Requirements
------------

To use ansible docker module, docker-py >= 0.3.0 is required. 

Role Variables
--------------

stash_version, nginx_version, storage_version is use to replace tag versioning.


Dependencies
------------


Example Playbook
-------------------------

 - name: Manage Stash container
   hosts: vagrant
   gather_facts: true
   roles:
       -  role: manage-atlassian-stash-container
License
-------


Author Information
------------------

Lenfree Yeung, lenfree.yeung@gmail.com
