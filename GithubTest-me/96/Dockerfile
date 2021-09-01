FROM python:3.9-buster
ADD doge doge
RUN ["pip","install","doge"]
RUN cd doge && pip install . --no-deps
CMD doge
