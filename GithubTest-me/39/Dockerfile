FROM python:3.9-buster
ADD babel babel
RUN ["pip","install","requests"]
RUN ["pip","install","Babel"]
RUN ["pip","install","six"]
RUN ["pip","install","pytest"]
RUN ["pip","install","py"]
RUN ["pip","install","pytz"]
RUN ["pip","install","babel_util"]
CMD cd babel && python test.py

