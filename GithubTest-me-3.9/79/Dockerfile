FROM python:3.9
ADD flops-counter.pytorch flops-counter.pytorch
RUN pip install torchvision
CMD cd flops-counter.pytorch && python test.py

