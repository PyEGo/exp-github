FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD sentry-python sentry-python
CMD cd sentry-python && python test.py
