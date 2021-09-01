FROM python:3.9-buster
ADD gplearn gplearn
RUN ["pip","install","geoplot"]
RUN ["pip","install","notifications-python-client"]
RUN ["pip","install","functions"]
RUN ["pip","install","numpy"]
RUN ["pip","install","joblib"]
RUN ["pip","install","veriloggen"]
RUN ["pip","install","utils"]
RUN ["pip","install","scipy"]
RUN ["pip","install","scikit-learn"]
CMD cd gplearn && python test.py

