FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libquadmath0 -y
RUN apt-get install procps -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.19.4
RUN pip install pandas==1.1.5
RUN pip install keras==2.4.3
RUN pip install scikit-learn==0.23.2
RUN pip install matplotlib==3.3.3
ADD mnssp3-EEG mnssp3-EEG
# add CMD command to run your programs here
CMD cd mnssp3-EEG/EEG/EpilepsyDetection/Python/EEG && python predict.py
