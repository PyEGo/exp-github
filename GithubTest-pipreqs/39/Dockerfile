FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD babel babel
RUN python setup.py import_cldr
CMD cd babel && python test.py
