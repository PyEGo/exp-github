FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install urllib3==1.26.2
RUN pip install requests==2.25.0
RUN pip install flask==1.1.2
ADD SSRFmap SSRFmap
# add CMD command to run your programs here
CMD cd SSRFmap && python ssrfmap.py -r data/request.txt -p url -m readfiles,portscan
