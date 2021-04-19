FROM python:2.7
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libquadmath0 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install ngram==3.3.2
RUN pip install numpy==1.16.6
RUN pip install python-levenshtein==0.12.0
RUN pip install pandas==0.22.0
RUN pip install scikit-learn==0.20.4
ADD mnssp3-DNA mnssp3-DNA
# add CMD command to run your programs here
CMD cd mnssp3-DNA/DNA/MotifFinding/Python/n-gram/simple && python test.py
