FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip install scikit-learn
ADD m2cgen m2cgen
CMD cd m2cgen && python test.py
