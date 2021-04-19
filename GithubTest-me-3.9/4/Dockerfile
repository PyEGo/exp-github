FROM python:3.9
ADD scalene scalene
RUN ["pip","install","scalene"]
RUN cd scalene && pip install . --no-deps
CMD scalene test/testme.py

