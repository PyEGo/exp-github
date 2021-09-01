FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD GeneralNewsExtractor GeneralNewsExtractor
CMD cd GeneralNewsExtractor && python test.py
