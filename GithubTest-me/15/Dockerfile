FROM python:3.9-buster
ADD pyts pyts
RUN ["pip","install","numpy"]
RUN ["pip","install","scikit-learn"]
RUN pip install matplotlib
cd pyts && python plot_dft.py

