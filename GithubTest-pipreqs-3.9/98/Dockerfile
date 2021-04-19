FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD jina jina
RUN pip install jina --no-deps
CMD jina hello-world
