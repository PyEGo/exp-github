FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install curl -y
RUN apt-get install git -y
RUN apt-get install libblas3 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libquadmath0 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.19.4
RUN pip install setuptools==51.0.0
RUN pip install jinja2==2.11.2
RUN pip install tqdm==4.54.1
RUN pip install scipy==1.5.4
RUN pip install pandas==1.1.5
RUN pip install matplotlib==3.3.3
RUN pip install ipython==7.19.0
ADD sweetviz sweetviz
RUN pip install pandas
# add CMD command to run your programs here
CMD cd sweetviz && python test.py
