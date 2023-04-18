
# cinema-docker-api

API service for cinema management written on DRF


## Installing using GitHub

Install PostgreSQL and create db

```bash
git clone https://github.com/ViktorKrUA/cinema-docker-api.git
cd cinema-docker-api
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

Inside the directory you'll see .env.sample
It's an example which data must contain .env file which you need to create and fill

```bash
set POSTGRES_HOST=POSTGRES_HOST
set POSTGRES_DB=POSTGRES_DB
set POSTGRES_USER=POSTGRES_USER
set POSTGRES_PASSWORD=POSTGRES_PASSWORD
set SECRET_KEY=SECRET_KEY
```

## Run with docker

Docker should be installed

```bash
docker-compose build
docker-compose up
```

## Getting access

- create user via api/user/register
- get access token via api/user/token

    
## Features

- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions
