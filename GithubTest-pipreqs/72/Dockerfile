FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD karateclub karateclub
RUN pip install networkx
CMD cd karateclub && python test.py
