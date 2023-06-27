# Cinema API

-----------------------------------

API for cinema with the ability to view movie screenings and buy tickets. You can also add or view genres and actors, available screening locations, and get a description of the movie with its duration and all its data.

## Installing using GitHub

-----------------------------------

Install PostgreSQL and create a database

1. Clone the repository:
git clone https://github.com/MaksNochvai/dockerize_drf_cinema.git

2. Set up a virtual environment and activate it:
```
python -m venv venv
source venv/bin/activate # Activation of the virtual environment (Unix)
venv\Scripts\activate # Activation of the virtual environment (Windows)
```
3. Install the required dependencies:
```
pip install -r requirements.txt
```
4. Set the following environment variables:
```
set POSTGRES_HOST=<your POSTGRES HOST name>
set POSTGRES_DB=<your POSTGRES DB name>
set POSTGRES_USER=<your POSTGRES USER name>
set POSTGRES_PASSWORD=<your POSTGRES PASSWORD>
set SECRET_KEY=<your SECRET_KEY>
```
5. Start the development server:
```
python manage.py migrate
python manage.py runserver
```
# Run with docker

-----------------------------------
docker should be installed
```
docker-compose build
docker-compose up
```
# Getting access

------------------------------------
- create user via /api/user/register/
- get access token via /api/user/token

# Features

-------------------------------------
- JWT authenticated
- Admin panel /admin/
- Managing orders and tickets
- Documentation is located at /api/doc/swagger/
- Creating movies with genres and actors
- Creating cinema halls
- Adding movie sessions
- Filtering movies and movie sessions
