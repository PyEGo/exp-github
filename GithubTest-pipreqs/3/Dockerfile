FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD sktime sktime
CMD cd sktime && python test.py
