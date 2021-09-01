FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libblas3 -y
RUN apt-get install liblapack3 -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pyahocorasick==1.4.1
RUN pip install setuptools==56.2.0
RUN pip install folium==0.12.1
RUN pip install pandas==1.2.4
RUN pip install pyecharts==1.9.0
ADD chinese_province_city_area_mapper chinese_province_city_area_mapper
# add CMD command to run your programs here
CMD cd chinese_province_city_area_mapper && python test.py
