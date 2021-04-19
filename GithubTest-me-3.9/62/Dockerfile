FROM python:3.9
ADD mnssp3-EEG mnssp3-EEG
RUN ["pip","install","pan-python"]
RUN ["pip","install","pandacan"]
RUN ["pip","install","numpy"]
RUN ["pip","install","Keras"]
RUN ["pip","install","scikit-learn"]
RUN ["pip","install","matplotlib"]
RUN ["pip","install","pandas"]
RUN ["pip","install","keras-models"]
CMD cd mnssp3-EEG/EEG/EpilepsyDetection/Python/EEG && python predict.py

