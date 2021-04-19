FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD pipx pipx
RUN cd pipx && pip install . --no-deps
CMD pipx completions
