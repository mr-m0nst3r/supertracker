# supertracker

This repo is a fork of [zebulgar/supertracker](https://github.com/zebulgar/supertracker) and is customized for Digital Ocean App Platform Deployment.

## Requirements
Set enviorment variables for the following:

DJANGO_ALLOWED_HOSTS -> ${APP_DOMAIN}<br>
This allows us to know the randomly generated URL that App Platform provides and provide it to our app


DATABASE_URL -> ${<NAME_OF_YOUR_DATABASE>.DATABASE_URL}<br>
In this case, we’ll name our database db in the next step, so this should be ${db.DATABASE_URL}


DEBUG -> True<br>
Set this to True for now to verify your app is functioning and set to False when it’s time for this app to be in production


DJANGO_SECRET_KEY -> <A RANDOM SECRET KEY><br>
You can either allow your app to generate this at every launch or pick a strong password with at least 32 characters to use as this key. Using a secure password generator is a good option for this
Don’t forget to click the Encrypt check box to ensure that your credentials are encrypted for safety
