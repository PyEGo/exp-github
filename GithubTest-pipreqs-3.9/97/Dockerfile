FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD mars mars
RUN pip install mars --no-deps
CMD cd mars/tests && python test.py
