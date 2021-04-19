FROM debian:10
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install python3 python3-pip -y
RUN cp /usr/bin/python3 /usr/bin/python
RUN cp /usr/bin/pip3 /usr/bin/pip
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN apt-get install python3-requests-toolbelt -y
RUN apt-get install python3-qrcode -y
RUN apt-get install python3-requests -y
RUN apt-get install python3-rsa -y
RUN apt-get install python3-crypto -y
RUN pip install pyexecjs==1.5.1
ADD DecryptLogin DecryptLogin
# add CMD command to run your programs here
CMD cd DecryptLogin && python test.py
