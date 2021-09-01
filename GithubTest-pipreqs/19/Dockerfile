FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD w9scan w9scan
CMD cd w9scan && python w9scan.py -u "https://x.hacking8.com"
