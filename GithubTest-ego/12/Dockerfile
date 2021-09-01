FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
ADD learn_math_fast learn_math_fast
# add CMD command to run your programs here
CMD cd learn_math_fast && python build_toc.py
