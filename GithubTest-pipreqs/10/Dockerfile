FROM python:3.9-buster
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD chinese_province_city_area_mapper chinese_province_city_area_mapper
CMD cd chinese_province_city_area_mapper && python test.py
