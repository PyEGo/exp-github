FROM python:3.8
ADD efficientnet efficientnet
RUN ["pip","install","six"]
RUN ["pip","install","preprocessing"]
RUN ["pip","install","numpy"]
RUN ["pip","install","Keras"]
RUN ["pip","install","scikit-image"]
CMD cd efficientnet && python test.py

