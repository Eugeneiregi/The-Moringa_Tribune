## Installation
- set up a virtual environment using the following command
- python3 -m venv  virtual
And activate virtual
[source virtual/bin/activate]



Install the requirements using:
- pip install -r requirements.txt/ pip freeze > requirements.txt
- create a .env file and add
- SECRET_KEY='<random-string>'
- DEBUG=True
- ALLOWED_HOSTS='*'
- DATABASE_URL='postgres://databaseowner:password@localhost/databasename'
- create a database using postgresql(recommend)
* CREATE DATABASE <your-database-name>
- create a migration using the following command
- python3 manage.py makemigrations
- python manage.py migrate

- create a super user for admin account
* python 3.6 manage.py createsuperuser
* add your password and username , email is not a must.

