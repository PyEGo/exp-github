FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install libbz2-dev -y
RUN apt-get install libreadline-dev -y
RUN apt-get install libsqlite3-dev -y
RUN apt-get install libssl-dev -y
RUN apt-get install tk-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install hypothesis==1.18.1
RUN pip install typing-extensions==3.7.4.3
RUN pip install mypy==0.790
RUN pip install pytest==6.2.1
ADD returns returns
# add CMD command to run your programs here
CMD cd returns && python test.py
