FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
RUN pip install pandas
ADD sweetviz sweetviz
CMD cd sweetviz && python test.py
