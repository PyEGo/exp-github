FROM python:3.8
ADD PrettyErrors PrettyErrors
RUN ["pip","install","requests"]
RUN ["pip","install","colorama"]
CMD cd PrettyErrors && python test.py

