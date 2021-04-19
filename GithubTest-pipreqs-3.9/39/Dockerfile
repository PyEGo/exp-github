FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD SegLoss SegLoss
CMD cd SegLoss/losses_pytorch && python focal_loss.py
