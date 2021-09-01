FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD WeblogicScan WeblogicScan
CMD cd WeblogicScan && python WeblogicScan.py -u 127.0.0.1 -p 7001
