
# Networking Notes

This file explains the networking setup used in the Azure Cloud Operations Lab.

## Virtual Network

The VM was deployed inside an Azure Virtual Network.

The virtual network provides private networking for Azure resources.

## Subnet

The VM was placed inside a subnet.

A subnet is a smaller section of the virtual network used to organize resources.

## Public IP Address

A public IP address was assigned to the VM.

This allowed the VM to be reached from the internet for:

- SSH connection
- NGINX web server testing

## Network Security Group

A Network Security Group was attached to control traffic.

Allowed inbound rules:

- SSH 22 for remote Linux access
- HTTP 80 for web server access

## Result

The VM was successfully connected to the internet using a public IP address, while inbound traffic was controlled using a Network Security Group.
