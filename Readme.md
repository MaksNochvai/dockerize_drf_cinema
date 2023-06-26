# Cinema API
API for cinema with the ability to view movie screenings and buy tickets,
you can also add or view genres and actors, available screening locations,
a description of the movie with its duration and all its data

# Installing using GitHub
## Install PostgresSQL and create db

```
git clone https://github.com/MaksNochvai/dockerize_drf_cinema.git
python -m venv venv
    source venv/bin/activate # Activation of the virtual environment (Unix)
    venv\Scripts\activate # Activation of the virtual environment (Windows)
pip install -r requirements.txt
set POSTGRES_HOST=<your POSTGRES HOST name>
set POSTGRES_DB=<your POSTGRES DB name>
set POSTGRES_USER=<your POSTGRES USER name>
set POSTGRES_PASSWORD=<your POSTGRES PASSWORD>
set SECRET_KEY=<your SECRET_KEY>
python manage.py migrate
python manage.py runserver
```