FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libxml2 -y
RUN apt-get install libxslt1.1 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install lxml==4.6.2
RUN pip install pyyaml==5.3.1
RUN pip install numpy==1.19.4
ADD GeneralNewsExtractor GeneralNewsExtractor
# add CMD command to run your programs here
CMD cd GeneralNewsExtractor && python test.py
