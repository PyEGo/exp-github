FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libxml2 -y
RUN apt-get install libxslt1.1 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pyyaml==5.4.1
RUN pip install numpy==1.20.3
RUN pip install lxml==4.6.2
ADD GeneralNewsExtractor GeneralNewsExtractor
# add CMD command to run your programs here
CMD cd GeneralNewsExtractor && python test.py
