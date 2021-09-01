FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD doublepulsar-detection-script doublepulsar-detection-script
CMD cd doublepulsar-detection-script && python detect_doublepulsar_smb.py --ip 133.133.133.120
