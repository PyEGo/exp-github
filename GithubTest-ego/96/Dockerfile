FROM python:3.8
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install libblas3 -y
RUN apt-get install libjs-sphinxdoc -y
RUN apt-get install liblapack3 -y
RUN apt-get install libprotobuf17 -y
RUN apt-get install libssl-dev -y
RUN apt-get install libzmq5 -y
RUN apt-get install sphinx-rtd-theme-common -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install setuptools==51.0.0
RUN pip install flask-cors==3.0.9
RUN pip install numpy==1.19.4
RUN pip install six==1.15.0
RUN pip install gputil==1.4.0
RUN pip install chumpy==0.66
RUN pip install termcolor==1.1.0
RUN pip install flask==1.1.2
RUN pip install tensorflow==2.4.0
RUN pip install pyzmq==20.0.0
RUN pip install flask-compress==1.8.0
ADD BERT-BiLSTM-CRF-NER BERT-BiLSTM-CRF-NER
RUN cd BERT-BiLSTM-CRF-NER && pip install . --no-deps
# add CMD command to run your programs here
CMD bert-base-serving-start -help && bert-base-ner-train -help
