FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD tensorflow-yolov3 tensorflow-yolov3
CMD cd tensorflow-yolov3 && python image_demo.py
