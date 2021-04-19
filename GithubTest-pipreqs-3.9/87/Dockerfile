FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD blackhat-python3 blackhat-python3
CMD cd blackhat-python3/chapter04 && python pic_carver.py
