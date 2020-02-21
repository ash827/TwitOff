# TwitOff
pipenv install --python 3.7

pipenv install Flask Flask-SQLAlchemy Flask-Migrate

FLASK_APP=app.py flask db init    #generates app/migrations dir

#run both when changing the schema:

FLASK_APP=app.py flask db migrate
FLASK_APP=app.py flask db upgrade

FLASK_APP=app.py flask run

