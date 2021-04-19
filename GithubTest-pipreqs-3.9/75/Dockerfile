FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD leedeeprl-notes leedeeprl-notes
CMD cd leedeeprl-notes/codes/A2C && python main.py
