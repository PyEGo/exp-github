FROM debian:10
RUN apt-get clean
RUN apt-get update
RUN apt-get install python3 python3-pip -y
RUN cp /usr/bin/python3 /usr/bin/python
RUN cp /usr/bin/pip3 /usr/bin/pip
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN apt-get install python3-munkres -y
RUN apt-get install python3-pil -y
RUN apt-get install python3-six -y
RUN apt-get install python3-pytest -y
RUN apt-get install python3-numpy -y
RUN apt-get install python3-requests -y
RUN apt-get install python3-tqdm -y
RUN apt-get install python3-pandas -y
RUN apt-get install python3-h5py -y
RUN pip install ordered-set==4.0.2
RUN pip install torch==1.8.1
RUN pip install torchvision==0.9.1
RUN pip install torchmeta==1.7.0
ADD pytorch-meta pytorch-meta
# add CMD command to run your programs here
CMD cd pytorch-meta && python test.py
