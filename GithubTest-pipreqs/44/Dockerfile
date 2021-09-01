FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD blind_watermark blind_watermark
CMD cd blind_watermark && python test.py
