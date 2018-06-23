# traefik
traefik template using docker-compose

1. Rename traefik_sample.toml to traefik.toml

2. Edit traefik and update [test:$apr1$iT82Z453$soPTsIhDKjBq9Yy9BTB0U/] (test:test) to your username and MD5 hashed password.
  
3. You can generate a new user:password with `htpasswd -nb username password`
  
4. Rename docker-compose_sample.yml to docker-compose.yml

5. Edit docker-compose.yml and change monitor.senthebrickscom to your domain (traefik.frontend.rule=Host:monitor.sendthebricks.com)

6. Run `docker-compose up -d`
