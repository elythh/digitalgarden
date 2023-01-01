---
{"dg-publish":true,"permalink":"/self-hosting/services/internal/traefik/"}
---


> Traefik (pronounced _traffic_) is a modern HTTP reverse proxy and load balancer that makes deploying microservices easy. [Source](https://github.com/traefik/traefik)

## How do I use Traefik ?
I'm using Traefik as a reverse proxy to expose the needed services.

##  Configuration

* As everything else, I'm running [[Self hosting/Services/Internal/Traefik\|Traefik]] in a Docker Container. 
* I use LetsEncrypt to generate the certificates.
* It exposes port 443 and 80 of my machine. 
* I have a few security middleware for my needs
	* a basic auth, reading username and password from a simple `.txt` file
	* ip whitelisting, defined as an environment variable
	* [[Self hosting/Services/External/Authelia\|Authelia]] as an SSO
## Which services are currently being exposed ?


| Icon | Name            |
| ---- | --------------- |
|      | [[Self hosting/Services/External/Jellyfin\|Jellyfin]]    |
|      | [[Self hosting/Services/External/Jellyseerr\|Jellyseerr]]  |
|      | [[Self hosting/Services/External/Linkding\|Linkding]]    |
|      | [[Self hosting/Services/External/Neko\|Neko]]        |
|      | [[Self hosting/Services/External/Owncast\|Owncast]]     |
|      | [[Self hosting/Services/External/Authelia\|Authelia]]    |
|      | [[Self hosting/Services/External/BookStack\|BookStack]]   |
|      | [[Self hosting/Services/External/Outline\|Outline]]     |
|      | [[Self hosting/Services/External/Vaultwarden\|Vaultwarden]] |
|      | [[Self hosting/Services/External/Forgejo\|Forgejo]]     |
|      | [[Self hosting/Services/External/n8n\|n8n]]         |
|      |                 |
