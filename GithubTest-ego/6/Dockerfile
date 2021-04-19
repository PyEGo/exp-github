FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pycryptodome==3.9.9
RUN pip install requests==2.25.0
RUN pip install beautifulsoup4==4.9.3
ADD jd-assistant jd-assistant
# add CMD command to run your programs here
CMD cd jd-assistant && python main.py
