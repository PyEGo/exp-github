FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD python-for-absolute-beginners-course python-for-absolute-beginners-course
CMD cd python-for-absolute-beginners-course && python code/07-data-structures/rocks-game/rpsgame.py
