FROM python:3.7-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install build-essential -y
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install git -y
RUN apt-get install libblas3 -y
RUN apt-get install libbz2-dev -y
RUN apt-get install libffi-dev -y
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
RUN apt-get install libreadline-dev -y
RUN apt-get install libsqlite3-dev -y
RUN apt-get install libssl-dev -y
RUN apt-get install libzmq5 -y
RUN apt-get install software-properties-common -y
RUN apt-get install tk-dev -y
RUN apt-get install unzip -y
RUN apt-get install wget -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install psutil==5.8.0
RUN pip install pyspark==3.1.1
RUN pip install pytz==2021.1
RUN pip install six==1.15.0
RUN pip install py4j==0.10.9.1
RUN pip install dill==0.3.3
RUN pip install numpy==1.20.3
RUN pip install future==0.18.2
RUN pip install pillow==8.2.0
RUN pip install mock==4.0.3
RUN pip install diskcache==5.2.1
RUN pip install opencv-python==4.5.2.52
RUN pip install pyarrow==0.14.1
RUN pip install packaging==20.9
RUN pip install tensorflow==2.4.0
RUN pip install pandas==1.1.5
RUN pip install pyzmq==22.0.3
RUN pip install torch==1.8.1
RUN pip install torchvision==0.9.1
RUN pip install pytest==6.2.1
RUN pip install gcsfs==2021.4.0
RUN pip install s3fs==2021.4.0
RUN pip install hops-petastorm==0.9.4
ADD petastorm petastorm
# add CMD command to run your programs here
CMD cd petastorm && python test.py
