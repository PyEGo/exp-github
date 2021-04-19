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
RUN pip install pyyaml==5.3.1
RUN pip install schema==0.7.3
RUN pip install requests==2.25.0
RUN pip install beautifulsoup4==4.9.3
ADD policy_sentry policy_sentry
RUN cd policy_sentry && pip install . --no-deps
# add CMD command to run your programs here
CMD policy_sentry create-template --output-file crud.yml --template-type crud
