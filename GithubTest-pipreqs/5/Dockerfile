FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD Python-crawler-tutorial-starts-from-zero Python-crawler-tutorial-starts-from-zero
CMD python Python-crawler-tutorial-starts-from-zero/code_demo/Tieba.py
