# Linux Server Setup

## Project Overview

This project prepares an Ubuntu server to host a simple web application.

## Environment

- OS: Ubuntu 26.10
- Hostname: ubuntu1
- Deployment user: deploy
- Web server: Nginx
- Application directory: /var/www/kai-app

## Implemented

- Created the deploy user and added it to the sudo group.
- Configured SSH access and disabled root login.
- Enabled UFW firewall.
- Allowed ports 22, 80, and 443.
- Installed and enabled Nginx.
- Created a test web page.
- Configured the /health endpoint.
- Verified service status and Nginx logs.

## Verification

Check the homepage:

    curl -i http://localhost/

Check the health endpoint:

    curl -i http://localhost/health

Check Nginx:

    sudo systemctl status nginx

Check firewall:

    sudo ufw status verbose

## Health Check

The /health endpoint returns HTTP 200 and the text OK.
