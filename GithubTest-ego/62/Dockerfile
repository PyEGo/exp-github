FROM debian:10
RUN apt-get clean
RUN apt-get update
RUN apt-get install python3 python3-pip -y
RUN cp /usr/bin/python3 /usr/bin/python
RUN cp /usr/bin/pip3 /usr/bin/pip
RUN apt-get update
RUN apt-get install libjs-jquery -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN apt-get install python3-flask-mail -y
RUN apt-get install python3-flask -y
RUN apt-get install python3-celery -y
RUN pip install flask==0.8.1
ADD flask-celery-example flask-celery-example
# add CMD command to run your programs here
CMD cd flask-celery-example && python app.py
