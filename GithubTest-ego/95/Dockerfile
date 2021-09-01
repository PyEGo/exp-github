FROM python:3.8-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install git -y
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libopencv-calib3d3.2 -y
RUN apt-get install libopencv-contrib3.2 -y
RUN apt-get install libopencv-core3.2 -y
RUN apt-get install libopencv-features2d3.2 -y
RUN apt-get install libopencv-flann3.2 -y
RUN apt-get install libopencv-highgui3.2 -y
RUN apt-get install libopencv-imgcodecs3.2 -y
RUN apt-get install libopencv-imgproc3.2 -y
RUN apt-get install libopencv-ml3.2 -y
RUN apt-get install libopencv-objdetect3.2 -y
RUN apt-get install libopencv-photo3.2 -y
RUN apt-get install libopencv-shape3.2 -y
RUN apt-get install libopencv-stitching3.2 -y
RUN apt-get install libopencv-superres3.2 -y
RUN apt-get install libopencv-video3.2 -y
RUN apt-get install libopencv-videoio3.2 -y
RUN apt-get install libopencv-videostab3.2 -y
RUN apt-get install libopencv-viz3.2 -y
RUN apt-get install libprotobuf17 -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install tqdm==4.60.0
RUN pip install easydict==1.9
RUN pip install numpy==1.20.3
RUN pip install pillow==8.2.0
RUN pip install opencv-python==4.5.2.52
RUN pip install tensorflow==2.4.0
RUN pip install matplotlib==3.4.2
ADD tensorflow-yolov3 tensorflow-yolov3
# add CMD command to run your programs here
CMD cd tensorflow-yolov3 && python image_demo.py
