FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD efficientnet efficientnet
RUN pip install keras
CMD cd efficientnet && python test.py
