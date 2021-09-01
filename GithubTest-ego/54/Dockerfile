FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install libgeos-c1v5 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libquadmath0 -y
RUN apt-get install procps -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.20.3
RUN pip install shapely==1.7.1
RUN pip install tqdm==4.60.0
RUN pip install scipy==1.6.3
RUN pip install matplotlib==3.4.2
RUN pip install scikit-learn==0.24.2
RUN pip install seaborn==0.11.0
ADD uncertainty-toolbox uncertainty-toolbox
# add CMD command to run your programs here
CMD cd uncertainty-toolbox && python test.py
