FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD Flask-HTTPAuth Flask-HTTPAuth
CMD cd Flask-HTTPAuth/src && python test.py
