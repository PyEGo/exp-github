FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD latexify_py latexify_py
CMD cd latexify_py && python test.py
