# Nginx Installation

This file documents the installation steps for nginx on Ubuntu 24.04.

## Update system packages

```bash
sudo apt update
sudo apt upgrade -y


Install nginx

sudo apt install nginx


Check nginx service status

sudo systemctl status nginx

Expected result: active (running)


Restart nginx if needed

sudo systemctl restart nginx


Enable nginx at boot

sudo systemctl enable nginx


Test locally

curl localhost
