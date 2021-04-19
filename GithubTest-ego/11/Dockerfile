FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install bind9utils -y
RUN apt-get install ca-certificates -y
RUN apt-get install curl -y
RUN apt-get install dbus-x11 -y
RUN apt-get install ffmpeg -y
RUN apt-get install g++ -y
RUN apt-get install imagemagick -y
RUN apt-get install kmod -y
RUN apt-get install libjpeg-dev -y
RUN apt-get install libssl-dev -y
RUN apt-get install net-tools -y
RUN apt-get install nodejs -y
RUN apt-get install psmisc -y
RUN apt-get install software-properties-common -y
RUN apt-get install sudo -y
RUN apt-get install tcpdump -y
RUN apt-get install traceroute -y
RUN apt-get install wget -y
RUN apt-get install xvfb -y
RUN apt-get install zlib1g-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install tqdm==4.54.1
RUN pip install dnspython==2.0.0
RUN pip install idna==2.10
RUN pip install exrex==0.10.5
RUN pip install sqlalchemy==1.3.20
RUN pip install dnsdiag==1.4.3
RUN pip install tenacity==6.3.0
RUN pip install fire==0.3.1
RUN pip install requests==2.25.0
RUN pip install treelib==1.6.1
RUN pip install beautifulsoup4==4.9.3
RUN pip install loguru==0.5.3
ADD OneForAll OneForAll
# add CMD command to run your programs here
CMD cd OneForAll && python oneforall.py --target example.com run
