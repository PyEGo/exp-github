FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD springer_free_books springer_free_books
CMD cd springer_free_books && python main.py -i 2
