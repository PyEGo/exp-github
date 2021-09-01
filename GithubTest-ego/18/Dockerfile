FROM debian:10
RUN apt-get clean
RUN apt-get update
RUN apt-get install python3 python3-pip -y
RUN cp /usr/bin/python3 /usr/bin/python
RUN cp /usr/bin/pip3 /usr/bin/pip
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN apt-get install python3-crypto -y
RUN apt-get install python3-pil -y
RUN apt-get install python3-demjson -y
RUN apt-get install python3-requests -y
RUN apt-get install python3-numpy -y
RUN apt-get install python3-matplotlib -y
RUN apt-get install python3-bs4 -y
RUN apt-get install python3-progressbar -y
RUN apt-get install python3-pandas -y
RUN pip install pytesseract==0.3.7
ADD OpenData OpenData
# add CMD command to run your programs here
CMD cd OpenData && python test.py
