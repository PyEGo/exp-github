FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install dj-database-url==0.5.0
RUN pip install django==3.2.2
RUN pip install djangorestframework==3.12.2
ADD django-vue-template django-vue-template
# add CMD command to run your programs here
CMD cd django-vue-template && python manage.py runserver
