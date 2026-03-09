# Firewall Configuration

This document describes the basic firewall setup using UFW on Ubuntu.

## Install firewall

```bash
sudo apt install ufw

Allow SSH

sudo ufw allow 22

Allow HTTP

sudo ufw allow 80

Enable firewall

sudo ufw enable

Check firewall status

sudo ufw status

Expected output: Status: active


This ensures that the server allows SSH and web traffic while blocking unnecessary ports.

```
