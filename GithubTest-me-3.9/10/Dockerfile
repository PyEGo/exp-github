FROM python:3.9
ADD DeepLearning DeepLearning
RUN ["apt-get","update"]
RUN ["pip","install","progress"]
RUN ["pip","install","chapter"]
RUN ["pip","install","numpy"]
RUN ["apt-get","install","-y","git"]
RUN ["apt-get","install","-y","build-essential"]
RUN ["pip","install","pytz"]
RUN ["pip","install","progressbar2"]
RUN ["pip","install","progressbar"]
CMD cd DeepLearning/code && python chapter7.py

