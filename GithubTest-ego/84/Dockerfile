FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install libssl-dev -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pyopenssl==20.0.1
RUN pip install impacket==0.9.22
ADD BlueKeep BlueKeep
# add CMD command to run your programs here
CMD cd BlueKeep && python bluekeep_dos.py -i 127.0.0.1
