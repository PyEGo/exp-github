FROM python:3.8
ADD scalene scalene
RUN ["pip","install","scalene"]
RUN cd scalene && pip install . --no-deps
CMD scalene test/testme.py

