FROM python:2.7
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD machine_learning_examples machine_learning_example
CMD cd machine_learning_examples/airline/ && python rnn.py
