FROM python:3.8
ADD pandarallel pandarallel
RUN ["pip","install","pandacan"]
RUN ["pip","install","pan-python"]
RUN ["pip","install","pandarallel"]
CMD cd pandarallel && python test.py

