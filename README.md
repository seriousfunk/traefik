# traefik
traefik template using docker-compose

1. Rename traefik_sample.toml to traefik.toml

2. Edit **traefik.toml** and update [test:$apr1$iT82Z453$soPTsIhDKjBq9Yy9BTB0U/] in the [api.auth.basic] section to your username and htpasswd'd password.
* You can generate a new user:password with `htpasswd -nb username password`
  
3. Rename docker-compose_sample.yml to docker-compose.yml

4. Edit **docker-compose.yml** and change monitor.senthebricks.com to your domain (traefik.frontend.rule=Host:monitor.sendthebricks.com)

5. Run `docker-compose up -d`
