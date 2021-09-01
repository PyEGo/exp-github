FROM python:3.9-buster
RUN apt-get clean
RUN apt-get update
RUN apt-get install ca-certificates -y
RUN apt-get install g++ -y
RUN apt-get install libssl-dev -y
RUN pip install --upgrade pip
RUN pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip install jinja2==2.11.2
RUN pip install requests==2.25.0
RUN pip install pyinquirer==1.0.3
RUN pip install beautifulsoup4==4.9.3
ADD Profil3r Profil3r
RUN pip install profil3r --no-deps
# add CMD command to run your programs here
CMD profil3r -p john doe -r ./OSINT
