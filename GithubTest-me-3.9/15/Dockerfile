FROM python:3.9
ADD koalas koalas
RUN ["pip","install","pan-python"]
RUN ["pip","install","six"]
RUN ["pip","install","pytest"]
RUN ["pip","install","py"]
RUN ["pip","install","access_points"]
RUN ["pip","install","tensorlayer"]
RUN ["pip","install","pandas"]
RUN ["pip","install","pandacan"]
RUN ["pip","install","pyte"]
RUN ["pip","install","numpy"]
RUN ["pip","install","matplotlib"]
RUN ["pip","install","pyspark"]
RUN ["pip","install","di-py"]
RUN ["pip","install","pyarrow"]
RUN ["pip","install","databricks"]
CMD cd koalas && python test.py

