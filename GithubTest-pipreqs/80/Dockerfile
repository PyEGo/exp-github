FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD Profil3r Profil3r
RUN pip install profil3r --no-deps
CMD profil3r -p john doe -r ./OSINT
