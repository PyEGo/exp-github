FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD learn_math_fast learn_math_fast
CMD python learn_math_fast/build_toc.py
