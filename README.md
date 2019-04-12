# Cargo

Docker env for Craft CMS

## Setup

- Clone this repo
- `composer install`
- `docker-compose up -d --build`
- `docker-compose exec php bash`
- `./craft setup`
- Follow prompts:
    - Which database driver are you using?: **mysql**
    - Database server name or IP address: **db**
    - Database port: **3306**
    - Database username: **root**
    - Database password: **secret**
    - Database name: **craft3**
    - Database table prefix: **leave blank**

## Quirks

- Slow AF on macOS
