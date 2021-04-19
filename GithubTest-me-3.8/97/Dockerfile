FROM python:3.8
ADD mars mars
RUN ["pip","install","configobj"]
RUN ["pip","install","notifications-python-client"]
RUN ["pip","install","gdctools"]
RUN ["pip","install","hyhyhy"]
RUN ["pip","install","geoplot"]
RUN ["pip","install","OpsletsEc2"]
RUN ["pip","install","veriloggen"]
RUN ["pip","install","psutil"]
RUN ["pip","install","actors"]
RUN ["pip","install","numpy"]
RUN ["pip","install","lib"]
RUN ["pip","install","config"]
RUN ["pip","install","utils"]
RUN pip install mars --no-deps
CMD cd mars/tests && python test.py

