FROM python:3.9-buster
ADD SSRFmap SSRFmap
CMD cd SSRFmap && python ssrfmap.py -r data/request.txt -p url -m readfiles,portscan

