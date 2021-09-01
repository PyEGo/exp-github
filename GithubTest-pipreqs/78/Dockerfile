FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD kaldi-gstreamer-server kaldi-gstreamer-server
CMD cd kaldi-gstreamer-server && python kaldigstserver/master_server.py --port=8888
