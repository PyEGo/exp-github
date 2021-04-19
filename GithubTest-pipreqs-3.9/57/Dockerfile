FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD CVE-2020-1472 CVE-2020-1472
CMD cd CVE-2020-1472 && python ./zerologon_tester.py EXAMPLE-DC 1.2.3.4
