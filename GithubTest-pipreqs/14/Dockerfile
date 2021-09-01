FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD ASCII-generator ASCII-generator
CMD cd ASCII-generator && python img2img.py
