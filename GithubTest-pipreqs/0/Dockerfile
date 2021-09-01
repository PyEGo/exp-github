FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD tiler tiler
CMD cd tiler && python gen_tiles.py images/cake_at_simple.png
