FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD mnssp3-DNA mnssp3-DNA
CMD cd mnssp3-DNA/DNA/MotifFinding/Python/n-gram/simple && python test.py
