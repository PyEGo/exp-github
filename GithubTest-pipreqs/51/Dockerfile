FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD weakfilescan weakfilescan
CMD cd weakfilescan && python wyspider.py 133.133.133.47:8000
