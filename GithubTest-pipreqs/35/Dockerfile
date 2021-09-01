FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD dirmap dirmap
CMD cd dirmap && python dirmap.py -i 192.168.1.1 -lcf
