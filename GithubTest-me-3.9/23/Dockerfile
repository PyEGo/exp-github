FROM python:3.9
ADD vit-pytorch vit-pytorch
RUN ["pip","install","torch"]
RUN ["pip","install","vit-pytorch"]
CMD cd vit-pytorch && python test.py

