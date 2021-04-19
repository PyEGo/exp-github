FROM python:3.8
ADD links-uteis links-uteis
RUN ["pip","install","pan-python"]
RUN ["pip","install","pandacan"]
RUN ["pip","install","pandas"]
CMD cd links-uteis && python ordena_md_categoria.py
