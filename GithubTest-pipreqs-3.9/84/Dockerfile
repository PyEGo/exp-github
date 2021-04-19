FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD BlueKeep BlueKeep
CMD cd BlueKeep && python bluekeep_dos.py -i 127.0.0.1
