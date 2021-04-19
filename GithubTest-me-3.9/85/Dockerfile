FROM python:3.9
ADD wechat_friends wechat_friends
RUN ["pip","install","jieba"]
RUN ["pip","install","six"]
RUN ["pip","install","pytest"]
RUN ["pip","install","py"]
RUN ["pip","install","itchat"]
RUN ["pip","install","pyecharts"]
RUN ["pip","install","Pillow"]
CMD cd wechat_friends && python get_user_info.py

