FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD Vxscan Vxscan
CMD cd Vxscan && python Vxscan.py -i 127.0.0.0/24
