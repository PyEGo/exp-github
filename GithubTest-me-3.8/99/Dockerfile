FROM python:3.8
ADD starlette starlette
RUN ["pip","install","requests"]
RUN ["pip","install","six"]
RUN ["pip","install","typing"]
CMD cd starlette && python test.py
