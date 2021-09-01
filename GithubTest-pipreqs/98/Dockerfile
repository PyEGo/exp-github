FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD peru peru
RUN cd peru && pip install . --no-deps
CMD cd peru && peru sync
