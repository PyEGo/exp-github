FROM python:3.9-buster
ADD bilibili-api bilibili-api
RUN ["pip","install","notifications-python-client"]
RUN ["pip","install","geoplot"]
RUN ["pip","install","veriloggen"]
RUN ["pip","install","requests"]
RUN ["pip","install","asyncio"]
CMD cd bilibili-api && python test.py
