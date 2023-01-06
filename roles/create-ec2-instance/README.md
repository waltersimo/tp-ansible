create-ec2-instance
=========

This is a role to create an ec2 instance on AWS 


Requirements
------------

* AWS credentials to create resources.
* boto3
* botocore

Role Variables
--------------

* region: The region which the resources will be created 
* vpc_cidr: CIDR Block of VPC
* subnet_cidr: CIDR Block of Subnet
* igw_name: IGW Name
* route_name: Route Name
* etc... (look in yaml file in the directory vars)


Example Playbook
----------------

- name: Create an EC2 instance with VPC, Internet Gateway Security group and  keypair
  hosts: localhost
  connection: local
  gather_facts: true
  roles:
    - { role: create-ec2-instance, register_vars: true}

License
-------
BSD

Author Information
------------------
Walter Simo (01/2023)
