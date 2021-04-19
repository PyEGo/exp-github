FROM python:3.8
ADD GeneralNewsExtractor GeneralNewsExtractor
RUN ["pip","install","geoplot"]
RUN ["pip","install","veriloggen"]
RUN ["pip","install","notifications-python-client"]
RUN ["pip","install","utils"]
CMD cd GeneralNewsExtractor && python test.py

