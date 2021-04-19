FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD gitGraber gitGraber
CMD cd gitGraber && python gitGraber.py -k keywordsfile.txt -q "yahoo.com" -s -m
