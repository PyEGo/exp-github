FROM python:3.9-buster
ADD newscatcher newscatcher
RUN ["apt-get","update"]
RUN ["apt-get","install","-y","python-pip"]
RUN ["apt-get","install","-y","python-dev"]
RUN ["apt-get","install","-y","git"]
RUN ["pip","install","Flask"]
RUN ["pip","install","tldextract"]
RUN ["pip","install","feedparser"]
RUN ["pip","install","tld"]
CMD cd newscatcher && python test.py

