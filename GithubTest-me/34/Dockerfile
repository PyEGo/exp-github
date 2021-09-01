FROM python:3.9-buster
ADD m2cgen m2cgen
RUN ["pip","install","m2cgen"]
RUN ["pip","install","exporters"]
RUN ["pip","install","django-export"]
RUN pip install scikit-learn
CMD cd m2cgen && python test.py

