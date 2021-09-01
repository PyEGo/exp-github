FROM python:3.8-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libblas3 -y
RUN apt-get install libc-ares2 -y
RUN apt-get install libffi-dev -y
RUN apt-get install libgfortran5 -y
RUN apt-get install libjs-jquery -y
RUN apt-get install liblapack3 -y
RUN apt-get install libprotobuf17 -y
RUN apt-get install libquadmath0 -y
RUN apt-get install libssl-dev -y
RUN apt-get install libssl1.1 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install six==1.16.0
RUN pip install numpy==1.18.5
RUN pip install keras-applications==1.0.8
RUN pip install scikit-image==0.18.0
RUN pip install tensorflow==2.3.1
ADD efficientnet efficientnet
RUN pip install keras
# add CMD command to run your programs here
CMD cd efficientnet && python test.py
