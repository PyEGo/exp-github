FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD flops-counter.pytorch flops-counter.pytorch
RUN pip install torchvision
CMD cd flops-counter.pytorch && python test.py
