FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD plotman plotman
RUN cd plotman & pip install . --no-deps
CMD plotman -h
