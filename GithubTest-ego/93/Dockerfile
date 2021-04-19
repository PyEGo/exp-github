FROM debian:10
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install python python-pip -y
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN apt-get install python-scipy -y
RUN apt-get install python-pyaudio -y
RUN pip install simpleaudio==1.0.4
ADD pydub pydub
# add CMD command to run your programs here
CMD cd pydub && python test.py
