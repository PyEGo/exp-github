FROM python:3.9-buster
ADD starlette starlette
RUN ["pip","install","requests"]
RUN ["pip","install","six"]
RUN ["pip","install","typing"]
CMD cd starlette && python test.py
