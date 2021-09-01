FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pyyaml==5.4.1
RUN pip install pexpect==4.8.0
ADD xxh xxh
RUN cd xxh && pip install . --no-deps
# add CMD command to run your programs here
CMD xxh -h
