FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install gfortran -y
RUN apt-get install git -y
RUN apt-get install libblas3 -y
RUN apt-get install libedit-dev -y
RUN apt-get install libgfortran5 -y
RUN apt-get install libgomp1 -y
RUN apt-get install libhdf5-dev -y
RUN apt-get install liblapack-dev -y
RUN apt-get install liblapack3 -y
RUN apt-get install libopenblas-dev -y
RUN apt-get install libquadmath0 -y
RUN apt-get install libtbb2 -y
RUN apt-get install pkg-config -y
RUN apt-get install wget -y
RUN apt-get install zlib1g-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install setuptools==51.0.0
RUN pip install numpy==1.19.4
RUN pip install scipy==1.5.4
RUN pip install numba==0.44.1
RUN pip install stumpy==1.6.1
ADD stumpy stumpy
# add CMD command to run your programs here
CMD cd stumpy && python test.py
