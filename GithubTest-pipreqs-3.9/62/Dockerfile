FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD mnssp3-EEG mnssp3-EEG
CMD cd mnssp3-EEG/EEG/EpilepsyDetection/Python/EEG && python predict.py
