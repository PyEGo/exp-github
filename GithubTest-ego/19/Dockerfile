FROM python:2.7-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
ADD w9scan w9scan
# add CMD command to run your programs here
CMD cd w9scan && python w9scan.py -u "https://x.hacking8.com"
