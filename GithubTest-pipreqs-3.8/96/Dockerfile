FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD BERT-BiLSTM-CRF-NER BERT-BiLSTM-CRF-NER
RUN cd BERT-BiLSTM-CRF-NER && pip install . --no-deps
CMD bert-base-serving-start -help && bert-base-ner-train -help
