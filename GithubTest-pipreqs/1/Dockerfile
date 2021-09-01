FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD metaflow metaflow
CMD cd metaflow && python test.py
