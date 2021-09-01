FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD GitHub520 GitHub520
CMD cd GitHub520 && python fetch_ips.py
