FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install cython3 -y
RUN apt-get install g++ -y
RUN apt-get install libblas3 -y
RUN apt-get install libgfortran5 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libquadmath0 -y
RUN apt-get install libssl-dev -y
RUN apt-get install procps -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install numpy==1.20.3
RUN pip install tqdm==4.60.0
RUN pip install scikit-learn==0.24.2
RUN pip install ftfy==6.0
RUN pip install pandas==1.2.4
RUN pip install torch==1.8.1
RUN pip install spacy==3.0.6
ADD pytorch-openai-transformer-lm pytorch-openai-transformer-lm
# add CMD command to run your programs here
CMD cd pytorch-openai-transformer-lm && python test.py
