FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD OneForAll OneForAll
CMD cd OneForAll && python oneforall.py --target example.com run
