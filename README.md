# Snibox

Deployement Snibox service with traefik

## Dependency

[Traefik v2 configuration](https://github.com/mbeurel/traefik)

## Config

**Copy environnement file**
```bash
cp .env.dist .env
```

**Edit environnement file**
```bash
vi .env
```
_Enter your parameters_

**Start Docker composer**
```bash
docker-compose up # -d to detach container
```

If your domain is local so comment line "...tls.certresolver" in your docker-compose file and add your domain to /etc/hosts

**Add 'TRAEFIK_DOMAIN' to your host**
```bash
sudo echo "127.0.0.1  YOUR_TRAEFIK_DOMAIN"  >> /etc/hosts
```

Open your favorite navigator and enter your 'SNIBOX_DOMAIN'

Great, your snibox is configure and start !


## Credits

Created by [Matthieu Beurel](https://www.mbeurel.com). Sponsored by [Nexboard](https://www.nexboard.fr).