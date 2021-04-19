FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip install torchvision
ADD flops-counter.pytorch flops-counter.pytorch
CMD cd flops-counter.pytorch && python test.py
