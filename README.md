# Schaakclublievegem.be source code

## Setup

```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
export FLASK_APP=server.py # or use a dot-file (.env), the python-dotenv will load the variables defined in it for you
python -m flask run
```
### Configuring debug mode

There are two ways of doing this, you either enable all development features (including debug mode) via FLASK_ENV=development,
which does the following things:

- activates the debugger
- activates the automatic reloader (very usefull to develop locally)
- enabled debug mode on the Flask application

You can also control debug mode separately from the environment by exporting FLASK_DEBUG=1