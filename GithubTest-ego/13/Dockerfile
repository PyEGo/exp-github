FROM debian:10
RUN apt-get clean
RUN apt-get update
RUN apt-get install python3 python3-pip -y
RUN cp /usr/bin/python3 /usr/bin/python
RUN cp /usr/bin/pip3 /usr/bin/pip
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libxml2 -y
RUN apt-get install libxslt1.1 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN apt-get install python3-urllib3 -y
RUN apt-get install python3-lxml -y
RUN apt-get install python3-decorator -y
RUN apt-get install python3-pil -y
RUN apt-get install python3-tabulate -y
RUN apt-get install python3-requests -y
RUN apt-get install python3-demjson -y
RUN apt-get install python3-numpy -y
RUN apt-get install python3-appdirs -y
RUN apt-get install python3-tqdm -y
RUN apt-get install python3-matplotlib -y
RUN apt-get install python3-bs4 -y
RUN apt-get install python3-pandas -y
RUN apt-get install python3-websocket -y
RUN pip install py-mini-racer==0.6.0
RUN pip install lxml==4.6.2
RUN pip install pypinyin==0.41.0
RUN pip install pandas==1.2.4
ADD akshare akshare
# add CMD command to run your programs here
CMD cd akshare && python test.py
