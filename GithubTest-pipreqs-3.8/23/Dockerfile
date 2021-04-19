FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD vit-pytorch vit-pytorch
CMD cd vit-pytorch && python test.py
