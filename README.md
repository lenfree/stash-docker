Role Name: stash-docker
========

This role is to manage Atlassian Stash stack in a Docker container.

Tested on EL6.

Requirements
------------

To use ansible docker module, docker-py >= 0.3.0 is required. 

Stash, Nginx and data containers should be available from your repository/registry.

Role Variables
--------------

stash_version, nginx_version, storage_version is use to replace tag versioning.

Note: Replace myregistry with your registry/repo name.

Dependencies
------------



Example Playbook
-------------------------

 - name: Manage Stash container
   hosts: vagrant
   gather_facts: true
   roles:
       -  role: stash-docker
License
-------

GPLv2
Author Information
------------------

Lenfree Yeung, lenfree.yeung@gmail.com
