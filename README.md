# tf-ansible-django
Using Terraform and Ansible to provisioning Django App.

## Requirements

1. Terraform
2. Ansible
3. AWS CLI

### Instructions

Remember to have your server ip address and your ssh key in place before run the commands bellow:

1. Run terraform to provisioning the EC2 instance:
```
terraform apply
```

2. Run ansible playbook to install python3 and django dependencies:
```
ansible-playbook playbook.yml -u <server-user> --private-key <your-private-key> -i hosts.yml
```

Done! :)