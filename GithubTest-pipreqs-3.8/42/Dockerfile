FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD returns returns
CMD cd returns && python test.py
