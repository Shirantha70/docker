# Automating the Installation of Docker Engine on CentOS 8

__1. Introduction__

This Ansible Playbook will automate the installation the latest version of Docker engine on CentOS 8 nodes.

__2. Guidelines__

- Setup your Ansible environment by adding the list of docker nodes into /etc/ansible/hosts file in Ansible host Also, by configuring key based authentication
from Ansible host to listed nodes.
  _Example entry:_
  ```
  [docker-nodes]
  docker-node1 ansible_host=192.168.10.10 ansible_user=root
  docker-node2 ansible_host=192.168.10.11 ansible_user=root
  docker-node3 ansible_host=192.168.10.12 ansible_user=root
  ```
  
  More on key-based authentication
  - ssh-keygen
  - ssh-copy-id
  
- Configure and enable a yum repository for your centOS nodes.
  

__3. Reference__
- https://docs.docker.com/engine/install/centos/
  
