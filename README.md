# Rancher-nginx-letsencrypt

Setup [Rancher v2](https://rancher.com/) behind nginx proxy, with [Let's Encrypt](https://letsencrypt.org/) certificates, within a docker environment.

Based on:
- [The rancher doc](https://rancher.com/docs/rancher/v2.x/en/installation/single-node-install-external-lb/) that provides sample to configure nginx
- [Docker-nginx-certbot](https://github.com/reallyreally/docker-nginx-certbot) a docker container providing nginx with certbot for Let's Encrypt SSL certificates
- [Let's Encrypt](https://letsencrypt.org/) a free, automated, and open Certificate Authority

### How to use ?

- Edit env file and update *CERTBOT_EMAIL* with your email
- Edit the nginx proxy config and replace *rancher.yourdomain.com*
- Run the docker stack on your server
- Start certbot to generate your certificates, within the docker container

### How to run ?

Start the docker stack

```
docker-compose up -d --build
```

Generate your certificates with certbot within the docker container

```
```

