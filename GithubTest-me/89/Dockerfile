FROM python:3.9-buster
ADD pyp pyp
RUN cd pyp && pip install . --no-deps
CMD ps x | pyp 'line.split()[4]'

