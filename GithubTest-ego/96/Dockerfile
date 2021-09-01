FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
ADD doge doge
RUN cd doge && pip install . --no-deps
# add CMD command to run your programs here
CMD doge
