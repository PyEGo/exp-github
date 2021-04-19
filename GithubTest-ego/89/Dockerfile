FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install astunparse==1.6.3
ADD pyp pyp
RUN cd pyp && pip install . --no-deps
# add CMD command to run your programs here
CMD ps x | pyp 'line.split()[4]'
