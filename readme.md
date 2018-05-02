# Terraform & Ansible EC2

A simple repository to create and provision an EC2 instance using Terraform & Ansible.

## Install 
In the root directory run `terraform init` to pull in the dependencies needed.

## Run
`terraform apply` will prompt you for some details regarding the new EC2 setup. 
Once this is completed you should have a fully provisioned EC2 instance with PHP7.2 & Nginx. Hit the IP address in the console
and you should see the PHP Info page confirming that PHP7.2 was installed.

### Domain
To use a domain, you need to change the `roles/nginx/defaults/main.yml` file.

## Destroy
`terraform destroy`

## Todo
- [ ] SSL Certificate with Lets Encrypt
- [x] Install Composer
- [x] Change Nginx web root