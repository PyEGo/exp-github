FROM python:3.9-buster
ADD flask-celery-example flask-celery-example
RUN ["apt-get","update"]
RUN ["pip","install","Flask"]
RUN ["pip","install","celery"]
RUN ["pip","install","Jinja2"]
RUN ["apt-get","install","-y","python-pip"]
RUN ["apt-get","install","-y","python-dev"]
RUN ["pip","install","requests"]
RUN ["pip","install","Flask-Login"]
RUN ["pip","install","Flask-SQLAlchemy"]
RUN ["pip","install","Flask-WTF"]
RUN ["pip","install","Flask-Mail"]
CMD cd flask-celery-example && python app.py

