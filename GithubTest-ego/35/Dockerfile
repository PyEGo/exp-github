FROM python:3.9-buster
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
RUN pip install ipy==1.01
RUN pip install requests==2.25.0
RUN pip install gevent==21.1.2
RUN pip install progressbar2==3.53.1
ADD dirmap dirmap
# add CMD command to run your programs here
CMD cd dirmap && python dirmap.py -i 192.168.1.1 -lcf
