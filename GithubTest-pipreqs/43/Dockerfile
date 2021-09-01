FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD xxh xxh
RUN cd xxh && pip install . --no-deps
CMD xxh -h
