FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libyara3 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install yara-python==4.1.0
RUN pip install setuptools==56.2.0
ADD GScan GScan
# add CMD command to run your programs here
CMD cd GScan && python GScan.py
