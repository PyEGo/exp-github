FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pygments==2.7.3
RUN pip install executing==0.5.3
RUN pip install flask==1.1.2
ADD heartrate heartrate
# add CMD command to run your programs here
CMD cd heartrate && python test.py
