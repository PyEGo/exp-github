FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD facenet-pytorch facenet-pytorch
CMD cd facenet-pytorch && python test.py
