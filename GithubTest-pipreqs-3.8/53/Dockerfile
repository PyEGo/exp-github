FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD finetune-transformer-lm finetune-transformer-lm
CMD cd finetune-transformer-lm && python train.py
