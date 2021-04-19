FROM debian:10
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install python3 python3-pip -y
RUN cp /usr/bin/python3 /usr/bin/python
RUN cp /usr/bin/pip3 /usr/bin/pip
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libmaxminddb0 -y
RUN apt-get install libssl-dev -y
RUN apt-get install libxml2 -y
RUN apt-get install libxslt1.1 -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN apt-get install python3-nmap -y
RUN apt-get install python3-dnspython -y
RUN apt-get install python3-openssl -y
RUN apt-get install python3-lxml -y
RUN apt-get install python3-tldextract -y
RUN apt-get install python3-aiohttp -y
RUN apt-get install python3-pymongo -y
RUN apt-get install python3-socks -y
RUN apt-get install python3-uvloop -y
RUN apt-get install python3-pyfiglet -y
RUN apt-get install python3-requests -y
RUN apt-get install python3-bs4 -y
RUN apt-get install python3-chardet -y
RUN apt-get install python3-geoip2 -y
RUN apt-get install python3-urllib3 -y
RUN pip install fake-useragent==0.1.11
RUN pip install dnsdiag==1.4.3
RUN pip install lxml==4.5.2
RUN pip install geoip2==4.1.0
ADD Vxscan Vxscan
# add CMD command to run your programs here
CMD cd Vxscan && python Vxscan.py -i 127.0.0.0/24
