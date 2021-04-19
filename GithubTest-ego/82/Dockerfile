FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.19.4
RUN pip install torch==1.7.1
RUN pip install torchvision==0.8.2
ADD micronet micronet
# add CMD command to run your programs here
CMD cd micronet && python -c "import micronet; print(micronet.__version__)"
