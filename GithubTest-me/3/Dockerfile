FROM python:3.9-buster
ADD sktime sktime
RUN ["pip","install","numpy"]
CMD cd sktime && python test.py

