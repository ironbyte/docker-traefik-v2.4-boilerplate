# Docker Traefik v2.4 Boilerplate

## Features

- Automatic Let's Encrypt Certificate management
- Traefik/TLS configuration for Qualys SSL Labs A+ rating
- Traefik Basic Auth/Rate Limit middlewares
- Global HTTP to HTTPS redirection
- Secure Traefik Dashboard, Portainer-CE and Traefik/whoami services

## Setup

- Run `docker network create traefik_proxy`
- Run `cp .env.example .env`
- Run `docker run --rm httpd:2.4-alpine htpasswd -nbB <YOUR_USER_NAME> <YOUR_PLAINTEXT_PASSWORD> >> .htpasswd && chmod 600 .htpasswd`
- Run `docker-compose up -d`
