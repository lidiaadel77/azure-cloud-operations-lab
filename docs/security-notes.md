# Security Notes

This file documents the basic security decisions used in the Azure Cloud Operations Lab.

## Network Security Group

The virtual machine uses a Network Security Group to control inbound network traffic.

Allowed inbound ports:

- SSH 22
- HTTP 80

## SSH Access

SSH port 22 was opened to allow secure remote access to the Linux VM.

In a production environment, SSH access should be restricted to trusted IP addresses only.  
Leaving SSH open to the internet can increase the risk of brute-force login attempts.

## HTTP Access

HTTP port 80 was opened to test the NGINX web server from a browser.

In a production environment, HTTPS should be used instead of HTTP to encrypt traffic.

## Security Best Practices

Recommended improvements for production:

- Restrict SSH access to a trusted IP address.
- Use SSH keys instead of passwords.
- Use HTTPS instead of HTTP.
- Close unused ports.
- Monitor failed login attempts.
- Apply least privilege access.
- Delete unused public IP addresses and cloud resources.

## Result

The lab demonstrates basic cloud network security by using inbound rules to control access to the VM.
