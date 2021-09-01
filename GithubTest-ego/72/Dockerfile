FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libquadmath0 -y
RUN apt-get install procps -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install six==1.16.0
RUN pip install numpy==1.20.3
RUN pip install networkx==2.5
RUN pip install scipy==1.6.3
RUN pip install gensim==4.0.1
RUN pip install python-louvain==0.15
RUN pip install scikit-learn==0.24.2
RUN pip install pandas==1.2.4
RUN pip install karateclub==0.45.31
ADD karateclub karateclub
RUN pip install networkx
# add CMD command to run your programs here
CMD cd karateclub && python test.py
