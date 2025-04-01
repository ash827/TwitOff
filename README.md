# TwitOff
pipenv install --python 3.9

pipenv install Flask Flask-SQLAlchemy Flask-Migrate

FLASK_APP=app.py flask db init    #generates app/migrations dir

#run both when changing the schema:

FLASK_APP=app.py flask db migrate
FLASK_APP=app.py flask db upgrade

FLASK_APP=app.py flask run

    #users = [
    #    {"id":1, "name":"First User"},
    #    {"id":2, "name":"Second User"},
    #    {"id":3, "name":"Third User"}
    #]
    #return jsonify(users)
