FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD dirsearch dirsearch
CMD cd dirsearch && python dirsearch.py http://www.watchman-pypi.com
