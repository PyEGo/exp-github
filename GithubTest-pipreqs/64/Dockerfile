FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD sweetviz sweetviz
RUN pip install pandas
CMD cd sweetviz && python test.py
