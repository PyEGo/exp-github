FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install ca-certificates -y
RUN apt-get install jupyter-nbextension-jupyter-js-widgets -y
RUN apt-get install libblas3 -y
RUN apt-get install libffi-dev -y
RUN apt-get install liblapack3 -y
RUN apt-get install libssl-dev -y
RUN apt-get install libyaml-dev -y
RUN apt-get install libzmq5 -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install dill==0.3.3
RUN pip install pandas==1.2.4
RUN pip install ipython==7.23.1
RUN pip install ipywidgets==7.6.3
ADD pandarallel pandarallel
# add CMD command to run your programs here
CMD cd pandarallel && python test.py
