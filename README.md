This is a bare bone example of running [Wagtail](https://github.com/wagtail/wagtail) on Google App Engine Standard Environment. Since Wagtail is Django-based CMS, it is runs almost out of the box on GAE with a few minor tweaks. The basis of this is [Running Django on App Engine standard environment](https://cloud.google.com/python/django/appengine) tutorial.

##Setup on Ubuntu 14.0.4 LTS

Clone the repo.

Follow Django on GAE tutorial to setup Cloud SQL and proxy.

Configure database settings in env.yaml 

pip install -r requirements.txt -t lib/

python manage.py migrate

python manage.py createsuperuser

python manage.py runserver

python manage.py collectstatic

gcloud app deploy

