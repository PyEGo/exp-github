FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD newscatcher newscatcher
CMD cd newscatcher && python test.py
