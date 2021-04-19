FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libffi-dev -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install markdown2==2.3.10
RUN pip install beautifulsoup4==4.9.3
RUN pip install gspread==3.6.0
ADD Summer2021-Internships Summer2021-Internships
# add CMD command to run your programs here
CMD python Summer2021-Internships/sync.py
