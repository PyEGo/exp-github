FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD neural_prophet neural_prophet
CMD cd neural_prophet && python test.py
