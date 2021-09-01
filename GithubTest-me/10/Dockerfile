FROM python:3.9-buster
ADD chinese_province_city_area_mapper chinese_province_city_area_mapper
RUN ["pip","install","pandacan"]
RUN ["pip","install","six"]
RUN ["pip","install","pytest"]
RUN ["pip","install","py"]
RUN ["pip","install","folium"]
RUN ["pip","install","pan-python"]
RUN ["pip","install","pyecharts"]
RUN ["pip","install","pandas"]
CMD cd chinese_province_city_area_mapper && python test.py

