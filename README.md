# Nginx Web Server Lab

This project demonstrates how to install and configure a basic **Nginx web server** on **Ubuntu 24.04** in a virtualized lab environment.

The goal of this lab is to practice essential Linux system administration tasks such as service management, network configuration, firewall setup and log analysis.

## Installation Steps

### Update the system

```bash
sudo apt update
sudo apt upgrade -y
```

### Install required tools

```bash
sudo apt install -y curl wget git vim htop net-tools
```

### Install Nginx

```bash
sudo apt install nginx
```

### Check service status

```bash
sudo systemctl status nginx
```

Expected output:

```
active (running)
```

### Test the web server locally

```bash
curl localhost
```

---

## Firewall Configuration

Install firewall:

```bash
sudo apt install ufw
```

Allow required services:

```bash
sudo ufw allow 22
sudo ufw allow 80
```

Enable firewall:

```bash
sudo ufw enable
```

Check status:

```bash
sudo ufw status
```

---

## Nginx Logs

Important log files:

```
/var/log/nginx/access.log
/var/log/nginx/error.log
```

Example command to monitor logs:

```bash
tail -f /var/log/nginx/access.log
