this is a fork from https://github.com/linuxserver/docker-letsencrypt hacked to solve 3 problems:

1. Give hability to run certbot in staging mode so you can test your site without offending letsencrypt request limit
2. Remove php7 and disable fmp service from S6
3. Generate domain.key and domain.crt certificates from certbot result to be used by registry

current working tag: rubentrancoso/docker-letsencrypt:nophp

this branch was meant to explore and discover how s6 works and how to tweak with it, so it's basicaly a very dirty hack.
once it's working the next step will be to create a new clean solution from master branch
