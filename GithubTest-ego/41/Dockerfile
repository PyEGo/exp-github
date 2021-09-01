FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install setuptools==56.2.0
ADD dongbei dongbei
# add CMD command to run your programs here
CMD cd dongbei && test/dongbei_test.py
