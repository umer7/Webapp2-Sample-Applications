### Install instructions


These sample applications uses the python2.7 runtime for applengine.

The git repository includes a virtualenv script to setup a virtual sandbox environment, we don't want to install things all over our system.
To install the virtualenv for this project (or another) and activate it simply do:

python virtualenv.py .
. bin/activate

To exit the virtualenv the exit command is:

deactivate


To run test install nosetest runner with:

pip install nose


## Running the application

The Makefile that's included presumes that your google appengine installation is in /usr/local/google_appengine, you can always change the path in the Makefile


Run the sample-auth app execute the command:

make serve-sample-auth


# NOTES:
- NDB folder is included in application due to a import statement in webapp2_extras/appengine/auth/models.py
