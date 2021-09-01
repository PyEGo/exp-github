FROM python:3.9-buster
ADD Flask-HTTPAuth Flask-HTTPAuth
RUN ["pip","install","Flask"]
RUN ["pip","install","itsdangerous"]
RUN ["pip","install","Werkzeug"]
CMD cd Flask-HTTPAuth/src && python test.py
