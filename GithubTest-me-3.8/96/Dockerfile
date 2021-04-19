FROM python:3.8
ADD BERT-BiLSTM-CRF-NER BERT-BiLSTM-CRF-NER
RUN ["pip","install","be"]
RUN ["pip","install","bert"]
RUN ["pip","install","tensorflow"]
RUN ["pip","install","numpy"]
RUN cd BERT-BiLSTM-CRF-NER && pip install . --no-deps
CMD bert-base-serving-start -help && bert-base-ner-train -help

