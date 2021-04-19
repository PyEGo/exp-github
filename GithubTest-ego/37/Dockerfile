FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install tqdm==4.54.1
RUN pip install numpy==1.19.4
RUN pip install requests==2.25.0
RUN pip install beautifulsoup4==4.9.3
RUN pip install pandas==1.1.5
ADD springer_free_books springer_free_books
# add CMD command to run your programs here
CMD cd springer_free_books && python main.py -i 2
