FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD pytorch-openai-transformer-lm pytorch-openai-transformer-lm
CMD cd pytorch-openai-transformer-lm && python test.py
