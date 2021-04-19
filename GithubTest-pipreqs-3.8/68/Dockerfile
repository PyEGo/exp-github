FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD links-uteis links-uteis
CMD cd links-uteis && python ordena_md_categoria.py
