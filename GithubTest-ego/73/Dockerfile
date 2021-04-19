FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install git -y
RUN apt-get install libjs-jquery -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install appdirs==1.4.4
RUN pip install wtforms==2.3.3
RUN pip install html2text==2020.1.16
RUN pip install attrs==20.2.0
RUN pip install setuptools==51.0.0
RUN pip install jinja2==2.11.2
RUN pip install werkzeug==1.0.1
RUN pip install tinydb==4.3.0
RUN pip install click==7.1.2
RUN pip install pyyaml==5.3.1
RUN pip install flask-login==0.5.0
RUN pip install python-frontmatter==0.5.0
RUN pip install flask==1.1.2
RUN pip install elasticsearch==7.10.1
RUN pip install flask-wtf==0.14.3
RUN pip install click-plugins==1.1.1
RUN pip install validators==0.15.0
RUN pip install requests==2.24.0
RUN pip install beautifulsoup4==4.9.3
RUN pip install flask-compress==1.8.0
RUN pip install archivy==1.1.1
ADD archivy archivy
RUN cd archivy && pip install . --no-deps
# add CMD command to run your programs here
CMD archivy --help
