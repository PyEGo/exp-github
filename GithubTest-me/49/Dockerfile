FROM python:3.9-buster
ADD doublepulsar-detection-script doublepulsar-detection-script
RUN ["pip","install","netaddr"]
CMD cd doublepulsar-detection-script && python detect_doublepulsar_smb.py --ip 133.133.133.120
