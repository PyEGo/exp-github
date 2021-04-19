FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD petastorm petastorm
CMD cd petastorm && python test.py
