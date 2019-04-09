# Cargo

Docker env for Craft CMS

## Setup

- Clone this repo
- `composer install`
- `docker-compose up -d --build`
- Go to [localhost:5000](localhost:5000)
    - User: `root` Pass: `secret` db: leave blank
    - Create new database: `craft_db_name_you_pick`
- `docker-compose exec db bash`
- `./craft setup`
- Follow prompts:
    - Which database driver are you using?: **mysql**
    - Database server name or IP address: **db**
    - Database port: **3306**
    - Database username: **root**
    - Database password: **secret**
    - Database name: **craft_db_name_you_pick**
    - Database table prefix: leave blank

To add:
    - Redis
    - Debug Toolbar
    - docker-sync? for faster page loads...
