FROM python:3.8-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libprotobuf17 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install einops==0.3.0
RUN pip install tensorflow==2.4.0
RUN pip install torch==1.8.1
ADD lambda-networks lambda-networks
# add CMD command to run your programs here
CMD cd lambda-networks && python test.py
