# Setup Steps

This file documents the setup steps for the Azure Cloud Operations Lab.

## 1. Resource Group

Created a resource group named `rg-cloud-ops-lab`.

The resource group is used to keep all project resources in one place.

Resources inside this group include:

- Virtual machine
- Virtual network
- Network security group
- Public IP address

Screenshot: `screenshots/resource-group.png`

## 2. Virtual Machine

Created an Azure Linux virtual machine named `vm-cloud-ops-lab`.

Main settings used:

- Region: France Central
- Image: Ubuntu Server 24.04 LTS
- Authentication: SSH public key
- Username: azureuser
- Inbound ports: SSH 22 and HTTP 80

The VM is used as the main cloud server for this project.

Screenshots:

- `screenshots/virtual-machine-overview.png`
- `screenshots/vm-networking.png`

## 3. SSH Connection

Connected to the VM using SSH from Windows PowerShell.

SSH command format:

`ssh -i "path-to-key.pem" azureuser@public-ip-address`

This confirms that the VM can be accessed securely using an SSH private key.

## 4. NGINX Installation

Installed NGINX on the Linux VM using:

- `sudo apt update`
- `sudo apt install nginx -y`

Checked the NGINX service status using:

- `sudo systemctl status nginx`

The NGINX web server was successfully installed and is reachable from the browser using the VM public IP address.

Screenshot: `screenshots/nginx-running.png`

## 5. Result

The Azure VM was successfully deployed, connected through SSH, and configured to serve a web page using NGINX.

This proves that the project includes:

- Cloud VM deployment
- Basic Linux server setup
- SSH access
- Public IP testing
- HTTP web server access
