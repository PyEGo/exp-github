FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD ECommerceCrawlers-East_money ECommerceCrawlers-East_money
CMD cd ECommerceCrawlers-East_money/East_money && python main.py
