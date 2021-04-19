FROM python:3.8
ADD flops-counter.pytorch flops-counter.pytorch
RUN pip install torchvision
CMD cd flops-counter.pytorch && python test.py

