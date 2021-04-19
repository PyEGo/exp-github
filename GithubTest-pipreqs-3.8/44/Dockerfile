FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD apistar apistar
RUN cd apistar && pip install . --no-deps
CMD cd apistar/mytest && apistar validate
