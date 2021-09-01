FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD mitm6 mitm6
RUN cd mitm6 && pip install . --no-deps
CMD mitm6 -h
