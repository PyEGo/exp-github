FROM python:3.9-buster
ADD SimCSE SimCSE
RUN ["pip","install","torch"]
RUN ["pip","install","trans"]
RUN ["pip","install","tool"]
RUN ["pip","install","transformers"]
cd SimCSE && python test.py

