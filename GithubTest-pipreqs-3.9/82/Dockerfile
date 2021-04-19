FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD micronet micronet
CMD cd micronet && python -c "import micronet; print(micronet.__version__)"
