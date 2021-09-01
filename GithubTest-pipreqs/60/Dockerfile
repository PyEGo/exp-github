FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD galaxy-integrations-python-api galaxy-integrations-python-api
CMD cd galaxy-integrations-python-api/src && python test.py
