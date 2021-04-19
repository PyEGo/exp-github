FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN apt-get install libxml2 -y
RUN apt-get install libxslt1.1 -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install lxml==4.5.2
RUN pip install requests==2.25.0
RUN pip install scrapy==2.4.1
ADD ECommerceCrawlers-East_money ECommerceCrawlers-East_money
# add CMD command to run your programs here
CMD cd ECommerceCrawlers-East_money/East_money && python main.py
