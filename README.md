# PhpIPAM + LDAP via Docker Compose

Once upon a time I was tasked with deploying PhpIPAM with LDAP authentication to a Debian server, and expose it via HTTPS. In order to make this ordeal more bearable, I took to the mighty Docker Compose + Nginx duo, which turned out to be quite a pleasurable experience, despite the [underlying technologies involved](https://eev.ee/blog/2012/04/09/php-a-fractal-of-bad-design/).

## Features
- OpenLDAP server
- LDAP Account Manager
- PhpIPAM that optionally uses the LDAP server
- Nginx with automatic SSL management via ZeroSSL and subdomain management

## Setup
1. Install docker and docker compose
2. Copy the repo to the target server
3. Rename .env.example to .env and fill in the missing variables
4. run `docker compose up -d`
