FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD ECommerceCrawlers-TouTiao ECommerceCrawlers-TouTiao
CMD cd ECommerceCrawlers-TouTiao/TouTiao && python toutiao.py
