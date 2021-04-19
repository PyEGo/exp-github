FROM python:3.9
ADD pytorch-meta pytorch-meta
RUN ["pip","install","torchmeta"]
CMD cd pytorch-meta && python test.py
