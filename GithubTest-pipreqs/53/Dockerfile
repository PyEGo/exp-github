FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD pwncat pwncat
RUN cd pwncat && pip install . --no-deps
CMD cd pwncat && pwncat 133.133.133.47:8000
