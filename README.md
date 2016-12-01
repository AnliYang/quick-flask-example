### Quick Start for a local Python-Flask server with a PostgreSQL database (using Flask-SQLAlchemy ORM).

#### To run (from the command line):
1. get this repo onto your machine, by either:
  - cloning the repo:
    - with SSH: `git clone git@github.com:AnliYang/quick-flask-example.git`
    - with HTTPS: `git clone https://github.com/AnliYang/quick-flask-example.git`
  - or downloading it from GitHub: [https://github.com/AnliYang/quick-flask-example]
- navigate into the new directory: `cd quick-flask-example`
- create your virtual environment: `virtualenv env`
  - note: requires [virtualenv](https://virtualenv.pypa.io/) to be installed
- activate your virtual environment: `source env/bin/activate`
- install requirements: `pip install -r requirements.txt`
- import environment variables: `source secrets.sh`
  - note: you'll need to add export statements for any necessary environment variables to the secrets.sh file
- create a db `createdb example`
  - note: make sure you have [PostgreSQL](https://www.postgresql.org/) running
- launch: `python server.py`
- direct your browser to [http://localhost:5000] to see the index page
- play around!

#### Sample File Structure:
- .gitignore (files for git to ignore, especially if they contain sensitive information)
- env/ (your virtual environment)
- static/ (static assets)
  - css/
    - css stylesheets (.css)
  - js/
    - javascript files (.js)
  - images files (.png, .jpeg, etc.)
- templates/
  - html templates (.html)
- model.py (data model, class definitions)
- server.py (the file to run to launch your app)
- requirements.txt
- secrets.sh
