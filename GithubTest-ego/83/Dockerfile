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
RUN pip install joblib==1.0.0
RUN pip install numpy==1.20.3
RUN pip install six==1.16.0
RUN pip install networkx==2.5
RUN pip install scipy==1.6.3
RUN pip install nltk==3.6.2
RUN pip install scikit-learn==0.24.2
RUN pip install spacy==3.0.6
ADD pke pke
RUN python -m nltk.downloader stopwords && python -m nltk.downloader universal_tagset && python -m spacy download en
# add CMD command to run your programs here
CMD cd pke && python test.py
