FROM python:3.9
ADD neural_prophet neural_prophet
RUN ["pip","install","pandacan"]
RUN ["pip","install","geoplot"]
RUN ["pip","install","pan-python"]
RUN ["pip","install","convertdate"]
RUN ["pip","install","python-dateutil"]
RUN ["pip","install","notifications-python-client"]
RUN ["pip","install","holidays"]
RUN ["pip","install","neural-fmri"]
RUN ["pip","install","LunarCalendar"]
RUN ["pip","install","forecaster"]
RUN ["pip","install","torch"]
RUN ["pip","install","veriloggen"]
RUN ["pip","install","numpy"]
RUN ["pip","install","matplotlib"]
RUN ["pip","install","utils"]
RUN ["pip","install","pandas"]
RUN ["pip","install","neuralprophet"]
CMD cd neural_prophet && python test.py

