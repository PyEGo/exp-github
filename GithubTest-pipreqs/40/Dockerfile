FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD coding-problems coding-problems
CMD cd coding-problems/LinkedLists && python odd_even_ll.py
