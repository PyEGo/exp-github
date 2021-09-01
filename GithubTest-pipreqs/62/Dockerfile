FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD flask-celery-example flask-celery-example
CMD cd flask-celery-example && python app.py
