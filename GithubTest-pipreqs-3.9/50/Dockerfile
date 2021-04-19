FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD lambda-networks lambda-networks
CMD cd lambda-networks && python test.py
