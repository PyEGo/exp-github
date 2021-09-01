FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install feedparser==6.0.2
RUN pip install setuptools==56.2.0
RUN pip install tldextract==3.1.0
ADD newscatcher newscatcher
# add CMD command to run your programs here
CMD cd newscatcher && python test.py
