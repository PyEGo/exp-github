FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip install keras
ADD efficientnet efficientnet
CMD cd efficientnet && python test.py
