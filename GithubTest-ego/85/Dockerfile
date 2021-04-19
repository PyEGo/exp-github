FROM python:2.7
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pillow==6.0.0
RUN pip install jieba==0.42.1
RUN pip install requests==2.25.0
RUN pip install itchat==1.3.10
RUN pip install pyecharts==1.9.0
ADD wechat_friends wechat_friends
# add CMD command to run your programs here
CMD cd wechat_friends && python get_user_info.py
