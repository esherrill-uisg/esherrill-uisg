# FlaskDbFrontend
* This is a simple web app using Python 3, Flask https://flask.palletsprojects.com/ (Web framework), psycopg2 https://www.psycopg.org/ (PostgreSQL module),  and HTML.
* It can be built into a single-file executable for Windows, Linux, or macOS, using pyinstaller https://pyinstaller.org/ - but only on the same platform as the target.

## Usage
* This is a simple read-only database browser, for uip_int tables, intended as a starting point for future development.
* See below for instructions on how to build and deploy.

## Get Started
* See below:

## Prerequisites
* See below:

```
Setup examples (Linux):
...
# pull code
cd ~/Developer
git clone https://git.us-west-2.codecatalyst.aws/v1/UISOLUTIONS/FlaskDbFrontend/FlaskDbFrontend
cd FlaskDBFrontend
# create a virtualenv
python -m venv .venv
# activate it
source .venv/bin/activate
# install requirements
pip install -r ./requirements.txt
# create binary
pyinstaller --clean -F -p . --add-data templates:templates  ./app.py
# set env vars
source ~/db_vars
# run binary
./dist/app
# done!
```
Minor differences for building on Windows and macOS, are left as an exercise for the reader.

Or there's a shell script to do the last bit after pyinstaller runs:

applocal.sh

## Install
* Create the binary for your platform.
* Move and rename app (or other named binary) as built above. 
* Run and enjoy!

## Testing
* Run the app.
* Let me know if it breaks.

## Contact
* Eric Sherrill 
* eric.sherrill(@)gmail.com