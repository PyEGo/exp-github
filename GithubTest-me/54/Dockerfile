FROM python:3.9-buster
ADD uncertainty-toolbox uncertainty-toolbox
RUN ["apt-get","update"]
RUN ["pip","install","seaborn"]
RUN ["pip","install","access_points"]
RUN ["pip","install","sh"]
RUN ["pip","install","metrics"]
RUN ["apt-get","install","-y","git"]
RUN ["pip","install","Shapely"]
RUN ["pip","install","tqdm"]
RUN ["pip","install","numpy"]
RUN ["pip","install","scikit-learn"]
RUN ["pip","install","tensorlayer"]
RUN ["pip","install","data"]
RUN ["pip","install","matplotlib"]
RUN ["pip","install","scipy"]
CMD cd uncertainty-toolbox && python test.py

