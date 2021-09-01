FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pyyaml==5.4.1
RUN pip install beautifulsoup4==4.9.3
RUN pip install aiohttp==3.7.3
ADD bilibili-api bilibili-api
# add CMD command to run your programs here
CMD cd bilibili-api && python test.py
