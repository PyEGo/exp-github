FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install dill==0.3.3
ADD latexify_py latexify_py
# add CMD command to run your programs here
CMD cd latexify_py && python test.py
