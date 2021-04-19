FROM python:3.8
ADD ECommerceCrawlers-TouTiao ECommerceCrawlers-TouTiao
RUN ["apt-get","update"]
RUN ["pip","install","pan-python"]
RUN ["pip","install","pandacan"]
RUN ["pip","install","requests"]
RUN ["apt-get","install","-y","git"]
RUN ["apt-get","install","-y","build-essential"]
RUN ["apt-get","install","-y","curl"]
RUN ["apt-get","install","-y","bzip2"]
RUN ["pip","install","versioneer"]
RUN ["pip","install","fake-useragent"]
RUN ["pip","install","pandas"]
RUN ["pip","install","selenium"]
RUN ["pip","install","url"]
RUN ["pip","install","lxml"]
CMD cd ECommerceCrawlers-TouTiao/TouTiao && python toutiao.py

