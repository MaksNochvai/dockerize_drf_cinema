# Cinema API

API for cinema with the ability to view movie screenings and buy tickets. You can also add or view genres and actors, available screening locations, and get a description of the movie with its duration and all its data.

## Installing using GitHub

### Install PostgreSQL and create a database

1. Clone the repository:
git clone https://github.com/MaksNochvai/dockerize_drf_cinema.git

bash
Copy code

2. Set up a virtual environment and activate it:
```shell
python -m venv venv
source venv/bin/activate # Activation of the virtual environment (Unix)
venv\Scripts\activate # Activation of the virtual environment (Windows)
Install the required dependencies:

shell
Copy code
pip install -r requirements.txt
Set the following environment variables:

POSTGRES_HOST: Your PostgreSQL host name
POSTGRES_DB: Your PostgreSQL database name
POSTGRES_USER: Your PostgreSQL user name
POSTGRES_PASSWORD: Your PostgreSQL password
SECRET_KEY: Your secret key
On Windows, you can use the set command:

shell
Copy code
set POSTGRES_HOST=<your POSTGRES HOST name>
set POSTGRES_DB=<your POSTGRES DB name>
set POSTGRES_USER=<your POSTGRES USER name>
set POSTGRES_PASSWORD=<your POSTGRES PASSWORD>
set SECRET_KEY=<your SECRET_KEY>
Run the database migrations:

shell
Copy code
python manage.py migrate
Start the development server:

shell
Copy code
python manage.py runserver