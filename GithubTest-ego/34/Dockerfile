FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.20.3
RUN pip install m2cgen==0.9.0
ADD m2cgen m2cgen
RUN pip install scikit-learn
# add CMD command to run your programs here
CMD cd m2cgen && python test.py
