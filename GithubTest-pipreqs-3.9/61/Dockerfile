FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD mnssp3-EMR mnssp3-EMR
CMD cd mnssp3-EMR/EMR/DiabeticRetinopathyDetection/Python/Diabetic_Retinopathy_Detection && python test.py
