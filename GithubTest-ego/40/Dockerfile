FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
ADD coding-problems coding-problems
# add CMD command to run your programs here
CMD cd coding-problems/LinkedLists && python odd_even_ll.py
