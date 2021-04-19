FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install ca-certificates -y
RUN apt-get install curl -y
RUN apt-get install fonts-font-awesome -y
RUN apt-get install git -y
RUN apt-get install libblas3 -y
RUN apt-get install libffi-dev -y
RUN apt-get install libjs-backbone -y
RUN apt-get install libjs-bootstrap -y
RUN apt-get install libjs-bootstrap-tour -y
RUN apt-get install libjs-codemirror -y
RUN apt-get install libjs-es6-promise -y
RUN apt-get install libjs-jed -y
RUN apt-get install libjs-jquery -y
RUN apt-get install libjs-jquery-typeahead -y
RUN apt-get install libjs-jquery-ui -y
RUN apt-get install libjs-marked -y
RUN apt-get install libjs-mathjax -y
RUN apt-get install libjs-moment -y
RUN apt-get install libjs-requirejs -y
RUN apt-get install libjs-requirejs-text -y
RUN apt-get install libjs-term.js -y
RUN apt-get install libjs-text-encoding -y
RUN apt-get install libjs-underscore -y
RUN apt-get install liblapack3 -y
RUN apt-get install libssl-dev -y
RUN apt-get install libyaml-dev -y
RUN apt-get install libzmq5 -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install tqdm==4.54.1
RUN pip install numpy==1.19.4
RUN pip install attrdict==2.0.1
RUN pip install convertdate==2.3.0
RUN pip install python-dateutil==2.8.1
RUN pip install torch==1.7.1
RUN pip install matplotlib==3.3.3
RUN pip install holidays==0.9.12
RUN pip install pandas==1.1.5
RUN pip install livelossplot==0.4.2
ADD neural_prophet neural_prophet
# add CMD command to run your programs here
CMD cd neural_prophet && python test.py
