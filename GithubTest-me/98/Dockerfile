FROM python:3.9-buster
ADD peru peru
RUN ["pip","install","requests"]
RUN ["pip","install","psycopg2"]
RUN ["pip","install","python-dateutil"]
RUN ["pip","install","pathlib"]
RUN ["pip","install","pytest"]
RUN ["pip","install","path.py"]
RUN ["pip","install","main"]
CMD cd peru && pip install . --no-deps

