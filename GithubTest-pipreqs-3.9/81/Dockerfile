FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD sparse_attention sparse_attention
CMD cd sparse_attention && python attention.py
