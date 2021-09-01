FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pyyaml==5.4.1
RUN pip install docopt==0.6.2
ADD peru peru
RUN cd peru && pip install . --no-deps
# add CMD command to run your programs here
CMD cd peru && peru sync
