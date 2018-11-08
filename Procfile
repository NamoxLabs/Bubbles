release: python manage.py migrate --no-input
web: uwsgi bubbles/wsgi/uwsgi.ini
celeryworker: celery worker -A bubbles.celeryconf:app --loglevel=info -E