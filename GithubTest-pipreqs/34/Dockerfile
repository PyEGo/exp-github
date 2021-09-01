FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD m2cgen m2cgen
RUN pip install scikit-learn
CMD cd m2cgen && python test.py
