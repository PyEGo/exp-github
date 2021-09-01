FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install setuptools==56.2.0
RUN pip install einops==0.3.0
RUN pip install torch==1.8.1
ADD vit-pytorch vit-pytorch
# add CMD command to run your programs here
CMD cd vit-pytorch && python test.py
