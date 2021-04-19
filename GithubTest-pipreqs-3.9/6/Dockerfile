FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD jd-assistant jd-assistant
CMD cd jd-assistant && python main.py
