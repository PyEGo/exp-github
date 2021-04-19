FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install docutils-common -y
RUN apt-get install libblas3 -y
RUN apt-get install libbz2-dev -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libquadmath0 -y
RUN apt-get install libreadline-dev -y
RUN apt-get install libsqlite3-dev -y
RUN apt-get install libssl-dev -y
RUN apt-get install procps -y
RUN apt-get install tk-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install six==1.15.0
RUN pip install numpy==1.19.4
RUN pip install scipy==1.5.4
RUN pip install networkx==2.5
RUN pip install pandas==1.1.5
RUN pip install python-louvain==0.14
RUN pip install scikit-learn==0.23.2
RUN pip install gensim==3.8.3
RUN pip install karateclub==1.0.23
ADD karateclub karateclub
RUN pip install networkx
# add CMD command to run your programs here
CMD cd karateclub && python test.py
