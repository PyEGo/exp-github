FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD pytorch-meta pytorch-meta
CMD cd pytorch-meta && python test.py
