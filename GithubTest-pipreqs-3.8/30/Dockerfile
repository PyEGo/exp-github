FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD GeneralNewsExtractor GeneralNewsExtractor
CMD cd GeneralNewsExtractor && python test.py
