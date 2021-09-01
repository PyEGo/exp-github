FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD archivy archivy
RUN cd archivy && pip install . --no-deps
CMD archivy --help
