FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install requests==2.25.0
ADD Python-crawler-tutorial-starts-from-zero Python-crawler-tutorial-starts-from-zero
# add CMD command to run your programs here
CMD python Python-crawler-tutorial-starts-from-zero/code_demo/Tieba.py
