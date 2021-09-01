FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD doge doge
RUN cd doge && pip install . --no-deps
CMD doge
