FROM python:3.9
ADD ResNeSt ResNeSt
RUN ["pip","install","tqdm"]
RUN ["pip","install","requests"]
RUN ["pip","install","psycopg2"]
RUN ["pip","install","python-dateutil"]
RUN ["pip","install","pathlib"]
RUN ["pip","install","pytest"]
RUN ["pip","install","path.py"]
RUN ["pip","install","torchvision"]
RUN ["pip","install","Pillow"]
RUN ["pip","install","numpy"]
CMD cd ResNeSt && python test.py

