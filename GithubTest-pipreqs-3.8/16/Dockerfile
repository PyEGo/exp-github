FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD kb kb
RUN cd kb && pip install . --no-deps
CMD kb list
