FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD pyts pyts
RUN pip install matplotlib
CMD cd pyts && python plot_dft.py
