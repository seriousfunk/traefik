# traefik
traefik template using docker-compose

1. Rename traefik_sample.toml to traefik.toml
  a. Edit traefik and update [user:password] to your username and MD5 hashed password.
2. Rename docker-compose_sample.yml to docker-compose.yml
  a. Edit docker-compose.yml and change monitor.senthebrickscom to your domain (traefik.frontend.rule=Host:monitor.sendthebricks.com)
3. Run `docker-compose up -d`
