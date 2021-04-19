FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD machine_learning_examples machine_learning_examples
CMD cd machine_learning_examples/airline && python rnn.py
