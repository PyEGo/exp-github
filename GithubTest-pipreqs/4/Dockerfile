FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD scalene scalene
RUN cd scalene && pip install . --no-deps
CMD scalene test/testme.py
