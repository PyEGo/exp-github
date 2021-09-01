FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libjs-jquery -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install werkzeug==1.0.1
RUN pip install flask==0.8.1
ADD Flask-HTTPAuth Flask-HTTPAuth
# add CMD command to run your programs here
CMD cd Flask-HTTPAuth/src && python test.py
