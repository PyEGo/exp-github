FROM python:3.9-buster
ADD policy_sentry policy_sentry
RUN cd policy_sentry && pip install . --no-deps
CMD policy_sentry create-template --output-file crud.yml --template-type crud

