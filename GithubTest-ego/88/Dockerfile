FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install curl -y
RUN apt-get install git -y
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install tqdm==4.60.0
RUN pip install numpy==1.16.6
RUN pip install attrdict==2.0.1
RUN pip install python-dateutil==2.8.1
RUN pip install convertdate==2.3.0
RUN pip install pandas==1.2.4
RUN pip install holidays==0.11.1
RUN pip install matplotlib==3.4.2
RUN pip install torch==1.8.1
RUN pip install livelossplot==0.5.3
ADD neural_prophet neural_prophet
# add CMD command to run your programs here
CMD cd neural_prophet && python test.py
