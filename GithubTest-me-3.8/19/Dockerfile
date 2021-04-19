FROM python:3.8
ADD ECommerceCrawlers-East_money ECommerceCrawlers-East_money
RUN ["apt-get","update"]
RUN ["apt-get","install","-y","python-pip"]
RUN ["apt-get","install","-y","python-dev"]
RUN ["apt-get","install","-y","libssl-dev"]
RUN ["apt-get","install","-y","libffi-dev"]
RUN ["pip","install","service_identity"]
RUN ["pip","install","Scrapy"]
CMD cd ECommerceCrawlers-East_money/East_money && python main.py
