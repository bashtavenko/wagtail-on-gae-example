This is a bare bone example of running [Wagtail](https://github.com/wagtail/wagtail) on Google App Engine Standard Environment. Since Wagtail is Django-based CMS, it is runs almost out of the box on GAE with a few minor tweaks. The basis of this is [Running Django on App Engine standard environment](https://cloud.google.com/python/django/appengine) tutorial.

In addition to the bare bone example, there's another nice library called [Djangae](https://github.com/potatolondon/djangae) which provides many helpful features notably storage backend for the blog images, authentication, Datastore backend and others.


##Setup on Ubuntu 14.0.4 LTS
Follow Django on GAE tutorial to setup Cloud SQL and proxy.

Clone the repo.

Configure database settings in env.yaml 

./install_deps

./manage.py migrate

./manage.py createsuperuser

./manage.py runserver

./manage.py collectstatic

gcloud app deploy
