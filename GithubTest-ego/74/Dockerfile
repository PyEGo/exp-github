FROM python:3.8-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libprotobuf17 -y
RUN apt-get install libquadmath0 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.20.3
RUN pip install networkx==2.5
RUN pip install scipy==1.6.3
RUN pip install tensorflow==2.4.0
ADD gcn gcn
# add CMD command to run your programs here
CMD cd gcn && python train.py
