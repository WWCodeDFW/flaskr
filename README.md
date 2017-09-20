# Flaskr
A minimal blog application built with the Python web framework Flask that supports one user's posting entries. Initial code from: http://flask.pocoo.org/docs/0.12/tutorial/.

# Requirements
* Python

## Installation
Install the app from the root directory (where setup.py lives).
```
$ pip install --editable .
```

## Run Flaskr
Set our environment variables, so Flask knows what application to run and whether to give you debug information. If you are on Windows, use `set` instead of `export` in the following commands. Do not set `FLASK_DEBUG` to `true` with a publicly exposed application, because it makes your system vulnerable.
```
$ export FLASK_APP=flaskr
$ export FLASK_DEBUG=true
```

Start our web server to run Flaskr.
```
$ flask run
```

Initialize the database (only do this once unless you want to delete any blog posts you create).
```
$ flask initdb
```
