FROM python:2.7-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ieee-data -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install netaddr==0.8.0
ADD doublepulsar-detection-script doublepulsar-detection-script
# add CMD command to run your programs here
CMD cd doublepulsar-detection-script && python detect_doublepulsar_smb.py --ip 133.133.133.120
