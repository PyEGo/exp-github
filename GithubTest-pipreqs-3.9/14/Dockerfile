FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD Summer2021-Internships Summer2021-Internships
CMD python Summer2021-Internships/sync.py
