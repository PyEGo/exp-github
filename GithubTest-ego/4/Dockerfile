FROM python:3.6-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install cloudpickle==1.6.0
RUN pip install rich==10.1.0
ADD scalene scalene
RUN cd scalene && pip install . --no-deps
# add CMD command to run your programs here
CMD scalene test/testme.py
