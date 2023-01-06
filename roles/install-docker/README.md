docker-install
=========

This is a role to install docker and docker-compose on a linux machine

Example Playbook
----------------

example of playbook

- name: installation docker et docker compose
  hosts: server
  gather_facts: true
  become: true
  roles:
     - install-docker

License
-------
BSD

Author Information
------------------
Walter Simo (01/2023)
