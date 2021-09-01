FROM python:3.9-buster
ADD path path
RUN ["pip","install","pyte"]
RUN ["pip","install","six"]
RUN ["pip","install","pytest"]
RUN ["pip","install","py"]
RUN ["pip","install","path.py"]
RUN ["pip","install","path"]
CMD cd path && python test.py
