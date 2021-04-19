FROM python:3.8
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libprotobuf17 -y
RUN apt-get install libquadmath0 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install six==1.15.0
RUN pip install numpy==1.19.4
RUN pip install tensorflow==2.4.0
RUN pip install keras-applications==1.0.8
RUN pip install scikit-image==0.18.0
ADD efficientnet efficientnet
RUN pip install keras
# add CMD command to run your programs here
CMD cd efficientnet && python test.py
