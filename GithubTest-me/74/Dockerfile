FROM python:3.9-buster
ADD gcn gcn
RUN ["pip","install","networkx"]
RUN ["pip","install","numpy"]
RUN ["pip","install","scipy"]
RUN ["pip","install","tensorflow"]
CMD cd gcn && python train.py
