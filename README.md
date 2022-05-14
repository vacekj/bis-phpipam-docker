# PhpIPAM + LDAP via Docker Compose

Once upon a time I was tasked with deploying PhpIPAM with LDAP authentication to a Debian server, and expose it via HTTPS. In order to make this ordeal more bearable, I took to the mighty Docker Compose + Nginx duo, which turned out to be quite a pleasurable experience, despite the underlying technologies involved ([php sucks](https://eev.ee/blog/2012/04/09/php-a-fractal-of-bad-design/)).

## Features
- OpenLDAP server
- LDAP Account Manager
- PhpIPAM that can use LDAP
- Nginx with automatic SSL management via ZeroSSL and subdomain management