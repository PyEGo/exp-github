FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD DXY-COVID-19-Crawler DXY-COVID-19-Crawler
CMD cd DXY-COVID-19-Crawler && python main.py
