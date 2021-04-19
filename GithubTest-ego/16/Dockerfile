FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install libjs-jquery -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install werkzeug==1.0.1
RUN pip install markupsafe==1.1.1
RUN pip install attrs==20.3.0
RUN pip install colored==1.4.2
RUN pip install toml==0.10.2
RUN pip install flask==1.1.2
ADD kb kb
RUN cd kb && pip install . --no-deps
# add CMD command to run your programs here
CMD kb list
