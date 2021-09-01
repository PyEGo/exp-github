FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD nba_api nba_api
CMD cd nba_api && python test.py
