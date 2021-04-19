FROM python:3.8
ADD BlueKeep BlueKeep
RUN ["pip","install","pyOpenSSL"]
RUN ["pip","install","impacket"]
CMD cd BlueKeep && python bluekeep_dos.py -i 127.0.0.1

