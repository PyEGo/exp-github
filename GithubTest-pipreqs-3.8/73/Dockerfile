FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN cd archivy && pip install . --no-deps
ADD archivy archivy
CMD archivy --help
