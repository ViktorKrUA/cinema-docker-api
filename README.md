
# cinema-docker-api

API service for cinema management written on DRF



## Installing using GitHub

Install PostgreSQL and create db

```bash
git clone https://github.com/ViktorKrUA/cinema-docker-api.git
cd cinema-docker-api
python -m venv venv
source venv/bin/activate
pip install -r requirements.txt
set DB_HOST=<your db hostname>
set DB_NAME=<your db name>
set DB_USER=<your db username>
set DB PASSWORD=<your db user password>
set SECRET_KEY=<your Django secret key>
python manage. py migrate
python manage. py runserver
```
    
## Features

- JWT authenticated
- Admin panel /admin/
- Documentation is located at /api/doc/swagger/
- Managing orders and tickets
- Creating movies with genres, actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions


## Run with docker

Docker should be installed

```bash
docker-compose build
docker-compose up
```


## Getting access

- create user via api/user/register
- get access token via api/user/token