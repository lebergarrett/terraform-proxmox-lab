# Simple Terraform template for spawning VMs in one of my local Proxmox servers

This is to be used as a basis for future projects that will involve IaC.

## Quick Start

Create a terraform.tfvars file that contains the 'proxmox_username' and 'proxmox_password' variables and their values
```
#terraform.tfvars
proxmox_username = "user@pve"
proxmox_password = "password"
```

Initialize terraform in the directory
```
terraform init
```

Format and validate the config
```
terraform fmt
terraform validate
```

Plan out the changes that will be made, if necessary
```
terraform plan
```

Apply the configuration and create the vms on proxmox server
```
terraform apply
```

Tear down resources
```
terraform destroy
```