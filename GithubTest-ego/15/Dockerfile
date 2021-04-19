FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install apt-utils -y
RUN apt-get install build-essential -y
RUN apt-get install ca-certificates -y
RUN apt-get install curl -y
RUN apt-get install g++ -y
RUN apt-get install git -y
RUN apt-get install less -y
RUN apt-get install libblas3 -y
RUN apt-get install libbz2-dev -y
RUN apt-get install liblapack3 -y
RUN apt-get install libprotobuf17 -y
RUN apt-get install libreadline-dev -y
RUN apt-get install libsqlite3-dev -y
RUN apt-get install libssl-dev -y
RUN apt-get install nano -y
RUN apt-get install net-tools -y
RUN apt-get install netcat -y
RUN apt-get install nmap -y
RUN apt-get install openssh-client -y
RUN apt-get install telnet -y
RUN apt-get install tk-dev -y
RUN apt-get install vim -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.19.4
RUN pip install setuptools==51.0.0
RUN pip install pyspark==3.0.1
RUN pip install py4j==0.10.9.1
RUN pip install pyarrow==2.0.0
RUN pip install plotly==4.14.1
RUN pip install matplotlib==3.2.2
RUN pip install pandas==1.1.5
RUN pip install koalas==1.5.0
RUN pip install ipython==7.19.0
RUN pip install mlflow==1.12.1
RUN pip install pytest==6.2.1
ADD koalas koalas
# add CMD command to run your programs here
CMD cd koalas && python test.py
