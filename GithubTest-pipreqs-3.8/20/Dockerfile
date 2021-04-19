FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD RAdam RAdam
CMD cd RAdam && python test.py
