# Cinema API

API service for cinema management written on DRF

### Test user
* Login: Admin
* Password: test2023

## Features
* JWT authenticated
* Admin panel /admin/
* Documentation is located at /api/doc/swagger/
* Managing orders and tickets
* Creating movies with genres, actors
* Creating cinema halls
* Adding movie sessions
* Filtering movies and movie sessions

## Installing using GitHub
1. Install PostgresSQL and create db
2. git clone https://github.com/IvanGLS/api-cinema.git
3. cd cinema_API
4. python -m venv venv
5. venv activate
   * source venv/bin/activate (on macOS)
   * venv\Scripts\activate (on Windows)
6. pip install -r requirements.txt
7. add db settings to .env (load_dotenv use that automatically)
   * DB_HOST= your db hostname
   * DB_NAME= your db name
   * DB_USER= your db username
   * DB_PASSWORD= your db user password
   * SECRET_KEY= your secret key
8. python manage.py migrate
9. python manage.py runserver

## Run with docker
Docker should be installed
* docker-compose build
* docker-compose up

## Getting access
* create user via /api/user/register/
* get access token via /api/user/token/