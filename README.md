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

Initialize the database (only do this once unless you want to delete any blog posts you create).
```
$ flask initdb
```

Start our web server to run Flaskr.
```
$ flask run
```

## Exercise
For a next step, create another page on your blog site that serves up a single blog entry based on the blog entry's id:
* The page should be accessed at the path '/entry/<id>'. For example, a page to serve up your first entry, that would have id 1, would be at http://127.0.0.1:5000/entry/1.
* You can create a new template, perhaps called entry.html, that inherits from the layout.html template.
Bonus: modify the show_entries.html template to provide a link to individual entries from each entry shown in the list of entries.

## Other tutorials
 * https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world - More robust Flask tutorial that considers production relevant issues such as virtual environments, SQLAlchemy extension to provide an Object Relational Mapper that abstracts working with the database, database migrations, multiple users, handling logins, creating user profile pages with avatars via gravatar, etc.
 * https://www.tutorialspoint.com/flask/flask_overview.htm - Separate brief lessons covering various Flask topics.
