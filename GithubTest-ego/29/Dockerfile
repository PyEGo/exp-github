FROM python:3.9
RUN sed -i s@/archive.ubuntu.com/@/mirrors.aliyun.com/@g /etc/apt/sources.list
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pillow==8.0.1
RUN pip install pyyaml==5.3.1
RUN pip install absl-py==0.11.0
ADD arxiv-latex-cleaner arxiv-latex-cleaner
RUN cd arxiv-latex-cleaner && pip install . --no-deps
# add CMD command to run your programs here
CMD arxiv_latex_cleaner -h
