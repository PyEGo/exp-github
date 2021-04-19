FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD UGATIT-pytorch UGATIT-pytorch
CMD cd UGATIT-pytorch && python main.py --dataset selfie2anime --phase test
