FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install flask==1.1.2
ADD 30-Days-Of-Python 30-Days-Of-Python
# add CMD command to run your programs here
CMD cd 30-Days-Of-Python/python_for_web && python app.py
