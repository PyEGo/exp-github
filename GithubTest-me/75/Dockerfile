FROM python:3.9-buster
ADD sentry-python sentry-python
RUN ["pip","install","requests"]
RUN ["pip","install","six"]
RUN ["pip","install","typing"]
RUN ["pip","install","sen"]
RUN ["pip","install","url"]
RUN ["pip","install","aiocontextvars"]
RUN ["pip","install","typing-extensions"]
RUN ["pip","install","eventlet"]
RUN ["pip","install","uws-client"]
RUN ["pip","install","contextvars"]
RUN ["pip","install","uWSGI"]
RUN ["pip","install","urllib3"]
RUN ["pip","install","sentry-sdk"]
RUN ["pip","install","gevent"]
CMD cd sentry-python && python test.py
