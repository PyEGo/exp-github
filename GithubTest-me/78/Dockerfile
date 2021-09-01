FROM python:3.9-buster
ADD kaldi-gstreamer-server kaldi-gstreamer-server
RUN ["pip","install","deco"]
RUN ["pip","install","ws4py"]
RUN ["pip","install","tornado"]
RUN ["pip","install","futures"]
RUN ["pip","install","logging-config"]
RUN ["pip","install","decoder"]
RUN ["pip","install","androidviewclient"]
RUN ["pip","install","common"]
CMD cd kaldi-gstreamer-server && python kaldigstserver/master_server.py --port=8888

