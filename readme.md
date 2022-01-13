Create cert

1. run docker-compose up
because you need that nginx be up to work with certbot

2. run command (with required domain in the end after -d)
docker compose run --rm  certbot certonly --webroot --webroot-path /var/www/certbot/ -d exmapledomain.com

3. check that domain succesfully created
- output from command should be succesfull
- dir for domain should appears in certbot\conf\live\domainname\*.*

Detailed instruction:
https://mindsers.blog/post/https-using-nginx-certbot-docker/# letsnginx
