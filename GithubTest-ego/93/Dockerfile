FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN apt-get install libxml2 -y
RUN apt-get install libxslt1.1 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install tqdm==4.60.0
RUN pip install urllib3==1.26.2
RUN pip install python-docx==0.8.10
RUN pip install requests==2.25.0
RUN pip install beautifulsoup4==4.9.3
ADD Packer-Fuzzer Packer-Fuzzer
# add CMD command to run your programs here
CMD cd Packer-Fuzzer && python PackerFuzzer.py -u http://133.133.133.47:8000
