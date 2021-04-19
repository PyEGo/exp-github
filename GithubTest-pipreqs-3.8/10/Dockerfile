FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD DeepLearning DeepLearning
CMD cd DeepLearning/code && python chapter7.py
