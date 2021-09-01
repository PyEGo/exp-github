FROM python:2.7-buster.13
ADD WeblogicScan WeblogicScan
RUN ["pip","install","gdctools"]
RUN ["pip","install","OpsletsEc2"]
CMD cd WeblogicScan && python WeblogicScan.py -u 127.0.0.1 -p 7001

