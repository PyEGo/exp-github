FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install libbz2-dev -y
RUN apt-get install libreadline-dev -y
RUN apt-get install libsqlite3-dev -y
RUN apt-get install libssl-dev -y
RUN apt-get install tk-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pyfakefs==4.4.0
RUN pip install marshmallow==3.12.1
RUN pip install pyyaml==5.4.1
RUN pip install appdirs==1.4.4
RUN pip install psutil==5.8.0
RUN pip install texttable==1.6.3
RUN pip install click==7.1.2
RUN pip install setuptools==56.2.0
RUN pip install attrs==21.2.0
RUN pip install packaging==20.9
RUN pip install typing-extensions==3.10.0.0
RUN pip install pendulum==2.1.2
RUN pip install pytest==6.2.1
ADD plotman plotman
RUN cd plotman & pip install . --no-deps
# add CMD command to run your programs here
CMD plotman -h
