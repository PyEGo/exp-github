FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install scapy==2.4.4
RUN pip install netifaces==0.10.9
RUN pip install twisted==21.2.0
ADD mitm6 mitm6
RUN cd mitm6 && pip install . --no-deps
# add CMD command to run your programs here
CMD mitm6 -h
