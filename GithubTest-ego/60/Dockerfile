FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install docutils-common -y
RUN apt-get install g++ -y
RUN apt-get install libjs-sphinxdoc -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install psutil==5.8.0
RUN pip install certifi==2020.12.5
RUN pip install galaxy-util==21.1.0
RUN pip install aiohttp==3.7.3
ADD galaxy-integrations-python-api galaxy-integrations-python-api
# add CMD command to run your programs here
CMD cd galaxy-integrations-python-api/src && python test.py
