FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install pymongo==3.11.2
RUN pip install requests==2.25.0
RUN pip install beautifulsoup4==4.9.3
ADD DXY-COVID-19-Crawler DXY-COVID-19-Crawler
# add CMD command to run your programs here
CMD cd DXY-COVID-19-Crawler && python main.py
