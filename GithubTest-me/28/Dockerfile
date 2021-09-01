FROM python:3.9-buster
ADD logzero logzero 
RUN ["pip","install","requests"]
RUN ["pip","install","colorama"]
RUN ["pip","install","gunicorn"]
RUN ["pip","install","logzero"]
CMD cd logzero && python test.py

