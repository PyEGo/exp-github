FROM python:3.9
ADD noisy noisy
RUN ["pip","install","url"]
RUN ["pip","install","requests"]
RUN ["pip","install","urllib3"]
CMD cd noisy && python noisy.py

