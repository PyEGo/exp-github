FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD Packer-Fuzzer Packer-Fuzzer
CMD cd Packer-Fuzzer && python PackerFuzzer.py -u http://133.133.133.47:8000
