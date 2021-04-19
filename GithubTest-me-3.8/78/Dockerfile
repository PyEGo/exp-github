FROM python:3.8
ADD distribution-is-all-you-need distribution-is-all-you-need
RUN ["pip","install","numpy"]
RUN ["pip","install","matplotlib"]
CMD cd distribution-is-all-you-need && python uniform.py

