FROM python:3.8
ADD heartrate
RUN ["pip","install","Flask"]
RUN ["pip","install","six"]
RUN ["pip","install","pytest"]
RUN ["pip","install","py"]
RUN ["pip","install","Pygments"]
RUN ["pip","install","heartrate"]
RUN ["pip","install","executing"]
CMD cd heartrate && python test.py

