# ProdGoGuestbook

This is a PROD-ready deployment of a Go-service with a postgress DB on an AWS VPS; The frontend is purely from https://github.com/dreamsofcode-io/guestbook
The compose.yaml will have the full list of services maintaining the availability for the website. 
services:
- Watchtower -> https://github.com/containrrr/watchtower | automated deployment
- Traefik -> HTTPS TLS certificate, reverse-proxy, http redirect to https
- postgres -> database
- docker guestbook -> 3 instances running parallel for availability

## Usage

To deploy this application, you'll need both docker and docker compose installed on your system, and then deploy it on to your
VPS using the `docker compose up` command.

To install docker compose, please refer to the official docker instructions.

https://docs.docker.com/engine/install/ubuntu/
