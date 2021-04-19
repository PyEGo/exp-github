FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install click==7.1.2
RUN pip install typesystem==0.2.4
RUN pip install jinja2==2.11.2
RUN pip install pygments==2.7.3
RUN pip install requests==2.25.0
ADD apistar apistar
RUN cd apistar && pip install . --no-deps
# add CMD command to run your programs here
CMD cd apistar/mytest && apistar validate
