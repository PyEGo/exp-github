FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD django-vue-template django-vue-template
CMD cd django-vue-template && python manage.py runserver
