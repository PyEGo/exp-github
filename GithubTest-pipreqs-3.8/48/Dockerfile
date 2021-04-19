FROM python:3.8
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD SSRFmap SSRFmap
CMD cd SSRFmap && python ssrfmap.py -r data/request.txt -p url -m readfiles,portscan
