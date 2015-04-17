# OpenIDTest
A simple django app where you can log in and log out using openid: really just an example for openid using python-social-auth in django.

Setting up
------------------
1. Clone this repository
2. `cd` into repo
3. Create a virtual env.  It's preferable to create the environment outside of the repository folder.  For example: 
`virtualenv ../OpenIDTestEnv`
4. Activate the virtual env:
`source ../OpenIDTest/bin/activate`
5. Install the required modules from requirements.txt:
`pip install -r requirements.txt`
6. Set up the django database by running:
`python manage.py makemigrations`
and then 
`python manage.py migrate`
7. Run the django server:
`python manage.py runserver`
8. You can kill the server with Ctrl-C.


Now you can point your browser at http://localhost:8000 to see the simple log in and log out functionality that uses openid. 
To test it out, just enter an openid URI. You can go to [Yahoo](http://openid.yahoo.com/) to get one. The one provided by my locally running crowdid server is http://localhost:8095/openidserver/users/vikram while the one from the coop’s dev server would be https://login-dev.psfc.coop/openidserver/users/vikram, however this one doesn’t work.
