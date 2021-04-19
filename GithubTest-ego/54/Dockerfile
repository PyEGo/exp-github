FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install feedparser==6.0.2
ADD data-science-blogs data-science-blogs
# add CMD command to run your programs here
CMD cd data-science-blogs && python generate_opml.py && python frequency.py
