FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install setuptools==51.0.0
RUN pip install packaging==20.8
RUN pip install argcomplete==1.12.2
ADD pipx pipx
RUN cd pipx && pip install . --no-deps
# add CMD command to run your programs here
CMD pipx completions
