FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install colorama==0.4.4
RUN pip install logzero==1.7.0
ADD logzero logzero
# add CMD command to run your programs here
CMD cd logzero && python test.py
