FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD SuperGluePretrainedNetwork SuperGluePretrainedNetwork
CMD cd SuperGluePretrainedNetwork && python match_pairs.py
