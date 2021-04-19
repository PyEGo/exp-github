FROM python:3.8
ADD SSRSpeed SSRSpeed
RUN ["apt-get","update"]
RUN ["pip","install","gdctools"]
RUN ["pip","install","OpsletsEc2"]
RUN ["pip","install","Flask"]
RUN ["apt-get","install","-y","git"]
RUN ["pip","install","colorlog"]
RUN ["pip","install","url"]
RUN ["pip","install","Flask-Cors"]
RUN ["pip","install","itsdangerous"]
RUN ["pip","install","Werkzeug"]
RUN ["pip","install","config"]
CMD cd SSRSpeed && python main.py -c ssrspeed_config.example.json --include 韩国 --include-remark Azure --include-group YoYu

