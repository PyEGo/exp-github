FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD noisy noisy
CMD cd noisy && python noisy.py --config config.json
