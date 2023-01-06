#commands to launch

```bash
ansible-playbook playbook.yml -i inventory.ini
ansible-playbook playbook2.yml -i inventory.ini -y
```

1. The first command create the instance and update the inventory inventory.ini by adding the newly created host and all necessary information (host, user, path_to_ssh_key)

2. The second command install docker and docker-compose on the newly created ec2 instance and check by launching an nginx container


## Remark:

You need to custom some variable in the file main.yml located in /roles/create-ec2-instance/tasks such as
* aws_access_key*
* aws_secret_key*
* ec2_key_directory*
* keypair_name
* ami 
* instance_type
* region
* path_my_inventory*

the variables marked * must be customed !!!
