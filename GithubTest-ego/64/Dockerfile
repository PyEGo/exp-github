FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install libblas3 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libquadmath0 -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install jinja2==2.11.2
RUN pip install numpy==1.20.3
RUN pip install tqdm==4.60.0
RUN pip install setuptools==56.2.0
RUN pip install scipy==1.6.3
RUN pip install matplotlib==3.4.2
RUN pip install pandas==1.2.4
RUN pip install ipython==7.23.1
ADD sweetviz sweetviz
RUN pip install pandas
# add CMD command to run your programs here
CMD cd sweetviz && python test.py
