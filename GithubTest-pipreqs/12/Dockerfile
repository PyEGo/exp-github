FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD learn_math_fast learn_math_fast
CMD cd learn_math_fast && python build_toc.py
