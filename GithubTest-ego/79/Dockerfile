FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.20.3
RUN pip install torch==1.8.1
ADD flops-counter.pytorch flops-counter.pytorch
RUN pip install torchvision
# add CMD command to run your programs here
CMD cd flops-counter.pytorch && python test.py
