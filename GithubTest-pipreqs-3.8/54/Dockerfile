FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD data-science-blogs data-science-blogs
CMD cd data-science-blogs && python generate_opml.py && python frequency.py
