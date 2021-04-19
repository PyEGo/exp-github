FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD 30-Days-Of-Python 30-Days-Of-Python
CMD cd 30-Days-Of-Python/python_for_web && python app.py
