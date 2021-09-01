FROM python:3.9-buster
ADD pwncat pwncat
RUN cd pwncat && pip install . --no-deps
CMD cd pwncat && pwncat 133.133.133.47:8000

