FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install jinja2==2.11.2
RUN pip install pyyaml==5.4.1
RUN pip install aiofiles==0.6.0
RUN pip install itsdangerous==1.1.0
RUN pip install starlette==0.14.1
RUN pip install graphene==2.1.8
ADD starlette starlette
# add CMD command to run your programs here
CMD cd starlette && python test.py
