FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip install networkx
ADD karateclub karateclub
CMD cd karateclub && python test.py
