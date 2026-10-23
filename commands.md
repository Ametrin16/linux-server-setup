# Commands Used

## User

    id deploy
    groups deploy

## SSH

    sudo sshd -t
    sudo sshd -T | grep -i '^permitrootlogin'

## Firewall

    sudo ufw status verbose

## Nginx

    nginx -v
    sudo nginx -t
    sudo systemctl enable --now nginx
    sudo systemctl status nginx

## Website

    curl -i http://localhost/

## Health Check

    curl -i http://localhost/health

## Logs

    sudo tail -n 20 /var/log/nginx/access.log
    sudo tail -n 20 /var/log/nginx/error.log
