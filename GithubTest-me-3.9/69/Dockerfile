FROM python:3.9
ADD WeblogicScan WeblogicScan
RUN ["pip","install","OpsletsEc2"]
RUN ["pip","install","gdctools"]
CMD cd WeblogicScan && python WeblogicScan.py -u 127.0.0.1 -p 7001

