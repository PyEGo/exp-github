FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD pke pke
RUN python -m nltk.downloader stopwords && python -m nltk.downloader universal_tagset && python -m spacy download en
CMD cd pke && python test.py
