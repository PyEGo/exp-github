FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip install mars --no-deps
ADD mars mars
CMD cd mars/tests && python test.py
