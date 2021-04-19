FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD SSRSpeed SSRSpeed
CMD cd SSRSpeed && python main.py -c ssrspeed_config.example.json --include 韩国 --include-remark Azure --include-group YoYu
