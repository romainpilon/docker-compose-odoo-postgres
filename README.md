#Odoo + Postgresql

This repository helps set up Odoo 8 + Postgresql 9.4.

##Setup

Fill the .env file with your credentials and your domain:

```
ODOO_USER=
ODOO_PASS=
ODOO_TRAEFIK_URL=
TRAEFIK_DEFAULT_DOMAIN=
ACME_EMAIL=
```

You'll need to set the same credentials inside the odoo/config/odoo.conf file:

```
db_user =
db_password =
```

ODOO_USER will be used by Odoo to connect to the database (which will be created as well with the ODOO_PASS password).

##Run

```bash
cd docker-compose-traefik-odoo-postgres
docker-compose up -d
```

### Tested with
![Docker version](https://img.shields.io/badge/Docker-19.03.5-blue)
![Docker-compose version](https://img.shields.io/badge/Docker--compose-1.24.1-informational)
