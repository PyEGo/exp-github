FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pillow==8.2.0
RUN pip install pyyaml==5.4.1
RUN pip install absl-py==0.12.0
ADD arxiv-latex-cleaner arxiv-latex-cleaner
RUN cd arxiv-latex-cleaner && pip install . --no-deps
# add CMD command to run your programs here
CMD arxiv_latex_cleaner -h
