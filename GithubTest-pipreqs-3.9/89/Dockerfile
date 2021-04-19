FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD pyp pyp
RUN cd pyp && pip install . --no-deps
CMD ps x | pyp 'line.split()[4]'
