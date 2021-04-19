FROM python:3.8
ADD SegLoss SegLoss
RUN ["pip","install","torch"]
RUN ["pip","install","numpy"]
RUN ["pip","install","scipy"]
CMD cd SegLoss/losses_pytorch && python focal_loss.py

