FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD distribution-is-all-you-need distribution-is-all-you-need
CMD cd distribution-is-all-you-need && python uniform.py
